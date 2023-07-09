# Comparing `tmp/python-telegram-bot-raw-20.3.tar.gz` & `tmp/python-telegram-bot-raw-20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-bot-raw-20.3.tar", last modified: Sun May  7 13:32:51 2023, max compression
+gzip compressed data, was "python-telegram-bot-raw-20.4.tar", last modified: Sun Jul  9 10:20:08 2023, max compression
```

## Comparing `python-telegram-bot-raw-20.3.tar` & `python-telegram-bot-raw-20.4.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE.dual
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE.lesser
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/MANIFEST.in
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12744 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12922 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/README.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11058 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/README_RAW.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      464 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/pyproject.toml
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.081768 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12744 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4840 2023-05-07 13:32:51.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/SOURCES.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/dependency_links.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      205 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/requires.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/top_level.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/requirements-opts.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      373 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/requirements.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      199 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/setup-raw.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1841 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/setup.cfg
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4701 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/setup.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.089768 python-telegram-bot-raw-20.3/telegram/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13278 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1880 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/__main__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   346047 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3268 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10225 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2462 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1791 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_botname.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29315 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   115940 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8854 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6714 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8353 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3295 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    24730 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7961 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11291 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4244 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7002 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_dice.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.093768 python-telegram-bot-raw-20.3/telegram/_files/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3506 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/_basemedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4834 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_files/_basethumbedmedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4419 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/animation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4656 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/audio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7065 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/chatphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2680 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/contact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3698 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/document.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14404 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/file.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4156 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputfile.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29640 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputmedia.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4407 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4724 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/location.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2777 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/photosize.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17115 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/sticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4416 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/venue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4236 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/video.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/videonote.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3001 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/voice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4329 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6855 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_forumtopic.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.093768 python-telegram-bot-raw-20.3/telegram/_games/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1270 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/callbackgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8064 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/game.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2494 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/gamehighscore.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_inline/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15081 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5591 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9344 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2770 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7967 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultarticle.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5625 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5088 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5606 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcacheddocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5363 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5454 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5609 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5526 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5301 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8252 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcontact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9875 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultdocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2715 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10543 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12054 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10114 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8583 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5363 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultsbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9874 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvenue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10492 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5527 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2716 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputcontactmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12680 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputinvoicemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6528 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputlocationmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1528 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3691 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputtextmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4511 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputvenuemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9173 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2417 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9333 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5096 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6744 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   160309 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1976 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8171 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1665 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageid.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_passport/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22561 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/credentials.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6303 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/data.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12481 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/encryptedpassportelement.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5161 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16944 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportelementerrors.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6186 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportfile.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_payment/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5016 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/invoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2664 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/labeledprice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3044 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/orderinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5918 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/precheckoutquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2938 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingaddress.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2516 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingoption.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4493 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4909 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/successfulpayment.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16254 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2813 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16268 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3198 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2165 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4286 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4076 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_switchinlinequerychosenchat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    25884 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19406 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    60726 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2897 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_userprofilephotos.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/telegram/_utils/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1520 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/argumentparsing.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8956 2023-04-26 19:48:31.000000 python-telegram-bot-raw-20.3/telegram/_utils/datetime.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4060 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/defaultvalue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2662 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/enum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5735 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/files.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1932 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/logging.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/markup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3276 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/types.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2010 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3941 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_utils/warnings_transition.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2148 2023-05-07 13:02:55.000000 python-telegram-bot-raw-20.3/telegram/_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5982 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2405 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2083 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7600 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1825 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_writeaccessallowed.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    68271 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6288 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7146 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/py.typed
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/telegram/request/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18113 2023-04-26 19:48:31.000000 python-telegram-bot-raw-20.3/telegram/request/_baserequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10362 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_httpxrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5155 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_requestdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7394 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_requestparameter.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1900 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/warnings.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.4/LICENSE
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.4/LICENSE.dual
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.4/LICENSE.lesser
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.4/MANIFEST.in
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12715 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12941 2023-07-09 10:12:31.000000 python-telegram-bot-raw-20.4/README.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11079 2023-07-09 10:12:31.000000 python-telegram-bot-raw-20.4/README_RAW.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      594 2023-07-09 09:30:36.000000 python-telegram-bot-raw-20.4/pyproject.toml
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.189761 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12715 2023-07-09 10:20:08.000000 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4840 2023-07-09 10:20:08.000000 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/SOURCES.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2023-07-09 10:20:08.000000 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/dependency_links.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      205 2023-07-09 10:20:08.000000 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/requires.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2023-07-09 10:20:08.000000 python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/top_level.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2023-06-04 15:34:31.000000 python-telegram-bot-raw-20.4/requirements-opts.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      373 2023-06-04 15:34:31.000000 python-telegram-bot-raw-20.4/requirements.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      199 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/setup-raw.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1816 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/setup.cfg
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4648 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/setup.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.197761 python-telegram-bot-raw-20.4/telegram/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13278 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1880 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/__main__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   351078 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_bot.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3273 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_botcommand.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10295 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_botcommandscope.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2511 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_botdescription.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1805 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_botname.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29739 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_callbackquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   118810 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8904 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatadministratorrights.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6764 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatinvitelink.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8745 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatjoinrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3296 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    24839 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatmember.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7991 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatmemberupdated.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11451 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_chatpermissions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4274 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_choseninlineresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6977 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_dice.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.197761 python-telegram-bot-raw-20.4/telegram/_files/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3536 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/_basemedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4874 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/_basethumbedmedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4479 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/animation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4736 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/audio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7096 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/chatphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2720 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/contact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3758 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/document.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14454 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/file.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4191 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/inputfile.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    30090 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/inputmedia.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4475 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/inputsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4762 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/location.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2826 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/photosize.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17231 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/sticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4466 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/venue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4296 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/video.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3698 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/videonote.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3031 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_files/voice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4350 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_forcereply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6965 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_forumtopic.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.197761 python-telegram-bot-raw-20.4/telegram/_games/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_games/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1309 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_games/callbackgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8114 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_games/game.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2518 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_games/gamehighscore.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.201761 python-telegram-bot-raw-20.4/telegram/_inline/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15172 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinekeyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5601 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinekeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9436 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2781 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8077 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultarticle.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5695 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5138 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5666 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcacheddocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5423 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5514 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5679 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3659 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5586 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5351 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8362 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcontact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9995 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultdocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2735 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10673 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12160 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10244 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8693 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5384 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultsbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10004 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvenue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10612 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5587 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2746 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputcontactmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12830 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputinvoicemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6554 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputlocationmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1567 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3721 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputtextmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4561 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_inline/inputvenuemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9252 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_keyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2462 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_keyboardbuttonpolltype.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9433 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_keyboardbuttonrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5136 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_loginurl.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6772 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_menubutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   163640 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_message.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2015 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_messageautodeletetimerchanged.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8164 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_messageentity.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1704 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_messageid.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.201761 python-telegram-bot-raw-20.4/telegram/_passport/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22805 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/credentials.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6373 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/data.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12581 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/encryptedpassportelement.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5171 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/passportdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17199 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/passportelementerrors.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6216 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_passport/passportfile.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/telegram/_payment/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5012 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/invoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2703 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/labeledprice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3094 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/orderinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5968 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/precheckoutquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2977 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/shippingaddress.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2536 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/shippingoption.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4533 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/shippingquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4939 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_payment/successfulpayment.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16354 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_poll.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2864 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_proximityalerttriggered.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16379 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_replykeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3218 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_replykeyboardremove.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2199 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_sentwebappmessage.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4335 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_shared.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4136 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_switchinlinequerychosenchat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    25953 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_telegramobject.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19523 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_update.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    62794 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_user.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2907 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_userprofilephotos.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/telegram/_utils/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1520 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/argumentparsing.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8996 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/datetime.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4060 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/defaultvalue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2662 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/enum.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5755 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/files.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1970 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/logging.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/markup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3510 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/types.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2010 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/warnings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3941 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_utils/warnings_transition.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2276 2023-07-09 10:15:18.000000 python-telegram-bot-raw-20.4/telegram/_version.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6022 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_videochat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2444 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_webappdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2122 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_webappinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7670 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_webhookinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1859 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/_writeaccessallowed.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    68320 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/constants.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6318 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/error.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7252 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/helpers.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.4/telegram/py.typed
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-07-09 10:20:08.205761 python-telegram-bot-raw-20.4/telegram/request/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/request/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17937 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/request/_baserequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10409 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/request/_httpxrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5204 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/request/_requestdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7408 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/request/_requestparameter.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1900 2023-07-09 10:12:29.000000 python-telegram-bot-raw-20.4/telegram/warnings.py
```

### Comparing `python-telegram-bot-raw-20.3/LICENSE` & `python-telegram-bot-raw-20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/LICENSE.dual` & `python-telegram-bot-raw-20.4/LICENSE.dual`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/LICENSE.lesser` & `python-telegram-bot-raw-20.4/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/PKG-INFO` & `python-telegram-bot-raw-20.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 20.3
+Version: 20.4
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -18,20 +18,19 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: socks
 Provides-Extra: all
 Provides-Extra: http2
 Provides-Extra: passport
 License-File: LICENSE
 License-File: LICENSE.dual
@@ -112,15 +111,15 @@
 *Stay tuned for library updates and new releases on our* `Telegram Channel <https://telegram.me/pythontelegrambotchannel>`_.
 
 Introduction
 ============
 
 This library provides a pure Python, asynchronous interface for the
 `Telegram Bot API <https://core.telegram.org/bots/api>`_.
-It's compatible with Python versions **3.7+**.
+It's compatible with Python versions **3.8+**.
 
 ``python-telegram-bot-raw`` is part of the `python-telegram-bot <https://python-telegram-bot.org>`_ ecosystem and provides the pure API functionality extracted from PTB. It therefore does not have independent release schedules, changelogs or documentation.
 
 Note
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
@@ -171,34 +170,34 @@
 
 ``python-telegram-bot`` tries to use as few 3rd party dependencies as possible.
 However, for some features using a 3rd party library is more sane than implementing the functionality again.
 As these features are *optional*, the corresponding 3rd party dependencies are not installed by default.
 Instead, they are listed as optional dependencies.
 This allows to avoid unnecessary dependency conflicts for users who don't need the optional features.
 
-The only required dependency is `httpx ~= 0.23.3 <https://www.python-httpx.org>`_ for
+The only required dependency is `httpx ~= 0.24.1 <https://www.python-httpx.org>`_ for
 ``telegram.request.HTTPXRequest``, the default networking backend.
 
 ``python-telegram-bot`` is most useful when used along with additional libraries.
 To minimize dependency conflicts, we try to be liberal in terms of version requirements on the (optional) dependencies.
 On the other hand, we have to ensure stability of ``python-telegram-bot``, which is why we do apply version bounds.
 If you encounter dependency conflicts due to these bounds, feel free to reach out.
 
 Optional Dependencies
 #####################
 
 PTB can be installed with optional dependencies:
 
-* ``pip install python-telegram-bot-raw[passport]`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
-* ``pip install python-telegram-bot-raw[socks]`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
-* ``pip install python-telegram-bot[http2]`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
+* ``pip install "python-telegram-bot-raw[passport]"`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
+* ``pip install "python-telegram-bot-raw[socks]"`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
+* ``pip install "python-telegram-bot-raw[http2]"`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
 
-To install multiple optional dependencies, separate them by commas, e.g. ``pip install python-telegram-bot-raw[passport,socks]``.
+To install multiple optional dependencies, separate them by commas, e.g. ``pip install "python-telegram-bot-raw[passport,socks]"``.
 
-Additionally, the shortcut ``pip install python-telegram-bot-raw[all]`` installs all optional dependencies.
+Additionally, the shortcut ``pip install "python-telegram-bot-raw[all]"`` installs all optional dependencies.
 
 Quick Start
 ===========
 
 Our Wiki contains an `Introduction to the API <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API>`_ explaining how the pure Bot API can be accessed via ``python-telegram-bot``.
 
 Resources
@@ -230,15 +229,15 @@
 Because ``asyncio`` is in general single-threaded, ``python-telegram-bot`` does currently not aim to be thread-safe.
 
 Contributing
 ============
 
 Contributions of all sizes are welcome.
 Please review our `contribution guidelines <https://github.com/python-telegram-bot/python-telegram-bot/blob/master/.github/CONTRIBUTING.rst>`_ to get started.
-You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new>`_.
+You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new/choose>`_.
 
 Donating
 ========
 Occasionally we are asked if we accept donations to support the development.
 While we appreciate the thought, maintaining PTB is our hobby, and we have almost no running costs for it. We therefore have nothing set up to accept donations.
 If you still want to donate, we kindly ask you to donate to another open source project/initiative of your choice instead.
```

### Comparing `python-telegram-bot-raw-20.3/README.rst` & `python-telegram-bot-raw-20.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 *Stay tuned for library updates and new releases on our* `Telegram Channel <https://telegram.me/pythontelegrambotchannel>`_.
 
 Introduction
 ============
 
 This library provides a pure Python, asynchronous interface for the
 `Telegram Bot API <https://core.telegram.org/bots/api>`_.
-It's compatible with Python versions **3.7+**.
+It's compatible with Python versions **3.8+**.
 
 In addition to the pure API implementation, this library features a number of high-level classes to
 make the development of bots easy and straightforward. These classes are contained in the
 ``telegram.ext`` submodule.
 
 A pure API implementation *without* ``telegram.ext`` is available as the standalone package ``python-telegram-bot-raw``.  `See here for details. <https://github.com/python-telegram-bot/python-telegram-bot/blob/master/README_RAW.rst>`_
 
@@ -131,47 +131,47 @@
 
 ``python-telegram-bot`` tries to use as few 3rd party dependencies as possible.
 However, for some features using a 3rd party library is more sane than implementing the functionality again.
 As these features are *optional*, the corresponding 3rd party dependencies are not installed by default.
 Instead, they are listed as optional dependencies.
 This allows to avoid unnecessary dependency conflicts for users who don't need the optional features.
 
-The only required dependency is `httpx ~= 0.23.3 <https://www.python-httpx.org>`_ for
+The only required dependency is `httpx ~= 0.24.1 <https://www.python-httpx.org>`_ for
 ``telegram.request.HTTPXRequest``, the default networking backend.
 
 ``python-telegram-bot`` is most useful when used along with additional libraries.
 To minimize dependency conflicts, we try to be liberal in terms of version requirements on the (optional) dependencies.
 On the other hand, we have to ensure stability of ``python-telegram-bot``, which is why we do apply version bounds.
 If you encounter dependency conflicts due to these bounds, feel free to reach out.
 
 Optional Dependencies
 #####################
 
 PTB can be installed with optional dependencies:
 
-* ``pip install python-telegram-bot[passport]`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
-* ``pip install python-telegram-bot[socks]`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
-* ``pip install python-telegram-bot[http2]`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
-* ``pip install python-telegram-bot[rate-limiter]`` installs `aiolimiter~=1.0.0 <https://aiolimiter.readthedocs.io/en/stable/>`_. Use this, if you want to use ``telegram.ext.AIORateLimiter``.
-* ``pip install python-telegram-bot[webhooks]`` installs the `tornado~=6.2 <https://www.tornadoweb.org/en/stable/>`_ library. Use this, if you want to use ``telegram.ext.Updater.start_webhook``/``telegram.ext.Application.run_webhook``.
-* ``pip install python-telegram-bot[callback-data]`` installs the `cachetools~=5.3.0 <https://cachetools.readthedocs.io/en/latest/>`_ library. Use this, if you want to use `arbitrary callback_data <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Arbitrary-callback_data>`_.
-* ``pip install python-telegram-bot[job-queue]`` installs the `APScheduler~=3.10.1 <https://apscheduler.readthedocs.io/en/3.x/>`_ library and enforces `pytz>=2018.6 <https://pypi.org/project/pytz/>`_, where ``pytz`` is a dependency of ``APScheduler``. Use this, if you want to use the ``telegram.ext.JobQueue``.
+* ``pip install "python-telegram-bot[passport]"`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
+* ``pip install "python-telegram-bot[socks]"`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
+* ``pip install "python-telegram-bot[http2]"`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
+* ``pip install "python-telegram-bot[rate-limiter]"`` installs `aiolimiter~=1.1.0 <https://aiolimiter.readthedocs.io/en/stable/>`_. Use this, if you want to use ``telegram.ext.AIORateLimiter``.
+* ``pip install "python-telegram-bot[webhooks]"`` installs the `tornado~=6.2 <https://www.tornadoweb.org/en/stable/>`_ library. Use this, if you want to use ``telegram.ext.Updater.start_webhook``/``telegram.ext.Application.run_webhook``.
+* ``pip install "python-telegram-bot[callback-data]"`` installs the `cachetools~=5.3.1 <https://cachetools.readthedocs.io/en/latest/>`_ library. Use this, if you want to use `arbitrary callback_data <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Arbitrary-callback_data>`_.
+* ``pip install "python-telegram-bot[job-queue]"`` installs the `APScheduler~=3.10.1 <https://apscheduler.readthedocs.io/en/3.x/>`_ library and enforces `pytz>=2018.6 <https://pypi.org/project/pytz/>`_, where ``pytz`` is a dependency of ``APScheduler``. Use this, if you want to use the ``telegram.ext.JobQueue``.
 
-To install multiple optional dependencies, separate them by commas, e.g. ``pip install python-telegram-bot[socks,webhooks]``.
+To install multiple optional dependencies, separate them by commas, e.g. ``pip install "python-telegram-bot[socks,webhooks]"``.
 
 Additionally, two shortcuts are provided:
 
-* ``pip install python-telegram-bot[all]`` installs all optional dependencies.
-* ``pip install python-telegram-bot[ext]`` installs all optional dependencies that are related to ``telegram.ext``, i.e. ``[rate-limiter, webhooks, callback-data, job-queue]``.
+* ``pip install "python-telegram-bot[all]"`` installs all optional dependencies.
+* ``pip install "python-telegram-bot[ext]"`` installs all optional dependencies that are related to ``telegram.ext``, i.e. ``[rate-limiter, webhooks, callback-data, job-queue]``.
 
 Quick Start
 ===========
 
 Our Wiki contains an `Introduction to the API <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API>`_ explaining how the pure Bot API can be accessed via ``python-telegram-bot``.
-Moreover, the `Tutorial: Your first Bot <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Extensions-%E2%80%93-Your-first-Bot>`_ gives an introduction on how chatbots can be easily programmed with the help of the ``telegram.ext`` module.
+Moreover, the `Tutorial: Your first Bot <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Extensions---Your-first-Bot>`_ gives an introduction on how chatbots can be easily programmed with the help of the ``telegram.ext`` module.
 
 Resources
 =========
 
 - The `package documentation <https://docs.python-telegram-bot.org/>`_ is the technical reference for ``python-telegram-bot``.
   It contains descriptions of all available classes, modules, methods and arguments as well as the `changelog <https://docs.python-telegram-bot.org/changelog.html>`_.
 - The `wiki <https://github.com/python-telegram-bot/python-telegram-bot/wiki/>`_ is home to number of more elaborate introductions of the different features of ``python-telegram-bot`` and other useful resources that go beyond the technical documentation.
@@ -205,15 +205,15 @@
 * all classes in the ``telegram.ext.filters`` module that allow to add/remove allowed users/chats at runtime
 
 Contributing
 ============
 
 Contributions of all sizes are welcome.
 Please review our `contribution guidelines <https://github.com/python-telegram-bot/python-telegram-bot/blob/master/.github/CONTRIBUTING.rst>`_ to get started.
-You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new>`_.
+You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new/choose>`_.
 
 Donating
 ========
 Occasionally we are asked if we accept donations to support the development.
 While we appreciate the thought, maintaining PTB is our hobby, and we have almost no running costs for it. We therefore have nothing set up to accept donations.
 If you still want to donate, we kindly ask you to donate to another open source project/initiative of your choice instead.
```

### Comparing `python-telegram-bot-raw-20.3/README_RAW.rst` & `python-telegram-bot-raw-20.4/README_RAW.rst`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 *Stay tuned for library updates and new releases on our* `Telegram Channel <https://telegram.me/pythontelegrambotchannel>`_.
 
 Introduction
 ============
 
 This library provides a pure Python, asynchronous interface for the
 `Telegram Bot API <https://core.telegram.org/bots/api>`_.
-It's compatible with Python versions **3.7+**.
+It's compatible with Python versions **3.8+**.
 
 ``python-telegram-bot-raw`` is part of the `python-telegram-bot <https://python-telegram-bot.org>`_ ecosystem and provides the pure API functionality extracted from PTB. It therefore does not have independent release schedules, changelogs or documentation.
 
 Note
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
@@ -132,34 +132,34 @@
 
 ``python-telegram-bot`` tries to use as few 3rd party dependencies as possible.
 However, for some features using a 3rd party library is more sane than implementing the functionality again.
 As these features are *optional*, the corresponding 3rd party dependencies are not installed by default.
 Instead, they are listed as optional dependencies.
 This allows to avoid unnecessary dependency conflicts for users who don't need the optional features.
 
-The only required dependency is `httpx ~= 0.23.3 <https://www.python-httpx.org>`_ for
+The only required dependency is `httpx ~= 0.24.1 <https://www.python-httpx.org>`_ for
 ``telegram.request.HTTPXRequest``, the default networking backend.
 
 ``python-telegram-bot`` is most useful when used along with additional libraries.
 To minimize dependency conflicts, we try to be liberal in terms of version requirements on the (optional) dependencies.
 On the other hand, we have to ensure stability of ``python-telegram-bot``, which is why we do apply version bounds.
 If you encounter dependency conflicts due to these bounds, feel free to reach out.
 
 Optional Dependencies
 #####################
 
 PTB can be installed with optional dependencies:
 
-* ``pip install python-telegram-bot-raw[passport]`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
-* ``pip install python-telegram-bot-raw[socks]`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
-* ``pip install python-telegram-bot[http2]`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
+* ``pip install "python-telegram-bot-raw[passport]"`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
+* ``pip install "python-telegram-bot-raw[socks]"`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
+* ``pip install "python-telegram-bot-raw[http2]"`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
 
-To install multiple optional dependencies, separate them by commas, e.g. ``pip install python-telegram-bot-raw[passport,socks]``.
+To install multiple optional dependencies, separate them by commas, e.g. ``pip install "python-telegram-bot-raw[passport,socks]"``.
 
-Additionally, the shortcut ``pip install python-telegram-bot-raw[all]`` installs all optional dependencies.
+Additionally, the shortcut ``pip install "python-telegram-bot-raw[all]"`` installs all optional dependencies.
 
 Quick Start
 ===========
 
 Our Wiki contains an `Introduction to the API <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API>`_ explaining how the pure Bot API can be accessed via ``python-telegram-bot``.
 
 Resources
@@ -191,15 +191,15 @@
 Because ``asyncio`` is in general single-threaded, ``python-telegram-bot`` does currently not aim to be thread-safe.
 
 Contributing
 ============
 
 Contributions of all sizes are welcome.
 Please review our `contribution guidelines <https://github.com/python-telegram-bot/python-telegram-bot/blob/master/.github/CONTRIBUTING.rst>`_ to get started.
-You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new>`_.
+You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new/choose>`_.
 
 Donating
 ========
 Occasionally we are asked if we accept donations to support the development.
 While we appreciate the thought, maintaining PTB is our hobby, and we have almost no running costs for it. We therefore have nothing set up to accept donations.
 If you still want to donate, we kindly ask you to donate to another open source project/initiative of your choice instead.
```

### Comparing `python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/PKG-INFO` & `python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 20.3
+Version: 20.4
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -18,20 +18,19 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: socks
 Provides-Extra: all
 Provides-Extra: http2
 Provides-Extra: passport
 License-File: LICENSE
 License-File: LICENSE.dual
@@ -112,15 +111,15 @@
 *Stay tuned for library updates and new releases on our* `Telegram Channel <https://telegram.me/pythontelegrambotchannel>`_.
 
 Introduction
 ============
 
 This library provides a pure Python, asynchronous interface for the
 `Telegram Bot API <https://core.telegram.org/bots/api>`_.
-It's compatible with Python versions **3.7+**.
+It's compatible with Python versions **3.8+**.
 
 ``python-telegram-bot-raw`` is part of the `python-telegram-bot <https://python-telegram-bot.org>`_ ecosystem and provides the pure API functionality extracted from PTB. It therefore does not have independent release schedules, changelogs or documentation.
 
 Note
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
@@ -171,34 +170,34 @@
 
 ``python-telegram-bot`` tries to use as few 3rd party dependencies as possible.
 However, for some features using a 3rd party library is more sane than implementing the functionality again.
 As these features are *optional*, the corresponding 3rd party dependencies are not installed by default.
 Instead, they are listed as optional dependencies.
 This allows to avoid unnecessary dependency conflicts for users who don't need the optional features.
 
-The only required dependency is `httpx ~= 0.23.3 <https://www.python-httpx.org>`_ for
+The only required dependency is `httpx ~= 0.24.1 <https://www.python-httpx.org>`_ for
 ``telegram.request.HTTPXRequest``, the default networking backend.
 
 ``python-telegram-bot`` is most useful when used along with additional libraries.
 To minimize dependency conflicts, we try to be liberal in terms of version requirements on the (optional) dependencies.
 On the other hand, we have to ensure stability of ``python-telegram-bot``, which is why we do apply version bounds.
 If you encounter dependency conflicts due to these bounds, feel free to reach out.
 
 Optional Dependencies
 #####################
 
 PTB can be installed with optional dependencies:
 
-* ``pip install python-telegram-bot-raw[passport]`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
-* ``pip install python-telegram-bot-raw[socks]`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
-* ``pip install python-telegram-bot[http2]`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
+* ``pip install "python-telegram-bot-raw[passport]"`` installs the `cryptography>=39.0.1 <https://cryptography.io/en/stable>`_ library. Use this, if you want to use Telegram Passport related functionality.
+* ``pip install "python-telegram-bot-raw[socks]"`` installs `httpx[socks] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to work behind a Socks5 server.
+* ``pip install "python-telegram-bot-raw[http2]"`` installs `httpx[http2] <https://www.python-httpx.org/#dependencies>`_. Use this, if you want to use HTTP/2.
 
-To install multiple optional dependencies, separate them by commas, e.g. ``pip install python-telegram-bot-raw[passport,socks]``.
+To install multiple optional dependencies, separate them by commas, e.g. ``pip install "python-telegram-bot-raw[passport,socks]"``.
 
-Additionally, the shortcut ``pip install python-telegram-bot-raw[all]`` installs all optional dependencies.
+Additionally, the shortcut ``pip install "python-telegram-bot-raw[all]"`` installs all optional dependencies.
 
 Quick Start
 ===========
 
 Our Wiki contains an `Introduction to the API <https://github.com/python-telegram-bot/python-telegram-bot/wiki/Introduction-to-the-API>`_ explaining how the pure Bot API can be accessed via ``python-telegram-bot``.
 
 Resources
@@ -230,15 +229,15 @@
 Because ``asyncio`` is in general single-threaded, ``python-telegram-bot`` does currently not aim to be thread-safe.
 
 Contributing
 ============
 
 Contributions of all sizes are welcome.
 Please review our `contribution guidelines <https://github.com/python-telegram-bot/python-telegram-bot/blob/master/.github/CONTRIBUTING.rst>`_ to get started.
-You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new>`_.
+You can also help by `reporting bugs or feature requests <https://github.com/python-telegram-bot/python-telegram-bot/issues/new/choose>`_.
 
 Donating
 ========
 Occasionally we are asked if we accept donations to support the development.
 While we appreciate the thought, maintaining PTB is our hobby, and we have almost no running costs for it. We therefore have nothing set up to accept donations.
 If you still want to donate, we kindly ask you to donate to another open source project/initiative of your choice instead.
```

### Comparing `python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/SOURCES.txt` & `python-telegram-bot-raw-20.4/python_telegram_bot_raw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/requirements-opts.txt` & `python-telegram-bot-raw-20.4/requirements-opts.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 # When dependencies release new versions and tests succeed, we should try to expand the allowed
 # versions and only increase the lower bound if necessary
 
 httpx[socks] # socks
 httpx[http2] # http2
 cryptography!=3.4,!=3.4.1,!=3.4.2,!=3.4.3,>=39.0.1 # passport
-aiolimiter~=1.0.0 # rate-limiter!ext
+aiolimiter~=1.1.0 # rate-limiter!ext
 
 # tornado is rather stable, but let's not allow the next mayor release without prior testing
 tornado~=6.2 # webhooks!ext
 
 # Cachetools and APS don't have a strict stability policy.
 # Let's be cautious for now.
-cachetools~=5.3.0 # callback-data!ext
+cachetools~=5.3.1 # callback-data!ext
 APScheduler~=3.10.1 # job-queue!ext
 
 # pytz is required by APS and just needs the lower bound due to #2120
 pytz>=2018.6 # job-queue!ext
```

### Comparing `python-telegram-bot-raw-20.3/setup.cfg` & `python-telegram-bot-raw-20.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 [mypy]
 warn_unused_ignores = True
 warn_unused_configs = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 disallow_untyped_decorators = True
 show_error_codes = True
-implicit_optional = True
 
 [mypy-telegram._callbackquery,telegram._file,telegram._message,telegram._files.file]
 strict_optional = False
 
 [mypy-telegram.ext._utils.webhookhandler]
 warn_unused_ignores = False
```

### Comparing `python-telegram-bot-raw-20.3/setup.py` & `python-telegram-bot-raw-20.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,21 +101,20 @@
             "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
             "Operating System :: OS Independent",
             "Topic :: Software Development :: Libraries :: Python Modules",
             "Topic :: Communications :: Chat",
             "Topic :: Internet",
             "Programming Language :: Python",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
         ],
-        python_requires=">=3.7",
+        python_requires=">=3.8",
     )
 
     return kwargs
 
 
 def main():
     # If we're building, build ptb-raw as well
```

### Comparing `python-telegram-bot-raw-20.3/telegram/__init__.py` & `python-telegram-bot-raw-20.4/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/__main__.py` & `python-telegram-bot-raw-20.4/telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_bot.py` & `python-telegram-bot-raw-20.4/telegram/_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,22 @@
 from telegram._update import Update
 from telegram._user import User
 from telegram._userprofilephotos import UserProfilePhotos
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE, DefaultValue
 from telegram._utils.files import is_local_file, parse_file_input
 from telegram._utils.logging import get_logger
-from telegram._utils.types import DVInput, FileInput, JSONDict, ODVInput, ReplyMarkup
+from telegram._utils.types import (
+    CorrectOptionID,
+    DVInput,
+    FileInput,
+    JSONDict,
+    ODVInput,
+    ReplyMarkup,
+)
 from telegram._utils.warnings import warn
 from telegram._utils.warnings_transition import warn_about_thumb_return_thumbnail
 from telegram._webhookinfo import WebhookInfo
 from telegram.constants import InlineQueryLimit
 from telegram.error import InvalidToken
 from telegram.request import BaseRequest, RequestData
 from telegram.request._httpxrequest import HTTPXRequest
@@ -224,18 +231,18 @@
     )
 
     def __init__(
         self,
         token: str,
         base_url: str = "https://api.telegram.org/bot",
         base_file_url: str = "https://api.telegram.org/file/bot",
-        request: BaseRequest = None,
-        get_updates_request: BaseRequest = None,
-        private_key: bytes = None,
-        private_key_password: bytes = None,
+        request: Optional[BaseRequest] = None,
+        get_updates_request: Optional[BaseRequest] = None,
+        private_key: Optional[bytes] = None,
+        private_key_password: Optional[bytes] = None,
         local_mode: bool = False,
     ):
         super().__init__(api_kwargs=None)
         if not token:
             raise InvalidToken("You must pass the token you received from https://t.me/Botfather!")
         self._token: str = token
 
@@ -283,15 +290,15 @@
                 stacklevel=2,
             )
 
         if private_key:
             if not CRYPTO_INSTALLED:
                 raise RuntimeError(
                     "To use Telegram Passports, PTB must be installed via `pip install "
-                    "python-telegram-bot[passport]`."
+                    '"python-telegram-bot[passport]"`.'
                 )
             self._private_key = serialization.load_pem_private_key(
                 private_key, password=private_key_password, backend=default_backend()
             )
 
         self._freeze()
 
@@ -384,16 +391,16 @@
             return result
 
         return decorator
 
     def _parse_file_input(
         self,
         file_input: Union[FileInput, "TelegramObject"],
-        tg_type: Type["TelegramObject"] = None,
-        filename: str = None,
+        tg_type: Optional[Type["TelegramObject"]] = None,
+        filename: Optional[str] = None,
         attach: bool = False,
     ) -> Union[str, "InputFile", Any]:
         return parse_file_input(
             file_input=file_input,
             tg_type=tg_type,
             filename=filename,
             attach=attach,
@@ -439,21 +446,21 @@
             # 2)
             else:
                 data[key] = DefaultValue.get_value(val)
 
     async def _post(
         self,
         endpoint: str,
-        data: JSONDict = None,
+        data: Optional[JSONDict] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Any:
         # We know that the return type is Union[bool, JSONDict, List[JSONDict]], but it's hard
         # to tell mypy which methods expects which of these return values and `Any` saves us a
         # lot of `type: ignore` comments
         if data is None:
             data = {}
 
@@ -503,30 +510,30 @@
             pool_timeout=pool_timeout,
         )
 
     async def _send_message(
         self,
         endpoint: str,
         data: JSONDict,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        caption: str = None,
+        message_thread_id: Optional[int] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Any:
         """Protected method to send or edit messages of any type.
 
         It is here to reduce repetition of if-else closes in the different bot methods,
         i.e. this method takes care of adding its parameters to `data` if appropriate.
 
         Depending on the bot method, returns either `True` or the message.
@@ -717,15 +724,15 @@
     async def get_me(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> User:
         """A simple method for testing your bot's auth token. Requires no parameters.
 
         Returns:
             :class:`telegram.User`: A :class:`telegram.User` instance representing that bot if the
             credentials are valid, :obj:`None` otherwise.
 
@@ -746,28 +753,28 @@
 
     @_log
     async def send_message(
         self,
         chat_id: Union[int, str],
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
-        message_thread_id: int = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send text messages.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             text (:obj:`str`): Text of the message to be sent. Max
                 :tg-const:`telegram.constants.MessageLimit.MAX_TEXT_LENGTH` characters after
@@ -828,15 +835,15 @@
         chat_id: Union[str, int],
         message_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to delete a message, including service messages, with the following
         limitations:
 
         - A message can only be deleted if it was sent less than 48 hours ago.
         - Service messages about a supergroup, channel, or forum topic creation can't be deleted.
@@ -885,21 +892,21 @@
     async def forward_message(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_id: int,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to forward messages of any kind. Service messages can't be forwarded.
 
         Note:
             Since the release of Bot API 5.5 it can be impossible to forward messages from
             some chats. Use the attributes :attr:`telegram.Message.has_protected_content` and
@@ -948,31 +955,31 @@
         )
 
     @_log
     async def send_photo(
         self,
         chat_id: Union[int, str],
         photo: Union[FileInput, "PhotoSize"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send photos.
 
         .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
@@ -1059,35 +1066,35 @@
         )
 
     @_log
     async def send_audio(
         self,
         chat_id: Union[int, str],
         audio: Union[FileInput, "Audio"],
-        duration: int = None,
-        performer: str = None,
-        title: str = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        performer: Optional[str] = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send audio files, if you want Telegram clients to display them in the
         music player. Your audio must be in the ``.mp3`` or ``.m4a`` format.
 
         Bots can currently send audio files of up to
         :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD` in size, this limit may be
@@ -1204,33 +1211,33 @@
         )
 
     @_log
     async def send_document(
         self,
         chat_id: Union[int, str],
         document: Union[FileInput, "Document"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
-        disable_content_type_detection: bool = None,
+        thumb: Optional[FileInput] = None,
+        disable_content_type_detection: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send general files.
 
         Bots can currently send files of any type of up to
         :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD` in size, this limit may be
         changed in the future.
@@ -1344,26 +1351,26 @@
 
     @_log
     async def send_sticker(
         self,
         chat_id: Union[int, str],
         sticker: Union[FileInput, "Sticker"],
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        emoji: str = None,
+        message_thread_id: Optional[int] = None,
+        emoji: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send static ``.WEBP``, animated ``.TGS``, or video ``.WEBM`` stickers.
 
         .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
         Args:
@@ -1429,37 +1436,37 @@
         )
 
     @_log
     async def send_video(
         self,
         chat_id: Union[int, str],
         video: Union[FileInput, "Video"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        width: int = None,
-        height: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        supports_streaming: bool = None,
-        thumb: FileInput = None,
+        supports_streaming: Optional[bool] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send video files, Telegram clients support mp4 videos
         (other formats may be sent as Document).
 
         Bots can currently send video files of up to
         :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD` in size, this limit may be
         changed in the future.
@@ -1586,31 +1593,31 @@
         )
 
     @_log
     async def send_video_note(
         self,
         chat_id: Union[int, str],
         video_note: Union[FileInput, "VideoNote"],
-        duration: int = None,
-        length: int = None,
+        duration: Optional[int] = None,
+        length: Optional[int] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        thumb: FileInput = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         As of v.4.0, Telegram clients support rounded square mp4 videos of up to 1 minute long.
         Use this method to send video messages.
 
         Note:
             :paramref:`thumb` will be ignored for small video files, for which Telegram can
@@ -1716,36 +1723,36 @@
         )
 
     @_log
     async def send_animation(
         self,
         chat_id: Union[int, str],
         animation: Union[FileInput, "Animation"],
-        duration: int = None,
-        width: int = None,
-        height: int = None,
-        thumb: FileInput = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send animation files (GIF or H.264/MPEG-4 AVC video without sound).
         Bots can currently send animation files of up to
         :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD` in size, this limit may be
         changed in the future.
 
@@ -1865,31 +1872,31 @@
         )
 
     @_log
     async def send_voice(
         self,
         chat_id: Union[int, str],
         voice: Union[FileInput, "Voice"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send audio files, if you want Telegram clients to display the file
         as a playable voice message. For this to work, your audio must be in an ``.ogg`` file
         encoded with OPUS (other formats may be sent as Audio or Document). Bots can currently
         send voice messages of up to :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_UPLOAD`
         in size, this limit may be changed in the future.
@@ -1984,27 +1991,27 @@
     async def send_media_group(
         self,
         chat_id: Union[int, str],
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
     ) -> Tuple[Message, ...]:
         """Use this method to send a group of photos, videos, documents or audios as an album.
         Documents and audio files can be only grouped in an album with messages of the same type.
 
         Note:
             If you supply a :paramref:`caption` (along with either :paramref:`parse_mode` or
             :paramref:`caption_entities`), then items in :paramref:`media` must have no captions,
@@ -2109,33 +2116,33 @@
 
         return Message.de_list(result, self)
 
     @_log
     async def send_location(
         self,
         chat_id: Union[int, str],
-        latitude: float = None,
-        longitude: float = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        live_period: int = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        live_period: Optional[int] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        location: Location = None,
+        location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send point on the map.
 
         Note:
             You can either supply a :paramref:`latitude` and :paramref:`longitude` or a
             :paramref:`location`.
 
@@ -2223,30 +2230,30 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def edit_message_live_location(
         self,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
-        latitude: float = None,
-        longitude: float = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         *,
-        location: Location = None,
+        location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Use this method to edit live location messages sent by the bot or via the bot
         (for inline bots). A location can be edited until its :attr:`telegram.Location.live_period`
         expires or editing is explicitly disabled by a call to :meth:`stop_message_live_location`.
 
         Note:
             You can either supply a :paramref:`latitude` and :paramref:`longitude` or a
@@ -2318,24 +2325,24 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def stop_message_live_location(
         self,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Use this method to stop updating a live location message sent by the bot or via the bot
         (for inline bots) before :paramref:`~telegram.Location.live_period` expires.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`, optional): Required if :paramref:`inline_message_id`
                 is not specified. |chat_id_channel|
@@ -2367,35 +2374,35 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def send_venue(
         self,
         chat_id: Union[int, str],
-        latitude: float = None,
-        longitude: float = None,
-        title: str = None,
-        address: str = None,
-        foursquare_id: str = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        title: Optional[str] = None,
+        address: Optional[str] = None,
+        foursquare_id: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        venue: Venue = None,
+        venue: Optional[Venue] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send information about a venue.
 
         Note:
             * You can either supply :paramref:`venue`, or :paramref:`latitude`,
               :paramref:`longitude`, :paramref:`title` and :paramref:`address` and optionally
               :paramref:`foursquare_id` and :paramref:`foursquare_type` or optionally
@@ -2493,31 +2500,31 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def send_contact(
         self,
         chat_id: Union[int, str],
-        phone_number: str = None,
-        first_name: str = None,
-        last_name: str = None,
+        phone_number: Optional[str] = None,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        vcard: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        vcard: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        contact: Contact = None,
+        contact: Optional[Contact] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send phone contacts.
 
         Note:
             You can either supply :paramref:`contact` or :paramref:`phone_number` and
             :paramref:`first_name` with optionally :paramref:`last_name` and optionally
             :paramref:`vcard`.
@@ -2598,25 +2605,25 @@
 
     @_log
     async def send_game(
         self,
         chat_id: Union[int, str],
         game_short_name: str,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send a game.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): Unique identifier for the target chat.
             game_short_name (:obj:`str`): Short name of the game, serves as the unique identifier
                 for the game. Set up your games via `@BotFather <https://t.me/BotFather>`_.
@@ -2660,21 +2667,21 @@
         )
 
     @_log
     async def send_chat_action(
         self,
         chat_id: Union[str, int],
         action: str,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method when you need to tell the user that something is happening on the bot's
         side. The status is set for 5 seconds or less (when a message arrives from your bot,
         Telegram clients clear its typing status). Telegram only recommends using this method when
         a response from the bot will take a noticeable amount of time to arrive.
 
@@ -2710,16 +2717,16 @@
         )
 
     def _effective_inline_results(  # skipcq: PYL-R0201
         self,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
-        next_offset: str = None,
-        current_offset: str = None,
+        next_offset: Optional[str] = None,
+        current_offset: Optional[str] = None,
     ) -> Tuple[Sequence["InlineQueryResult"], Optional[str]]:
         """
         Builds the effective results from the results input.
         We make this a stand-alone method so tg.ext.ExtBot can wrap it.
 
         Returns:
             Tuple of 1. the effective results and 2. correct the next_offset
@@ -2806,33 +2813,33 @@
     @_log
     async def answer_inline_query(
         self,
         inline_query_id: str,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
-        cache_time: int = None,
-        is_personal: bool = None,
-        next_offset: str = None,
+        cache_time: Optional[int] = None,
+        is_personal: Optional[bool] = None,
+        next_offset: Optional[str] = None,
         # Deprecated params since bot api 6.7
         # <----
-        switch_pm_text: str = None,
-        switch_pm_parameter: str = None,
+        switch_pm_text: Optional[str] = None,
+        switch_pm_parameter: Optional[str] = None,
         # --->
         # New params since bot api 6.7
         # <----
-        button: InlineQueryResultsButton = None,
+        button: Optional[InlineQueryResultsButton] = None,
         # --->
         *,
-        current_offset: str = None,
+        current_offset: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to send answers to an inline query. No more than
         :tg-const:`telegram.InlineQuery.MAX_RESULTS` results per query are allowed.
 
         Warning:
             In most use cases :paramref:`current_offset` should not be passed manually. Instead of
@@ -2942,22 +2949,22 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_user_profile_photos(
         self,
         user_id: Union[str, int],
-        offset: int = None,
-        limit: int = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> UserProfilePhotos:
         """Use this method to get a list of profile pictures for a user.
 
         Args:
             user_id (:obj:`int`): Unique identifier of the target user.
             offset (:obj:`int`, optional): Sequential number of the first photo to be returned.
                 By default, all photos are returned.
@@ -2994,15 +3001,15 @@
             str, Animation, Audio, ChatPhoto, Document, PhotoSize, Sticker, Video, VideoNote, Voice
         ],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> File:
         """
         Use this method to get basic info about a file and prepare it for downloading. For the
         moment, bots can download files of up to
         :tg-const:`telegram.constants.FileSizeLimit.FILESIZE_DOWNLOAD` in size. The file can then
         be e.g. downloaded with :meth:`telegram.File.download_to_drive`. It is guaranteed that
         the link will be valid for at least 1 hour. When the link expires, a new one can be
@@ -3054,22 +3061,22 @@
         return File.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def ban_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
-        until_date: Union[int, datetime] = None,
-        revoke_messages: bool = None,
+        until_date: Optional[Union[int, datetime]] = None,
+        revoke_messages: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to ban a user from a group, supergroup or a channel. In the case of
         supergroups and channels, the user will not be able to return to the group on their own
         using invite links, etc., unless unbanned first. The bot must be an administrator in the
         chat for this to work and must have the appropriate admin rights.
 
@@ -3123,15 +3130,15 @@
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to ban a channel chat in a supergroup or a channel. Until the chat is
         unbanned, the owner of the banned chat won't be able to send messages on behalf of **any of
         their channels**. The bot must be an administrator in the supergroup or channel for this
         to work and must have the appropriate administrator rights.
 
@@ -3162,21 +3169,21 @@
         )
 
     @_log
     async def unban_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
-        only_if_banned: bool = None,
+        only_if_banned: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to unban a previously kicked user in a supergroup or channel.
 
         The user will *not* return to the group or channel automatically, but will be able to join
         via link, etc. The bot must be an administrator for this to work. By default, this method
         guarantees that after the call the user is not a member of the chat, but will be able to
         join it. So if the user is a member of the chat they will also be *removed* from the chat.
@@ -3212,15 +3219,15 @@
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to unban a previously banned channel in a supergroup or channel.
         The bot must be an administrator for this to work and must have the
         appropriate administrator rights.
 
         .. versionadded:: 13.9
 
@@ -3247,24 +3254,24 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def answer_callback_query(
         self,
         callback_query_id: str,
-        text: str = None,
-        show_alert: bool = None,
-        url: str = None,
-        cache_time: int = None,
+        text: Optional[str] = None,
+        show_alert: Optional[bool] = None,
+        url: Optional[str] = None,
+        cache_time: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to send answers to callback queries sent from inline keyboards. The answer
         will be displayed to the user as a notification at the top of the chat screen or as an
         alert.
         Alternatively, the user can be redirected to the specified Game URL. For this option to
         work, you must first create a game for your bot via `@BotFather <https://t.me/BotFather>`_
@@ -3313,27 +3320,27 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def edit_message_text(
         self,
         text: str,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
-        reply_markup: InlineKeyboardMarkup = None,
-        entities: Sequence["MessageEntity"] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """
         Use this method to edit text and game messages.
 
         Note:
             |editreplymarkup|.
 
@@ -3390,27 +3397,27 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def edit_message_caption(
         self,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """
         Use this method to edit captions of messages.
 
         Note:
             |editreplymarkup|
 
@@ -3461,24 +3468,24 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def edit_message_media(
         self,
         media: "InputMedia",
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """
         Use this method to edit animation, audio, document, photo, or video messages. If a message
         is part of a message album, then it can be edited only to an audio for audio albums, only
         to a document for document albums and to a photo or a video otherwise. When an inline
         message is edited, a new file can't be uploaded; use a previously uploaded file via its
         :attr:`~telegram.File.file_id` or specify a URL.
@@ -3524,24 +3531,24 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def edit_message_reply_markup(
         self,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """
         Use this method to edit only the reply markup of messages sent by the bot or via the bot
         (for inline bots).
 
         Note:
             |editreplymarkup|
@@ -3580,24 +3587,24 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_updates(
         self,
-        offset: int = None,
-        limit: int = None,
-        timeout: float = None,
-        allowed_updates: Sequence[str] = None,
+        offset: Optional[int] = None,
+        limit: Optional[int] = None,
+        timeout: Optional[int] = None,
+        allowed_updates: Optional[Sequence[str]] = None,
         *,
         read_timeout: float = 2,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[Update, ...]:
         """Use this method to receive incoming updates using long polling.
 
         Note:
             1. This method will not work if an outgoing webhook is set up.
             2. In order to avoid getting duplicate updates, recalculate offset after each
                server response.
@@ -3676,26 +3683,26 @@
 
         return Update.de_list(result, self)
 
     @_log
     async def set_webhook(
         self,
         url: str,
-        certificate: FileInput = None,
-        max_connections: int = None,
-        allowed_updates: Sequence[str] = None,
-        ip_address: str = None,
-        drop_pending_updates: bool = None,
-        secret_token: str = None,
+        certificate: Optional[FileInput] = None,
+        max_connections: Optional[int] = None,
+        allowed_updates: Optional[Sequence[str]] = None,
+        ip_address: Optional[str] = None,
+        drop_pending_updates: Optional[bool] = None,
+        secret_token: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to specify a url and receive incoming updates via an outgoing webhook.
         Whenever there is an update for the bot, Telegram will send an HTTPS POST request to the
         specified url, containing An Update. In case of an unsuccessful request,
         Telegram will give up after a reasonable amount of attempts.
 
@@ -3800,21 +3807,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def delete_webhook(
         self,
-        drop_pending_updates: bool = None,
+        drop_pending_updates: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to remove webhook integration if you decide to switch back to
         :meth:`get_updates()`.
 
         Args:
             drop_pending_updates (:obj:`bool`, optional): Pass :obj:`True` to drop all pending
@@ -3844,15 +3851,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method for your bot to leave a group, supergroup or channel.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
 
         Returns:
@@ -3879,15 +3886,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Chat:
         """
         Use this method to get up to date information about the chat (current name of the user for
         one-on-one conversations, current username of a user, group or channel, etc.).
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
@@ -3918,15 +3925,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[ChatMember, ...]:
         """
         Use this method to get a list of administrators in a chat.
 
         .. versionchanged:: 20.0
             Returns a tuple instead of a list.
 
@@ -3960,15 +3967,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> int:
         """Use this method to get the number of members in a chat.
 
         .. versionadded:: 13.7
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
@@ -3997,15 +4004,15 @@
         chat_id: Union[str, int],
         user_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ChatMember:
         """Use this method to get information about a member of a chat. The method is only
         guaranteed to work for other users if the bot is an administrator in the chat.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             user_id (:obj:`int`): Unique identifier of the target user.
@@ -4035,15 +4042,15 @@
         chat_id: Union[str, int],
         sticker_set_name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to set a new group sticker set for a supergroup.
         The bot must be an administrator in the chat for this to work and must have the appropriate
         admin rights. Use the field :attr:`telegram.Chat.can_set_sticker_set` optionally returned
         in :meth:`get_chat` requests to check if the bot can use this method.
 
         Args:
@@ -4070,15 +4077,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to delete a group sticker set from a supergroup. The bot must be an
         administrator in the chat for this to work and must have the appropriate admin rights.
         Use the field :attr:`telegram.Chat.can_set_sticker_set` optionally returned in
         :meth:`get_chat` requests to check if the bot can use this method.
 
         Args:
@@ -4102,15 +4109,15 @@
     async def get_webhook_info(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> WebhookInfo:
         """Use this method to get current webhook status. Requires no parameters.
 
         If the bot is using :meth:`get_updates`, will return an object with the
         :attr:`telegram.WebhookInfo.url` field empty.
 
         Returns:
@@ -4128,25 +4135,25 @@
         return WebhookInfo.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def set_game_score(
         self,
         user_id: Union[int, str],
         score: int,
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
-        force: bool = None,
-        disable_edit_message: bool = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
+        force: Optional[bool] = None,
+        disable_edit_message: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """
         Use this method to set the score of the specified user in a game message.
 
         .. seealso:: :attr:`telegram.Game.text`
 
         Args:
@@ -4192,23 +4199,23 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_game_high_scores(
         self,
         user_id: Union[int, str],
-        chat_id: Union[str, int] = None,
-        message_id: int = None,
-        inline_message_id: str = None,
+        chat_id: Optional[Union[str, int]] = None,
+        message_id: Optional[int] = None,
+        inline_message_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[GameHighScore, ...]:
         """
         Use this method to get data for high score tables. Will return the score of the specified
         user and several of their neighbors in a game.
 
         Note:
             This method will currently return scores for the target user, plus two of their
@@ -4259,41 +4266,41 @@
         chat_id: Union[int, str],
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: Sequence["LabeledPrice"],
-        start_parameter: str = None,
-        photo_url: str = None,
-        photo_size: int = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        need_name: bool = None,
-        need_phone_number: bool = None,
-        need_email: bool = None,
-        need_shipping_address: bool = None,
-        is_flexible: bool = None,
+        start_parameter: Optional[str] = None,
+        photo_url: Optional[str] = None,
+        photo_size: Optional[int] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        need_name: Optional[bool] = None,
+        need_phone_number: Optional[bool] = None,
+        need_email: Optional[bool] = None,
+        need_shipping_address: Optional[bool] = None,
+        is_flexible: Optional[bool] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        provider_data: Union[str, object] = None,
-        send_phone_number_to_provider: bool = None,
-        send_email_to_provider: bool = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        provider_data: Optional[Union[str, object]] = None,
+        send_phone_number_to_provider: Optional[bool] = None,
+        send_email_to_provider: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        max_tip_amount: int = None,
-        suggested_tip_amounts: Sequence[int] = None,
+        max_tip_amount: Optional[int] = None,
+        suggested_tip_amounts: Optional[Sequence[int]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """Use this method to send invoices.
 
         Warning:
             As of API 5.2 :paramref:`start_parameter` is an optional argument and therefore the
             order of the arguments had to be changed. Use keyword arguments to make sure that the
             arguments are passed correctly.
@@ -4436,22 +4443,22 @@
         )
 
     @_log
     async def answer_shipping_query(  # pylint: disable=invalid-name
         self,
         shipping_query_id: str,
         ok: bool,
-        shipping_options: Sequence[ShippingOption] = None,
-        error_message: str = None,
+        shipping_options: Optional[Sequence[ShippingOption]] = None,
+        error_message: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         If you sent an invoice requesting a shipping address and the parameter
         :paramref:`send_invoice.is_flexible` was specified, the Bot API will send an
         :class:`telegram.Update` with a :attr:`telegram.Update.shipping_query` field to the bot.
         Use this method to reply to shipping queries.
 
@@ -4495,21 +4502,21 @@
         )
 
     @_log
     async def answer_pre_checkout_query(  # pylint: disable=invalid-name
         self,
         pre_checkout_query_id: str,
         ok: bool,
-        error_message: str = None,
+        error_message: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Once the user has confirmed their payment and shipping details, the Bot API sends the final
         confirmation in the form of an :class:`telegram.Update` with the field
         :attr:`telegram.Update.pre_checkout_query`. Use this method to respond to such pre-checkout
         queries.
 
@@ -4557,15 +4564,15 @@
         web_app_query_id: str,
         result: "InlineQueryResult",
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> SentWebAppMessage:
         """Use this method to set the result of an interaction with a Web App and send a
         corresponding message on behalf of the user to the chat from which the query originated.
 
         .. versionadded:: 20.0
 
         Args:
@@ -4600,22 +4607,22 @@
 
     @_log
     async def restrict_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
         permissions: ChatPermissions,
-        until_date: Union[int, datetime] = None,
-        use_independent_chat_permissions: bool = None,
+        until_date: Optional[Union[int, datetime]] = None,
+        use_independent_chat_permissions: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to restrict a user in a supergroup. The bot must be an administrator in
         the supergroup for this to work and must have the appropriate admin rights. Pass
         :obj:`True` for all boolean parameters to lift restrictions from a user.
 
         .. seealso:: :meth:`telegram.ChatPermissions.all_permissions`
@@ -4673,32 +4680,32 @@
         )
 
     @_log
     async def promote_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
-        can_change_info: bool = None,
-        can_post_messages: bool = None,
-        can_edit_messages: bool = None,
-        can_delete_messages: bool = None,
-        can_invite_users: bool = None,
-        can_restrict_members: bool = None,
-        can_pin_messages: bool = None,
-        can_promote_members: bool = None,
-        is_anonymous: bool = None,
-        can_manage_chat: bool = None,
-        can_manage_video_chats: bool = None,
-        can_manage_topics: bool = None,
+        can_change_info: Optional[bool] = None,
+        can_post_messages: Optional[bool] = None,
+        can_edit_messages: Optional[bool] = None,
+        can_delete_messages: Optional[bool] = None,
+        can_invite_users: Optional[bool] = None,
+        can_restrict_members: Optional[bool] = None,
+        can_pin_messages: Optional[bool] = None,
+        can_promote_members: Optional[bool] = None,
+        is_anonymous: Optional[bool] = None,
+        can_manage_chat: Optional[bool] = None,
+        can_manage_video_chats: Optional[bool] = None,
+        can_manage_topics: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to promote or demote a user in a supergroup or a channel. The bot must be
         an administrator in the chat for this to work and must have the appropriate admin rights.
         Pass :obj:`False` for all boolean parameters to demote a user.
 
         .. versionchanged:: 20.0
@@ -4780,21 +4787,21 @@
         )
 
     @_log
     async def set_chat_permissions(
         self,
         chat_id: Union[str, int],
         permissions: ChatPermissions,
-        use_independent_chat_permissions: bool = None,
+        use_independent_chat_permissions: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to set default chat permissions for all members. The bot must be an
         administrator in the group or a supergroup for this to work and must have the
         :attr:`telegram.ChatMemberAdministrator.can_restrict_members` admin rights.
 
         Args:
@@ -4845,15 +4852,15 @@
         user_id: Union[int, str],
         custom_title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to set a custom title for administrators promoted by the bot in a
         supergroup. The bot must be an administrator for this to work.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_group|
@@ -4886,15 +4893,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> str:
         """
         Use this method to generate a new primary invite link for a chat; any previously generated
         link is revoked. The bot must be an administrator in the chat for this to work and must
         have the appropriate admin rights.
 
         Note:
@@ -4925,30 +4932,38 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def create_chat_invite_link(
         self,
         chat_id: Union[str, int],
-        expire_date: Union[int, datetime] = None,
-        member_limit: int = None,
-        name: str = None,
-        creates_join_request: bool = None,
+        expire_date: Optional[Union[int, datetime]] = None,
+        member_limit: Optional[int] = None,
+        name: Optional[str] = None,
+        creates_join_request: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ChatInviteLink:
         """
         Use this method to create an additional invite link for a chat. The bot must be an
         administrator in the chat for this to work and must have the appropriate admin rights.
         The link can be revoked using the method :meth:`revoke_chat_invite_link`.
 
+        Note:
+            When joining *public* groups via an invite link, Telegram clients may display the
+            usual "Join" button, effectively ignoring the invite link. In particular, the parameter
+            :paramref:`creates_join_request` has no effect in this case.
+            However, this behavior is undocument and may be subject to change.
+            See `this GitHub thread <https://github.com/tdlib/telegram-bot-api/issues/429>`_
+            for some discussion.
+
         .. versionadded:: 13.4
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             expire_date (:obj:`int` | :obj:`datetime.datetime`, optional): Date when the link will
                 expire. Integer input will be interpreted as Unix timestamp.
                 For timezone naive :obj:`datetime.datetime` objects, the default timezone of the
@@ -4996,24 +5011,24 @@
         return ChatInviteLink.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def edit_chat_invite_link(
         self,
         chat_id: Union[str, int],
         invite_link: Union[str, "ChatInviteLink"],
-        expire_date: Union[int, datetime] = None,
-        member_limit: int = None,
-        name: str = None,
-        creates_join_request: bool = None,
+        expire_date: Optional[Union[int, datetime]] = None,
+        member_limit: Optional[int] = None,
+        name: Optional[str] = None,
+        creates_join_request: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ChatInviteLink:
         """
         Use this method to edit a non-primary invite link created by the bot. The bot must be an
         administrator in the chat for this to work and must have the appropriate admin rights.
 
         Note:
             Though not stated explicitly in the official docs, Telegram changes not only the
@@ -5083,15 +5098,15 @@
         chat_id: Union[str, int],
         invite_link: Union[str, "ChatInviteLink"],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ChatInviteLink:
         """
         Use this method to revoke an invite link created by the bot. If the primary link is
         revoked, a new link is automatically generated. The bot must be an administrator in the
         chat for this to work and must have the appropriate admin rights.
 
         .. versionadded:: 13.4
@@ -5131,15 +5146,15 @@
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to approve a chat join request.
 
         The bot must be an administrator in the chat for this to work and must have the
         :attr:`telegram.ChatPermissions.can_invite_users` administrator right.
 
         .. versionadded:: 13.8
@@ -5172,15 +5187,15 @@
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to decline a chat join request.
 
         The bot must be an administrator in the chat for this to work and must have the
         :attr:`telegram.ChatPermissions.can_invite_users` administrator right.
 
         .. versionadded:: 13.8
@@ -5213,15 +5228,15 @@
         chat_id: Union[str, int],
         photo: FileInput,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to set a new profile photo for the chat.
 
         Photos can't be changed for private chats. The bot must be an administrator in the chat
         for this to work and must have the appropriate admin rights.
 
         Args:
@@ -5259,15 +5274,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to delete a chat photo. Photos can't be changed for private chats. The bot
         must be an administrator in the chat for this to work and must have the appropriate admin
         rights.
 
         Args:
@@ -5297,15 +5312,15 @@
         chat_id: Union[str, int],
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the title of a chat. Titles can't be changed for private chats.
         The bot must be an administrator in the chat for this to work and must have the appropriate
         admin rights.
 
         Args:
@@ -5332,21 +5347,21 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_chat_description(
         self,
         chat_id: Union[str, int],
-        description: str = None,
+        description: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the description of a group, a supergroup or a channel. The bot
         must be an administrator in the chat for this to work and must have the appropriate admin
         rights.
 
         Args:
@@ -5381,15 +5396,15 @@
         message_id: int,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to add a message to the list of pinned messages in a chat. If the
         chat is not a private chat, the bot must be an administrator in the chat for this to work
         and must have the :paramref:`~telegram.ChatAdministratorRights.can_pin_messages` admin
         right in a supergroup or :attr:`~telegram.ChatMemberAdministrator.can_edit_messages` admin
         right in a channel.
@@ -5424,21 +5439,21 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def unpin_chat_message(
         self,
         chat_id: Union[str, int],
-        message_id: int = None,
+        message_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to remove a message from the list of pinned messages in a chat. If the
         chat is not a private chat, the bot must be an administrator in the chat for this to work
         and must have the :paramref:`~telegram.ChatAdministratorRights.can_pin_messages` admin
         right in a supergroup or :attr:`~telegram.ChatMemberAdministrator.can_edit_messages` admin
         right in a channel.
@@ -5472,15 +5487,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to clear the list of pinned messages in a chat. If the
         chat is not a private chat, the bot must be an administrator in the chat for this
         to work and must have the :paramref:`~telegram.ChatAdministratorRights.can_pin_messages`
         admin right in a supergroup or :attr:`~telegram.ChatMemberAdministrator.can_edit_messages`
         admin right in a channel.
@@ -5511,15 +5526,15 @@
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> StickerSet:
         """Use this method to get a sticker set.
 
         Args:
             name (:obj:`str`): Name of the sticker set.
 
         Returns:
@@ -5546,15 +5561,15 @@
         self,
         custom_emoji_ids: Sequence[str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[Sticker, ...]:
         # skipcq: FLK-D207
         """
         Use this method to get information about emoji stickers by their identifiers.
 
         .. versionchanged:: 20.0
             Returns a tuple instead of a list.
@@ -5586,26 +5601,28 @@
         )
         return Sticker.de_list(result, self)
 
     @_log
     async def upload_sticker_file(
         self,
         user_id: Union[str, int],
-        png_sticker: FileInput = None,  # Deprecated since bot api 6.6. Optional for compatiblity.
+        png_sticker: Optional[
+            FileInput
+        ] = None,  # Deprecated since bot api 6.6. Optional for compatiblity.
         # New parameters since bot api 6.6:
         # <---
-        sticker: FileInput = None,  # Actually required, but optional for compatibility.
-        sticker_format: str = None,  # Actually required, but optional for compatibility.
+        sticker: Optional[FileInput] = None,  # Actually required, but optional for compatibility.
+        sticker_format: Optional[str] = None,  # Actually required, but optional for compatibility.
         # --->
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> File:
         """
         Use this method to upload a file with a sticker for later use in the
         :meth:`create_new_sticker_set` and :meth:`add_sticker_to_set` methods (can be used multiple
         times).
 
         Args:
@@ -5699,33 +5716,35 @@
     async def create_new_sticker_set(
         self,
         user_id: Union[str, int],
         name: str,
         title: str,
         # Deprecated params since bot api 6.6
         # <----
-        emojis: str = None,  # Was made optional for compatibility purposes
-        png_sticker: FileInput = None,
-        mask_position: MaskPosition = None,
-        tgs_sticker: FileInput = None,
-        webm_sticker: FileInput = None,
+        emojis: Optional[str] = None,  # Was made optional for compatibility purposes
+        png_sticker: Optional[FileInput] = None,
+        mask_position: Optional[MaskPosition] = None,
+        tgs_sticker: Optional[FileInput] = None,
+        webm_sticker: Optional[FileInput] = None,
         # ---->
-        sticker_type: str = None,
+        sticker_type: Optional[str] = None,
         # New params since bot api 6.6
         # <----
-        stickers: Sequence[InputSticker] = None,  # Actually a required param. Optional for compat.
-        sticker_format: str = None,  # Actually a required param. Optional for compat.
-        needs_repainting: bool = None,
+        stickers: Optional[
+            Sequence[InputSticker]
+        ] = None,  # Actually a required param. Optional for compat.
+        sticker_format: Optional[str] = None,  # Actually a required param. Optional for compat.
+        needs_repainting: Optional[bool] = None,
         # ---->
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to create new sticker set owned by a user.
         The bot will be able to edit the created sticker set thus created.
 
         .. versionchanged:: 20.0
             The parameter ``contains_masks`` has been removed. Use :paramref:`sticker_type`
@@ -5906,28 +5925,30 @@
     @_log
     async def add_sticker_to_set(
         self,
         user_id: Union[str, int],
         name: str,
         # Deprecated params since bot api 6.6
         # ----
-        emojis: str = None,  # Was made optional for compatibility reasons
-        png_sticker: FileInput = None,
-        mask_position: MaskPosition = None,
-        tgs_sticker: FileInput = None,
-        webm_sticker: FileInput = None,
+        emojis: Optional[str] = None,  # Was made optional for compatibility reasons
+        png_sticker: Optional[FileInput] = None,
+        mask_position: Optional[MaskPosition] = None,
+        tgs_sticker: Optional[FileInput] = None,
+        webm_sticker: Optional[FileInput] = None,
         # ----
         # New in bot api 6.6:
-        sticker: InputSticker = None,  # Actually a required param, but is optional for compat.
+        sticker: Optional[
+            InputSticker
+        ] = None,  # Actually a required param, but is optional for compat.
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to add a new sticker to a set created by the bot. The format of the added
         sticker must match the format of the other stickers in the set. Emoji sticker sets can have
         up to :tg-const:`telegram.constants.StickerSetLimit.MAX_EMOJI_STICKERS` stickers. Animated
         and video sticker sets can have up to
         :tg-const:`telegram.constants.StickerSetLimit.MAX_ANIMATED_STICKERS` stickers. Static
@@ -6077,15 +6098,15 @@
         sticker: str,
         position: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to move a sticker in a set created by the bot to a specific position.
 
         Args:
             sticker (:obj:`str`): File identifier of the sticker.
             position (:obj:`int`): New sticker position in the set, zero-based.
 
@@ -6112,15 +6133,15 @@
         self,
         sticker: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to delete a sticker from a set created by the bot.
 
         Args:
             sticker (:obj:`str`): File identifier of the sticker.
 
         Returns:
@@ -6146,15 +6167,15 @@
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to delete a sticker set that was created by the bot.
 
         .. versionadded:: 20.2
 
         Args:
@@ -6179,21 +6200,21 @@
         )
 
     @_log
     async def set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: Union[str, int],
-        thumbnail: FileInput = None,
+        thumbnail: Optional[FileInput] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to set the thumbnail of a regular or mask sticker set. The format of the
         thumbnail file must match the format of the stickers in the set.
 
         .. versionadded:: 20.2
 
         Args:
@@ -6239,21 +6260,21 @@
         )
 
     @_log
     async def set_sticker_set_thumb(
         self,
         name: str,
         user_id: Union[str, int],
-        thumb: FileInput = None,
+        thumb: Optional[FileInput] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to set the thumbnail of a sticker set. Animated thumbnails can be set
         for animated sticker sets only. Video thumbnails can be set only for video sticker sets
         only.
 
         .. deprecated:: 20.2
            Bot API 6.6 renamed this method to :meth:`~Bot.set_sticker_set_thumbnail`.
@@ -6304,21 +6325,21 @@
         )
 
     @_log
     async def _set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: Union[str, int],
-        thumbnail: FileInput = None,
+        thumbnail: Optional[FileInput] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         data: JSONDict = {
             "name": name,
             "user_id": user_id,
             "thumbnail": self._parse_file_input(thumbnail) if thumbnail else None,
         }
 
@@ -6338,15 +6359,15 @@
         name: str,
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to set the title of a created sticker set.
 
         .. versionadded:: 20.2
 
         Args:
@@ -6379,15 +6400,15 @@
         sticker: str,
         emoji_list: Sequence[str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the list of emoji assigned to a regular or custom emoji sticker.
         The sticker must belong to a sticker set created by the bot.
 
         .. versionadded:: 20.2
 
@@ -6415,21 +6436,21 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_sticker_keywords(
         self,
         sticker: str,
-        keywords: Sequence[str] = None,
+        keywords: Optional[Sequence[str]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change search keywords assigned to a regular or custom emoji sticker.
         The sticker must belong to a sticker set created by the bot.
 
         .. versionadded:: 20.2
 
@@ -6457,21 +6478,21 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_sticker_mask_position(
         self,
         sticker: str,
-        mask_position: MaskPosition = None,
+        mask_position: Optional[MaskPosition] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the mask position of a mask sticker.
         The sticker must belong to a sticker set that was created by the bot.
 
         .. versionadded:: 20.2
 
@@ -6498,21 +6519,21 @@
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_custom_emoji_sticker_set_thumbnail(
         self,
         name: str,
-        custom_emoji_id: str = None,
+        custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to set the thumbnail of a custom emoji sticker set.
 
         .. versionadded:: 20.2
 
         Args:
@@ -6546,15 +6567,15 @@
         user_id: Union[str, int],
         errors: Sequence[PassportElementError],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Informs a user that some of the Telegram Passport elements they provided contains errors.
         The user will not be able to re-submit their Passport to you until the errors are fixed
         (the contents of the field for which you returned the error must change).
 
         Use this if the data submitted by the user doesn't satisfy the standards your service
@@ -6589,36 +6610,36 @@
 
     @_log
     async def send_poll(
         self,
         chat_id: Union[int, str],
         question: str,
         options: Sequence[str],
-        is_anonymous: bool = None,
-        type: str = None,  # pylint: disable=redefined-builtin
-        allows_multiple_answers: bool = None,
-        correct_option_id: int = None,
-        is_closed: bool = None,
+        is_anonymous: Optional[bool] = None,
+        type: Optional[str] = None,  # pylint: disable=redefined-builtin
+        allows_multiple_answers: Optional[bool] = None,
+        correct_option_id: Optional[CorrectOptionID] = None,
+        is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        explanation: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        explanation: Optional[str] = None,
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
-        open_period: int = None,
-        close_date: Union[int, datetime] = None,
+        open_period: Optional[int] = None,
+        close_date: Optional[Union[int, datetime]] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        explanation_entities: Sequence["MessageEntity"] = None,
+        explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send a native poll.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             question (:obj:`str`): Poll question, :tg-const:`telegram.Poll.MIN_QUESTION_LENGTH`-
@@ -6722,21 +6743,21 @@
         )
 
     @_log
     async def stop_poll(
         self,
         chat_id: Union[int, str],
         message_id: int,
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Poll:
         """
         Use this method to stop a poll which was sent by the bot.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             message_id (:obj:`int`): Identifier of the original message with the poll.
@@ -6768,26 +6789,26 @@
         return Poll.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def send_dice(
         self,
         chat_id: Union[int, str],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        emoji: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        emoji: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Message:
         """
         Use this method to send an animated emoji that will display a random value.
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             disable_notification (:obj:`bool`, optional): |disable_notification|
@@ -6843,21 +6864,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_my_default_administrator_rights(
         self,
-        for_channels: bool = None,
+        for_channels: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ChatAdministratorRights:
         """Use this method to get the current default administrator rights of the bot.
 
         .. seealso:: :meth:`set_my_default_administrator_rights`
 
         .. versionadded:: 20.0
 
@@ -6885,22 +6906,22 @@
         )
 
         return ChatAdministratorRights.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def set_my_default_administrator_rights(
         self,
-        rights: ChatAdministratorRights = None,
-        for_channels: bool = None,
+        rights: Optional[ChatAdministratorRights] = None,
+        for_channels: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to change the default administrator rights requested by the bot when
         it's added as an administrator to groups or channels. These rights will be suggested to
         users, but they are are free to modify the list before adding the bot.
 
         .. seealso:: :meth:`get_my_default_administrator_rights`
 
@@ -6931,22 +6952,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_my_commands(
         self,
-        scope: BotCommandScope = None,
-        language_code: str = None,
+        scope: Optional[BotCommandScope] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[BotCommand, ...]:
         """
         Use this method to get the current list of the bot's commands for the given scope and user
         language.
 
         .. seealso:: :meth:`set_my_commands`, :meth:`delete_my_commands`
 
@@ -6986,22 +7007,22 @@
 
         return BotCommand.de_list(result, self)
 
     @_log
     async def set_my_commands(
         self,
         commands: Sequence[Union[BotCommand, Tuple[str, str]]],
-        scope: BotCommandScope = None,
-        language_code: str = None,
+        scope: Optional[BotCommandScope] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the list of the bot's commands. See the
         `Telegram docs <https://core.telegram.org/bots/features#commands>`_ for more details about
         bot commands.
 
         .. seealso:: :meth:`get_my_commands`, :meth:`delete_my_commands`
@@ -7050,22 +7071,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def delete_my_commands(
         self,
-        scope: BotCommandScope = None,
-        language_code: str = None,
+        scope: Optional[BotCommandScope] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to delete the list of the bot's commands for the given scope and user
         language. After deletion,
         `higher level commands <https://core.telegram.org/bots/api#determining-list-of-commands>`_
         will be shown to affected users.
 
@@ -7103,15 +7124,15 @@
     async def log_out(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to log out from the cloud Bot API server before launching the bot locally.
         You *must* log out the bot before running it locally, otherwise there is no guarantee that
         the bot will receive updates. After a successful call, you can immediately log in on a
         local server, but will not be able to log in back to the cloud Bot API server for 10
         minutes.
@@ -7136,15 +7157,15 @@
     async def close(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to close the bot instance before moving it from one local server to
         another. You need to delete the webhook before calling this method to ensure that the bot
         isn't launched again after server restart. The method will return error 429 in the first
         10 minutes after the bot is launched.
 
@@ -7166,29 +7187,29 @@
 
     @_log
     async def copy_message(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_id: int,
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> MessageId:
         """
         Use this method to copy messages of any kind. Service messages and invoice messages can't
         be copied. The method is analogous to the method :meth:`forward_message`, but the copied
         message doesn't have a link to the original message.
 
         Args:
@@ -7253,22 +7274,22 @@
             api_kwargs=api_kwargs,
         )
         return MessageId.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def set_chat_menu_button(
         self,
-        chat_id: int = None,
-        menu_button: MenuButton = None,
+        chat_id: Optional[int] = None,
+        menu_button: Optional[MenuButton] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Use this method to change the bot's menu button in a private chat, or the default menu
         button.
 
         .. seealso:: :meth:`get_chat_menu_button`, :meth:`telegram.Chat.get_menu_button`
             :meth:`telegram.User.get_menu_button`
 
@@ -7295,21 +7316,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_chat_menu_button(
         self,
-        chat_id: int = None,
+        chat_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> MenuButton:
         """Use this method to get the current value of the bot's menu button in a private chat, or
         the default menu button.
 
         .. seealso:: :meth:`set_chat_menu_button`, :meth:`telegram.Chat.set_menu_button`,
             :meth:`telegram.User.set_menu_button`
 
@@ -7341,34 +7362,34 @@
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: Sequence["LabeledPrice"],
-        max_tip_amount: int = None,
-        suggested_tip_amounts: Sequence[int] = None,
-        provider_data: Union[str, object] = None,
-        photo_url: str = None,
-        photo_size: int = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        need_name: bool = None,
-        need_phone_number: bool = None,
-        need_email: bool = None,
-        need_shipping_address: bool = None,
-        send_phone_number_to_provider: bool = None,
-        send_email_to_provider: bool = None,
-        is_flexible: bool = None,
+        max_tip_amount: Optional[int] = None,
+        suggested_tip_amounts: Optional[Sequence[int]] = None,
+        provider_data: Optional[Union[str, object]] = None,
+        photo_url: Optional[str] = None,
+        photo_size: Optional[int] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        need_name: Optional[bool] = None,
+        need_phone_number: Optional[bool] = None,
+        need_email: Optional[bool] = None,
+        need_shipping_address: Optional[bool] = None,
+        send_phone_number_to_provider: Optional[bool] = None,
+        send_email_to_provider: Optional[bool] = None,
+        is_flexible: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> str:
         """Use this method to create a link for an invoice.
 
         .. versionadded:: 20.0
 
         Args:
             title (:obj:`str`): Product name. :tg-const:`telegram.Invoice.MIN_TITLE_LENGTH`-
@@ -7469,15 +7490,15 @@
     async def get_forum_topic_icon_stickers(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple[Sticker, ...]:
         """Use this method to get custom emoji stickers, which can be used as a forum topic
         icon by any user. Requires no parameters.
 
         .. versionadded:: 20.0
 
         Returns:
@@ -7498,22 +7519,22 @@
         return Sticker.de_list(result, self)
 
     @_log
     async def create_forum_topic(
         self,
         chat_id: Union[str, int],
         name: str,
-        icon_color: int = None,
-        icon_custom_emoji_id: str = None,
+        icon_color: Optional[int] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ForumTopic:
         """
         Use this method to create a topic in a forum supergroup chat. The bot must be
         an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
 
         .. versionadded:: 20.0
@@ -7558,22 +7579,22 @@
         return ForumTopic.de_json(result, self)  # type: ignore[return-value]
 
     @_log
     async def edit_forum_topic(
         self,
         chat_id: Union[str, int],
         message_thread_id: int,
-        name: str = None,
-        icon_custom_emoji_id: str = None,
+        name: Optional[str] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to edit name and icon of a topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights,
         unless it is the creator of the topic.
 
@@ -7620,15 +7641,15 @@
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to close an open topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights,
         unless it is the creator of the topic.
 
@@ -7665,15 +7686,15 @@
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to reopen a closed topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights,
         unless it is the creator of the topic.
 
@@ -7710,15 +7731,15 @@
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to delete a forum topic along with all its messages in a forum supergroup
         chat. The bot must be an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_delete_messages` administrator rights.
 
         .. versionadded:: 20.0
@@ -7754,15 +7775,15 @@
         chat_id: Union[str, int],
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to clear the list of pinned messages in a forum topic. The bot must
         be an administrator in the chat for this to work and must have
         :paramref:`~telegram.ChatAdministratorRights.can_pin_messages` administrator rights
         in the supergroup.
 
@@ -7799,15 +7820,15 @@
         chat_id: Union[str, int],
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to edit the name of the 'General' topic in a forum supergroup chat. The bot
         must be an administrator in the chat for this to work and must have
         :attr:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
 
         .. versionadded:: 20.0
@@ -7842,15 +7863,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to close an open 'General' topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :attr:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
 
         .. versionadded:: 20.0
@@ -7882,15 +7903,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to reopen a closed 'General' topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :attr:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
         The topic will be automatically unhidden if it was hidden.
 
@@ -7923,15 +7944,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to hide the 'General' topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :attr:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
         The topic will be automatically closed if it was open.
 
@@ -7964,15 +7985,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to unhide the 'General' topic in a forum supergroup chat. The bot must
         be an administrator in the chat for this to work and must have
         :attr:`~telegram.ChatAdministratorRights.can_manage_topics` administrator rights.
 
         .. versionadded:: 20.0
@@ -7998,22 +8019,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_my_description(
         self,
-        description: str = None,
-        language_code: str = None,
+        description: Optional[str] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the bot's description, which is shown in the chat with the bot
         if the chat is empty.
 
         .. versionadded:: 20.2
 
@@ -8044,22 +8065,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def set_my_short_description(
         self,
-        short_description: str = None,
-        language_code: str = None,
+        short_description: Optional[str] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the bot's short description, which is shown on the bot's profile
         page and is sent together with the link when users share the bot.
 
         .. versionadded:: 20.2
 
@@ -8090,21 +8111,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_my_description(
         self,
-        language_code: str = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> BotDescription:
         """
         Use this method to get the current bot description for the given user language.
 
         Args:
             language_code (:obj:`str`, optional): A two-letter ISO 639-1 language code or an empty
                 string.
@@ -8129,21 +8150,21 @@
             ),
             bot=self,
         )
 
     @_log
     async def get_my_short_description(
         self,
-        language_code: str = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> BotShortDescription:
         """
         Use this method to get the current bot short description for the given user language.
 
         Args:
             language_code (:obj:`str`, optional): A two-letter ISO 639-1 language code or an empty
                 string.
@@ -8169,22 +8190,22 @@
             ),
             bot=self,
         )
 
     @_log
     async def set_my_name(
         self,
-        name: str = None,
-        language_code: str = None,
+        name: Optional[str] = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """
         Use this method to change the bot's name.
 
         .. versionadded:: 20.3
 
         Args:
@@ -8218,21 +8239,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     @_log
     async def get_my_name(
         self,
-        language_code: str = None,
+        language_code: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> BotName:
         """
         Use this method to get the current bot name for the given user language.
 
         Args:
             language_code (:obj:`str`, optional): A two-letter ISO 639-1 language code or an empty
                 string.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_botcommand.py` & `python-telegram-bot-raw-20.4/telegram/_botcommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Bot Command."""
 
-from typing import ClassVar
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class BotCommand(TelegramObject):
@@ -48,36 +48,36 @@
             :tg-const:`telegram.BotCommand.MIN_DESCRIPTION`-
             :tg-const:`telegram.BotCommand.MAX_DESCRIPTION` characters.
 
     """
 
     __slots__ = ("description", "command")
 
-    def __init__(self, command: str, description: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, command: str, description: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.command: str = command
         self.description: str = description
 
         self._id_attrs = (self.command, self.description)
 
         self._freeze()
 
-    MIN_COMMAND: ClassVar[int] = constants.BotCommandLimit.MIN_COMMAND
+    MIN_COMMAND: Final[int] = constants.BotCommandLimit.MIN_COMMAND
     """:const:`telegram.constants.BotCommandLimit.MIN_COMMAND`
 
     .. versionadded:: 20.0
     """
-    MAX_COMMAND: ClassVar[int] = constants.BotCommandLimit.MAX_COMMAND
+    MAX_COMMAND: Final[int] = constants.BotCommandLimit.MAX_COMMAND
     """:const:`telegram.constants.BotCommandLimit.MAX_COMMAND`
 
     .. versionadded:: 20.0
     """
-    MIN_DESCRIPTION: ClassVar[int] = constants.BotCommandLimit.MIN_DESCRIPTION
+    MIN_DESCRIPTION: Final[int] = constants.BotCommandLimit.MIN_DESCRIPTION
     """:const:`telegram.constants.BotCommandLimit.MIN_DESCRIPTION`
 
     .. versionadded:: 20.0
     """
-    MAX_DESCRIPTION: ClassVar[int] = constants.BotCommandLimit.MAX_DESCRIPTION
+    MAX_DESCRIPTION: Final[int] = constants.BotCommandLimit.MAX_DESCRIPTION
     """:const:`telegram.constants.BotCommandLimit.MAX_DESCRIPTION`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_botcommandscope.py` & `python-telegram-bot-raw-20.4/telegram/_botcommandscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=redefined-builtin
 """This module contains objects representing Telegram bot command scopes."""
-from typing import TYPE_CHECKING, ClassVar, Dict, Optional, Type, Union
+from typing import TYPE_CHECKING, Dict, Final, Optional, Type, Union
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
@@ -56,30 +56,30 @@
 
     Attributes:
         type (:obj:`str`): Scope type.
     """
 
     __slots__ = ("type",)
 
-    DEFAULT: ClassVar[str] = constants.BotCommandScopeType.DEFAULT
+    DEFAULT: Final[str] = constants.BotCommandScopeType.DEFAULT
     """:const:`telegram.constants.BotCommandScopeType.DEFAULT`"""
-    ALL_PRIVATE_CHATS: ClassVar[str] = constants.BotCommandScopeType.ALL_PRIVATE_CHATS
+    ALL_PRIVATE_CHATS: Final[str] = constants.BotCommandScopeType.ALL_PRIVATE_CHATS
     """:const:`telegram.constants.BotCommandScopeType.ALL_PRIVATE_CHATS`"""
-    ALL_GROUP_CHATS: ClassVar[str] = constants.BotCommandScopeType.ALL_GROUP_CHATS
+    ALL_GROUP_CHATS: Final[str] = constants.BotCommandScopeType.ALL_GROUP_CHATS
     """:const:`telegram.constants.BotCommandScopeType.ALL_GROUP_CHATS`"""
-    ALL_CHAT_ADMINISTRATORS: ClassVar[str] = constants.BotCommandScopeType.ALL_CHAT_ADMINISTRATORS
+    ALL_CHAT_ADMINISTRATORS: Final[str] = constants.BotCommandScopeType.ALL_CHAT_ADMINISTRATORS
     """:const:`telegram.constants.BotCommandScopeType.ALL_CHAT_ADMINISTRATORS`"""
-    CHAT: ClassVar[str] = constants.BotCommandScopeType.CHAT
+    CHAT: Final[str] = constants.BotCommandScopeType.CHAT
     """:const:`telegram.constants.BotCommandScopeType.CHAT`"""
-    CHAT_ADMINISTRATORS: ClassVar[str] = constants.BotCommandScopeType.CHAT_ADMINISTRATORS
+    CHAT_ADMINISTRATORS: Final[str] = constants.BotCommandScopeType.CHAT_ADMINISTRATORS
     """:const:`telegram.constants.BotCommandScopeType.CHAT_ADMINISTRATORS`"""
-    CHAT_MEMBER: ClassVar[str] = constants.BotCommandScopeType.CHAT_MEMBER
+    CHAT_MEMBER: Final[str] = constants.BotCommandScopeType.CHAT_MEMBER
     """:const:`telegram.constants.BotCommandScopeType.CHAT_MEMBER`"""
 
-    def __init__(self, type: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, type: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.type: str = type
         self._id_attrs = (self.type,)
 
         self._freeze()
 
     @classmethod
@@ -124,15 +124,15 @@
     .. versionadded:: 13.7
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.DEFAULT`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.DEFAULT, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class BotCommandScopeAllPrivateChats(BotCommandScope):
     """Represents the scope of bot commands, covering all private chats.
 
@@ -140,45 +140,45 @@
 
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.ALL_PRIVATE_CHATS`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.ALL_PRIVATE_CHATS, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class BotCommandScopeAllGroupChats(BotCommandScope):
     """Represents the scope of bot commands, covering all group and supergroup chats.
 
     .. versionadded:: 13.7
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.ALL_GROUP_CHATS`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.ALL_GROUP_CHATS, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class BotCommandScopeAllChatAdministrators(BotCommandScope):
     """Represents the scope of bot commands, covering all group and supergroup chat administrators.
 
     .. versionadded:: 13.7
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.ALL_CHAT_ADMINISTRATORS`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.ALL_CHAT_ADMINISTRATORS, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class BotCommandScopeChat(BotCommandScope):
     """Represents the scope of bot commands, covering a specific chat.
 
@@ -193,15 +193,15 @@
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.CHAT`.
         chat_id (:obj:`str` | :obj:`int`): |chat_id_group|
     """
 
     __slots__ = ("chat_id",)
 
-    def __init__(self, chat_id: Union[str, int], *, api_kwargs: JSONDict = None):
+    def __init__(self, chat_id: Union[str, int], *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.CHAT, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.chat_id: Union[str, int] = (
                 chat_id if isinstance(chat_id, str) and chat_id.startswith("@") else int(chat_id)
             )
             self._id_attrs = (self.type, self.chat_id)
 
@@ -220,15 +220,15 @@
     Attributes:
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.CHAT_ADMINISTRATORS`.
         chat_id (:obj:`str` | :obj:`int`): |chat_id_group|
     """
 
     __slots__ = ("chat_id",)
 
-    def __init__(self, chat_id: Union[str, int], *, api_kwargs: JSONDict = None):
+    def __init__(self, chat_id: Union[str, int], *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=BotCommandScope.CHAT_ADMINISTRATORS, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.chat_id: Union[str, int] = (
                 chat_id if isinstance(chat_id, str) and chat_id.startswith("@") else int(chat_id)
             )
             self._id_attrs = (self.type, self.chat_id)
 
@@ -250,15 +250,17 @@
         type (:obj:`str`): Scope type :tg-const:`telegram.BotCommandScope.CHAT_MEMBER`.
         chat_id (:obj:`str` | :obj:`int`): |chat_id_group|
         user_id (:obj:`int`): Unique identifier of the target user.
     """
 
     __slots__ = ("chat_id", "user_id")
 
-    def __init__(self, chat_id: Union[str, int], user_id: int, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, chat_id: Union[str, int], user_id: int, *, api_kwargs: Optional[JSONDict] = None
+    ):
         super().__init__(type=BotCommandScope.CHAT_MEMBER, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.chat_id: Union[str, int] = (
                 chat_id if isinstance(chat_id, str) and chat_id.startswith("@") else int(chat_id)
             )
             self.user_id: int = user_id
             self._id_attrs = (self.type, self.chat_id, self.user_id)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_botdescription.py` & `python-telegram-bot-raw-20.4/telegram/_botdescription.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains two objects that represent a Telegram bots (short) description."""
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class BotDescription(TelegramObject):
     """This object represents the bot's description.
 
@@ -35,15 +37,15 @@
     Attributes:
         description (:obj:`str`): The bot's description.
 
     """
 
     __slots__ = ("description",)
 
-    def __init__(self, description: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, description: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.description: str = description
 
         self._id_attrs = (self.description,)
 
         self._freeze()
 
@@ -62,14 +64,14 @@
     Attributes:
         short_description (:obj:`str`): The bot's short description.
 
     """
 
     __slots__ = ("short_description",)
 
-    def __init__(self, short_description: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, short_description: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.short_description: str = short_description
 
         self._id_attrs = (self.short_description,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_botname.py` & `python-telegram-bot-raw-20.4/telegram/_botname.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represent a Telegram bots name."""
-from typing import ClassVar
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class BotName(TelegramObject):
@@ -38,17 +38,17 @@
     Attributes:
         name (:obj:`str`): The bot's name.
 
     """
 
     __slots__ = ("name",)
 
-    def __init__(self, name: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, name: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.name: str = name
 
         self._id_attrs = (self.name,)
 
         self._freeze()
 
-    MAX_LENGTH: ClassVar[int] = constants.BotNameLimit.MAX_NAME_LENGTH
+    MAX_LENGTH: Final[int] = constants.BotNameLimit.MAX_NAME_LENGTH
     """:const:`telegram.constants.BotNameLimit.MAX_NAME_LENGTH`"""
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_callbackquery.py` & `python-telegram-bot-raw-20.4/telegram/_callbackquery.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=redefined-builtin
 """This module contains an object that represents a Telegram CallbackQuery"""
-from typing import TYPE_CHECKING, ClassVar, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Final, Optional, Sequence, Tuple, Union
 
 from telegram import constants
 from telegram._files.location import Location
 from telegram._message import Message
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.defaultvalue import DEFAULT_NONE
@@ -114,20 +114,20 @@
     )
 
     def __init__(
         self,
         id: str,
         from_user: User,
         chat_instance: str,
-        message: Message = None,
-        data: str = None,
-        inline_message_id: str = None,
-        game_short_name: str = None,
+        message: Optional[Message] = None,
+        data: Optional[str] = None,
+        inline_message_id: Optional[str] = None,
+        game_short_name: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.id: str = id  # pylint: disable=invalid-name
         self.from_user: User = from_user
         self.chat_instance: str = chat_instance
         # Optionals
@@ -151,24 +151,24 @@
         data["from_user"] = User.de_json(data.pop("from", None), bot)
         data["message"] = Message.de_json(data.get("message"), bot)
 
         return super().de_json(data=data, bot=bot)
 
     async def answer(
         self,
-        text: str = None,
-        show_alert: bool = None,
-        url: str = None,
-        cache_time: int = None,
+        text: Optional[str] = None,
+        show_alert: Optional[bool] = None,
+        url: Optional[str] = None,
+        cache_time: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.answer_callback_query(update.callback_query.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.answer_callback_query`.
@@ -191,22 +191,22 @@
         )
 
     async def edit_message_text(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
-        reply_markup: "InlineKeyboardMarkup" = None,
-        entities: Sequence["MessageEntity"] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.edit_text(*args, **kwargs)
 
         or::
 
@@ -249,24 +249,24 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             entities=entities,
         )
 
     async def edit_message_caption(
         self,
-        caption: str = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.edit_caption(*args, **kwargs)
 
         or::
 
@@ -313,15 +313,15 @@
         self,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.edit_reply_markup(*args, **kwargs)
 
         or::
 
@@ -358,21 +358,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def edit_message_media(
         self,
         media: "InputMedia",
-        reply_markup: "InlineKeyboardMarkup" = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.edit_media(*args, **kwargs)
 
         or::
 
@@ -409,27 +409,27 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def edit_message_live_location(
         self,
-        latitude: float = None,
-        longitude: float = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         *,
-        location: Location = None,
+        location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.edit_live_location(*args, **kwargs)
 
         or::
 
@@ -477,21 +477,21 @@
             horizontal_accuracy=horizontal_accuracy,
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
         )
 
     async def stop_message_live_location(
         self,
-        reply_markup: "InlineKeyboardMarkup" = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
             await update.callback_query.message.stop_live_location(*args, **kwargs)
 
         or::
 
@@ -529,22 +529,22 @@
             api_kwargs=api_kwargs,
         )
 
     async def set_game_score(
         self,
         user_id: Union[int, str],
         score: int,
-        force: bool = None,
-        disable_edit_message: bool = None,
+        force: Optional[bool] = None,
+        disable_edit_message: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union[Message, bool]:
         """Shortcut for either::
 
            await update.callback_query.message.set_game_score(*args, **kwargs)
 
         or::
 
@@ -591,15 +591,15 @@
         self,
         user_id: Union[int, str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple["GameHighScore", ...]:
         """Shortcut for either::
 
             await update.callback_query.message.get_game_high_score(*args, **kwargs)
 
         or::
 
@@ -639,15 +639,15 @@
     async def delete_message(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await update.callback_query.message.delete(*args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Message.delete`.
 
@@ -667,15 +667,15 @@
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await update.callback_query.message.pin(*args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Message.pin`.
 
@@ -695,15 +695,15 @@
     async def unpin_message(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await update.callback_query.message.unpin(*args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Message.unpin`.
 
@@ -718,29 +718,29 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def copy_message(
         self,
         chat_id: Union[int, str],
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
             await update.callback_query.message.copy(
                 from_chat_id=update.message.chat_id,
                 message_id=update.message.message_id,
                 *args,
@@ -767,15 +767,15 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
-    MAX_ANSWER_TEXT_LENGTH: ClassVar[
+    MAX_ANSWER_TEXT_LENGTH: Final[
         int
     ] = constants.CallbackQueryLimit.ANSWER_CALLBACK_QUERY_TEXT_LENGTH
     """
     :const:`telegram.constants.CallbackQueryLimit.ANSWER_CALLBACK_QUERY_TEXT_LENGTH`
 
     .. versionadded:: 13.2
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chat.py` & `python-telegram-bot-raw-20.4/telegram/_chat.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,27 +16,34 @@
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Chat."""
 from datetime import datetime
 from html import escape
-from typing import TYPE_CHECKING, ClassVar, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Final, Optional, Sequence, Tuple, Union
 
 from telegram import constants
 from telegram._chatlocation import ChatLocation
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.chatphoto import ChatPhoto
 from telegram._forumtopic import ForumTopic
 from telegram._menubutton import MenuButton
 from telegram._telegramobject import TelegramObject
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
-from telegram._utils.types import DVInput, FileInput, JSONDict, ODVInput, ReplyMarkup
+from telegram._utils.types import (
+    CorrectOptionID,
+    DVInput,
+    FileInput,
+    JSONDict,
+    ODVInput,
+    ReplyMarkup,
+)
 from telegram.helpers import escape_markdown
 from telegram.helpers import mention_html as helpers_mention_html
 from telegram.helpers import mention_markdown as helpers_mention_markdown
 
 if TYPE_CHECKING:
     from telegram import (
         Animation,
@@ -299,60 +306,60 @@
         "is_forum",
         "active_usernames",
         "emoji_status_custom_emoji_id",
         "has_hidden_members",
         "has_aggressive_anti_spam_enabled",
     )
 
-    SENDER: ClassVar[str] = constants.ChatType.SENDER
+    SENDER: Final[str] = constants.ChatType.SENDER
     """:const:`telegram.constants.ChatType.SENDER`
 
     .. versionadded:: 13.5
     """
-    PRIVATE: ClassVar[str] = constants.ChatType.PRIVATE
+    PRIVATE: Final[str] = constants.ChatType.PRIVATE
     """:const:`telegram.constants.ChatType.PRIVATE`"""
-    GROUP: ClassVar[str] = constants.ChatType.GROUP
+    GROUP: Final[str] = constants.ChatType.GROUP
     """:const:`telegram.constants.ChatType.GROUP`"""
-    SUPERGROUP: ClassVar[str] = constants.ChatType.SUPERGROUP
+    SUPERGROUP: Final[str] = constants.ChatType.SUPERGROUP
     """:const:`telegram.constants.ChatType.SUPERGROUP`"""
-    CHANNEL: ClassVar[str] = constants.ChatType.CHANNEL
+    CHANNEL: Final[str] = constants.ChatType.CHANNEL
     """:const:`telegram.constants.ChatType.CHANNEL`"""
 
     def __init__(
         self,
         id: int,
         type: str,
-        title: str = None,
-        username: str = None,
-        first_name: str = None,
-        last_name: str = None,
-        photo: ChatPhoto = None,
-        description: str = None,
-        invite_link: str = None,
-        pinned_message: "Message" = None,
-        permissions: ChatPermissions = None,
-        sticker_set_name: str = None,
-        can_set_sticker_set: bool = None,
-        slow_mode_delay: int = None,
-        bio: str = None,
-        linked_chat_id: int = None,
-        location: ChatLocation = None,
-        message_auto_delete_time: int = None,
-        has_private_forwards: bool = None,
-        has_protected_content: bool = None,
-        join_to_send_messages: bool = None,
-        join_by_request: bool = None,
-        has_restricted_voice_and_video_messages: bool = None,
-        is_forum: bool = None,
-        active_usernames: Sequence[str] = None,
-        emoji_status_custom_emoji_id: str = None,
-        has_aggressive_anti_spam_enabled: bool = None,
-        has_hidden_members: bool = None,
+        title: Optional[str] = None,
+        username: Optional[str] = None,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
+        photo: Optional[ChatPhoto] = None,
+        description: Optional[str] = None,
+        invite_link: Optional[str] = None,
+        pinned_message: Optional["Message"] = None,
+        permissions: Optional[ChatPermissions] = None,
+        sticker_set_name: Optional[str] = None,
+        can_set_sticker_set: Optional[bool] = None,
+        slow_mode_delay: Optional[int] = None,
+        bio: Optional[str] = None,
+        linked_chat_id: Optional[int] = None,
+        location: Optional[ChatLocation] = None,
+        message_auto_delete_time: Optional[int] = None,
+        has_private_forwards: Optional[bool] = None,
+        has_protected_content: Optional[bool] = None,
+        join_to_send_messages: Optional[bool] = None,
+        join_by_request: Optional[bool] = None,
+        has_restricted_voice_and_video_messages: Optional[bool] = None,
+        is_forum: Optional[bool] = None,
+        active_usernames: Optional[Sequence[str]] = None,
+        emoji_status_custom_emoji_id: Optional[str] = None,
+        has_aggressive_anti_spam_enabled: Optional[bool] = None,
+        has_hidden_members: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.id: int = id  # pylint: disable=invalid-name
         self.type: str = enum.get_member(constants.ChatType, type, type)
         # Optionals
         self.title: Optional[str] = title
@@ -452,15 +459,15 @@
         if "all_members_are_administrators" in data:
             api_kwargs["all_members_are_administrators"] = data.pop(
                 "all_members_are_administrators"
             )
 
         return super()._de_json(data=data, bot=bot, api_kwargs=api_kwargs)
 
-    def mention_markdown(self, name: str = None) -> str:
+    def mention_markdown(self, name: Optional[str] = None) -> str:
         """
         Note:
             :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
             Telegram for backward compatibility. You should use :meth:`mention_markdown_v2`
             instead.
 
         .. versionadded:: 20.0
@@ -489,15 +496,15 @@
             if name:
                 return f"[{name}]({self.link})"
             if self.title:
                 return f"[{self.title}]({self.link})"
             raise TypeError("Can not create a mention to a public chat without title")
         raise TypeError("Can not create a mention to a private group chat")
 
-    def mention_markdown_v2(self, name: str = None) -> str:
+    def mention_markdown_v2(self, name: Optional[str] = None) -> str:
         """
         .. versionadded:: 20.0
 
         Args:
             name (:obj:`str`): The name used as a link for the chat. Defaults to :attr:`full_name`.
 
         Returns:
@@ -521,15 +528,15 @@
             if name:
                 return f"[{escape_markdown(name, version=2)}]({self.link})"
             if self.title:
                 return f"[{escape_markdown(self.title, version=2)}]({self.link})"
             raise TypeError("Can not create a mention to a public chat without title")
         raise TypeError("Can not create a mention to a private group chat")
 
-    def mention_html(self, name: str = None) -> str:
+    def mention_html(self, name: Optional[str] = None) -> str:
         """
         .. versionadded:: 20.0
 
         Args:
             name (:obj:`str`): The name used as a link for the chat. Defaults to :attr:`full_name`.
 
         Returns:
@@ -560,15 +567,15 @@
     async def leave(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.leave_chat(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.leave_chat`.
 
@@ -588,15 +595,15 @@
     async def get_administrators(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple["ChatMember", ...]:
         """Shortcut for::
 
              await bot.get_chat_administrators(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.get_chat_administrators`.
@@ -620,15 +627,15 @@
     async def get_member_count(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> int:
         """Shortcut for::
 
              await bot.get_chat_member_count(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.get_chat_member_count`.
@@ -649,15 +656,15 @@
         self,
         user_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "ChatMember":
         """Shortcut for::
 
              await bot.get_chat_member(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.get_chat_member`.
 
@@ -674,22 +681,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def ban_member(
         self,
         user_id: Union[str, int],
-        revoke_messages: bool = None,
-        until_date: Union[int, datetime] = None,
+        revoke_messages: Optional[bool] = None,
+        until_date: Optional[Union[int, datetime]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.ban_chat_member(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.ban_chat_member`.
@@ -713,15 +720,15 @@
         self,
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.ban_chat_sender_chat(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.ban_chat_sender_chat`.
@@ -746,15 +753,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.ban_chat_sender_chat(
                  sender_chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -781,15 +788,15 @@
         self,
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unban_chat_sender_chat(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.unban_chat_sender_chat`.
@@ -814,15 +821,15 @@
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unban_chat_sender_chat(
                  sender_chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -844,21 +851,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def unban_member(
         self,
         user_id: Union[str, int],
-        only_if_banned: bool = None,
+        only_if_banned: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unban_chat_member(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.unban_chat_member`.
 
@@ -876,32 +883,32 @@
             api_kwargs=api_kwargs,
             only_if_banned=only_if_banned,
         )
 
     async def promote_member(
         self,
         user_id: Union[str, int],
-        can_change_info: bool = None,
-        can_post_messages: bool = None,
-        can_edit_messages: bool = None,
-        can_delete_messages: bool = None,
-        can_invite_users: bool = None,
-        can_restrict_members: bool = None,
-        can_pin_messages: bool = None,
-        can_promote_members: bool = None,
-        is_anonymous: bool = None,
-        can_manage_chat: bool = None,
-        can_manage_video_chats: bool = None,
-        can_manage_topics: bool = None,
+        can_change_info: Optional[bool] = None,
+        can_post_messages: Optional[bool] = None,
+        can_edit_messages: Optional[bool] = None,
+        can_delete_messages: Optional[bool] = None,
+        can_invite_users: Optional[bool] = None,
+        can_restrict_members: Optional[bool] = None,
+        can_pin_messages: Optional[bool] = None,
+        can_promote_members: Optional[bool] = None,
+        is_anonymous: Optional[bool] = None,
+        can_manage_chat: Optional[bool] = None,
+        can_manage_video_chats: Optional[bool] = None,
+        can_manage_topics: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.promote_chat_member(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.promote_chat_member`.
@@ -938,22 +945,22 @@
             can_manage_topics=can_manage_topics,
         )
 
     async def restrict_member(
         self,
         user_id: Union[str, int],
         permissions: ChatPermissions,
-        until_date: Union[int, datetime] = None,
-        use_independent_chat_permissions: bool = None,
+        until_date: Optional[Union[int, datetime]] = None,
+        use_independent_chat_permissions: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.restrict_chat_member(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.restrict_chat_member`.
@@ -979,21 +986,21 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def set_permissions(
         self,
         permissions: ChatPermissions,
-        use_independent_chat_permissions: bool = None,
+        use_independent_chat_permissions: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_permissions(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.set_chat_permissions`.
@@ -1021,15 +1028,15 @@
         user_id: Union[int, str],
         custom_title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_administrator_custom_title(
                  update.effective_chat.id, *args, **kwargs
              )
 
@@ -1055,15 +1062,15 @@
         self,
         photo: FileInput,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_photo(
                  chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -1089,15 +1096,15 @@
     async def delete_photo(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.delete_chat_photo(
                  chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -1123,15 +1130,15 @@
         self,
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_title(
                  chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -1152,21 +1159,21 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def set_description(
         self,
-        description: str = None,
+        description: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_description(
                  chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -1194,15 +1201,15 @@
         message_id: int,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.pin_chat_message(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.pin_chat_message`.
@@ -1220,21 +1227,21 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def unpin_message(
         self,
-        message_id: int = None,
+        message_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.unpin_chat_message(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.unpin_chat_message`.
@@ -1256,15 +1263,15 @@
     async def unpin_all_messages(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.unpin_all_chat_messages(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.unpin_all_chat_messages`.
@@ -1284,26 +1291,26 @@
 
     async def send_message(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_message(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
@@ -1332,27 +1339,27 @@
 
     async def send_media_group(
         self,
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
     ) -> Tuple["Message", ...]:
         """Shortcut for::
 
              await bot.send_media_group(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_media_group`.
 
@@ -1378,21 +1385,21 @@
             parse_mode=parse_mode,
             caption_entities=caption_entities,
         )
 
     async def send_chat_action(
         self,
         action: str,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.send_chat_action(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_chat_action`.
 
@@ -1413,31 +1420,31 @@
 
     send_action = send_chat_action
     """Alias for :attr:`send_chat_action`"""
 
     async def send_photo(
         self,
         photo: Union[FileInput, "PhotoSize"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_photo(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_photo`.
 
@@ -1464,31 +1471,31 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             has_spoiler=has_spoiler,
         )
 
     async def send_contact(
         self,
-        phone_number: str = None,
-        first_name: str = None,
-        last_name: str = None,
+        phone_number: Optional[str] = None,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        vcard: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        vcard: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        contact: "Contact" = None,
+        contact: Optional["Contact"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_contact(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_contact`.
 
@@ -1515,35 +1522,35 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_audio(
         self,
         audio: Union[FileInput, "Audio"],
-        duration: int = None,
-        performer: str = None,
-        title: str = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        performer: Optional[str] = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_audio(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_audio`.
 
@@ -1575,33 +1582,33 @@
             api_kwargs=api_kwargs,
             thumbnail=thumbnail,
         )
 
     async def send_document(
         self,
         document: Union[FileInput, "Document"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
-        disable_content_type_detection: bool = None,
+        thumb: Optional[FileInput] = None,
+        disable_content_type_detection: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_document(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_document`.
 
@@ -1631,26 +1638,26 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        emoji: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        emoji: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_dice(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_dice`.
 
@@ -1674,25 +1681,25 @@
             message_thread_id=message_thread_id,
         )
 
     async def send_game(
         self,
         game_short_name: str,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_game(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_game`.
 
@@ -1720,41 +1727,41 @@
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: Sequence["LabeledPrice"],
-        start_parameter: str = None,
-        photo_url: str = None,
-        photo_size: int = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        need_name: bool = None,
-        need_phone_number: bool = None,
-        need_email: bool = None,
-        need_shipping_address: bool = None,
-        is_flexible: bool = None,
+        start_parameter: Optional[str] = None,
+        photo_url: Optional[str] = None,
+        photo_size: Optional[int] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        need_name: Optional[bool] = None,
+        need_phone_number: Optional[bool] = None,
+        need_email: Optional[bool] = None,
+        need_shipping_address: Optional[bool] = None,
+        is_flexible: Optional[bool] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
-        provider_data: Union[str, object] = None,
-        send_phone_number_to_provider: bool = None,
-        send_email_to_provider: bool = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
+        provider_data: Optional[Union[str, object]] = None,
+        send_phone_number_to_provider: Optional[bool] = None,
+        send_email_to_provider: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        max_tip_amount: int = None,
-        suggested_tip_amounts: Sequence[int] = None,
+        max_tip_amount: Optional[int] = None,
+        suggested_tip_amounts: Optional[Sequence[int]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_invoice(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_invoice`.
 
@@ -1806,33 +1813,33 @@
             suggested_tip_amounts=suggested_tip_amounts,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_location(
         self,
-        latitude: float = None,
-        longitude: float = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        live_period: int = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        live_period: Optional[int] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        location: "Location" = None,
+        location: Optional["Location"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_location(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_location`.
 
@@ -1861,36 +1868,36 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_animation(
         self,
         animation: Union[FileInput, "Animation"],
-        duration: int = None,
-        width: int = None,
-        height: int = None,
-        thumb: FileInput = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_animation(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_animation`.
 
@@ -1924,26 +1931,26 @@
             thumbnail=thumbnail,
         )
 
     async def send_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        emoji: str = None,
+        message_thread_id: Optional[int] = None,
+        emoji: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_sticker(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_sticker`.
 
@@ -1966,35 +1973,35 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
             emoji=emoji,
         )
 
     async def send_venue(
         self,
-        latitude: float = None,
-        longitude: float = None,
-        title: str = None,
-        address: str = None,
-        foursquare_id: str = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        title: Optional[str] = None,
+        address: Optional[str] = None,
+        foursquare_id: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        venue: "Venue" = None,
+        venue: Optional["Venue"] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_venue(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_venue`.
 
@@ -2025,37 +2032,37 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_video(
         self,
         video: Union[FileInput, "Video"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        width: int = None,
-        height: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        supports_streaming: bool = None,
-        thumb: FileInput = None,
+        supports_streaming: Optional[bool] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_video(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video`.
 
@@ -2089,31 +2096,31 @@
             message_thread_id=message_thread_id,
             has_spoiler=has_spoiler,
         )
 
     async def send_video_note(
         self,
         video_note: Union[FileInput, "VideoNote"],
-        duration: int = None,
-        length: int = None,
+        duration: Optional[int] = None,
+        length: Optional[int] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        thumb: FileInput = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_video_note(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video_note`.
 
@@ -2141,31 +2148,31 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def send_voice(
         self,
         voice: Union[FileInput, "Voice"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        filename: str = None,
+        filename: Optional[str] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_voice(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_voice`.
 
@@ -2194,36 +2201,36 @@
             message_thread_id=message_thread_id,
         )
 
     async def send_poll(
         self,
         question: str,
         options: Sequence[str],
-        is_anonymous: bool = None,
-        type: str = None,
-        allows_multiple_answers: bool = None,
-        correct_option_id: int = None,
-        is_closed: bool = None,
+        is_anonymous: Optional[bool] = None,
+        type: Optional[str] = None,
+        allows_multiple_answers: Optional[bool] = None,
+        correct_option_id: Optional[CorrectOptionID] = None,
+        is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        explanation: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        explanation: Optional[str] = None,
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
-        open_period: int = None,
-        close_date: Union[int, datetime] = None,
+        open_period: Optional[int] = None,
+        close_date: Optional[Union[int, datetime]] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        explanation_entities: Sequence["MessageEntity"] = None,
+        explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_poll(update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_poll`.
 
@@ -2258,29 +2265,29 @@
             message_thread_id=message_thread_id,
         )
 
     async def send_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
              await bot.copy_message(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.copy_message`.
 
@@ -2308,29 +2315,29 @@
             message_thread_id=message_thread_id,
         )
 
     async def copy_message(
         self,
         chat_id: Union[int, str],
         message_id: int,
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
              await bot.copy_message(from_chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.copy_message`.
 
@@ -2360,21 +2367,21 @@
 
     async def forward_from(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.forward_message(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.forward_message`.
 
@@ -2402,21 +2409,21 @@
 
     async def forward_to(
         self,
         chat_id: Union[int, str],
         message_id: int,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.forward_message(from_chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.forward_message`.
 
@@ -2445,15 +2452,15 @@
     async def export_invite_link(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> str:
         """Shortcut for::
 
              await bot.export_chat_invite_link(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.export_chat_invite_link`.
@@ -2471,24 +2478,24 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def create_invite_link(
         self,
-        expire_date: Union[int, datetime] = None,
-        member_limit: int = None,
-        name: str = None,
-        creates_join_request: bool = None,
+        expire_date: Optional[Union[int, datetime]] = None,
+        member_limit: Optional[int] = None,
+        name: Optional[str] = None,
+        creates_join_request: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "ChatInviteLink":
         """Shortcut for::
 
              await bot.create_chat_invite_link(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.create_chat_invite_link`.
@@ -2515,24 +2522,24 @@
             name=name,
             creates_join_request=creates_join_request,
         )
 
     async def edit_invite_link(
         self,
         invite_link: Union[str, "ChatInviteLink"],
-        expire_date: Union[int, datetime] = None,
-        member_limit: int = None,
-        name: str = None,
-        creates_join_request: bool = None,
+        expire_date: Optional[Union[int, datetime]] = None,
+        member_limit: Optional[int] = None,
+        name: Optional[str] = None,
+        creates_join_request: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "ChatInviteLink":
         """Shortcut for::
 
              await bot.edit_chat_invite_link(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.edit_chat_invite_link`.
@@ -2564,15 +2571,15 @@
         self,
         invite_link: Union[str, "ChatInviteLink"],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "ChatInviteLink":
         """Shortcut for::
 
              await bot.revoke_chat_invite_link(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.revoke_chat_invite_link`.
@@ -2597,15 +2604,15 @@
         self,
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.approve_chat_join_request(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.approve_chat_join_request`.
@@ -2630,15 +2637,15 @@
         self,
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.decline_chat_join_request(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.decline_chat_join_request`.
@@ -2657,21 +2664,21 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def set_menu_button(
         self,
-        menu_button: MenuButton = None,
+        menu_button: Optional[MenuButton] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.set_chat_menu_button(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.set_chat_menu_button`.
@@ -2695,22 +2702,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def create_forum_topic(
         self,
         name: str,
-        icon_color: int = None,
-        icon_custom_emoji_id: str = None,
+        icon_color: Optional[int] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> ForumTopic:
         """Shortcut for::
 
              await bot.create_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.create_forum_topic`.
@@ -2731,22 +2738,22 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def edit_forum_topic(
         self,
         message_thread_id: int,
-        name: str = None,
-        icon_custom_emoji_id: str = None,
+        name: Optional[str] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.edit_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.edit_forum_topic`.
@@ -2772,15 +2779,15 @@
         self,
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.close_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.close_forum_topic`.
@@ -2804,15 +2811,15 @@
         self,
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.reopen_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.reopen_forum_topic`.
@@ -2836,15 +2843,15 @@
         self,
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.delete_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.delete_forum_topic`.
@@ -2868,15 +2875,15 @@
         self,
         message_thread_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unpin_all_forum_topic_messages(chat_id=update.effective_chat.id,
                 *args, **kwargs)
 
         For the documentation of the arguments, please see
@@ -2901,15 +2908,15 @@
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.edit_general_forum_topic(
                 chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -2934,15 +2941,15 @@
     async def close_general_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.close_general_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.close_general_forum_topic`.
@@ -2964,15 +2971,15 @@
     async def reopen_general_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.reopen_general_forum_topic(
                 chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -2996,15 +3003,15 @@
     async def hide_general_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.hide_general_forum_topic(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.hide_general_forum_topic`.
@@ -3026,15 +3033,15 @@
     async def unhide_general_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unhide_general_forum_topic (
                 chat_id=update.effective_chat.id, *args, **kwargs
              )
 
@@ -3058,15 +3065,15 @@
     async def get_menu_button(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> MenuButton:
         """Shortcut for::
 
              await bot.get_chat_menu_button(chat_id=update.effective_chat.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.get_chat_menu_button`.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatadministratorrights.py` & `python-telegram-bot-raw-20.4/telegram/_chatadministratorrights.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,20 +123,20 @@
         can_manage_chat: bool,
         can_delete_messages: bool,
         can_manage_video_chats: bool,
         can_restrict_members: bool,
         can_promote_members: bool,
         can_change_info: bool,
         can_invite_users: bool,
-        can_post_messages: bool = None,
-        can_edit_messages: bool = None,
-        can_pin_messages: bool = None,
-        can_manage_topics: bool = None,
+        can_post_messages: Optional[bool] = None,
+        can_edit_messages: Optional[bool] = None,
+        can_pin_messages: Optional[bool] = None,
+        can_manage_topics: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> None:
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.is_anonymous: bool = is_anonymous
         self.can_manage_chat: bool = can_manage_chat
         self.can_delete_messages: bool = can_delete_messages
         self.can_manage_video_chats: bool = can_manage_video_chats
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatinvitelink.py` & `python-telegram-bot-raw-20.4/telegram/_chatinvitelink.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,20 +114,20 @@
     def __init__(
         self,
         invite_link: str,
         creator: User,
         creates_join_request: bool,
         is_primary: bool,
         is_revoked: bool,
-        expire_date: datetime.datetime = None,
-        member_limit: int = None,
-        name: str = None,
-        pending_join_request_count: int = None,
+        expire_date: Optional[datetime.datetime] = None,
+        member_limit: Optional[int] = None,
+        name: Optional[str] = None,
+        pending_join_request_count: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.invite_link: str = invite_link
         self.creator: User = creator
         self.creates_join_request: bool = creates_join_request
         self.is_primary: bool = is_primary
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatjoinrequest.py` & `python-telegram-bot-raw-20.4/telegram/_chatjoinrequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,28 +88,34 @@
             user.
 
             .. versionadded:: 20.1
         bio (:obj:`str`): Optional. Bio of the user.
         invite_link (:class:`telegram.ChatInviteLink`): Optional. Chat invite link that was used
             by the user to send the join request.
 
+            Note:
+                When a user joins a *public* group via an invite link, this attribute may not
+                be present. However, this behavior is undocument and may be subject to change.
+                See `this GitHub thread <https://github.com/tdlib/telegram-bot-api/issues/428>`_
+                for some discussion.
+
     """
 
     __slots__ = ("chat", "from_user", "date", "bio", "invite_link", "user_chat_id")
 
     def __init__(
         self,
         chat: Chat,
         from_user: User,
         date: datetime.datetime,
         user_chat_id: int,
-        bio: str = None,
-        invite_link: ChatInviteLink = None,
+        bio: Optional[str] = None,
+        invite_link: Optional[ChatInviteLink] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.chat: Chat = chat
         self.from_user: User = from_user
         self.date: datetime.datetime = date
         self.user_chat_id: int = user_chat_id
@@ -143,15 +149,15 @@
     async def approve(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await bot.approve_chat_join_request(
                 chat_id=update.effective_chat.id, user_id=update.effective_user.id, *args, **kwargs
             )
 
@@ -175,15 +181,15 @@
     async def decline(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await bot.decline_chat_join_request(
                 chat_id=update.effective_chat.id, user_id=update.effective_user.id, *args, **kwargs
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatlocation.py` & `python-telegram-bot-raw-20.4/telegram/_chatlocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a location to which a chat is connected."""
 
-from typing import TYPE_CHECKING, ClassVar, Optional
+from typing import TYPE_CHECKING, Final, Optional
 
 from telegram import constants
 from telegram._files.location import Location
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
@@ -53,15 +53,15 @@
     __slots__ = ("location", "address")
 
     def __init__(
         self,
         location: Location,
         address: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.location: Location = location
         self.address: str = address
 
         self._id_attrs = (self.location,)
 
@@ -75,17 +75,17 @@
         if not data:
             return None
 
         data["location"] = Location.de_json(data.get("location"), bot)
 
         return super().de_json(data=data, bot=bot)
 
-    MIN_ADDRESS: ClassVar[int] = constants.LocationLimit.MIN_CHAT_LOCATION_ADDRESS
+    MIN_ADDRESS: Final[int] = constants.LocationLimit.MIN_CHAT_LOCATION_ADDRESS
     """:const:`telegram.constants.LocationLimit.MIN_CHAT_LOCATION_ADDRESS`
 
     .. versionadded:: 20.0
     """
-    MAX_ADDRESS: ClassVar[int] = constants.LocationLimit.MAX_CHAT_LOCATION_ADDRESS
+    MAX_ADDRESS: Final[int] = constants.LocationLimit.MAX_CHAT_LOCATION_ADDRESS
     """:const:`telegram.constants.LocationLimit.MAX_CHAT_LOCATION_ADDRESS`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatmember.py` & `python-telegram-bot-raw-20.4/telegram/_chatmember.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ChatMember."""
 import datetime
-from typing import TYPE_CHECKING, ClassVar, Dict, Optional, Type
+from typing import TYPE_CHECKING, Dict, Final, Optional, Type
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
@@ -70,33 +70,33 @@
             :attr:`~telegram.ChatMember.BANNED`, :attr:`~telegram.ChatMember.LEFT`,
             :attr:`~telegram.ChatMember.MEMBER` or :attr:`~telegram.ChatMember.RESTRICTED`.
 
     """
 
     __slots__ = ("user", "status")
 
-    ADMINISTRATOR: ClassVar[str] = constants.ChatMemberStatus.ADMINISTRATOR
+    ADMINISTRATOR: Final[str] = constants.ChatMemberStatus.ADMINISTRATOR
     """:const:`telegram.constants.ChatMemberStatus.ADMINISTRATOR`"""
-    OWNER: ClassVar[str] = constants.ChatMemberStatus.OWNER
+    OWNER: Final[str] = constants.ChatMemberStatus.OWNER
     """:const:`telegram.constants.ChatMemberStatus.OWNER`"""
-    BANNED: ClassVar[str] = constants.ChatMemberStatus.BANNED
+    BANNED: Final[str] = constants.ChatMemberStatus.BANNED
     """:const:`telegram.constants.ChatMemberStatus.BANNED`"""
-    LEFT: ClassVar[str] = constants.ChatMemberStatus.LEFT
+    LEFT: Final[str] = constants.ChatMemberStatus.LEFT
     """:const:`telegram.constants.ChatMemberStatus.LEFT`"""
-    MEMBER: ClassVar[str] = constants.ChatMemberStatus.MEMBER
+    MEMBER: Final[str] = constants.ChatMemberStatus.MEMBER
     """:const:`telegram.constants.ChatMemberStatus.MEMBER`"""
-    RESTRICTED: ClassVar[str] = constants.ChatMemberStatus.RESTRICTED
+    RESTRICTED: Final[str] = constants.ChatMemberStatus.RESTRICTED
     """:const:`telegram.constants.ChatMemberStatus.RESTRICTED`"""
 
     def __init__(
         self,
         user: User,
         status: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required by all subclasses
         self.user: User = user
         self.status: str = status
 
         self._id_attrs = (self.user, self.status)
@@ -158,17 +158,17 @@
 
     __slots__ = ("is_anonymous", "custom_title")
 
     def __init__(
         self,
         user: User,
         is_anonymous: bool,
-        custom_title: str = None,
+        custom_title: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.OWNER, user=user, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.is_anonymous: bool = is_anonymous
             self.custom_title: Optional[str] = custom_title
 
 
@@ -291,21 +291,21 @@
         can_manage_chat: bool,
         can_delete_messages: bool,
         can_manage_video_chats: bool,
         can_restrict_members: bool,
         can_promote_members: bool,
         can_change_info: bool,
         can_invite_users: bool,
-        can_post_messages: bool = None,
-        can_edit_messages: bool = None,
-        can_pin_messages: bool = None,
-        can_manage_topics: bool = None,
-        custom_title: str = None,
+        can_post_messages: Optional[bool] = None,
+        can_edit_messages: Optional[bool] = None,
+        can_pin_messages: Optional[bool] = None,
+        can_manage_topics: Optional[bool] = None,
+        custom_title: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.ADMINISTRATOR, user=user, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.can_be_edited: bool = can_be_edited
             self.is_anonymous: bool = is_anonymous
             self.can_manage_chat: bool = can_manage_chat
             self.can_delete_messages: bool = can_delete_messages
@@ -340,15 +340,15 @@
 
     __slots__ = ()
 
     def __init__(
         self,
         user: User,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.MEMBER, user=user, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class ChatMemberRestricted(ChatMember):
     """
@@ -507,15 +507,15 @@
         can_send_audios: bool,
         can_send_documents: bool,
         can_send_photos: bool,
         can_send_videos: bool,
         can_send_video_notes: bool,
         can_send_voice_notes: bool,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.RESTRICTED, user=user, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.is_member: bool = is_member
             self.can_change_info: bool = can_change_info
             self.can_invite_users: bool = can_invite_users
             self.can_pin_messages: bool = can_pin_messages
@@ -552,15 +552,15 @@
 
     __slots__ = ()
 
     def __init__(
         self,
         user: User,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.LEFT, user=user, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class ChatMemberBanned(ChatMember):
     """
@@ -592,12 +592,12 @@
     __slots__ = ("until_date",)
 
     def __init__(
         self,
         user: User,
         until_date: datetime.datetime,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(status=ChatMember.BANNED, user=user, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.until_date: datetime.datetime = until_date
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatmemberupdated.py` & `python-telegram-bot-raw-20.4/telegram/_chatmemberupdated.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,18 @@
     def __init__(
         self,
         chat: Chat,
         from_user: User,
         date: datetime.datetime,
         old_chat_member: ChatMember,
         new_chat_member: ChatMember,
-        invite_link: ChatInviteLink = None,
-        via_chat_folder_invite_link: bool = None,
+        invite_link: Optional[ChatInviteLink] = None,
+        via_chat_folder_invite_link: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.chat: Chat = chat
         self.from_user: User = from_user
         self.date: datetime.datetime = date
         self.old_chat_member: ChatMember = old_chat_member
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_chatpermissions.py` & `python-telegram-bot-raw-20.4/telegram/_chatpermissions.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,31 +162,31 @@
         "can_send_videos",
         "can_send_video_notes",
         "can_send_voice_notes",
     )
 
     def __init__(
         self,
-        can_send_messages: bool = None,
-        can_send_media_messages: bool = None,
-        can_send_polls: bool = None,
-        can_send_other_messages: bool = None,
-        can_add_web_page_previews: bool = None,
-        can_change_info: bool = None,
-        can_invite_users: bool = None,
-        can_pin_messages: bool = None,
-        can_manage_topics: bool = None,
-        can_send_audios: bool = None,
-        can_send_documents: bool = None,
-        can_send_photos: bool = None,
-        can_send_videos: bool = None,
-        can_send_video_notes: bool = None,
-        can_send_voice_notes: bool = None,
+        can_send_messages: Optional[bool] = None,
+        can_send_media_messages: Optional[bool] = None,
+        can_send_polls: Optional[bool] = None,
+        can_send_other_messages: Optional[bool] = None,
+        can_add_web_page_previews: Optional[bool] = None,
+        can_change_info: Optional[bool] = None,
+        can_invite_users: Optional[bool] = None,
+        can_pin_messages: Optional[bool] = None,
+        can_manage_topics: Optional[bool] = None,
+        can_send_audios: Optional[bool] = None,
+        can_send_documents: Optional[bool] = None,
+        can_send_photos: Optional[bool] = None,
+        can_send_videos: Optional[bool] = None,
+        can_send_video_notes: Optional[bool] = None,
+        can_send_voice_notes: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.can_send_messages: Optional[bool] = can_send_messages
         self.can_send_media_messages: Optional[bool] = can_send_media_messages
         self.can_send_polls: Optional[bool] = can_send_polls
         self.can_send_other_messages: Optional[bool] = can_send_other_messages
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_choseninlineresult.py` & `python-telegram-bot-raw-20.4/telegram/_choseninlineresult.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,18 +68,18 @@
     __slots__ = ("location", "result_id", "from_user", "inline_message_id", "query")
 
     def __init__(
         self,
         result_id: str,
         from_user: User,
         query: str,
-        location: Location = None,
-        inline_message_id: str = None,
+        location: Optional[Location] = None,
+        inline_message_id: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.result_id: str = result_id
         self.from_user: User = from_user
         self.query: str = query
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_dice.py` & `python-telegram-bot-raw-20.4/telegram/_dice.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Dice."""
-from typing import ClassVar, List
+from typing import Final, List, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class Dice(TelegramObject):
@@ -85,76 +85,76 @@
             for :tg-const:`telegram.Dice.SLOT_MACHINE` base emoji.
         emoji (:obj:`str`): Emoji on which the dice throw animation is based.
 
     """
 
     __slots__ = ("emoji", "value")
 
-    def __init__(self, value: int, emoji: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, value: int, emoji: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.value: int = value
         self.emoji: str = emoji
 
         self._id_attrs = (self.value, self.emoji)
 
         self._freeze()
 
-    DICE: ClassVar[str] = constants.DiceEmoji.DICE  # skipcq: PTC-W0052
+    DICE: Final[str] = constants.DiceEmoji.DICE  # skipcq: PTC-W0052
     """:const:`telegram.constants.DiceEmoji.DICE`"""
-    DARTS: ClassVar[str] = constants.DiceEmoji.DARTS
+    DARTS: Final[str] = constants.DiceEmoji.DARTS
     """:const:`telegram.constants.DiceEmoji.DARTS`"""
-    BASKETBALL: ClassVar[str] = constants.DiceEmoji.BASKETBALL
+    BASKETBALL: Final[str] = constants.DiceEmoji.BASKETBALL
     """:const:`telegram.constants.DiceEmoji.BASKETBALL`"""
-    FOOTBALL: ClassVar[str] = constants.DiceEmoji.FOOTBALL
+    FOOTBALL: Final[str] = constants.DiceEmoji.FOOTBALL
     """:const:`telegram.constants.DiceEmoji.FOOTBALL`"""
-    SLOT_MACHINE: ClassVar[str] = constants.DiceEmoji.SLOT_MACHINE
+    SLOT_MACHINE: Final[str] = constants.DiceEmoji.SLOT_MACHINE
     """:const:`telegram.constants.DiceEmoji.SLOT_MACHINE`"""
-    BOWLING: ClassVar[str] = constants.DiceEmoji.BOWLING
+    BOWLING: Final[str] = constants.DiceEmoji.BOWLING
     """
     :const:`telegram.constants.DiceEmoji.BOWLING`
 
     .. versionadded:: 13.4
     """
-    ALL_EMOJI: ClassVar[List[str]] = list(constants.DiceEmoji)
+    ALL_EMOJI: Final[List[str]] = list(constants.DiceEmoji)
     """List[:obj:`str`]: A list of all available dice emoji."""
 
-    MIN_VALUE: ClassVar[int] = constants.DiceLimit.MIN_VALUE
+    MIN_VALUE: Final[int] = constants.DiceLimit.MIN_VALUE
     """:const:`telegram.constants.DiceLimit.MIN_VALUE`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_BOWLING: ClassVar[int] = constants.DiceLimit.MAX_VALUE_BOWLING
+    MAX_VALUE_BOWLING: Final[int] = constants.DiceLimit.MAX_VALUE_BOWLING
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_BOWLING`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_DARTS: ClassVar[int] = constants.DiceLimit.MAX_VALUE_DARTS
+    MAX_VALUE_DARTS: Final[int] = constants.DiceLimit.MAX_VALUE_DARTS
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_DARTS`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_DICE: ClassVar[int] = constants.DiceLimit.MAX_VALUE_DICE
+    MAX_VALUE_DICE: Final[int] = constants.DiceLimit.MAX_VALUE_DICE
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_DICE`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_BASKETBALL: ClassVar[int] = constants.DiceLimit.MAX_VALUE_BASKETBALL
+    MAX_VALUE_BASKETBALL: Final[int] = constants.DiceLimit.MAX_VALUE_BASKETBALL
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_BASKETBALL`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_FOOTBALL: ClassVar[int] = constants.DiceLimit.MAX_VALUE_FOOTBALL
+    MAX_VALUE_FOOTBALL: Final[int] = constants.DiceLimit.MAX_VALUE_FOOTBALL
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_FOOTBALL`
 
     .. versionadded:: 20.0
     """
 
-    MAX_VALUE_SLOT_MACHINE: ClassVar[int] = constants.DiceLimit.MAX_VALUE_SLOT_MACHINE
+    MAX_VALUE_SLOT_MACHINE: Final[int] = constants.DiceLimit.MAX_VALUE_SLOT_MACHINE
     """:const:`telegram.constants.DiceLimit.MAX_VALUE_SLOT_MACHINE`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/_basemedium.py` & `python-telegram-bot-raw-20.4/telegram/_files/_basemedium.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
     __slots__ = ("file_id", "file_size", "file_unique_id")
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
-        file_size: int = None,
+        file_size: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.file_id: str = str(file_id)
         self.file_unique_id: str = str(file_unique_id)
         # Optionals
@@ -73,15 +73,15 @@
     async def get_file(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "File":
         """Convenience wrapper over :meth:`telegram.Bot.get_file`
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.get_file`.
 
         Returns:
             :class:`telegram.File`
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/_basethumbedmedium.py` & `python-telegram-bot-raw-20.4/telegram/_files/_basethumbedmedium.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,19 +70,19 @@
 
     __slots__ = ("thumbnail",)
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
-        file_size: int = None,
-        thumb: PhotoSize = None,
-        thumbnail: PhotoSize = None,
+        file_size: Optional[int] = None,
+        thumb: Optional[PhotoSize] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             api_kwargs=api_kwargs,
         )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/animation.py` & `python-telegram-bot-raw-20.4/telegram/_files/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         width: int,
         height: int,
         duration: int,
-        thumb: PhotoSize = None,
-        file_name: str = None,
-        mime_type: str = None,
-        file_size: int = None,
-        thumbnail: PhotoSize = None,
+        thumb: Optional[PhotoSize] = None,
+        file_name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             api_kwargs=api_kwargs,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/audio.py` & `python-telegram-bot-raw-20.4/telegram/_files/audio.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,23 +76,23 @@
     __slots__ = ("duration", "file_name", "mime_type", "performer", "title")
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         duration: int,
-        performer: str = None,
-        title: str = None,
-        mime_type: str = None,
-        file_size: int = None,
-        thumb: PhotoSize = None,
-        file_name: str = None,
-        thumbnail: PhotoSize = None,
+        performer: Optional[str] = None,
+        title: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None,
+        thumb: Optional[PhotoSize] = None,
+        file_name: Optional[str] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             thumbnail=thumbnail,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/chatphoto.py` & `python-telegram-bot-raw-20.4/telegram/_files/chatphoto.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ChatPhoto."""
-from typing import TYPE_CHECKING, ClassVar
+from typing import TYPE_CHECKING, Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 
 if TYPE_CHECKING:
@@ -83,15 +83,15 @@
     def __init__(
         self,
         small_file_id: str,
         small_file_unique_id: str,
         big_file_id: str,
         big_file_unique_id: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.small_file_id: str = small_file_id
         self.small_file_unique_id: str = small_file_unique_id
         self.big_file_id: str = big_file_id
         self.big_file_unique_id: str = big_file_unique_id
 
@@ -105,15 +105,15 @@
     async def get_small_file(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "File":
         """Convenience wrapper over :meth:`telegram.Bot.get_file` for getting the small
         (:tg-const:`telegram.ChatPhoto.SIZE_SMALL` x :tg-const:`telegram.ChatPhoto.SIZE_SMALL`)
         chat photo
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.get_file`.
 
@@ -136,15 +136,15 @@
     async def get_big_file(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "File":
         """Convenience wrapper over :meth:`telegram.Bot.get_file` for getting the
         big (:tg-const:`telegram.ChatPhoto.SIZE_BIG` x :tg-const:`telegram.ChatPhoto.SIZE_BIG`)
         chat photo
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.get_file`.
 
@@ -160,17 +160,17 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    SIZE_SMALL: ClassVar[int] = constants.ChatPhotoSize.SMALL
+    SIZE_SMALL: Final[int] = constants.ChatPhotoSize.SMALL
     """:const:`telegram.constants.ChatPhotoSize.SMALL`
 
     .. versionadded:: 20.0
     """
-    SIZE_BIG: ClassVar[int] = constants.ChatPhotoSize.BIG
+    SIZE_BIG: Final[int] = constants.ChatPhotoSize.BIG
     """:const:`telegram.constants.ChatPhotoSize.BIG`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/contact.py` & `python-telegram-bot-raw-20.4/telegram/_files/contact.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
     __slots__ = ("vcard", "user_id", "first_name", "last_name", "phone_number")
 
     def __init__(
         self,
         phone_number: str,
         first_name: str,
-        last_name: str = None,
-        user_id: int = None,
-        vcard: str = None,
+        last_name: Optional[str] = None,
+        user_id: Optional[int] = None,
+        vcard: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.phone_number: str = str(phone_number)
         self.first_name: str = first_name
         # Optionals
         self.last_name: Optional[str] = last_name
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/document.py` & `python-telegram-bot-raw-20.4/telegram/_files/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,21 +63,21 @@
 
     __slots__ = ("file_name", "mime_type")
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
-        thumb: PhotoSize = None,
-        file_name: str = None,
-        mime_type: str = None,
-        file_size: int = None,
-        thumbnail: PhotoSize = None,
+        thumb: Optional[PhotoSize] = None,
+        file_name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             thumbnail=thumbnail,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/file.py` & `python-telegram-bot-raw-20.4/telegram/_files/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         "_credentials",
     )
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
-        file_size: int = None,
-        file_path: str = None,
+        file_size: Optional[int] = None,
+        file_path: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.file_id: str = str(file_id)
         self.file_unique_id: str = str(file_unique_id)
         # Optionals
@@ -115,15 +115,15 @@
         )
 
     def _prepare_decrypt(self, buf: bytes) -> bytes:
         return decrypt(b64decode(self._credentials.secret), b64decode(self._credentials.hash), buf)
 
     async def download_to_drive(
         self,
-        custom_path: FilePathInput = None,
+        custom_path: Optional[FilePathInput] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
     ) -> Path:
         """
@@ -266,15 +266,15 @@
             )
         if self._credentials:
             buf = self._prepare_decrypt(buf)
         out.write(buf)
 
     async def download_as_bytearray(
         self,
-        buf: bytearray = None,
+        buf: Optional[bytearray] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
     ) -> bytearray:
         """Download this file and return it as a bytearray.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/inputfile.py` & `python-telegram-bot-raw-20.4/telegram/_files/inputfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
         mimetype (:obj:`str`): The mimetype inferred from the file to be sent.
 
     """
 
     __slots__ = ("filename", "attach_name", "input_file_content", "mimetype")
 
     def __init__(
-        self, obj: Union[IO[bytes], bytes, str], filename: str = None, attach: bool = False
+        self,
+        obj: Union[IO[bytes], bytes, str],
+        filename: Optional[str] = None,
+        attach: bool = False,
     ):
         if isinstance(obj, bytes):
             self.input_file_content: bytes = obj
         elif isinstance(obj, str):
             self.input_file_content = obj.encode("utf-8")
         else:
             reported_filename, self.input_file_content = load_file(obj)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/inputmedia.py` & `python-telegram-bot-raw-20.4/telegram/_files/inputmedia.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,19 +87,19 @@
 
     __slots__ = ("caption", "caption_entities", "media", "parse_mode", "type")
 
     def __init__(
         self,
         media_type: str,
         media: Union[str, InputFile, MediaType],
-        caption: str = None,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption: Optional[str] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.type: str = media_type
         self.media: Union[str, InputFile, Animation, Audio, Document, PhotoSize, Video] = media
         self.caption: Optional[str] = caption
         self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
         self.parse_mode: ODVInput[str] = parse_mode
@@ -192,26 +192,26 @@
     """
 
     __slots__ = ("duration", "height", "width", "has_spoiler", "thumbnail")
 
     def __init__(
         self,
         media: Union[FileInput, Animation],
-        thumb: FileInput = None,
-        caption: str = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        width: int = None,
-        height: int = None,
-        duration: int = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        filename: str = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        duration: Optional[int] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        filename: Optional[str] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if isinstance(media, Animation):
             width = media.width if width is None else width
             height = media.height if height is None else height
             duration = media.duration if duration is None else duration
             media = media.file_id
         else:
@@ -300,21 +300,21 @@
     """
 
     __slots__ = ("has_spoiler",)
 
     def __init__(
         self,
         media: Union[FileInput, PhotoSize],
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
-        filename: str = None,
-        has_spoiler: bool = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        filename: Optional[str] = None,
+        has_spoiler: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # We use local_mode=True because we don't have access to the actual setting and want
         # things to work in local mode.
         media = parse_file_input(media, PhotoSize, filename=filename, attach=True, local_mode=True)
         super().__init__(
             InputMediaType.PHOTO,
             media,
@@ -419,27 +419,27 @@
         "has_spoiler",
         "thumbnail",
     )
 
     def __init__(
         self,
         media: Union[FileInput, Video],
-        caption: str = None,
-        width: int = None,
-        height: int = None,
-        duration: int = None,
-        supports_streaming: bool = None,
+        caption: Optional[str] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        duration: Optional[int] = None,
+        supports_streaming: Optional[bool] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        filename: str = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        thumb: Optional[FileInput] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        filename: Optional[str] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if isinstance(media, Video):
             width = width if width is not None else media.width
             height = height if height is not None else media.height
             duration = duration if duration is not None else media.duration
             media = media.file_id
         else:
@@ -551,25 +551,25 @@
     """
 
     __slots__ = ("duration", "performer", "title", "thumbnail")
 
     def __init__(
         self,
         media: Union[FileInput, Audio],
-        thumb: FileInput = None,
-        caption: str = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        duration: int = None,
-        performer: str = None,
-        title: str = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        filename: str = None,
-        thumbnail: FileInput = None,
+        duration: Optional[int] = None,
+        performer: Optional[str] = None,
+        title: Optional[str] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        filename: Optional[str] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if isinstance(media, Audio):
             duration = media.duration if duration is None else duration
             performer = media.performer if performer is None else performer
             title = media.title if title is None else title
             media = media.file_id
         else:
@@ -671,23 +671,23 @@
     """
 
     __slots__ = ("disable_content_type_detection", "thumbnail")
 
     def __init__(
         self,
         media: Union[FileInput, Document],
-        thumb: FileInput = None,
-        caption: str = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        disable_content_type_detection: bool = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        filename: str = None,
-        thumbnail: FileInput = None,
+        disable_content_type_detection: Optional[bool] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        filename: Optional[str] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # We use local_mode=True because we don't have access to the actual setting and want
         # things to work in local mode.
         media = parse_file_input(media, Document, filename=filename, attach=True, local_mode=True)
 
         thumbnail = warn_about_thumb_return_thumbnail(deprecated_arg=thumb, new_arg=thumbnail)
         super().__init__(
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/inputsticker.py` & `python-telegram-bot-raw-20.4/telegram/_files/inputsticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram InputSticker."""
 
-from typing import Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Sequence, Tuple, Union
 
-from telegram._files.inputfile import InputFile
 from telegram._files.sticker import MaskPosition
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.files import parse_file_input
 from telegram._utils.types import FileInput, JSONDict
 
+if TYPE_CHECKING:
+    from telegram._files.inputfile import InputFile
+
 
 class InputSticker(TelegramObject):
     """
     This object describes a sticker to be added to a sticker set.
 
     .. versionadded:: 20.2
 
@@ -70,18 +72,18 @@
 
     __slots__ = ("sticker", "emoji_list", "mask_position", "keywords")
 
     def __init__(
         self,
         sticker: FileInput,
         emoji_list: Sequence[str],
-        mask_position: MaskPosition = None,
-        keywords: Sequence[str] = None,
+        mask_position: Optional[MaskPosition] = None,
+        keywords: Optional[Sequence[str]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # We use local_mode=True because we don't have access to the actual setting and want
         # things to work in local mode.
         self.sticker: Union[str, InputFile] = parse_file_input(
             sticker,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/location.py` & `python-telegram-bot-raw-20.4/telegram/_files/location.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Location."""
 
-from typing import ClassVar, Optional
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class Location(TelegramObject):
@@ -68,20 +68,20 @@
         "heading",
     )
 
     def __init__(
         self,
         longitude: float,
         latitude: float,
-        horizontal_accuracy: float = None,
-        live_period: int = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        horizontal_accuracy: Optional[float] = None,
+        live_period: Optional[int] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.longitude: float = longitude
         self.latitude: float = latitude
 
         # Optionals
@@ -92,22 +92,22 @@
             int(proximity_alert_radius) if proximity_alert_radius else None
         )
 
         self._id_attrs = (self.longitude, self.latitude)
 
         self._freeze()
 
-    HORIZONTAL_ACCURACY: ClassVar[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
+    HORIZONTAL_ACCURACY: Final[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
     """:const:`telegram.constants.LocationLimit.HORIZONTAL_ACCURACY`
 
     .. versionadded:: 20.0
     """
-    MIN_HEADING: ClassVar[int] = constants.LocationLimit.MIN_HEADING
+    MIN_HEADING: Final[int] = constants.LocationLimit.MIN_HEADING
     """:const:`telegram.constants.LocationLimit.MIN_HEADING`
 
     .. versionadded:: 20.0
     """
-    MAX_HEADING: ClassVar[int] = constants.LocationLimit.MAX_HEADING
+    MAX_HEADING: Final[int] = constants.LocationLimit.MAX_HEADING
     """:const:`telegram.constants.LocationLimit.MAX_HEADING`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/photosize.py` & `python-telegram-bot-raw-20.4/telegram/_files/photosize.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram PhotoSize."""
 
+from typing import Optional
+
 from telegram._files._basemedium import _BaseMedium
 from telegram._utils.types import JSONDict
 
 
 class PhotoSize(_BaseMedium):
     """This object represents one size of a photo or a file/sticker thumbnail.
 
@@ -55,17 +57,17 @@
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         width: int,
         height: int,
-        file_size: int = None,
+        file_size: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             api_kwargs=api_kwargs,
         )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/sticker.py` & `python-telegram-bot-raw-20.4/telegram/_files/sticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains objects that represent stickers."""
-from typing import TYPE_CHECKING, ClassVar, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Final, Optional, Sequence, Tuple
 
 from telegram import constants
 from telegram._files._basethumbedmedium import _BaseThumbedMedium
 from telegram._files.file import File
 from telegram._files.photosize import PhotoSize
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
@@ -153,25 +153,25 @@
         file_id: str,
         file_unique_id: str,
         width: int,
         height: int,
         is_animated: bool,
         is_video: bool,
         type: str,  # pylint: disable=redefined-builtin
-        thumb: PhotoSize = None,
-        emoji: str = None,
-        file_size: int = None,
-        set_name: str = None,
-        mask_position: "MaskPosition" = None,
-        premium_animation: "File" = None,
-        custom_emoji_id: str = None,
-        thumbnail: PhotoSize = None,
-        needs_repainting: bool = None,
+        thumb: Optional[PhotoSize] = None,
+        emoji: Optional[str] = None,
+        file_size: Optional[int] = None,
+        set_name: Optional[str] = None,
+        mask_position: Optional["MaskPosition"] = None,
+        premium_animation: Optional["File"] = None,
+        custom_emoji_id: Optional[str] = None,
+        thumbnail: Optional[PhotoSize] = None,
+        needs_repainting: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             thumbnail=thumbnail,
@@ -188,19 +188,19 @@
             self.emoji: Optional[str] = emoji
             self.set_name: Optional[str] = set_name
             self.mask_position: Optional[MaskPosition] = mask_position
             self.premium_animation: Optional[File] = premium_animation
             self.custom_emoji_id: Optional[str] = custom_emoji_id
             self.needs_repainting: Optional[bool] = needs_repainting
 
-    REGULAR: ClassVar[str] = constants.StickerType.REGULAR
+    REGULAR: Final[str] = constants.StickerType.REGULAR
     """:const:`telegram.constants.StickerType.REGULAR`"""
-    MASK: ClassVar[str] = constants.StickerType.MASK
+    MASK: Final[str] = constants.StickerType.MASK
     """:const:`telegram.constants.StickerType.MASK`"""
-    CUSTOM_EMOJI: ClassVar[str] = constants.StickerType.CUSTOM_EMOJI
+    CUSTOM_EMOJI: Final[str] = constants.StickerType.CUSTOM_EMOJI
     """:const:`telegram.constants.StickerType.CUSTOM_EMOJI`"""
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["Sticker"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
@@ -298,18 +298,18 @@
         self,
         name: str,
         title: str,
         is_animated: bool,
         stickers: Sequence[Sticker],
         is_video: bool,
         sticker_type: str,
-        thumb: PhotoSize = None,
-        thumbnail: PhotoSize = None,
+        thumb: Optional[PhotoSize] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: str = name
         self.title: str = title
         self.is_animated: bool = is_animated
         self.is_video: bool = is_video
         self.stickers: Tuple[Sticker, ...] = parse_sequence_arg(stickers)
@@ -386,31 +386,31 @@
             default mask position.
         scale (:obj:`float`): Mask scaling coefficient. For example, ``2.0`` means double size.
 
     """
 
     __slots__ = ("point", "scale", "x_shift", "y_shift")
 
-    FOREHEAD: ClassVar[str] = constants.MaskPosition.FOREHEAD
+    FOREHEAD: Final[str] = constants.MaskPosition.FOREHEAD
     """:const:`telegram.constants.MaskPosition.FOREHEAD`"""
-    EYES: ClassVar[str] = constants.MaskPosition.EYES
+    EYES: Final[str] = constants.MaskPosition.EYES
     """:const:`telegram.constants.MaskPosition.EYES`"""
-    MOUTH: ClassVar[str] = constants.MaskPosition.MOUTH
+    MOUTH: Final[str] = constants.MaskPosition.MOUTH
     """:const:`telegram.constants.MaskPosition.MOUTH`"""
-    CHIN: ClassVar[str] = constants.MaskPosition.CHIN
+    CHIN: Final[str] = constants.MaskPosition.CHIN
     """:const:`telegram.constants.MaskPosition.CHIN`"""
 
     def __init__(
         self,
         point: str,
         x_shift: float,
         y_shift: float,
         scale: float,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.point: str = point
         self.x_shift: float = x_shift
         self.y_shift: float = y_shift
         self.scale: float = scale
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/venue.py` & `python-telegram-bot-raw-20.4/telegram/_files/venue.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,20 +75,20 @@
     )
 
     def __init__(
         self,
         location: Location,
         title: str,
         address: str,
-        foursquare_id: str = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
+        foursquare_id: Optional[str] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.location: Location = location
         self.title: str = title
         self.address: str = address
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/video.py` & `python-telegram-bot-raw-20.4/telegram/_files/video.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,21 +72,21 @@
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         width: int,
         height: int,
         duration: int,
-        thumb: PhotoSize = None,
-        mime_type: str = None,
-        file_size: int = None,
-        file_name: str = None,
-        thumbnail: PhotoSize = None,
+        thumb: Optional[PhotoSize] = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None,
+        file_name: Optional[str] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             thumbnail=thumbnail,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/videonote.py` & `python-telegram-bot-raw-20.4/telegram/_files/videonote.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram VideoNote."""
 
+from typing import Optional
+
 from telegram._files._basethumbedmedium import _BaseThumbedMedium
 from telegram._files.photosize import PhotoSize
 from telegram._utils.types import JSONDict
 
 
 class VideoNote(_BaseThumbedMedium):
     """This object represents a video message (available in Telegram apps as of v.4.0).
@@ -67,19 +69,19 @@
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         length: int,
         duration: int,
-        thumb: PhotoSize = None,
-        file_size: int = None,
-        thumbnail: PhotoSize = None,
+        thumb: Optional[PhotoSize] = None,
+        file_size: Optional[int] = None,
+        thumbnail: Optional[PhotoSize] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             thumb=thumb,
             thumbnail=thumbnail,
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_files/voice.py` & `python-telegram-bot-raw-20.4/telegram/_files/voice.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     __slots__ = ("duration", "mime_type")
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         duration: int,
-        mime_type: str = None,
-        file_size: int = None,
+        mime_type: Optional[str] = None,
+        file_size: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(
             file_id=file_id,
             file_unique_id=file_unique_id,
             file_size=file_size,
             api_kwargs=api_kwargs,
         )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_forcereply.py` & `python-telegram-bot-raw-20.4/telegram/_forcereply.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ForceReply."""
 
-from typing import ClassVar, Optional
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class ForceReply(TelegramObject):
@@ -75,31 +75,31 @@
 
     """
 
     __slots__ = ("selective", "force_reply", "input_field_placeholder")
 
     def __init__(
         self,
-        selective: bool = None,
-        input_field_placeholder: str = None,
+        selective: Optional[bool] = None,
+        input_field_placeholder: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.force_reply: bool = True
         self.selective: Optional[bool] = selective
         self.input_field_placeholder: Optional[str] = input_field_placeholder
 
         self._id_attrs = (self.selective,)
 
         self._freeze()
 
-    MIN_INPUT_FIELD_PLACEHOLDER: ClassVar[int] = constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER
+    MIN_INPUT_FIELD_PLACEHOLDER: Final[int] = constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER
     """:const:`telegram.constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER`
 
     .. versionadded:: 20.0
     """
-    MAX_INPUT_FIELD_PLACEHOLDER: ClassVar[int] = constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER
+    MAX_INPUT_FIELD_PLACEHOLDER: Final[int] = constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER
     """:const:`telegram.constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_forumtopic.py` & `python-telegram-bot-raw-20.4/telegram/_forumtopic.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     __slots__ = ("message_thread_id", "name", "icon_color", "icon_custom_emoji_id")
 
     def __init__(
         self,
         message_thread_id: int,
         name: str,
         icon_color: int,
-        icon_custom_emoji_id: str = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.message_thread_id: int = message_thread_id
         self.name: str = name
         self.icon_color: int = icon_color
         self.icon_custom_emoji_id: Optional[str] = icon_custom_emoji_id
 
@@ -95,17 +95,17 @@
 
     __slots__ = ("name", "icon_color", "icon_custom_emoji_id")
 
     def __init__(
         self,
         name: str,
         icon_color: int,
-        icon_custom_emoji_id: str = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: str = name
         self.icon_color: int = icon_color
         self.icon_custom_emoji_id: Optional[str] = icon_custom_emoji_id
 
         self._id_attrs = (self.name, self.icon_color)
@@ -119,15 +119,15 @@
     Currently holds no information.
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
 
 
 class ForumTopicReopened(TelegramObject):
     """
@@ -135,15 +135,15 @@
     Currently holds no information.
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
 
 
 class ForumTopicEdited(TelegramObject):
     """
@@ -165,18 +165,18 @@
             the topic icon, if it was edited; an empty string if the icon was removed.
     """
 
     __slots__ = ("name", "icon_custom_emoji_id")
 
     def __init__(
         self,
-        name: str = None,
-        icon_custom_emoji_id: str = None,
+        name: Optional[str] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: Optional[str] = name
         self.icon_custom_emoji_id: Optional[str] = icon_custom_emoji_id
 
         self._id_attrs = (self.name, self.icon_custom_emoji_id)
 
@@ -189,15 +189,15 @@
     Currently holds no information.
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
 
 
 class GeneralForumTopicUnhidden(TelegramObject):
     """
@@ -205,11 +205,11 @@
     Currently holds no information.
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_games/callbackgame.py` & `python-telegram-bot-raw-20.4/telegram/_games/callbackgame.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram CallbackGame."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class CallbackGame(TelegramObject):
     """A placeholder, currently holds no information. Use BotFather to set up your game."""
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_games/game.py` & `python-telegram-bot-raw-20.4/telegram/_games/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,19 +97,19 @@
     )
 
     def __init__(
         self,
         title: str,
         description: str,
         photo: Sequence[PhotoSize],
-        text: str = None,
-        text_entities: Sequence[MessageEntity] = None,
-        animation: Animation = None,
+        text: Optional[str] = None,
+        text_entities: Optional[Sequence[MessageEntity]] = None,
+        animation: Optional[Animation] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.title: str = title
         self.description: str = description
         self.photo: Tuple[PhotoSize, ...] = parse_sequence_arg(photo)
         # Optionals
@@ -158,15 +158,15 @@
             raise RuntimeError("This Game has no 'text'.")
 
         entity_text = self.text.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
 
         return entity_text.decode("utf-16-le")
 
-    def parse_text_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
+    def parse_text_entities(self, types: Optional[List[str]] = None) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this message filtered by their
         :attr:`~telegram.MessageEntity.type` attribute as the key, and the text that each entity
         belongs to as the value of the :obj:`dict`.
 
         Note:
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_games/gamehighscore.py` & `python-telegram-bot-raw-20.4/telegram/_games/gamehighscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         user (:class:`telegram.User`): User.
         score (:obj:`int`): Score.
 
     """
 
     __slots__ = ("position", "user", "score")
 
-    def __init__(self, position: int, user: User, score: int, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, position: int, user: User, score: int, *, api_kwargs: Optional[JSONDict] = None
+    ):
         super().__init__(api_kwargs=api_kwargs)
         self.position: int = position
         self.user: User = user
         self.score: int = score
 
         self._id_attrs = (self.position, self.user, self.score)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardbutton.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinekeyboardbutton.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram InlineKeyboardButton."""
 
-from typing import TYPE_CHECKING, ClassVar, Optional, Union
+from typing import TYPE_CHECKING, Final, Optional, Union
 
 from telegram import constants
 from telegram._games.callbackgame import CallbackGame
 from telegram._loginurl import LoginUrl
 from telegram._switchinlinequerychosenchat import SwitchInlineQueryChosenChat
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
@@ -216,25 +216,25 @@
         "web_app",
         "switch_inline_query_chosen_chat",
     )
 
     def __init__(
         self,
         text: str,
-        url: str = None,
-        callback_data: Union[str, object] = None,
-        switch_inline_query: str = None,
-        switch_inline_query_current_chat: str = None,
-        callback_game: CallbackGame = None,
-        pay: bool = None,
-        login_url: LoginUrl = None,
-        web_app: WebAppInfo = None,
-        switch_inline_query_chosen_chat: SwitchInlineQueryChosenChat = None,
+        url: Optional[str] = None,
+        callback_data: Optional[Union[str, object]] = None,
+        switch_inline_query: Optional[str] = None,
+        switch_inline_query_current_chat: Optional[str] = None,
+        callback_game: Optional[CallbackGame] = None,
+        pay: Optional[bool] = None,
+        login_url: Optional[LoginUrl] = None,
+        web_app: Optional[WebAppInfo] = None,
+        switch_inline_query_chosen_chat: Optional[SwitchInlineQueryChosenChat] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.text: str = text
 
         # Optionals
         self.url: Optional[str] = url
@@ -293,17 +293,17 @@
         Args:
             callback_data (:class:`object`): The new callback data.
         """
         with self._unfrozen():
             self.callback_data = callback_data
             self._set_id_attrs()
 
-    MIN_CALLBACK_DATA: ClassVar[int] = constants.InlineKeyboardButtonLimit.MIN_CALLBACK_DATA
+    MIN_CALLBACK_DATA: Final[int] = constants.InlineKeyboardButtonLimit.MIN_CALLBACK_DATA
     """:const:`telegram.constants.InlineKeyboardButtonLimit.MIN_CALLBACK_DATA`
 
     .. versionadded:: 20.0
     """
-    MAX_CALLBACK_DATA: ClassVar[int] = constants.InlineKeyboardButtonLimit.MAX_CALLBACK_DATA
+    MAX_CALLBACK_DATA: Final[int] = constants.InlineKeyboardButtonLimit.MAX_CALLBACK_DATA
     """:const:`telegram.constants.InlineKeyboardButtonLimit.MAX_CALLBACK_DATA`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardmarkup.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinekeyboardmarkup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     __slots__ = ("inline_keyboard",)
 
     def __init__(
         self,
         inline_keyboard: Sequence[Sequence[InlineKeyboardButton]],
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         if not check_keyboard_type(inline_keyboard):
             raise ValueError(
                 "The parameter `inline_keyboard` should be a sequence of sequences of "
                 "InlineKeyboardButtons"
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequery.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequery.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram InlineQuery."""
 
-from typing import TYPE_CHECKING, Callable, ClassVar, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Callable, Final, Optional, Sequence, Union
 
 from telegram import constants
 from telegram._files.location import Location
 from telegram._inline.inlinequeryresultsbutton import InlineQueryResultsButton
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.defaultvalue import DEFAULT_NONE
@@ -100,18 +100,18 @@
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         from_user: User,
         query: str,
         offset: str,
-        location: Location = None,
-        chat_type: str = None,
+        location: Optional[Location] = None,
+        chat_type: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.id: str = id  # pylint: disable=invalid-name
         self.from_user: User = from_user
         self.query: str = query
         self.offset: str = offset
@@ -138,28 +138,28 @@
         return super().de_json(data=data, bot=bot)
 
     async def answer(
         self,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
-        cache_time: int = None,
-        is_personal: bool = None,
-        next_offset: str = None,
-        switch_pm_text: str = None,
-        switch_pm_parameter: str = None,
-        button: InlineQueryResultsButton = None,
+        cache_time: Optional[int] = None,
+        is_personal: Optional[bool] = None,
+        next_offset: Optional[str] = None,
+        switch_pm_text: Optional[str] = None,
+        switch_pm_parameter: Optional[str] = None,
+        button: Optional[InlineQueryResultsButton] = None,
         *,
-        current_offset: str = None,
+        current_offset: Optional[str] = None,
         auto_pagination: bool = False,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await bot.answer_inline_query(
                 update.inline_query.id,
                 *args,
                 current_offset=self.offset if auto_pagination else None,
@@ -198,32 +198,32 @@
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-    MAX_RESULTS: ClassVar[int] = constants.InlineQueryLimit.RESULTS
+    MAX_RESULTS: Final[int] = constants.InlineQueryLimit.RESULTS
     """:const:`telegram.constants.InlineQueryLimit.RESULTS`
 
     .. versionadded:: 13.2
     """
-    MIN_SWITCH_PM_TEXT_LENGTH: ClassVar[int] = constants.InlineQueryLimit.MIN_SWITCH_PM_TEXT_LENGTH
+    MIN_SWITCH_PM_TEXT_LENGTH: Final[int] = constants.InlineQueryLimit.MIN_SWITCH_PM_TEXT_LENGTH
     """:const:`telegram.constants.InlineQueryLimit.MIN_SWITCH_PM_TEXT_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_SWITCH_PM_TEXT_LENGTH: ClassVar[int] = constants.InlineQueryLimit.MAX_SWITCH_PM_TEXT_LENGTH
+    MAX_SWITCH_PM_TEXT_LENGTH: Final[int] = constants.InlineQueryLimit.MAX_SWITCH_PM_TEXT_LENGTH
     """:const:`telegram.constants.InlineQueryLimit.MAX_SWITCH_PM_TEXT_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_OFFSET_LENGTH: ClassVar[int] = constants.InlineQueryLimit.MAX_OFFSET_LENGTH
+    MAX_OFFSET_LENGTH: Final[int] = constants.InlineQueryLimit.MAX_OFFSET_LENGTH
     """:const:`telegram.constants.InlineQueryLimit.MAX_OFFSET_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_QUERY_LENGTH: ClassVar[int] = constants.InlineQueryLimit.MAX_QUERY_LENGTH
+    MAX_QUERY_LENGTH: Final[int] = constants.InlineQueryLimit.MAX_QUERY_LENGTH
     """:const:`telegram.constants.InlineQueryLimit.MAX_QUERY_LENGTH`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresult.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresult.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=redefined-builtin
 """This module contains the classes that represent Telegram InlineQueryResult."""
 
-from typing import ClassVar
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class InlineQueryResult(TelegramObject):
@@ -51,28 +51,28 @@
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
 
     """
 
     __slots__ = ("type", "id")
 
-    def __init__(self, type: str, id: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, type: str, id: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.type: str = type
         self.id: str = str(id)  # pylint: disable=invalid-name
 
         self._id_attrs = (self.id,)
 
         self._freeze()
 
-    MIN_ID_LENGTH: ClassVar[int] = constants.InlineQueryResultLimit.MIN_ID_LENGTH
+    MIN_ID_LENGTH: Final[int] = constants.InlineQueryResultLimit.MIN_ID_LENGTH
     """:const:`telegram.constants.InlineQueryResultLimit.MIN_ID_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_ID_LENGTH: ClassVar[int] = constants.InlineQueryResultLimit.MAX_ID_LENGTH
+    MAX_ID_LENGTH: Final[int] = constants.InlineQueryResultLimit.MAX_ID_LENGTH
     """:const:`telegram.constants.InlineQueryResultLimit.MAX_ID_LENGTH`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultarticle.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultarticle.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,26 +113,26 @@
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         title: str,
         input_message_content: "InputMessageContent",
-        reply_markup: InlineKeyboardMarkup = None,
-        url: str = None,
-        hide_url: bool = None,
-        description: str = None,
-        thumb_url: str = None,
-        thumb_width: int = None,
-        thumb_height: int = None,
-        thumbnail_url: str = None,
-        thumbnail_width: int = None,
-        thumbnail_height: int = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        url: Optional[str] = None,
+        hide_url: Optional[bool] = None,
+        description: Optional[str] = None,
+        thumb_url: Optional[str] = None,
+        thumb_width: Optional[int] = None,
+        thumb_height: Optional[int] = None,
+        thumbnail_url: Optional[str] = None,
+        thumbnail_width: Optional[int] = None,
+        thumbnail_height: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.ARTICLE, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.title: str = title
             self.input_message_content: InputMessageContent = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultaudio.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedaudio.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,67 +12,62 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultAudio."""
+"""This module contains the classes that represent Telegram InlineQueryResultCachedAudio."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultAudio(InlineQueryResult):
+class InlineQueryResultCachedAudio(InlineQueryResult):
     """
-    Represents a link to an mp3 audio file. By default, this audio file will be sent by the user.
-    Alternatively, you can use :attr:`input_message_content` to send a message with the specified
-    content instead of the audio.
+    Represents a link to an mp3 audio file stored on the Telegram servers. By default, this audio
+    file will be sent by the user. Alternatively, you can use :attr:`input_message_content` to
+    send a message with the specified content instead of the audio.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        audio_url (:obj:`str`): A valid URL for the audio file.
-        title (:obj:`str`): Title.
-        performer (:obj:`str`, optional): Performer.
-        audio_duration (:obj:`str`, optional): Audio duration in seconds.
+        audio_file_id (:obj:`str`): A valid file identifier for the audio file.
         caption (:obj:`str`, optional): Caption,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
             parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
         caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
+
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
             message to be sent instead of the audio.
 
     Attributes:
         type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.AUDIO`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        audio_url (:obj:`str`): A valid URL for the audio file.
-        title (:obj:`str`): Title.
-        performer (:obj:`str`): Optional. Performer.
-        audio_duration (:obj:`str`): Optional. Audio duration in seconds.
+        audio_file_id (:obj:`str`): A valid file identifier for the audio file.
         caption (:obj:`str`): Optional. Caption,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
             parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
         caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
 
             .. versionchanged:: 20.0
@@ -86,44 +81,35 @@
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
         "caption",
-        "title",
         "parse_mode",
-        "audio_url",
-        "performer",
+        "audio_file_id",
         "input_message_content",
-        "audio_duration",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        audio_url: str,
-        title: str,
-        performer: str = None,
-        audio_duration: int = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        audio_file_id: str,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.AUDIO, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.audio_url: str = audio_url
-            self.title: str = title
+            self.audio_file_id: str = audio_file_id
 
             # Optionals
-            self.performer: Optional[str] = performer
-            self.audio_duration: Optional[int] = audio_duration
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
             self.input_message_content: Optional[InputMessageContent] = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedaudio.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedgif.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,104 +12,110 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultCachedAudio."""
+"""This module contains the classes that represent Telegram InlineQueryResultCachedGif."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultCachedAudio(InlineQueryResult):
+class InlineQueryResultCachedGif(InlineQueryResult):
     """
-    Represents a link to an mp3 audio file stored on the Telegram servers. By default, this audio
-    file will be sent by the user. Alternatively, you can use :attr:`input_message_content` to
-    send a message with the specified content instead of the audio.
+    Represents a link to an animated GIF file stored on the Telegram servers. By default, this
+    animated GIF file will be sent by the user with an optional caption. Alternatively, you can
+    use :attr:`input_message_content` to send a message with specified content instead of
+    the animation.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        audio_file_id (:obj:`str`): A valid file identifier for the audio file.
-        caption (:obj:`str`, optional): Caption,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
-            parsing.
+        gif_file_id (:obj:`str`): A valid file identifier for the GIF file.
+        title (:obj:`str`, optional): Title for the result.
+        caption (:obj:`str`, optional): Caption of the GIF file to be sent,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
+            after entities parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
         caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
-            message to be sent instead of the audio.
+            message to be sent instead of the gif.
 
     Attributes:
-        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.AUDIO`.
+        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.GIF`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        audio_file_id (:obj:`str`): A valid file identifier for the audio file.
-        caption (:obj:`str`): Optional. Caption,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
-            parsing.
+        gif_file_id (:obj:`str`): A valid file identifier for the GIF file.
+        title (:obj:`str`): Optional. Title for the result.
+        caption (:obj:`str`): Optional. Caption of the GIF file to be sent,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
+            after entities parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
         caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`): Optional. Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`): Optional. Content of the
-            message to be sent instead of the audio.
+            message to be sent instead of the gif.
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
         "caption",
-        "parse_mode",
-        "audio_file_id",
+        "title",
         "input_message_content",
+        "parse_mode",
+        "gif_file_id",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        audio_file_id: str,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        gif_file_id: str,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
-        super().__init__(InlineQueryResultType.AUDIO, id, api_kwargs=api_kwargs)
+        super().__init__(InlineQueryResultType.GIF, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.audio_file_id: str = audio_file_id
+            self.gif_file_id: str = gif_file_id
 
             # Optionals
+            self.title: Optional[str] = title
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
             self.input_message_content: Optional[InputMessageContent] = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcacheddocument.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcacheddocument.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,22 +97,22 @@
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         title: str,
         document_file_id: str,
-        description: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        description: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.DOCUMENT, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.title: str = title
             self.document_file_id: str = document_file_id
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedgif.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedmpeg4gif.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,109 +12,109 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultCachedGif."""
+"""This module contains the classes that represent Telegram InlineQueryResultMpeg4Gif."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultCachedGif(InlineQueryResult):
+class InlineQueryResultCachedMpeg4Gif(InlineQueryResult):
     """
-    Represents a link to an animated GIF file stored on the Telegram servers. By default, this
-    animated GIF file will be sent by the user with an optional caption. Alternatively, you can
-    use :attr:`input_message_content` to send a message with specified content instead of
-    the animation.
+    Represents a link to a video animation (H.264/MPEG-4 AVC video without sound) stored on the
+    Telegram servers. By default, this animated MPEG-4 file will be sent by the user with an
+    optional caption. Alternatively, you can use :attr:`input_message_content` to send a message
+    with the specified content instead of the animation.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        gif_file_id (:obj:`str`): A valid file identifier for the GIF file.
+        mpeg4_file_id (:obj:`str`): A valid file identifier for the MP4 file.
         title (:obj:`str`, optional): Title for the result.
-        caption (:obj:`str`, optional): Caption of the GIF file to be sent,
+        caption (:obj:`str`, optional): Caption of the MPEG-4 file to be sent,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
             after entities parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
         caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
-            message to be sent instead of the gif.
+            message to be sent instead of the MPEG-4 file.
 
     Attributes:
-        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.GIF`.
+        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.MPEG4GIF`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        gif_file_id (:obj:`str`): A valid file identifier for the GIF file.
+        mpeg4_file_id (:obj:`str`): A valid file identifier for the MP4 file.
         title (:obj:`str`): Optional. Title for the result.
-        caption (:obj:`str`): Optional. Caption of the GIF file to be sent,
+        caption (:obj:`str`): Optional. Caption of the MPEG-4 file to be sent,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
             after entities parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
         caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`): Optional. Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`): Optional. Content of the
-            message to be sent instead of the gif.
+            message to be sent instead of the MPEG-4 file.
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
+        "mpeg4_file_id",
         "caption",
         "title",
-        "input_message_content",
         "parse_mode",
-        "gif_file_id",
+        "input_message_content",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        gif_file_id: str,
-        title: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        mpeg4_file_id: str,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
-        super().__init__(InlineQueryResultType.GIF, id, api_kwargs=api_kwargs)
+        super().__init__(InlineQueryResultType.MPEG4GIF, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.gif_file_id: str = gif_file_id
+            self.mpeg4_file_id: str = mpeg4_file_id
 
             # Optionals
             self.title: Optional[str] = title
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedmpeg4gif.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedvideo.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,110 +12,111 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultMpeg4Gif."""
+"""This module contains the classes that represent Telegram InlineQueryResultCachedVideo."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultCachedMpeg4Gif(InlineQueryResult):
+class InlineQueryResultCachedVideo(InlineQueryResult):
     """
-    Represents a link to a video animation (H.264/MPEG-4 AVC video without sound) stored on the
-    Telegram servers. By default, this animated MPEG-4 file will be sent by the user with an
-    optional caption. Alternatively, you can use :attr:`input_message_content` to send a message
-    with the specified content instead of the animation.
+    Represents a link to a video file stored on the Telegram servers. By default, this video file
+    will be sent by the user with an optional caption. Alternatively, you can use
+    :attr:`input_message_content` to send a message with the specified content instead
+    of the video.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        mpeg4_file_id (:obj:`str`): A valid file identifier for the MP4 file.
-        title (:obj:`str`, optional): Title for the result.
-        caption (:obj:`str`, optional): Caption of the MPEG-4 file to be sent,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
-            after entities parsing.
+        video_file_id (:obj:`str`): A valid file identifier for the video file.
+        title (:obj:`str`): Title for the result.
+        description (:obj:`str`, optional): Short description of the result.
+        caption (:obj:`str`, optional): Caption of the video to be sent,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after
+            entities parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
         caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
-
-            .. versionchanged:: 20.0
-                |sequenceclassargs|
-
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
-            message to be sent instead of the MPEG-4 file.
+            message to be sent instead of the video.
 
     Attributes:
-        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.MPEG4GIF`.
+        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.VIDEO`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        mpeg4_file_id (:obj:`str`): A valid file identifier for the MP4 file.
-        title (:obj:`str`): Optional. Title for the result.
-        caption (:obj:`str`): Optional. Caption of the MPEG-4 file to be sent,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters
-            after entities parsing.
+        video_file_id (:obj:`str`): A valid file identifier for the video file.
+        title (:obj:`str`): Title for the result.
+        description (:obj:`str`): Optional. Short description of the result.
+        caption (:obj:`str`): Optional. Caption of the video to be sent,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after
+            entities parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
         caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`): Optional. Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`): Optional. Content of the
-            message to be sent instead of the MPEG-4 file.
+            message to be sent instead of the video.
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
-        "mpeg4_file_id",
         "caption",
         "title",
+        "description",
         "parse_mode",
         "input_message_content",
+        "video_file_id",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        mpeg4_file_id: str,
-        title: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        video_file_id: str,
+        title: str,
+        description: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
-        super().__init__(InlineQueryResultType.MPEG4GIF, id, api_kwargs=api_kwargs)
+        super().__init__(InlineQueryResultType.VIDEO, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.mpeg4_file_id: str = mpeg4_file_id
+            self.video_file_id: str = video_file_id
+            self.title: str = title
 
             # Optionals
-            self.title: Optional[str] = title
+            self.description: Optional[str] = description
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
             self.input_message_content: Optional[InputMessageContent] = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedphoto.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedphoto.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,23 +97,23 @@
         "input_message_content",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         photo_file_id: str,
-        title: str = None,
-        description: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.PHOTO, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.photo_file_id: str = photo_file_id
 
             # Optionals
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedsticker.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedsticker.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 
     __slots__ = ("reply_markup", "input_message_content", "sticker_file_id")
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         sticker_file_id: str,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.STICKER, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.sticker_file_id: str = sticker_file_id
 
             # Optionals
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvideo.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcachedvoice.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,111 +12,109 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultCachedVideo."""
+"""This module contains the classes that represent Telegram InlineQueryResultCachedVoice."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultCachedVideo(InlineQueryResult):
+class InlineQueryResultCachedVoice(InlineQueryResult):
     """
-    Represents a link to a video file stored on the Telegram servers. By default, this video file
-    will be sent by the user with an optional caption. Alternatively, you can use
-    :attr:`input_message_content` to send a message with the specified content instead
-    of the video.
+    Represents a link to a voice message stored on the Telegram servers. By default, this voice
+    message will be sent by the user. Alternatively, you can use :attr:`input_message_content` to
+    send a message with the specified content instead of the voice message.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        video_file_id (:obj:`str`): A valid file identifier for the video file.
-        title (:obj:`str`): Title for the result.
-        description (:obj:`str`, optional): Short description of the result.
-        caption (:obj:`str`, optional): Caption of the video to be sent,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after
-            entities parsing.
+        voice_file_id (:obj:`str`): A valid file identifier for the voice message.
+        title (:obj:`str`): Voice message title.
+        caption (:obj:`str`, optional): Caption,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
+            parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
-        caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
+        caption_entities (Sequence[:class:`telegram.MessageEntity`], optional):
+            |captionentitiesattr|
+
+            .. versionchanged:: 20.0
+                |sequenceclassargs|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
-            message to be sent instead of the video.
+            message to be sent instead of the voice message.
 
     Attributes:
-        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.VIDEO`.
+        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.VOICE`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        video_file_id (:obj:`str`): A valid file identifier for the video file.
-        title (:obj:`str`): Title for the result.
-        description (:obj:`str`): Optional. Short description of the result.
-        caption (:obj:`str`): Optional. Caption of the video to be sent,
-            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after
-            entities parsing.
+        voice_file_id (:obj:`str`): A valid file identifier for the voice message.
+        title (:obj:`str`): Voice message title.
+        caption (:obj:`str`): Optional. Caption,
+            0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
+            parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
-        caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
+        caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |caption_entities|
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`): Optional. Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`): Optional. Content of the
-            message to be sent instead of the video.
+            message to be sent instead of the voice message.
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
         "caption",
         "title",
-        "description",
         "parse_mode",
+        "voice_file_id",
         "input_message_content",
-        "video_file_id",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        video_file_id: str,
+        voice_file_id: str,
         title: str,
-        description: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
-        super().__init__(InlineQueryResultType.VIDEO, id, api_kwargs=api_kwargs)
+        super().__init__(InlineQueryResultType.VOICE, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.video_file_id: str = video_file_id
+            self.voice_file_id: str = voice_file_id
             self.title: str = title
 
             # Optionals
-            self.description: Optional[str] = description
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
             self.input_message_content: Optional[InputMessageContent] = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvoice.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultaudio.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,109 +12,118 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
-"""This module contains the classes that represent Telegram InlineQueryResultCachedVoice."""
+"""This module contains the classes that represent Telegram InlineQueryResultAudio."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 from telegram.constants import InlineQueryResultType
 
 if TYPE_CHECKING:
     from telegram import InputMessageContent
 
 
-class InlineQueryResultCachedVoice(InlineQueryResult):
+class InlineQueryResultAudio(InlineQueryResult):
     """
-    Represents a link to a voice message stored on the Telegram servers. By default, this voice
-    message will be sent by the user. Alternatively, you can use :attr:`input_message_content` to
-    send a message with the specified content instead of the voice message.
+    Represents a link to an mp3 audio file. By default, this audio file will be sent by the user.
+    Alternatively, you can use :attr:`input_message_content` to send a message with the specified
+    content instead of the audio.
 
     .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
     Args:
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        voice_file_id (:obj:`str`): A valid file identifier for the voice message.
-        title (:obj:`str`): Voice message title.
+        audio_url (:obj:`str`): A valid URL for the audio file.
+        title (:obj:`str`): Title.
+        performer (:obj:`str`, optional): Performer.
+        audio_duration (:obj:`str`, optional): Audio duration in seconds.
         caption (:obj:`str`, optional): Caption,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
             parsing.
         parse_mode (:obj:`str`, optional): |parse_mode|
-        caption_entities (Sequence[:class:`telegram.MessageEntity`], optional):
-            |captionentitiesattr|
+        caption_entities (Sequence[:class:`telegram.MessageEntity`], optional): |caption_entities|
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`, optional): Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`, optional): Content of the
-            message to be sent instead of the voice message.
+            message to be sent instead of the audio.
 
     Attributes:
-        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.VOICE`.
+        type (:obj:`str`): :tg-const:`telegram.constants.InlineQueryResultType.AUDIO`.
         id (:obj:`str`): Unique identifier for this result,
             :tg-const:`telegram.InlineQueryResult.MIN_ID_LENGTH`-
             :tg-const:`telegram.InlineQueryResult.MAX_ID_LENGTH` Bytes.
-        voice_file_id (:obj:`str`): A valid file identifier for the voice message.
-        title (:obj:`str`): Voice message title.
+        audio_url (:obj:`str`): A valid URL for the audio file.
+        title (:obj:`str`): Title.
+        performer (:obj:`str`): Optional. Performer.
+        audio_duration (:obj:`str`): Optional. Audio duration in seconds.
         caption (:obj:`str`): Optional. Caption,
             0-:tg-const:`telegram.constants.MessageLimit.CAPTION_LENGTH` characters after entities
             parsing.
         parse_mode (:obj:`str`): Optional. |parse_mode|
-        caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |caption_entities|
+        caption_entities (Tuple[:class:`telegram.MessageEntity`]): Optional. |captionentitiesattr|
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
         reply_markup (:class:`telegram.InlineKeyboardMarkup`): Optional. Inline keyboard attached
             to the message.
         input_message_content (:class:`telegram.InputMessageContent`): Optional. Content of the
-            message to be sent instead of the voice message.
+            message to be sent instead of the audio.
 
     """
 
     __slots__ = (
         "reply_markup",
         "caption_entities",
         "caption",
         "title",
         "parse_mode",
-        "voice_file_id",
+        "audio_url",
+        "performer",
         "input_message_content",
+        "audio_duration",
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
-        voice_file_id: str,
+        audio_url: str,
         title: str,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        performer: Optional[str] = None,
+        audio_duration: Optional[int] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
-        super().__init__(InlineQueryResultType.VOICE, id, api_kwargs=api_kwargs)
+        super().__init__(InlineQueryResultType.AUDIO, id, api_kwargs=api_kwargs)
         with self._unfrozen():
-            self.voice_file_id: str = voice_file_id
+            self.audio_url: str = audio_url
             self.title: str = title
 
             # Optionals
+            self.performer: Optional[str] = performer
+            self.audio_duration: Optional[int] = audio_duration
             self.caption: Optional[str] = caption
             self.parse_mode: ODVInput[str] = parse_mode
             self.caption_entities: Tuple[MessageEntity, ...] = parse_sequence_arg(caption_entities)
             self.reply_markup: Optional[InlineKeyboardMarkup] = reply_markup
             self.input_message_content: Optional[InputMessageContent] = input_message_content
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcontact.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultcontact.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,26 +113,26 @@
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         phone_number: str,
         first_name: str,
-        last_name: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = None,
-        thumb_height: int = None,
-        vcard: str = None,
-        thumbnail_url: str = None,
-        thumbnail_width: int = None,
-        thumbnail_height: int = None,
+        last_name: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        thumb_url: Optional[str] = None,
+        thumb_width: Optional[int] = None,
+        thumb_height: Optional[int] = None,
+        vcard: Optional[str] = None,
+        thumbnail_url: Optional[str] = None,
+        thumbnail_width: Optional[int] = None,
+        thumbnail_height: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.CONTACT, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.phone_number: str = phone_number
             self.first_name: str = first_name
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultdocument.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultdocument.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,28 +142,28 @@
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         document_url: str,
         title: str,
         mime_type: str,
-        caption: str = None,
-        description: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = None,
-        thumb_height: int = None,
+        caption: Optional[str] = None,
+        description: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        thumb_url: Optional[str] = None,
+        thumb_width: Optional[int] = None,
+        thumb_height: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
-        thumbnail_url: str = None,
-        thumbnail_width: int = None,
-        thumbnail_height: int = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        thumbnail_url: Optional[str] = None,
+        thumbnail_width: Optional[int] = None,
+        thumbnail_height: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.DOCUMENT, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.document_url: str = document_url
             self.title: str = title
             self.mime_type: str = mime_type
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgame.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultgame.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 
     __slots__ = ("reply_markup", "game_short_name")
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         game_short_name: str,
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.GAME, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.id: str = id
             self.game_short_name: str = game_short_name
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgif.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultgif.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,30 +147,30 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         gif_url: str,
         # thumbnail_url is not optional in Telegram API, but we want to support thumb_url as well,
         # so thumbnail_url may not be passed.  We will raise ValueError manually if neither
         # thumbnail_url nor thumb_url are passed
-        thumbnail_url: str = None,
-        gif_width: int = None,
-        gif_height: int = None,
-        title: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        gif_duration: int = None,
+        thumbnail_url: Optional[str] = None,
+        gif_width: Optional[int] = None,
+        gif_height: Optional[int] = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        gif_duration: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb_mime_type: str = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        thumbnail_mime_type: str = None,
+        thumb_mime_type: Optional[str] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        thumbnail_mime_type: Optional[str] = None,
         # thumb_url is not optional in Telegram API, but it is here, along with thumbnail_url.
-        thumb_url: str = None,
+        thumb_url: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if not (thumbnail_url or thumb_url):
             raise ValueError(
                 "You must pass either 'thumbnail_url' or 'thumb_url'. Note that 'thumb_url' is "
                 "deprecated."
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultlocation.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultlocation.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains the classes that represent Telegram InlineQueryResultLocation."""
 
-from typing import TYPE_CHECKING, ClassVar, Optional
+from typing import TYPE_CHECKING, Final, Optional
 
 from telegram import constants
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
 from telegram._inline.inlinequeryresult import InlineQueryResult
 from telegram._utils.types import JSONDict
 from telegram._utils.warnings_transition import (
     warn_about_deprecated_arg_return_new_arg,
@@ -145,28 +145,28 @@
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         latitude: float,
         longitude: float,
         title: str,
-        live_period: int = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = None,
-        thumb_height: int = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
-        thumbnail_url: str = None,
-        thumbnail_width: int = None,
-        thumbnail_height: int = None,
+        live_period: Optional[int] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        thumb_url: Optional[str] = None,
+        thumb_width: Optional[int] = None,
+        thumb_height: Optional[int] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
+        thumbnail_url: Optional[str] = None,
+        thumbnail_width: Optional[int] = None,
+        thumbnail_height: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(constants.InlineQueryResultType.LOCATION, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.latitude: float = latitude
             self.longitude: float = longitude
             self.title: str = title
@@ -240,42 +240,42 @@
         warn_about_deprecated_attr_in_property(
             deprecated_attr_name="thumb_height",
             new_attr_name="thumbnail_height",
             bot_api_version="6.6",
         )
         return self.thumbnail_height
 
-    HORIZONTAL_ACCURACY: ClassVar[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
+    HORIZONTAL_ACCURACY: Final[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
     """:const:`telegram.constants.LocationLimit.HORIZONTAL_ACCURACY`
 
     .. versionadded:: 20.0
     """
-    MIN_HEADING: ClassVar[int] = constants.LocationLimit.MIN_HEADING
+    MIN_HEADING: Final[int] = constants.LocationLimit.MIN_HEADING
     """:const:`telegram.constants.LocationLimit.MIN_HEADING`
 
     .. versionadded:: 20.0
     """
-    MAX_HEADING: ClassVar[int] = constants.LocationLimit.MAX_HEADING
+    MAX_HEADING: Final[int] = constants.LocationLimit.MAX_HEADING
     """:const:`telegram.constants.LocationLimit.MAX_HEADING`
 
     .. versionadded:: 20.0
     """
-    MIN_LIVE_PERIOD: ClassVar[int] = constants.LocationLimit.MIN_LIVE_PERIOD
+    MIN_LIVE_PERIOD: Final[int] = constants.LocationLimit.MIN_LIVE_PERIOD
     """:const:`telegram.constants.LocationLimit.MIN_LIVE_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MAX_LIVE_PERIOD: ClassVar[int] = constants.LocationLimit.MAX_LIVE_PERIOD
+    MAX_LIVE_PERIOD: Final[int] = constants.LocationLimit.MAX_LIVE_PERIOD
     """:const:`telegram.constants.LocationLimit.MAX_LIVE_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MIN_PROXIMITY_ALERT_RADIUS: ClassVar[int] = constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS
+    MIN_PROXIMITY_ALERT_RADIUS: Final[int] = constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS
     """:const:`telegram.constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS`
 
     .. versionadded:: 20.0
     """
-    MAX_PROXIMITY_ALERT_RADIUS: ClassVar[int] = constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS
+    MAX_PROXIMITY_ALERT_RADIUS: Final[int] = constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS
     """:const:`telegram.constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultmpeg4gif.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultmpeg4gif.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,30 +140,30 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         mpeg4_url: str,
         # thumbnail_url is not optional in Telegram API, but we want to support thumb_url as well,
         # so thumbnail_url may not be passed.  We will raise ValueError manually if neither
         # thumbnail_url nor thumb_url are passed
-        thumbnail_url: str = None,
-        mpeg4_width: int = None,
-        mpeg4_height: int = None,
-        title: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        mpeg4_duration: int = None,
+        thumbnail_url: Optional[str] = None,
+        mpeg4_width: Optional[int] = None,
+        mpeg4_height: Optional[int] = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        mpeg4_duration: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb_mime_type: str = None,
-        caption_entities: Sequence[MessageEntity] = None,
-        thumbnail_mime_type: str = None,
+        thumb_mime_type: Optional[str] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
+        thumbnail_mime_type: Optional[str] = None,
         # thumb_url is not optional in Telegram API, but it is here, along with thumbnail_url.
-        thumb_url: str = None,
+        thumb_url: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if not (thumbnail_url or thumb_url):
             raise ValueError(
                 "You must pass either 'thumbnail_url' or 'thumb_url'. Note that 'thumb_url' is "
                 "deprecated."
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultphoto.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultphoto.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,28 +130,28 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         photo_url: str,
         # thumbnail_url is not optional in Telegram API, but we want to support thumb_url as well,
         # so thumbnail_url may not be passed.  We will raise ValueError manually if neither
         # thumbnail_url nor thumb_url are passed
-        thumbnail_url: str = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        title: str = None,
-        description: str = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        thumbnail_url: Optional[str] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         # thumb_url is not optional in Telegram API, but it is here, along with thumbnail_url.
-        thumb_url: str = None,
+        thumb_url: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if not (thumbnail_url or thumb_url):
             raise ValueError(
                 "You must pass either 'thumbnail_url' or 'thumb_url'. Note that 'thumb_url' is "
                 "deprecated."
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultsbutton.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultsbutton.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=redefined-builtin
 """This module contains the class that represent a Telegram InlineQueryResultsButton."""
 
-from typing import TYPE_CHECKING, ClassVar, Optional
+from typing import TYPE_CHECKING, Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 from telegram._webappinfo import WebAppInfo
 
 if TYPE_CHECKING:
@@ -75,18 +75,18 @@
     """
 
     __slots__ = ("text", "web_app", "start_parameter")
 
     def __init__(
         self,
         text: str,
-        web_app: WebAppInfo = None,
-        start_parameter: str = None,
+        web_app: Optional[WebAppInfo] = None,
+        start_parameter: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.text: str = text
 
         # Optional
@@ -103,15 +103,15 @@
         if not data:
             return None
 
         data["web_app"] = WebAppInfo.de_json(data.get("web_app"), bot)
 
         return super().de_json(data=data, bot=bot)
 
-    MIN_START_PARAMETER_LENGTH: ClassVar[
+    MIN_START_PARAMETER_LENGTH: Final[
         int
     ] = constants.InlineQueryResultsButtonLimit.MIN_START_PARAMETER_LENGTH
     """:const:`telegram.constants.InlineQueryResultsButtonLimit.MIN_START_PARAMETER_LENGTH`"""
-    MAX_START_PARAMETER_LENGTH: ClassVar[
+    MAX_START_PARAMETER_LENGTH: Final[
         int
     ] = constants.InlineQueryResultsButtonLimit.MAX_START_PARAMETER_LENGTH
     """:const:`telegram.constants.InlineQueryResultsButtonLimit.MAX_START_PARAMETER_LENGTH`"""
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvenue.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvenue.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,28 +137,28 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         latitude: float,
         longitude: float,
         title: str,
         address: str,
-        foursquare_id: str = None,
-        foursquare_type: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = None,
-        thumb_height: int = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
-        thumbnail_url: str = None,
-        thumbnail_width: int = None,
-        thumbnail_height: int = None,
+        foursquare_id: Optional[str] = None,
+        foursquare_type: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
+        thumb_url: Optional[str] = None,
+        thumb_width: Optional[int] = None,
+        thumb_height: Optional[int] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
+        thumbnail_url: Optional[str] = None,
+        thumbnail_width: Optional[int] = None,
+        thumbnail_height: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.VENUE, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.latitude: float = latitude
             self.longitude: float = longitude
             self.title: str = title
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvideo.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvideo.py`

 * *Files 7% similar despite different names*

```diff
@@ -155,31 +155,31 @@
         self,
         id: str,  # pylint: disable=redefined-builtin
         video_url: str,
         mime_type: str,
         # thumbnail_url and title are not optional in Telegram API, but we want to support
         # thumb_url as well, so thumbnail_url may not be passed if thumb_url is passed.
         # We will raise ValueError manually if neither thumbnail_url nor thumb_url are passed.
-        thumbnail_url: str = None,
+        thumbnail_url: Optional[str] = None,
         # title had to be made optional because of thumbnail_url. This is compensated by raising
         # TypeError manually if title is not passed.
-        title: str = None,
-        caption: str = None,
-        video_width: int = None,
-        video_height: int = None,
-        video_duration: int = None,
-        description: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
+        video_width: Optional[int] = None,
+        video_height: Optional[int] = None,
+        video_duration: Optional[int] = None,
+        description: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         # thumb_url is not optional in Telegram API, but it is here, along with thumbnail_url.
-        thumb_url: str = None,
+        thumb_url: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         if not (thumbnail_url or thumb_url):
             raise ValueError(
                 "You must pass either 'thumbnail_url' or 'thumb_url'. Note that 'thumb_url' is "
                 "deprecated."
             )
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvoice.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inlinequeryresultvoice.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,22 +98,22 @@
     )
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         voice_url: str,
         title: str,
-        voice_duration: int = None,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        input_message_content: "InputMessageContent" = None,
+        voice_duration: Optional[int] = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        input_message_content: Optional["InputMessageContent"] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence[MessageEntity] = None,
+        caption_entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__(InlineQueryResultType.VOICE, id, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.voice_url: str = voice_url
             self.title: str = title
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputcontactmessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputcontactmessagecontent.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 
     __slots__ = ("vcard", "first_name", "last_name", "phone_number")
 
     def __init__(
         self,
         phone_number: str,
         first_name: str,
-        last_name: str = None,
-        vcard: str = None,
+        last_name: Optional[str] = None,
+        vcard: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             # Required
             self.phone_number: str = phone_number
             self.first_name: str = first_name
             # Optionals
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputinvoicemessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputinvoicemessagecontent.py`

 * *Files 8% similar despite different names*

```diff
@@ -189,30 +189,30 @@
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: Sequence[LabeledPrice],
-        max_tip_amount: int = None,
-        suggested_tip_amounts: Sequence[int] = None,
-        provider_data: str = None,
-        photo_url: str = None,
-        photo_size: int = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        need_name: bool = None,
-        need_phone_number: bool = None,
-        need_email: bool = None,
-        need_shipping_address: bool = None,
-        send_phone_number_to_provider: bool = None,
-        send_email_to_provider: bool = None,
-        is_flexible: bool = None,
+        max_tip_amount: Optional[int] = None,
+        suggested_tip_amounts: Optional[Sequence[int]] = None,
+        provider_data: Optional[str] = None,
+        photo_url: Optional[str] = None,
+        photo_size: Optional[int] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        need_name: Optional[bool] = None,
+        need_phone_number: Optional[bool] = None,
+        need_email: Optional[bool] = None,
+        need_shipping_address: Optional[bool] = None,
+        send_phone_number_to_provider: Optional[bool] = None,
+        send_email_to_provider: Optional[bool] = None,
+        is_flexible: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             # Required
             self.title: str = title
             self.description: str = description
             self.payload: str = payload
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputlocationmessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputlocationmessagecontent.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains the classes that represent Telegram InputLocationMessageContent."""
 
-from typing import ClassVar, Optional
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._inline.inputmessagecontent import InputMessageContent
 from telegram._utils.types import JSONDict
 
 
 class InputLocationMessageContent(InputMessageContent):
@@ -79,20 +79,20 @@
                  'latitude', 'heading')
     # fmt: on
 
     def __init__(
         self,
         latitude: float,
         longitude: float,
-        live_period: int = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        live_period: Optional[int] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             # Required
             self.latitude: float = latitude
             self.longitude: float = longitude
 
@@ -102,42 +102,42 @@
             self.heading: Optional[int] = heading
             self.proximity_alert_radius: Optional[int] = (
                 int(proximity_alert_radius) if proximity_alert_radius else None
             )
 
             self._id_attrs = (self.latitude, self.longitude)
 
-    HORIZONTAL_ACCURACY: ClassVar[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
+    HORIZONTAL_ACCURACY: Final[int] = constants.LocationLimit.HORIZONTAL_ACCURACY
     """:const:`telegram.constants.LocationLimit.HORIZONTAL_ACCURACY`
 
     .. versionadded:: 20.0
     """
-    MIN_HEADING: ClassVar[int] = constants.LocationLimit.MIN_HEADING
+    MIN_HEADING: Final[int] = constants.LocationLimit.MIN_HEADING
     """:const:`telegram.constants.LocationLimit.MIN_HEADING`
 
     .. versionadded:: 20.0
     """
-    MAX_HEADING: ClassVar[int] = constants.LocationLimit.MAX_HEADING
+    MAX_HEADING: Final[int] = constants.LocationLimit.MAX_HEADING
     """:const:`telegram.constants.LocationLimit.MAX_HEADING`
 
     .. versionadded:: 20.0
     """
-    MIN_LIVE_PERIOD: ClassVar[int] = constants.LocationLimit.MIN_LIVE_PERIOD
+    MIN_LIVE_PERIOD: Final[int] = constants.LocationLimit.MIN_LIVE_PERIOD
     """:const:`telegram.constants.LocationLimit.MIN_LIVE_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MAX_LIVE_PERIOD: ClassVar[int] = constants.LocationLimit.MAX_LIVE_PERIOD
+    MAX_LIVE_PERIOD: Final[int] = constants.LocationLimit.MAX_LIVE_PERIOD
     """:const:`telegram.constants.LocationLimit.MAX_LIVE_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MIN_PROXIMITY_ALERT_RADIUS: ClassVar[int] = constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS
+    MIN_PROXIMITY_ALERT_RADIUS: Final[int] = constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS
     """:const:`telegram.constants.LocationLimit.MIN_PROXIMITY_ALERT_RADIUS`
 
     .. versionadded:: 20.0
     """
-    MAX_PROXIMITY_ALERT_RADIUS: ClassVar[int] = constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS
+    MAX_PROXIMITY_ALERT_RADIUS: Final[int] = constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS
     """:const:`telegram.constants.LocationLimit.MAX_PROXIMITY_ALERT_RADIUS`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputmessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputmessagecontent.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains the classes that represent Telegram InputMessageContent."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class InputMessageContent(TelegramObject):
     """Base class for Telegram InputMessageContent Objects.
 
@@ -30,11 +32,11 @@
     :class:`telegram.InputLocationMessageContent`, :class:`telegram.InputTextMessageContent` and
     :class:`telegram.InputVenueMessageContent` for more details.
 
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputtextmessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputtextmessagecontent.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains the classes that represent Telegram InputTextMessageContent."""
-from typing import Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 from telegram._inline.inputmessagecontent import InputMessageContent
 from telegram._messageentity import MessageEntity
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 
@@ -70,17 +70,17 @@
     __slots__ = ("disable_web_page_preview", "parse_mode", "entities", "message_text")
 
     def __init__(
         self,
         message_text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence[MessageEntity] = None,
+        entities: Optional[Sequence[MessageEntity]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             # Required
             self.message_text: str = message_text
             # Optionals
             self.parse_mode: ODVInput[str] = parse_mode
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_inline/inputvenuemessagecontent.py` & `python-telegram-bot-raw-20.4/telegram/_inline/inputvenuemessagecontent.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,20 +77,20 @@
 
     def __init__(
         self,
         latitude: float,
         longitude: float,
         title: str,
         address: str,
-        foursquare_id: str = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
+        foursquare_id: Optional[str] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             # Required
             self.latitude: float = latitude
             self.longitude: float = longitude
             self.title: str = title
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_keyboardbutton.py` & `python-telegram-bot-raw-20.4/telegram/_keyboardbutton.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,22 +127,22 @@
         "request_user",
         "request_chat",
     )
 
     def __init__(
         self,
         text: str,
-        request_contact: bool = None,
-        request_location: bool = None,
-        request_poll: KeyboardButtonPollType = None,
-        web_app: WebAppInfo = None,
-        request_user: KeyboardButtonRequestUser = None,
-        request_chat: KeyboardButtonRequestChat = None,
+        request_contact: Optional[bool] = None,
+        request_location: Optional[bool] = None,
+        request_poll: Optional[KeyboardButtonPollType] = None,
+        web_app: Optional[WebAppInfo] = None,
+        request_user: Optional[KeyboardButtonRequestUser] = None,
+        request_chat: Optional[KeyboardButtonRequestChat] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.text: str = text
         # Optionals
         self.request_contact: Optional[bool] = request_contact
         self.request_location: Optional[bool] = request_location
@@ -159,16 +159,16 @@
             self.web_app,
         )
 
         self._freeze()
 
     def __eq__(self, other: object) -> bool:
         warn(
-            "In v21, granular media settings will be considered as well when comparing"
-            " ChatPermissions instances.",
+            "In v21, `request_user` and `request_chat` will be considered as well when comparing"
+            " KeyboardButton instances.",
             PTBDeprecationWarning,
             stacklevel=2,
         )
         return super().__eq__(other)
 
     def __hash__(self) -> int:
         # Intend: Added so support the own __eq__ function (which otherwise breaks hashing)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_keyboardbuttonpolltype.py` & `python-telegram-bot-raw-20.4/telegram/_keyboardbuttonpolltype.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,15 +44,18 @@
             :tg-const:`telegram.Poll.REGULAR`, only regular polls will be allowed.
             Otherwise, the user will be allowed to create a poll of any type.
     """
 
     __slots__ = ("type",)
 
     def __init__(
-        self, type: str = None, *, api_kwargs: JSONDict = None  # skipcq: PYL-W0622
-    ):  # pylint: disable=redefined-builtin
+        self,
+        type: Optional[str] = None,  # pylint: disable=redefined-builtin
+        *,
+        api_kwargs: Optional[JSONDict] = None,  # skipcq: PYL-W0622
+    ):
         super().__init__(api_kwargs=api_kwargs)
         self.type: Optional[str] = type
 
         self._id_attrs = (self.type,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_keyboardbuttonrequest.py` & `python-telegram-bot-raw-20.4/telegram/_keyboardbuttonrequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,18 @@
         "user_is_bot",
         "user_is_premium",
     )
 
     def __init__(
         self,
         request_id: int,
-        user_is_bot: bool = None,
-        user_is_premium: bool = None,
+        user_is_bot: Optional[bool] = None,
+        user_is_premium: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,  # skipcq: PYL-W0622
+        api_kwargs: Optional[JSONDict] = None,  # skipcq: PYL-W0622
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.request_id: int = request_id
 
         # Optionals
         self.user_is_bot: Optional[bool] = user_is_bot
@@ -153,22 +153,22 @@
         "bot_is_member",
     )
 
     def __init__(
         self,
         request_id: int,
         chat_is_channel: bool,
-        chat_is_forum: bool = None,
-        chat_has_username: bool = None,
-        chat_is_created: bool = None,
-        user_administrator_rights: ChatAdministratorRights = None,
-        bot_administrator_rights: ChatAdministratorRights = None,
-        bot_is_member: bool = None,
+        chat_is_forum: Optional[bool] = None,
+        chat_has_username: Optional[bool] = None,
+        chat_is_created: Optional[bool] = None,
+        user_administrator_rights: Optional[ChatAdministratorRights] = None,
+        bot_administrator_rights: Optional[ChatAdministratorRights] = None,
+        bot_is_member: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,  # skipcq: PYL-W0622
+        api_kwargs: Optional[JSONDict] = None,  # skipcq: PYL-W0622
     ):
         super().__init__(api_kwargs=api_kwargs)
         # required
         self.request_id: int = request_id
         self.chat_is_channel: bool = chat_is_channel
 
         # optional
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_loginurl.py` & `python-telegram-bot-raw-20.4/telegram/_loginurl.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,19 +82,19 @@
     """
 
     __slots__ = ("bot_username", "request_write_access", "url", "forward_text")
 
     def __init__(
         self,
         url: str,
-        forward_text: bool = None,
-        bot_username: str = None,
-        request_write_access: bool = None,
+        forward_text: Optional[bool] = None,
+        bot_username: Optional[str] = None,
+        request_write_access: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.url: str = url
         # Optional
         self.forward_text: Optional[bool] = forward_text
         self.bot_username: Optional[str] = bot_username
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_menubutton.py` & `python-telegram-bot-raw-20.4/telegram/_menubutton.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains objects related to Telegram menu buttons."""
-from typing import TYPE_CHECKING, ClassVar, Dict, Optional, Type
+from typing import TYPE_CHECKING, Dict, Final, Optional, Type
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 from telegram._webappinfo import WebAppInfo
 
 if TYPE_CHECKING:
@@ -51,15 +51,15 @@
     Attributes:
         type (:obj:`str`): Type of menu button that the instance represents.
     """
 
     __slots__ = ("type",)
 
     def __init__(
-        self, type: str, *, api_kwargs: JSONDict = None  # skipcq: PYL-W0622
+        self, type: str, *, api_kwargs: Optional[JSONDict] = None  # skipcq: PYL-W0622
     ):  # pylint: disable=redefined-builtin
         super().__init__(api_kwargs=api_kwargs)
         self.type: str = type
 
         self._id_attrs = (self.type,)
 
         self._freeze()
@@ -91,19 +91,19 @@
             cls.DEFAULT: MenuButtonDefault,
         }
 
         if cls is MenuButton and data.get("type") in _class_mapping:
             return _class_mapping[data.pop("type")].de_json(data, bot=bot)
         return super().de_json(data=data, bot=bot)
 
-    COMMANDS: ClassVar[str] = constants.MenuButtonType.COMMANDS
+    COMMANDS: Final[str] = constants.MenuButtonType.COMMANDS
     """:const:`telegram.constants.MenuButtonType.COMMANDS`"""
-    WEB_APP: ClassVar[str] = constants.MenuButtonType.WEB_APP
+    WEB_APP: Final[str] = constants.MenuButtonType.WEB_APP
     """:const:`telegram.constants.MenuButtonType.WEB_APP`"""
-    DEFAULT: ClassVar[str] = constants.MenuButtonType.DEFAULT
+    DEFAULT: Final[str] = constants.MenuButtonType.DEFAULT
     """:const:`telegram.constants.MenuButtonType.DEFAULT`"""
 
 
 class MenuButtonCommands(MenuButton):
     """Represents a menu button, which opens the bot's list of commands.
 
     .. include:: inclusions/menu_button_command_video.rst
@@ -111,15 +111,15 @@
     .. versionadded:: 20.0
     Attributes:
         type (:obj:`str`): :tg-const:`telegram.constants.MenuButtonType.COMMANDS`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=constants.MenuButtonType.COMMANDS, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class MenuButtonWebApp(MenuButton):
     """Represents a menu button, which launches a
     `Web App <https://core.telegram.org/bots/webapps>`_.
@@ -144,15 +144,15 @@
             when the user presses the button. The Web App will be able to send an arbitrary
             message on behalf of the user using the method :meth:`~telegram.Bot.answerWebAppQuery`
             of :class:`~telegram.Bot`.
     """
 
     __slots__ = ("text", "web_app")
 
-    def __init__(self, text: str, web_app: WebAppInfo, *, api_kwargs: JSONDict = None):
+    def __init__(self, text: str, web_app: WebAppInfo, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=constants.MenuButtonType.WEB_APP, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.text: str = text
             self.web_app: WebAppInfo = web_app
 
             self._id_attrs = (self.type, self.text, self.web_app)
 
@@ -175,10 +175,10 @@
     .. versionadded:: 20.0
     Attributes:
         type (:obj:`str`): :tg-const:`telegram.constants.MenuButtonType.DEFAULT`.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(type=constants.MenuButtonType.DEFAULT, api_kwargs=api_kwargs)
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_message.py` & `python-telegram-bot-raw-20.4/telegram/_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,23 @@
 from telegram._proximityalerttriggered import ProximityAlertTriggered
 from telegram._shared import ChatShared, UserShared
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.defaultvalue import DEFAULT_NONE, DefaultValue
-from telegram._utils.types import DVInput, FileInput, JSONDict, ODVInput, ReplyMarkup
+from telegram._utils.types import (
+    CorrectOptionID,
+    DVInput,
+    FileInput,
+    JSONDict,
+    MarkdownVersion,
+    ODVInput,
+    ReplyMarkup,
+)
 from telegram._utils.warnings import warn
 from telegram._videochat import (
     VideoChatEnded,
     VideoChatParticipantsInvited,
     VideoChatScheduled,
     VideoChatStarted,
 )
@@ -666,84 +674,84 @@
     )
 
     def __init__(
         self,
         message_id: int,
         date: datetime.datetime,
         chat: Chat,
-        from_user: User = None,
-        forward_from: User = None,
-        forward_from_chat: Chat = None,
-        forward_from_message_id: int = None,
-        forward_date: datetime.datetime = None,
-        reply_to_message: "Message" = None,
-        edit_date: datetime.datetime = None,
-        text: str = None,
-        entities: Sequence["MessageEntity"] = None,
-        caption_entities: Sequence["MessageEntity"] = None,
-        audio: Audio = None,
-        document: Document = None,
-        game: Game = None,
-        photo: Sequence[PhotoSize] = None,
-        sticker: Sticker = None,
-        video: Video = None,
-        voice: Voice = None,
-        video_note: VideoNote = None,
-        new_chat_members: Sequence[User] = None,
-        caption: str = None,
-        contact: Contact = None,
-        location: Location = None,
-        venue: Venue = None,
-        left_chat_member: User = None,
-        new_chat_title: str = None,
-        new_chat_photo: Sequence[PhotoSize] = None,
-        delete_chat_photo: bool = None,
-        group_chat_created: bool = None,
-        supergroup_chat_created: bool = None,
-        channel_chat_created: bool = None,
-        migrate_to_chat_id: int = None,
-        migrate_from_chat_id: int = None,
-        pinned_message: "Message" = None,
-        invoice: Invoice = None,
-        successful_payment: SuccessfulPayment = None,
-        forward_signature: str = None,
-        author_signature: str = None,
-        media_group_id: str = None,
-        connected_website: str = None,
-        animation: Animation = None,
-        passport_data: PassportData = None,
-        poll: Poll = None,
-        forward_sender_name: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        dice: Dice = None,
-        via_bot: User = None,
-        proximity_alert_triggered: ProximityAlertTriggered = None,
-        sender_chat: Chat = None,
-        video_chat_started: VideoChatStarted = None,
-        video_chat_ended: VideoChatEnded = None,
-        video_chat_participants_invited: VideoChatParticipantsInvited = None,
-        message_auto_delete_timer_changed: MessageAutoDeleteTimerChanged = None,
-        video_chat_scheduled: VideoChatScheduled = None,
-        is_automatic_forward: bool = None,
-        has_protected_content: bool = None,
-        web_app_data: WebAppData = None,
-        is_topic_message: bool = None,
-        message_thread_id: int = None,
-        forum_topic_created: ForumTopicCreated = None,
-        forum_topic_closed: ForumTopicClosed = None,
-        forum_topic_reopened: ForumTopicReopened = None,
-        forum_topic_edited: ForumTopicEdited = None,
-        general_forum_topic_hidden: GeneralForumTopicHidden = None,
-        general_forum_topic_unhidden: GeneralForumTopicUnhidden = None,
-        write_access_allowed: WriteAccessAllowed = None,
-        has_media_spoiler: bool = None,
-        user_shared: UserShared = None,
-        chat_shared: ChatShared = None,
+        from_user: Optional[User] = None,
+        forward_from: Optional[User] = None,
+        forward_from_chat: Optional[Chat] = None,
+        forward_from_message_id: Optional[int] = None,
+        forward_date: Optional[datetime.datetime] = None,
+        reply_to_message: Optional["Message"] = None,
+        edit_date: Optional[datetime.datetime] = None,
+        text: Optional[str] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
+        audio: Optional[Audio] = None,
+        document: Optional[Document] = None,
+        game: Optional[Game] = None,
+        photo: Optional[Sequence[PhotoSize]] = None,
+        sticker: Optional[Sticker] = None,
+        video: Optional[Video] = None,
+        voice: Optional[Voice] = None,
+        video_note: Optional[VideoNote] = None,
+        new_chat_members: Optional[Sequence[User]] = None,
+        caption: Optional[str] = None,
+        contact: Optional[Contact] = None,
+        location: Optional[Location] = None,
+        venue: Optional[Venue] = None,
+        left_chat_member: Optional[User] = None,
+        new_chat_title: Optional[str] = None,
+        new_chat_photo: Optional[Sequence[PhotoSize]] = None,
+        delete_chat_photo: Optional[bool] = None,
+        group_chat_created: Optional[bool] = None,
+        supergroup_chat_created: Optional[bool] = None,
+        channel_chat_created: Optional[bool] = None,
+        migrate_to_chat_id: Optional[int] = None,
+        migrate_from_chat_id: Optional[int] = None,
+        pinned_message: Optional["Message"] = None,
+        invoice: Optional[Invoice] = None,
+        successful_payment: Optional[SuccessfulPayment] = None,
+        forward_signature: Optional[str] = None,
+        author_signature: Optional[str] = None,
+        media_group_id: Optional[str] = None,
+        connected_website: Optional[str] = None,
+        animation: Optional[Animation] = None,
+        passport_data: Optional[PassportData] = None,
+        poll: Optional[Poll] = None,
+        forward_sender_name: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        dice: Optional[Dice] = None,
+        via_bot: Optional[User] = None,
+        proximity_alert_triggered: Optional[ProximityAlertTriggered] = None,
+        sender_chat: Optional[Chat] = None,
+        video_chat_started: Optional[VideoChatStarted] = None,
+        video_chat_ended: Optional[VideoChatEnded] = None,
+        video_chat_participants_invited: Optional[VideoChatParticipantsInvited] = None,
+        message_auto_delete_timer_changed: Optional[MessageAutoDeleteTimerChanged] = None,
+        video_chat_scheduled: Optional[VideoChatScheduled] = None,
+        is_automatic_forward: Optional[bool] = None,
+        has_protected_content: Optional[bool] = None,
+        web_app_data: Optional[WebAppData] = None,
+        is_topic_message: Optional[bool] = None,
+        message_thread_id: Optional[int] = None,
+        forum_topic_created: Optional[ForumTopicCreated] = None,
+        forum_topic_closed: Optional[ForumTopicClosed] = None,
+        forum_topic_reopened: Optional[ForumTopicReopened] = None,
+        forum_topic_edited: Optional[ForumTopicEdited] = None,
+        general_forum_topic_hidden: Optional[GeneralForumTopicHidden] = None,
+        general_forum_topic_unhidden: Optional[GeneralForumTopicUnhidden] = None,
+        write_access_allowed: Optional[WriteAccessAllowed] = None,
+        has_media_spoiler: Optional[bool] = None,
+        user_shared: Optional[UserShared] = None,
+        chat_shared: Optional[ChatShared] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.message_id: int = message_id
         # Optionals
         self.from_user: Optional[User] = from_user
@@ -1037,27 +1045,27 @@
 
     async def reply_text(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_message(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_message`.
 
@@ -1091,27 +1099,27 @@
         )
 
     async def reply_markdown(
         self,
         text: str,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
                 parse_mode=ParseMode.MARKDOWN,
                 *args,
@@ -1155,27 +1163,27 @@
         )
 
     async def reply_markdown_v2(
         self,
         text: str,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
                 parse_mode=ParseMode.MARKDOWN_V2,
                 *args,
@@ -1215,27 +1223,27 @@
         )
 
     async def reply_html(
         self,
         text: str,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        entities: Sequence["MessageEntity"] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
             await bot.send_message(
                 update.effective_message.chat_id,
                 parse_mode=ParseMode.HTML,
                 *args,
@@ -1276,28 +1284,28 @@
 
     async def reply_media_group(
         self,
         media: Sequence[
             Union["InputMediaAudio", "InputMediaDocument", "InputMediaPhoto", "InputMediaVideo"]
         ],
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
         caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
     ) -> Tuple["Message", ...]:
         """Shortcut for::
 
              await bot.send_media_group(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_media_group`.
 
@@ -1331,32 +1339,32 @@
             parse_mode=parse_mode,
             caption_entities=caption_entities,
         )
 
     async def reply_photo(
         self,
         photo: Union[FileInput, "PhotoSize"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_photo(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_photo`.
 
@@ -1390,36 +1398,36 @@
             api_kwargs=api_kwargs,
             has_spoiler=has_spoiler,
         )
 
     async def reply_audio(
         self,
         audio: Union[FileInput, "Audio"],
-        duration: int = None,
-        performer: str = None,
-        title: str = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        performer: Optional[str] = None,
+        title: Optional[str] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_audio(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_audio`.
 
@@ -1457,34 +1465,34 @@
             api_kwargs=api_kwargs,
             thumbnail=thumbnail,
         )
 
     async def reply_document(
         self,
         document: Union[FileInput, "Document"],
-        caption: str = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        thumb: FileInput = None,
-        disable_content_type_detection: bool = None,
+        thumb: Optional[FileInput] = None,
+        disable_content_type_detection: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_document(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_document`.
 
@@ -1520,37 +1528,37 @@
             message_thread_id=message_thread_id,
             thumbnail=thumbnail,
         )
 
     async def reply_animation(
         self,
         animation: Union[FileInput, "Animation"],
-        duration: int = None,
-        width: int = None,
-        height: int = None,
-        thumb: FileInput = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        thumb: Optional[FileInput] = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_animation(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_animation`.
 
@@ -1591,27 +1599,27 @@
             thumbnail=thumbnail,
         )
 
     async def reply_sticker(
         self,
         sticker: Union[FileInput, "Sticker"],
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        emoji: str = None,
+        message_thread_id: Optional[int] = None,
+        emoji: Optional[str] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_sticker(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_sticker`.
 
@@ -1641,38 +1649,38 @@
             message_thread_id=message_thread_id,
             emoji=emoji,
         )
 
     async def reply_video(
         self,
         video: Union[FileInput, "Video"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        width: int = None,
-        height: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        supports_streaming: bool = None,
-        thumb: FileInput = None,
+        supports_streaming: Optional[bool] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        has_spoiler: bool = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        has_spoiler: Optional[bool] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_video(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video`.
 
@@ -1712,32 +1720,32 @@
             has_spoiler=has_spoiler,
             thumbnail=thumbnail,
         )
 
     async def reply_video_note(
         self,
         video_note: Union[FileInput, "VideoNote"],
-        duration: int = None,
-        length: int = None,
+        duration: Optional[int] = None,
+        length: Optional[int] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        thumb: FileInput = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        thumb: Optional[FileInput] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
-        thumbnail: FileInput = None,
+        message_thread_id: Optional[int] = None,
+        thumbnail: Optional[FileInput] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_video_note(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_video_note`.
 
@@ -1772,32 +1780,32 @@
             message_thread_id=message_thread_id,
             thumbnail=thumbnail,
         )
 
     async def reply_voice(
         self,
         voice: Union[FileInput, "Voice"],
-        duration: int = None,
-        caption: str = None,
+        duration: Optional[int] = None,
+        caption: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        filename: str = None,
-        quote: bool = None,
+        filename: Optional[str] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = 20,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_voice(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_voice`.
 
@@ -1831,34 +1839,34 @@
             filename=filename,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def reply_location(
         self,
-        latitude: float = None,
-        longitude: float = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        live_period: int = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        live_period: Optional[int] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        location: Location = None,
-        quote: bool = None,
+        location: Optional[Location] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_location(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_location`.
 
@@ -1892,36 +1900,36 @@
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def reply_venue(
         self,
-        latitude: float = None,
-        longitude: float = None,
-        title: str = None,
-        address: str = None,
-        foursquare_id: str = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        title: Optional[str] = None,
+        address: Optional[str] = None,
+        foursquare_id: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        foursquare_type: Optional[str] = None,
+        google_place_id: Optional[str] = None,
+        google_place_type: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        venue: Venue = None,
-        quote: bool = None,
+        venue: Optional[Venue] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_venue(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_venue`.
 
@@ -1957,32 +1965,32 @@
             allow_sending_without_reply=allow_sending_without_reply,
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def reply_contact(
         self,
-        phone_number: str = None,
-        first_name: str = None,
-        last_name: str = None,
+        phone_number: Optional[str] = None,
+        first_name: Optional[str] = None,
+        last_name: Optional[str] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        vcard: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        vcard: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        contact: Contact = None,
-        quote: bool = None,
+        contact: Optional[Contact] = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_contact(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_contact`.
 
@@ -2016,37 +2024,37 @@
             message_thread_id=message_thread_id,
         )
 
     async def reply_poll(
         self,
         question: str,
         options: Sequence[str],
-        is_anonymous: bool = None,
-        type: str = None,  # pylint: disable=redefined-builtin
-        allows_multiple_answers: bool = None,
-        correct_option_id: int = None,
-        is_closed: bool = None,
+        is_anonymous: Optional[bool] = None,
+        type: Optional[str] = None,  # pylint: disable=redefined-builtin
+        allows_multiple_answers: Optional[bool] = None,
+        correct_option_id: Optional[CorrectOptionID] = None,
+        is_closed: Optional[bool] = None,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        explanation: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        explanation: Optional[str] = None,
         explanation_parse_mode: ODVInput[str] = DEFAULT_NONE,
-        open_period: int = None,
-        close_date: Union[int, datetime.datetime] = None,
+        open_period: Optional[int] = None,
+        close_date: Optional[Union[int, datetime.datetime]] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        explanation_entities: Sequence["MessageEntity"] = None,
+        explanation_entities: Optional[Sequence["MessageEntity"]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_poll(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_poll`.
 
@@ -2086,27 +2094,27 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def reply_dice(
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: ReplyMarkup = None,
-        emoji: str = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional[ReplyMarkup] = None,
+        emoji: Optional[str] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_dice(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_dice`.
 
@@ -2135,21 +2143,21 @@
             protect_content=protect_content,
             message_thread_id=message_thread_id,
         )
 
     async def reply_chat_action(
         self,
         action: str,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.send_chat_action(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_chat_action`.
 
@@ -2170,26 +2178,26 @@
             api_kwargs=api_kwargs,
         )
 
     async def reply_game(
         self,
         game_short_name: str,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_game(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_game`.
 
@@ -2225,42 +2233,42 @@
         self,
         title: str,
         description: str,
         payload: str,
         provider_token: str,
         currency: str,
         prices: Sequence["LabeledPrice"],
-        start_parameter: str = None,
-        photo_url: str = None,
-        photo_size: int = None,
-        photo_width: int = None,
-        photo_height: int = None,
-        need_name: bool = None,
-        need_phone_number: bool = None,
-        need_email: bool = None,
-        need_shipping_address: bool = None,
-        is_flexible: bool = None,
+        start_parameter: Optional[str] = None,
+        photo_url: Optional[str] = None,
+        photo_size: Optional[int] = None,
+        photo_width: Optional[int] = None,
+        photo_height: Optional[int] = None,
+        need_name: Optional[bool] = None,
+        need_phone_number: Optional[bool] = None,
+        need_email: Optional[bool] = None,
+        need_shipping_address: Optional[bool] = None,
+        is_flexible: Optional[bool] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
-        reply_markup: "InlineKeyboardMarkup" = None,
-        provider_data: Union[str, object] = None,
-        send_phone_number_to_provider: bool = None,
-        send_email_to_provider: bool = None,
+        reply_to_message_id: Optional[int] = None,
+        reply_markup: Optional["InlineKeyboardMarkup"] = None,
+        provider_data: Optional[Union[str, object]] = None,
+        send_phone_number_to_provider: Optional[bool] = None,
+        send_email_to_provider: Optional[bool] = None,
         allow_sending_without_reply: ODVInput[bool] = DEFAULT_NONE,
-        max_tip_amount: int = None,
-        suggested_tip_amounts: Sequence[int] = None,
+        max_tip_amount: Optional[int] = None,
+        suggested_tip_amounts: Optional[Sequence[int]] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.send_invoice(update.effective_message.chat_id, *args, **kwargs)
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.send_invoice`.
 
@@ -2323,21 +2331,21 @@
         )
 
     async def forward(
         self,
         chat_id: Union[int, str],
         disable_notification: DVInput[bool] = DEFAULT_NONE,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "Message":
         """Shortcut for::
 
              await bot.forward_message(
                  from_chat_id=update.effective_message.chat_id,
                  message_id=update.effective_message.message_id,
                  *args,
@@ -2371,29 +2379,29 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def copy(
         self,
         chat_id: Union[int, str],
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
              await bot.copy_message(
                  chat_id=chat_id,
                  from_chat_id=update.effective_message.chat_id,
                  message_id=update.effective_message.message_id,
@@ -2427,30 +2435,30 @@
             message_thread_id=message_thread_id,
         )
 
     async def reply_copy(
         self,
         from_chat_id: Union[str, int],
         message_id: int,
-        caption: str = None,
+        caption: Optional[str] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         disable_notification: DVInput[bool] = DEFAULT_NONE,
-        reply_to_message_id: int = None,
+        reply_to_message_id: Optional[int] = None,
         allow_sending_without_reply: DVInput[bool] = DEFAULT_NONE,
-        reply_markup: ReplyMarkup = None,
+        reply_markup: Optional[ReplyMarkup] = None,
         protect_content: ODVInput[bool] = DEFAULT_NONE,
-        message_thread_id: int = None,
+        message_thread_id: Optional[int] = None,
         *,
-        quote: bool = None,
+        quote: Optional[bool] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "MessageId":
         """Shortcut for::
 
              await bot.copy_message(
                  chat_id=message.chat.id,
                  message_id=message_id,
                  *args,
@@ -2492,22 +2500,22 @@
         )
 
     async def edit_text(
         self,
         text: str,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
         disable_web_page_preview: ODVInput[bool] = DEFAULT_NONE,
-        reply_markup: InlineKeyboardMarkup = None,
-        entities: Sequence["MessageEntity"] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.edit_message_text(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2537,24 +2545,24 @@
             api_kwargs=api_kwargs,
             entities=entities,
             inline_message_id=None,
         )
 
     async def edit_caption(
         self,
-        caption: str = None,
-        reply_markup: InlineKeyboardMarkup = None,
+        caption: Optional[str] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         parse_mode: ODVInput[str] = DEFAULT_NONE,
-        caption_entities: Sequence["MessageEntity"] = None,
+        caption_entities: Optional[Sequence["MessageEntity"]] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.edit_message_caption(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2585,21 +2593,21 @@
             caption_entities=caption_entities,
             inline_message_id=None,
         )
 
     async def edit_media(
         self,
         media: "InputMedia",
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.edit_message_media(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2633,15 +2641,15 @@
         self,
         reply_markup: Optional["InlineKeyboardMarkup"] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.edit_message_reply_markup(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2667,27 +2675,27 @@
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
             inline_message_id=None,
         )
 
     async def edit_live_location(
         self,
-        latitude: float = None,
-        longitude: float = None,
-        reply_markup: InlineKeyboardMarkup = None,
-        horizontal_accuracy: float = None,
-        heading: int = None,
-        proximity_alert_radius: int = None,
+        latitude: Optional[float] = None,
+        longitude: Optional[float] = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
+        horizontal_accuracy: Optional[float] = None,
+        heading: Optional[int] = None,
+        proximity_alert_radius: Optional[int] = None,
         *,
-        location: Location = None,
+        location: Optional[Location] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.edit_message_live_location(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2719,21 +2727,21 @@
             heading=heading,
             proximity_alert_radius=proximity_alert_radius,
             inline_message_id=None,
         )
 
     async def stop_live_location(
         self,
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.stop_message_live_location(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2761,22 +2769,22 @@
             inline_message_id=None,
         )
 
     async def set_game_score(
         self,
         user_id: Union[int, str],
         score: int,
-        force: bool = None,
-        disable_edit_message: bool = None,
+        force: Optional[bool] = None,
+        disable_edit_message: Optional[bool] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Union["Message", bool]:
         """Shortcut for::
 
              await bot.set_game_score(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2810,15 +2818,15 @@
         self,
         user_id: Union[int, str],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Tuple["GameHighScore", ...]:
         """Shortcut for::
 
              await bot.get_game_high_scores(
                  chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
              )
 
@@ -2848,15 +2856,15 @@
     async def delete(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.delete_message(
                   chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
               )
 
@@ -2874,21 +2882,21 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def stop_poll(
         self,
-        reply_markup: InlineKeyboardMarkup = None,
+        reply_markup: Optional[InlineKeyboardMarkup] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Poll:
         """Shortcut for::
 
               await bot.stop_poll(
                   chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
               )
 
@@ -2914,15 +2922,15 @@
         self,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.pin_chat_message(
                   chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
               )
 
@@ -2946,15 +2954,15 @@
     async def unpin(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
               await bot.unpin_chat_message(
                   chat_id=message.chat_id, message_id=message.message_id, *args, **kwargs
               )
 
@@ -2972,22 +2980,22 @@
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
     async def edit_forum_topic(
         self,
-        name: str = None,
-        icon_custom_emoji_id: str = None,
+        name: Optional[str] = None,
+        icon_custom_emoji_id: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.edit_forum_topic(
                 chat_id=message.chat_id, message_thread_id=message.message_thread_id, *args,
                 **kwargs
              )
@@ -3015,15 +3023,15 @@
     async def close_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.close_forum_topic(
                 chat_id=message.chat_id, message_thread_id=message.message_thread_id, *args,
                 **kwargs
              )
@@ -3049,15 +3057,15 @@
     async def reopen_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
             await bot.reopen_forum_topic(
                 chat_id=message.chat_id, message_thread_id=message.message_thread_id, *args,
                 **kwargs
              )
@@ -3083,15 +3091,15 @@
     async def delete_forum_topic(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.delete_forum_topic(
                 chat_id=message.chat_id, message_thread_id=message.message_thread_id, *args,
                 **kwargs
              )
@@ -3117,15 +3125,15 @@
     async def unpin_all_forum_topic_messages(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.unpin_all_forum_topic_messages(
                 chat_id=message.chat_id, message_thread_id=message.message_thread_id, *args,
                 **kwargs
              )
@@ -3196,15 +3204,15 @@
         if not self.caption:
             raise RuntimeError("This Message has no 'caption'.")
 
         entity_text = self.caption.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
         return entity_text.decode("utf-16-le")
 
-    def parse_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
+    def parse_entities(self, types: Optional[List[str]] = None) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this message filtered by their
         :attr:`telegram.MessageEntity.type` attribute as the key, and the text that each entity
         belongs to as the value of the :obj:`dict`.
 
         Note:
@@ -3226,15 +3234,17 @@
         if types is None:
             types = MessageEntity.ALL_TYPES
 
         return {
             entity: self.parse_entity(entity) for entity in self.entities if entity.type in types
         }
 
-    def parse_caption_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
+    def parse_caption_entities(
+        self, types: Optional[List[str]] = None
+    ) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this message's caption filtered by their
         :attr:`telegram.MessageEntity.type` attribute as the key, and the text that each entity
         belongs to as the value of the :obj:`dict`.
 
         Note:
@@ -3436,18 +3446,18 @@
         return self._parse_html(self.caption, self.parse_caption_entities(), urled=True)
 
     @staticmethod
     def _parse_markdown(
         message_text: Optional[str],
         entities: Dict[MessageEntity, str],
         urled: bool = False,
-        version: int = 1,
+        version: MarkdownVersion = 1,
         offset: int = 0,
     ) -> Optional[str]:
-        version = int(version)
+        version = int(version)  # type: ignore
 
         if message_text is None:
             return None
 
         message_text = message_text.encode("utf-16-le")  # type: ignore
 
         markdown_text = ""
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_messageautodeletetimerchanged.py` & `python-telegram-bot-raw-20.4/telegram/_messageautodeletetimerchanged.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a change in the Telegram message auto
 deletion.
 """
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class MessageAutoDeleteTimerChanged(TelegramObject):
     """This object represents a service message about a change in auto-delete timer settings.
 
@@ -44,15 +46,15 @@
 
     __slots__ = ("message_auto_delete_time",)
 
     def __init__(
         self,
         message_auto_delete_time: int,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.message_auto_delete_time: int = message_auto_delete_time
 
         self._id_attrs = (self.message_auto_delete_time,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_messageentity.py` & `python-telegram-bot-raw-20.4/telegram/_messageentity.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram MessageEntity."""
 
-from typing import TYPE_CHECKING, ClassVar, List, Optional
+from typing import TYPE_CHECKING, Final, List, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils import enum
 from telegram._utils.types import JSONDict
 
@@ -92,20 +92,20 @@
     __slots__ = ("length", "url", "user", "type", "language", "offset", "custom_emoji_id")
 
     def __init__(
         self,
         type: str,  # pylint: disable=redefined-builtin
         offset: int,
         length: int,
-        url: str = None,
-        user: User = None,
-        language: str = None,
-        custom_emoji_id: str = None,
+        url: Optional[str] = None,
+        user: Optional[User] = None,
+        language: Optional[str] = None,
+        custom_emoji_id: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.type: str = enum.get_member(constants.MessageEntityType, type, type)
         self.offset: int = offset
         self.length: int = length
         # Optionals
@@ -126,49 +126,49 @@
         if not data:
             return None
 
         data["user"] = User.de_json(data.get("user"), bot)
 
         return super().de_json(data=data, bot=bot)
 
-    MENTION: ClassVar[str] = constants.MessageEntityType.MENTION
+    MENTION: Final[str] = constants.MessageEntityType.MENTION
     """:const:`telegram.constants.MessageEntityType.MENTION`"""
-    HASHTAG: ClassVar[str] = constants.MessageEntityType.HASHTAG
+    HASHTAG: Final[str] = constants.MessageEntityType.HASHTAG
     """:const:`telegram.constants.MessageEntityType.HASHTAG`"""
-    CASHTAG: ClassVar[str] = constants.MessageEntityType.CASHTAG
+    CASHTAG: Final[str] = constants.MessageEntityType.CASHTAG
     """:const:`telegram.constants.MessageEntityType.CASHTAG`"""
-    PHONE_NUMBER: ClassVar[str] = constants.MessageEntityType.PHONE_NUMBER
+    PHONE_NUMBER: Final[str] = constants.MessageEntityType.PHONE_NUMBER
     """:const:`telegram.constants.MessageEntityType.PHONE_NUMBER`"""
-    BOT_COMMAND: ClassVar[str] = constants.MessageEntityType.BOT_COMMAND
+    BOT_COMMAND: Final[str] = constants.MessageEntityType.BOT_COMMAND
     """:const:`telegram.constants.MessageEntityType.BOT_COMMAND`"""
-    URL: ClassVar[str] = constants.MessageEntityType.URL
+    URL: Final[str] = constants.MessageEntityType.URL
     """:const:`telegram.constants.MessageEntityType.URL`"""
-    EMAIL: ClassVar[str] = constants.MessageEntityType.EMAIL
+    EMAIL: Final[str] = constants.MessageEntityType.EMAIL
     """:const:`telegram.constants.MessageEntityType.EMAIL`"""
-    BOLD: ClassVar[str] = constants.MessageEntityType.BOLD
+    BOLD: Final[str] = constants.MessageEntityType.BOLD
     """:const:`telegram.constants.MessageEntityType.BOLD`"""
-    ITALIC: ClassVar[str] = constants.MessageEntityType.ITALIC
+    ITALIC: Final[str] = constants.MessageEntityType.ITALIC
     """:const:`telegram.constants.MessageEntityType.ITALIC`"""
-    CODE: ClassVar[str] = constants.MessageEntityType.CODE
+    CODE: Final[str] = constants.MessageEntityType.CODE
     """:const:`telegram.constants.MessageEntityType.CODE`"""
-    PRE: ClassVar[str] = constants.MessageEntityType.PRE
+    PRE: Final[str] = constants.MessageEntityType.PRE
     """:const:`telegram.constants.MessageEntityType.PRE`"""
-    TEXT_LINK: ClassVar[str] = constants.MessageEntityType.TEXT_LINK
+    TEXT_LINK: Final[str] = constants.MessageEntityType.TEXT_LINK
     """:const:`telegram.constants.MessageEntityType.TEXT_LINK`"""
-    TEXT_MENTION: ClassVar[str] = constants.MessageEntityType.TEXT_MENTION
+    TEXT_MENTION: Final[str] = constants.MessageEntityType.TEXT_MENTION
     """:const:`telegram.constants.MessageEntityType.TEXT_MENTION`"""
-    UNDERLINE: ClassVar[str] = constants.MessageEntityType.UNDERLINE
+    UNDERLINE: Final[str] = constants.MessageEntityType.UNDERLINE
     """:const:`telegram.constants.MessageEntityType.UNDERLINE`"""
-    STRIKETHROUGH: ClassVar[str] = constants.MessageEntityType.STRIKETHROUGH
+    STRIKETHROUGH: Final[str] = constants.MessageEntityType.STRIKETHROUGH
     """:const:`telegram.constants.MessageEntityType.STRIKETHROUGH`"""
-    SPOILER: ClassVar[str] = constants.MessageEntityType.SPOILER
+    SPOILER: Final[str] = constants.MessageEntityType.SPOILER
     """:const:`telegram.constants.MessageEntityType.SPOILER`
 
     .. versionadded:: 13.10
     """
-    CUSTOM_EMOJI: ClassVar[str] = constants.MessageEntityType.CUSTOM_EMOJI
+    CUSTOM_EMOJI: Final[str] = constants.MessageEntityType.CUSTOM_EMOJI
     """:const:`telegram.constants.MessageEntityType.CUSTOM_EMOJI`
 
     .. versionadded:: 20.0
     """
-    ALL_TYPES: ClassVar[List[str]] = list(constants.MessageEntityType)
+    ALL_TYPES: Final[List[str]] = list(constants.MessageEntityType)
     """List[:obj:`str`]: A list of all available message entity types."""
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_messageid.py` & `python-telegram-bot-raw-20.4/telegram/_messageid.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents an instance of a Telegram MessageId."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class MessageId(TelegramObject):
     """This object represents a unique message identifier.
 
@@ -33,14 +35,14 @@
 
     Attributes:
         message_id (:obj:`int`): Unique message identifier.
     """
 
     __slots__ = ("message_id",)
 
-    def __init__(self, message_id: int, *, api_kwargs: JSONDict = None):
+    def __init__(self, message_id: int, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.message_id: int = message_id
 
         self._id_attrs = (self.message_id,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/credentials.py` & `python-telegram-bot-raw-20.4/telegram/_passport/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     Returns:
         :obj:`bytes`: The decrypted data as bytes.
 
     """
     if not CRYPTO_INSTALLED:
         raise RuntimeError(
             "To use Telegram Passports, PTB must be installed via `pip install "
-            "python-telegram-bot[passport]`."
+            '"python-telegram-bot[passport]"`.'
         )
     # Make a SHA512 hash of secret + update
     digest = Hash(SHA512(), backend=default_backend())
     digest.update(secret + hash)
     secret_hash_hash = digest.finalize()
     # First 32 chars is our key, next 16 is the initialisation vector
     key, init_vector = secret_hash_hash[:32], secret_hash_hash[32 : 32 + 16]
@@ -139,15 +139,15 @@
 
     def __init__(
         self,
         data: str,
         hash: str,  # skipcq: PYL-W0622
         secret: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.data: str = data
         self.hash: str = hash
         self.secret: str = secret
 
@@ -167,15 +167,15 @@
             telegram.error.PassportDecryptionError: Decryption failed. Usually due to bad
                 private/public key but can also suggest malformed/tampered data.
         """
         if self._decrypted_secret is None:
             if not CRYPTO_INSTALLED:
                 raise RuntimeError(
                     "To use Telegram Passports, PTB must be installed via `pip install "
-                    "python-telegram-bot[passport]`."
+                    '"python-telegram-bot[passport]"`.'
                 )
             # Try decrypting according to step 1 at
             # https://core.telegram.org/passport#decrypting-data
             # We make sure to base64 decode the secret first.
             # Telegram says to use OAEP padding so we do that. The Mask Generation Function
             # is the default for OAEP, the algorithm is the default for PHP which is what
             # Telegram's backend servers run.
@@ -218,15 +218,15 @@
     __slots__ = ("nonce", "secure_data")
 
     def __init__(
         self,
         secure_data: "SecureData",
         nonce: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.secure_data: SecureData = secure_data
         self.nonce: str = nonce
 
         self._freeze()
@@ -306,27 +306,27 @@
         "bank_statement",
         "passport",
         "passport_registration",
     )
 
     def __init__(
         self,
-        personal_details: "SecureValue" = None,
-        passport: "SecureValue" = None,
-        internal_passport: "SecureValue" = None,
-        driver_license: "SecureValue" = None,
-        identity_card: "SecureValue" = None,
-        address: "SecureValue" = None,
-        utility_bill: "SecureValue" = None,
-        bank_statement: "SecureValue" = None,
-        rental_agreement: "SecureValue" = None,
-        passport_registration: "SecureValue" = None,
-        temporary_registration: "SecureValue" = None,
+        personal_details: Optional["SecureValue"] = None,
+        passport: Optional["SecureValue"] = None,
+        internal_passport: Optional["SecureValue"] = None,
+        driver_license: Optional["SecureValue"] = None,
+        identity_card: Optional["SecureValue"] = None,
+        address: Optional["SecureValue"] = None,
+        utility_bill: Optional["SecureValue"] = None,
+        bank_statement: Optional["SecureValue"] = None,
+        rental_agreement: Optional["SecureValue"] = None,
+        passport_registration: Optional["SecureValue"] = None,
+        temporary_registration: Optional["SecureValue"] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Optionals
         self.temporary_registration: Optional[SecureValue] = temporary_registration
         self.passport_registration: Optional[SecureValue] = passport_registration
         self.rental_agreement: Optional[SecureValue] = rental_agreement
@@ -424,22 +424,22 @@
 
     """
 
     __slots__ = ("data", "front_side", "reverse_side", "selfie", "files", "translation")
 
     def __init__(
         self,
-        data: "DataCredentials" = None,
-        front_side: "FileCredentials" = None,
-        reverse_side: "FileCredentials" = None,
-        selfie: "FileCredentials" = None,
-        files: Sequence["FileCredentials"] = None,
-        translation: Sequence["FileCredentials"] = None,
+        data: Optional["DataCredentials"] = None,
+        front_side: Optional["FileCredentials"] = None,
+        reverse_side: Optional["FileCredentials"] = None,
+        selfie: Optional["FileCredentials"] = None,
+        files: Optional[Sequence["FileCredentials"]] = None,
+        translation: Optional[Sequence["FileCredentials"]] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.data: Optional[DataCredentials] = data
         self.front_side: Optional[FileCredentials] = front_side
         self.reverse_side: Optional[FileCredentials] = reverse_side
         self.selfie: Optional[FileCredentials] = selfie
         self.files: Tuple["FileCredentials", ...] = parse_sequence_arg(files)
@@ -467,15 +467,15 @@
 
 class _CredentialsBase(TelegramObject):
     """Base class for DataCredentials and FileCredentials."""
 
     __slots__ = ("hash", "secret", "file_hash", "data_hash")
 
     def __init__(
-        self, hash: str, secret: str, *, api_kwargs: JSONDict = None  # skipcq: PYL-W0622
+        self, hash: str, secret: str, *, api_kwargs: Optional[JSONDict] = None  # skipcq: PYL-W0622
     ):
         super().__init__(api_kwargs=api_kwargs)
         with self._unfrozen():
             self.hash: str = hash
             self.secret: str = secret
 
             # Aliases just to be sure
@@ -495,15 +495,15 @@
     Attributes:
         hash (:obj:`str`): Checksum of encrypted data
         secret (:obj:`str`): Secret of encrypted data
     """
 
     __slots__ = ()
 
-    def __init__(self, data_hash: str, secret: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, data_hash: str, secret: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(hash=data_hash, secret=secret, api_kwargs=api_kwargs)
         self._freeze()
 
 
 class FileCredentials(_CredentialsBase):
     """
     These credentials can be used to decrypt encrypted files from the front_side,
@@ -516,10 +516,10 @@
     Attributes:
         hash (:obj:`str`): Checksum of encrypted file
         secret (:obj:`str`): Secret of encrypted file
     """
 
     __slots__ = ()
 
-    def __init__(self, file_hash: str, secret: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, file_hash: str, secret: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(hash=file_hash, secret=secret, api_kwargs=api_kwargs)
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/data.py` & `python-telegram-bot-raw-20.4/telegram/_passport/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,20 +77,20 @@
         self,
         first_name: str,
         last_name: str,
         birth_date: str,
         gender: str,
         country_code: str,
         residence_country_code: str,
-        first_name_native: str = None,
-        last_name_native: str = None,
-        middle_name: str = None,
-        middle_name_native: str = None,
+        first_name_native: Optional[str] = None,
+        last_name_native: Optional[str] = None,
+        middle_name: Optional[str] = None,
+        middle_name_native: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.first_name: str = first_name
         self.last_name: str = last_name
         self.middle_name: Optional[str] = middle_name
         self.birth_date: str = birth_date
@@ -139,15 +139,15 @@
         street_line1: str,
         street_line2: str,
         city: str,
         state: str,
         country_code: str,
         post_code: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.street_line1: str = street_line1
         self.street_line2: str = street_line2
         self.city: str = city
         self.state: str = state
@@ -173,14 +173,14 @@
     __slots__ = ("document_no", "expiry_date")
 
     def __init__(
         self,
         document_no: str,
         expiry_date: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.document_no: str = document_no
         self.expiry_date: str = expiry_date
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/encryptedpassportelement.py` & `python-telegram-bot-raw-20.4/telegram/_passport/encryptedpassportelement.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,25 +147,25 @@
         "data",
     )
 
     def __init__(
         self,
         type: str,  # pylint: disable=redefined-builtin
         hash: str,  # pylint: disable=redefined-builtin
-        data: PersonalDetails = None,
-        phone_number: str = None,
-        email: str = None,
-        files: Sequence[PassportFile] = None,
-        front_side: PassportFile = None,
-        reverse_side: PassportFile = None,
-        selfie: PassportFile = None,
-        translation: Sequence[PassportFile] = None,
-        credentials: "Credentials" = None,  # pylint: disable=unused-argument
+        data: Optional[PersonalDetails] = None,
+        phone_number: Optional[str] = None,
+        email: Optional[str] = None,
+        files: Optional[Sequence[PassportFile]] = None,
+        front_side: Optional[PassportFile] = None,
+        reverse_side: Optional[PassportFile] = None,
+        selfie: Optional[PassportFile] = None,
+        translation: Optional[Sequence[PassportFile]] = None,
+        credentials: Optional["Credentials"] = None,  # pylint: disable=unused-argument
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.type: str = type
         # Optionals
         self.data: Optional[PersonalDetails] = data
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/passportdata.py` & `python-telegram-bot-raw-20.4/telegram/_passport/passportdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     __slots__ = ("credentials", "data", "_decrypted_data")
 
     def __init__(
         self,
         data: Sequence[EncryptedPassportElement],
         credentials: EncryptedCredentials,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         self.data: Tuple[EncryptedPassportElement, ...] = parse_sequence_arg(data)
         self.credentials: EncryptedCredentials = credentials
 
         self._decrypted_data: Optional[Tuple[EncryptedPassportElement]] = None
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/passportelementerrors.py` & `python-telegram-bot-raw-20.4/telegram/_passport/passportelementerrors.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=redefined-builtin
 """This module contains the classes that represent Telegram PassportElementError."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class PassportElementError(TelegramObject):
     """Baseclass for the PassportElementError* classes.
 
@@ -42,15 +44,17 @@
         type (:obj:`str`): The section of the user's Telegram Passport which has the error.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("message", "source", "type")
 
-    def __init__(self, source: str, type: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, source: str, type: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.source: str = str(source)
         self.type: str = str(type)
         self.message: str = str(message)
 
         self._id_attrs = (self.source, self.type)
@@ -90,15 +94,15 @@
     def __init__(
         self,
         type: str,
         field_name: str,
         data_hash: str,
         message: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         # Required
         super().__init__("data", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.field_name: str = field_name
             self.data_hash: str = data_hash
 
@@ -134,15 +138,17 @@
         file_hash (:obj:`str`): Base64-encoded file hash.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hash",)
 
-    def __init__(self, type: str, file_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("file", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hash: str = file_hash
 
             self._id_attrs = (self.source, self.type, self.file_hash, self.message)
 
@@ -170,15 +176,17 @@
         file_hashes (List[:obj:`str`]): List of base64-encoded file hashes.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hashes",)
 
-    def __init__(self, type: str, file_hashes: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hashes: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("files", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hashes: str = file_hashes
 
             self._id_attrs = (self.source, self.type, self.message, *tuple(file_hashes))
 
@@ -206,15 +214,17 @@
             document.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hash",)
 
-    def __init__(self, type: str, file_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("front_side", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hash: str = file_hash
 
             self._id_attrs = (self.source, self.type, self.file_hash, self.message)
 
@@ -242,15 +252,17 @@
             document.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hash",)
 
-    def __init__(self, type: str, file_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("reverse_side", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hash: str = file_hash
 
             self._id_attrs = (self.source, self.type, self.file_hash, self.message)
 
@@ -276,15 +288,17 @@
         file_hash (:obj:`str`): Base64-encoded hash of the file with the selfie.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hash",)
 
-    def __init__(self, type: str, file_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("selfie", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hash: str = file_hash
 
             self._id_attrs = (self.source, self.type, self.file_hash, self.message)
 
@@ -314,15 +328,17 @@
         file_hash (:obj:`str`): Base64-encoded hash of the file.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hash",)
 
-    def __init__(self, type: str, file_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("translation_file", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hash: str = file_hash
 
             self._id_attrs = (self.source, self.type, self.file_hash, self.message)
 
@@ -352,15 +368,17 @@
         file_hashes (List[:obj:`str`]): List of base64-encoded file hashes.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("file_hashes",)
 
-    def __init__(self, type: str, file_hashes: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, file_hashes: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("translation_files", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hashes: str = file_hashes
 
             self._id_attrs = (self.source, self.type, self.message, *tuple(file_hashes))
 
@@ -384,14 +402,16 @@
         element_hash (:obj:`str`): Base64-encoded element hash.
         message (:obj:`str`): Error message.
 
     """
 
     __slots__ = ("element_hash",)
 
-    def __init__(self, type: str, element_hash: str, message: str, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, type: str, element_hash: str, message: str, *, api_kwargs: Optional[JSONDict] = None
+    ):
         # Required
         super().__init__("unspecified", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.element_hash: str = element_hash
 
             self._id_attrs = (self.source, self.type, self.element_hash, self.message)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_passport/passportfile.py` & `python-telegram-bot-raw-20.4/telegram/_passport/passportfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 
     def __init__(
         self,
         file_id: str,
         file_unique_id: str,
         file_date: int,
         file_size: int,
-        credentials: "FileCredentials" = None,
+        credentials: Optional["FileCredentials"] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         # Required
         self.file_id: str = file_id
         self.file_unique_id: str = file_unique_id
         self.file_size: int = file_size
@@ -151,15 +151,15 @@
     async def get_file(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> "File":
         """
         Wrapper over :meth:`telegram.Bot.get_file`. Will automatically assign the correct
         credentials to the returned :class:`telegram.File` if originating from
         :obj:`telegram.PassportData.decrypted_data`.
 
         For the documentation of the arguments, please see :meth:`telegram.Bot.get_file`.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/invoice.py` & `python-telegram-bot-raw-20.4/telegram/_payment/invoice.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Invoice."""
 
-from typing import ClassVar
+from typing import Final, Optional
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class Invoice(TelegramObject):
@@ -72,15 +72,15 @@
         self,
         title: str,
         description: str,
         start_parameter: str,
         currency: str,
         total_amount: int,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.title: str = title
         self.description: str = description
         self.start_parameter: str = start_parameter
         self.currency: str = currency
         self.total_amount: int = total_amount
@@ -91,42 +91,42 @@
             self.start_parameter,
             self.currency,
             self.total_amount,
         )
 
         self._freeze()
 
-    MIN_TITLE_LENGTH: ClassVar[int] = constants.InvoiceLimit.MIN_TITLE_LENGTH
+    MIN_TITLE_LENGTH: Final[int] = constants.InvoiceLimit.MIN_TITLE_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MIN_TITLE_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_TITLE_LENGTH: ClassVar[int] = constants.InvoiceLimit.MAX_TITLE_LENGTH
+    MAX_TITLE_LENGTH: Final[int] = constants.InvoiceLimit.MAX_TITLE_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MAX_TITLE_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MIN_DESCRIPTION_LENGTH: ClassVar[int] = constants.InvoiceLimit.MIN_DESCRIPTION_LENGTH
+    MIN_DESCRIPTION_LENGTH: Final[int] = constants.InvoiceLimit.MIN_DESCRIPTION_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MIN_DESCRIPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_DESCRIPTION_LENGTH: ClassVar[int] = constants.InvoiceLimit.MAX_DESCRIPTION_LENGTH
+    MAX_DESCRIPTION_LENGTH: Final[int] = constants.InvoiceLimit.MAX_DESCRIPTION_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MAX_DESCRIPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MIN_PAYLOAD_LENGTH: ClassVar[int] = constants.InvoiceLimit.MIN_PAYLOAD_LENGTH
+    MIN_PAYLOAD_LENGTH: Final[int] = constants.InvoiceLimit.MIN_PAYLOAD_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MIN_PAYLOAD_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_PAYLOAD_LENGTH: ClassVar[int] = constants.InvoiceLimit.MAX_PAYLOAD_LENGTH
+    MAX_PAYLOAD_LENGTH: Final[int] = constants.InvoiceLimit.MAX_PAYLOAD_LENGTH
     """:const:`telegram.constants.InvoiceLimit.MAX_PAYLOAD_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_TIP_AMOUNTS: ClassVar[int] = constants.InvoiceLimit.MAX_TIP_AMOUNTS
+    MAX_TIP_AMOUNTS: Final[int] = constants.InvoiceLimit.MAX_TIP_AMOUNTS
     """:const:`telegram.constants.InvoiceLimit.MAX_TIP_AMOUNTS`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/labeledprice.py` & `python-telegram-bot-raw-20.4/telegram/_payment/labeledprice.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram LabeledPrice."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class LabeledPrice(TelegramObject):
     """This object represents a portion of the price for goods or services.
 
@@ -49,15 +51,15 @@
             it shows the number of digits past the decimal point for each currency
             (2 for the majority of currencies).
 
     """
 
     __slots__ = ("label", "amount")
 
-    def __init__(self, label: str, amount: int, *, api_kwargs: JSONDict = None):
+    def __init__(self, label: str, amount: int, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.label: str = label
         self.amount: int = amount
 
         self._id_attrs = (self.label, self.amount)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/orderinfo.py` & `python-telegram-bot-raw-20.4/telegram/_payment/orderinfo.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,20 +49,20 @@
 
     """
 
     __slots__ = ("email", "shipping_address", "phone_number", "name")
 
     def __init__(
         self,
-        name: str = None,
-        phone_number: str = None,
-        email: str = None,
-        shipping_address: str = None,
+        name: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        email: Optional[str] = None,
+        shipping_address: Optional[str] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.name: Optional[str] = name
         self.phone_number: Optional[str] = phone_number
         self.email: Optional[str] = email
         self.shipping_address: Optional[str] = shipping_address
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/precheckoutquery.py` & `python-telegram-bot-raw-20.4/telegram/_payment/precheckoutquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,18 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         from_user: User,
         currency: str,
         total_amount: int,
         invoice_payload: str,
-        shipping_option_id: str = None,
-        order_info: OrderInfo = None,
+        shipping_option_id: Optional[str] = None,
+        order_info: Optional[OrderInfo] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.id: str = id  # pylint: disable=invalid-name
         self.from_user: User = from_user
         self.currency: str = currency
         self.total_amount: int = total_amount
         self.invoice_payload: str = invoice_payload
@@ -119,21 +119,21 @@
         data["order_info"] = OrderInfo.de_json(data.get("order_info"), bot)
 
         return super().de_json(data=data, bot=bot)
 
     async def answer(  # pylint: disable=invalid-name
         self,
         ok: bool,
-        error_message: str = None,
+        error_message: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.answer_pre_checkout_query(update.pre_checkout_query.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.answer_pre_checkout_query`.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/shippingaddress.py` & `python-telegram-bot-raw-20.4/telegram/_payment/shippingaddress.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ShippingAddress."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class ShippingAddress(TelegramObject):
     """This object represents a Telegram ShippingAddress.
 
@@ -61,15 +63,15 @@
         country_code: str,
         state: str,
         city: str,
         street_line1: str,
         street_line2: str,
         post_code: str,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.country_code: str = country_code
         self.state: str = state
         self.city: str = city
         self.street_line1: str = street_line1
         self.street_line2: str = street_line2
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/shippingoption.py` & `python-telegram-bot-raw-20.4/telegram/_payment/shippingoption.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ShippingOption."""
-from typing import TYPE_CHECKING, Sequence, Tuple
+from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import LabeledPrice
@@ -58,15 +58,15 @@
 
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         title: str,
         prices: Sequence["LabeledPrice"],
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
 
         self.id: str = id  # pylint: disable=invalid-name
         self.title: str = title
         self.prices: Tuple["LabeledPrice", ...] = parse_sequence_arg(prices)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/shippingquery.py` & `python-telegram-bot-raw-20.4/telegram/_payment/shippingquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     def __init__(
         self,
         id: str,  # pylint: disable=redefined-builtin
         from_user: User,
         invoice_payload: str,
         shipping_address: ShippingAddress,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.id: str = id  # pylint: disable=invalid-name
         self.from_user: User = from_user
         self.invoice_payload: str = invoice_payload
         self.shipping_address: ShippingAddress = shipping_address
 
@@ -88,22 +88,22 @@
         data["shipping_address"] = ShippingAddress.de_json(data.get("shipping_address"), bot)
 
         return super().de_json(data=data, bot=bot)
 
     async def answer(  # pylint: disable=invalid-name
         self,
         ok: bool,
-        shipping_options: Sequence[ShippingOption] = None,
-        error_message: str = None,
+        shipping_options: Optional[Sequence[ShippingOption]] = None,
+        error_message: Optional[str] = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> bool:
         """Shortcut for::
 
              await bot.answer_shipping_query(update.shipping_query.id, *args, **kwargs)
 
         For the documentation of the arguments, please see
         :meth:`telegram.Bot.answer_shipping_query`.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_payment/successfulpayment.py` & `python-telegram-bot-raw-20.4/telegram/_payment/successfulpayment.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,18 +80,18 @@
     def __init__(
         self,
         currency: str,
         total_amount: int,
         invoice_payload: str,
         telegram_payment_charge_id: str,
         provider_payment_charge_id: str,
-        shipping_option_id: str = None,
-        order_info: OrderInfo = None,
+        shipping_option_id: Optional[str] = None,
+        order_info: Optional[OrderInfo] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.currency: str = currency
         self.total_amount: int = total_amount
         self.invoice_payload: str = invoice_payload
         self.shipping_option_id: Optional[str] = shipping_option_id
         self.order_info: Optional[OrderInfo] = order_info
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_poll.py` & `python-telegram-bot-raw-20.4/telegram/_poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Poll."""
 import datetime
-from typing import TYPE_CHECKING, ClassVar, Dict, List, Optional, Sequence, Tuple
+from typing import TYPE_CHECKING, Dict, Final, List, Optional, Sequence, Tuple
 
 from telegram import constants
 from telegram._messageentity import MessageEntity
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
@@ -52,29 +52,29 @@
             characters.
         voter_count (:obj:`int`): Number of users that voted for this option.
 
     """
 
     __slots__ = ("voter_count", "text")
 
-    def __init__(self, text: str, voter_count: int, *, api_kwargs: JSONDict = None):
+    def __init__(self, text: str, voter_count: int, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         self.text: str = text
         self.voter_count: int = voter_count
 
         self._id_attrs = (self.text, self.voter_count)
 
         self._freeze()
 
-    MIN_LENGTH: ClassVar[int] = constants.PollLimit.MIN_OPTION_LENGTH
+    MIN_LENGTH: Final[int] = constants.PollLimit.MIN_OPTION_LENGTH
     """:const:`telegram.constants.PollLimit.MIN_OPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_LENGTH: ClassVar[int] = constants.PollLimit.MAX_OPTION_LENGTH
+    MAX_LENGTH: Final[int] = constants.PollLimit.MAX_OPTION_LENGTH
     """:const:`telegram.constants.PollLimit.MAX_OPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
 
 
 class PollAnswer(TelegramObject):
@@ -103,15 +103,20 @@
                 |tupleclassattrs|
 
     """
 
     __slots__ = ("option_ids", "user", "poll_id")
 
     def __init__(
-        self, poll_id: str, user: User, option_ids: Sequence[int], *, api_kwargs: JSONDict = None
+        self,
+        poll_id: str,
+        user: User,
+        option_ids: Sequence[int],
+        *,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.poll_id: str = poll_id
         self.user: User = user
         self.option_ids: Tuple[int, ...] = parse_sequence_arg(option_ids)
 
         self._id_attrs = (self.poll_id, self.user, tuple(self.option_ids))
@@ -236,21 +241,21 @@
         question: str,
         options: Sequence[PollOption],
         total_voter_count: int,
         is_closed: bool,
         is_anonymous: bool,
         type: str,  # pylint: disable=redefined-builtin
         allows_multiple_answers: bool,
-        correct_option_id: int = None,
-        explanation: str = None,
-        explanation_entities: Sequence[MessageEntity] = None,
-        open_period: int = None,
-        close_date: datetime.datetime = None,
+        correct_option_id: Optional[int] = None,
+        explanation: Optional[str] = None,
+        explanation_entities: Optional[Sequence[MessageEntity]] = None,
+        open_period: Optional[int] = None,
+        close_date: Optional[datetime.datetime] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.id: str = id  # pylint: disable=invalid-name
         self.question: str = question
         self.options: Tuple[PollOption, ...] = parse_sequence_arg(options)
         self.total_voter_count: int = total_voter_count
         self.is_closed: bool = is_closed
@@ -309,15 +314,17 @@
             raise RuntimeError("This Poll has no 'explanation'.")
 
         entity_text = self.explanation.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
 
         return entity_text.decode("utf-16-le")
 
-    def parse_explanation_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
+    def parse_explanation_entities(
+        self, types: Optional[List[str]] = None
+    ) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
         It contains entities from this polls explanation filtered by their ``type`` attribute as
         the key, and the text that each entity belongs to as the value of the :obj:`dict`.
 
         Note:
             This method should always be used instead of the :attr:`explanation_entities`
@@ -339,61 +346,61 @@
 
         return {
             entity: self.parse_explanation_entity(entity)
             for entity in self.explanation_entities
             if entity.type in types
         }
 
-    REGULAR: ClassVar[str] = constants.PollType.REGULAR
+    REGULAR: Final[str] = constants.PollType.REGULAR
     """:const:`telegram.constants.PollType.REGULAR`"""
-    QUIZ: ClassVar[str] = constants.PollType.QUIZ
+    QUIZ: Final[str] = constants.PollType.QUIZ
     """:const:`telegram.constants.PollType.QUIZ`"""
-    MAX_EXPLANATION_LENGTH: ClassVar[int] = constants.PollLimit.MAX_EXPLANATION_LENGTH
+    MAX_EXPLANATION_LENGTH: Final[int] = constants.PollLimit.MAX_EXPLANATION_LENGTH
     """:const:`telegram.constants.PollLimit.MAX_EXPLANATION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_EXPLANATION_LINE_FEEDS: ClassVar[int] = constants.PollLimit.MAX_EXPLANATION_LINE_FEEDS
+    MAX_EXPLANATION_LINE_FEEDS: Final[int] = constants.PollLimit.MAX_EXPLANATION_LINE_FEEDS
     """:const:`telegram.constants.PollLimit.MAX_EXPLANATION_LINE_FEEDS`
 
     .. versionadded:: 20.0
     """
-    MIN_OPEN_PERIOD: ClassVar[int] = constants.PollLimit.MIN_OPEN_PERIOD
+    MIN_OPEN_PERIOD: Final[int] = constants.PollLimit.MIN_OPEN_PERIOD
     """:const:`telegram.constants.PollLimit.MIN_OPEN_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MAX_OPEN_PERIOD: ClassVar[int] = constants.PollLimit.MAX_OPEN_PERIOD
+    MAX_OPEN_PERIOD: Final[int] = constants.PollLimit.MAX_OPEN_PERIOD
     """:const:`telegram.constants.PollLimit.MAX_OPEN_PERIOD`
 
     .. versionadded:: 20.0
     """
-    MIN_QUESTION_LENGTH: ClassVar[int] = constants.PollLimit.MIN_QUESTION_LENGTH
+    MIN_QUESTION_LENGTH: Final[int] = constants.PollLimit.MIN_QUESTION_LENGTH
     """:const:`telegram.constants.PollLimit.MIN_QUESTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_QUESTION_LENGTH: ClassVar[int] = constants.PollLimit.MAX_QUESTION_LENGTH
+    MAX_QUESTION_LENGTH: Final[int] = constants.PollLimit.MAX_QUESTION_LENGTH
     """:const:`telegram.constants.PollLimit.MAX_QUESTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MIN_OPTION_LENGTH: ClassVar[int] = constants.PollLimit.MIN_OPTION_LENGTH
+    MIN_OPTION_LENGTH: Final[int] = constants.PollLimit.MIN_OPTION_LENGTH
     """:const:`telegram.constants.PollLimit.MIN_OPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MAX_OPTION_LENGTH: ClassVar[int] = constants.PollLimit.MAX_OPTION_LENGTH
+    MAX_OPTION_LENGTH: Final[int] = constants.PollLimit.MAX_OPTION_LENGTH
     """:const:`telegram.constants.PollLimit.MAX_OPTION_LENGTH`
 
     .. versionadded:: 20.0
     """
-    MIN_OPTION_NUMBER: ClassVar[int] = constants.PollLimit.MIN_OPTION_NUMBER
+    MIN_OPTION_NUMBER: Final[int] = constants.PollLimit.MIN_OPTION_NUMBER
     """:const:`telegram.constants.PollLimit.MIN_OPTION_NUMBER`
 
     .. versionadded:: 20.0
     """
-    MAX_OPTION_NUMBER: ClassVar[int] = constants.PollLimit.MAX_OPTION_NUMBER
+    MAX_OPTION_NUMBER: Final[int] = constants.PollLimit.MAX_OPTION_NUMBER
     """:const:`telegram.constants.PollLimit.MAX_OPTION_NUMBER`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_proximityalerttriggered.py` & `python-telegram-bot-raw-20.4/telegram/_proximityalerttriggered.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,15 +46,20 @@
         distance (:obj:`int`): The distance between the users
 
     """
 
     __slots__ = ("traveler", "distance", "watcher")
 
     def __init__(
-        self, traveler: User, watcher: User, distance: int, *, api_kwargs: JSONDict = None
+        self,
+        traveler: User,
+        watcher: User,
+        distance: int,
+        *,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.traveler: User = traveler
         self.watcher: User = watcher
         self.distance: int = distance
 
         self._id_attrs = (self.traveler, self.watcher, self.distance)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_replykeyboardmarkup.py` & `python-telegram-bot-raw-20.4/telegram/_replykeyboardmarkup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram ReplyKeyboardMarkup."""
 
-from typing import ClassVar, Optional, Sequence, Tuple, Union
+from typing import Final, Optional, Sequence, Tuple, Union
 
 from telegram import constants
 from telegram._keyboardbutton import KeyboardButton
 from telegram._telegramobject import TelegramObject
 from telegram._utils.markup import check_keyboard_type
 from telegram._utils.types import JSONDict
 
@@ -127,21 +127,21 @@
         "input_field_placeholder",
         "is_persistent",
     )
 
     def __init__(
         self,
         keyboard: Sequence[Sequence[Union[str, KeyboardButton]]],
-        resize_keyboard: bool = None,
-        one_time_keyboard: bool = None,
-        selective: bool = None,
-        input_field_placeholder: str = None,
-        is_persistent: bool = None,
+        resize_keyboard: Optional[bool] = None,
+        one_time_keyboard: Optional[bool] = None,
+        selective: Optional[bool] = None,
+        input_field_placeholder: Optional[str] = None,
+        is_persistent: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         if not check_keyboard_type(keyboard):
             raise ValueError(
                 "The parameter `keyboard` should be a sequence of sequences of "
                 "strings or KeyboardButtons"
             )
@@ -166,16 +166,16 @@
     @classmethod
     def from_button(
         cls,
         button: Union[KeyboardButton, str],
         resize_keyboard: bool = False,
         one_time_keyboard: bool = False,
         selective: bool = False,
-        input_field_placeholder: str = None,
-        is_persistent: bool = None,
+        input_field_placeholder: Optional[str] = None,
+        is_persistent: Optional[bool] = None,
         **kwargs: object,
     ) -> "ReplyKeyboardMarkup":
         """Shortcut for::
 
             ReplyKeyboardMarkup([[button]], **kwargs)
 
         Return a ReplyKeyboardMarkup from a single KeyboardButton.
@@ -224,16 +224,16 @@
     @classmethod
     def from_row(
         cls,
         button_row: Sequence[Union[str, KeyboardButton]],
         resize_keyboard: bool = False,
         one_time_keyboard: bool = False,
         selective: bool = False,
-        input_field_placeholder: str = None,
-        is_persistent: bool = None,
+        input_field_placeholder: Optional[str] = None,
+        is_persistent: Optional[bool] = None,
         **kwargs: object,
     ) -> "ReplyKeyboardMarkup":
         """Shortcut for::
 
             ReplyKeyboardMarkup([button_row], **kwargs)
 
         Return a ReplyKeyboardMarkup from a single row of KeyboardButtons.
@@ -286,16 +286,16 @@
     @classmethod
     def from_column(
         cls,
         button_column: Sequence[Union[str, KeyboardButton]],
         resize_keyboard: bool = False,
         one_time_keyboard: bool = False,
         selective: bool = False,
-        input_field_placeholder: str = None,
-        is_persistent: bool = None,
+        input_field_placeholder: Optional[str] = None,
+        is_persistent: Optional[bool] = None,
         **kwargs: object,
     ) -> "ReplyKeyboardMarkup":
         """Shortcut for::
 
             ReplyKeyboardMarkup([[button] for button in button_column], **kwargs)
 
         Return a ReplyKeyboardMarkup from a single column of KeyboardButtons.
@@ -342,17 +342,17 @@
             one_time_keyboard=one_time_keyboard,
             selective=selective,
             input_field_placeholder=input_field_placeholder,
             is_persistent=is_persistent,
             **kwargs,  # type: ignore[arg-type]
         )
 
-    MIN_INPUT_FIELD_PLACEHOLDER: ClassVar[int] = constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER
+    MIN_INPUT_FIELD_PLACEHOLDER: Final[int] = constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER
     """:const:`telegram.constants.ReplyLimit.MIN_INPUT_FIELD_PLACEHOLDER`
 
     .. versionadded:: 20.0
     """
-    MAX_INPUT_FIELD_PLACEHOLDER: ClassVar[int] = constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER
+    MAX_INPUT_FIELD_PLACEHOLDER: Final[int] = constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER
     """:const:`telegram.constants.ReplyLimit.MAX_INPUT_FIELD_PLACEHOLDER`
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_replykeyboardremove.py` & `python-telegram-bot-raw-20.4/telegram/_replykeyboardremove.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             2) If the bot's message is a reply (has ``reply_to_message_id``), sender of
                the original message.
 
     """
 
     __slots__ = ("selective", "remove_keyboard")
 
-    def __init__(self, selective: bool = None, *, api_kwargs: JSONDict = None):
+    def __init__(self, selective: Optional[bool] = None, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.remove_keyboard: bool = True
         # Optionals
         self.selective: Optional[bool] = selective
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_sentwebappmessage.py` & `python-telegram-bot-raw-20.4/telegram/_sentwebappmessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         inline_message_id (:obj:`str`): Optional. Identifier of the sent inline message. Available
             only if there is an :attr:`inline keyboard <telegram.InlineKeyboardMarkup>` attached to
             the message.
     """
 
     __slots__ = ("inline_message_id",)
 
-    def __init__(self, inline_message_id: str = None, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, inline_message_id: Optional[str] = None, *, api_kwargs: Optional[JSONDict] = None
+    ):
         super().__init__(api_kwargs=api_kwargs)
         # Optionals
         self.inline_message_id: Optional[str] = inline_message_id
 
         self._id_attrs = (self.inline_message_id,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_shared.py` & `python-telegram-bot-raw-20.4/telegram/_shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains two objects used for request chats/users service messages."""
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class UserShared(TelegramObject):
     """
     This object contains information about the user whose identifier was shared with the bot
@@ -49,15 +51,15 @@
     __slots__ = ("request_id", "user_id")
 
     def __init__(
         self,
         request_id: int,
         user_id: int,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.request_id: int = request_id
         self.user_id: int = user_id
 
         self._id_attrs = (self.request_id, self.user_id)
 
@@ -92,15 +94,15 @@
     __slots__ = ("request_id", "chat_id")
 
     def __init__(
         self,
         request_id: int,
         chat_id: int,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         self.request_id: int = request_id
         self.chat_id: int = chat_id
 
         self._id_attrs = (self.request_id, self.chat_id)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_switchinlinequerychosenchat.py` & `python-telegram-bot-raw-20.4/telegram/_switchinlinequerychosenchat.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,21 +69,21 @@
         "allow_bot_chats",
         "allow_group_chats",
         "allow_channel_chats",
     )
 
     def __init__(
         self,
-        query: str = None,
-        allow_user_chats: bool = None,
-        allow_bot_chats: bool = None,
-        allow_group_chats: bool = None,
-        allow_channel_chats: bool = None,
+        query: Optional[str] = None,
+        allow_user_chats: Optional[bool] = None,
+        allow_bot_chats: Optional[bool] = None,
+        allow_group_chats: Optional[bool] = None,
+        allow_channel_chats: Optional[bool] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Optional
         self.query: Optional[str] = query
         self.allow_user_chats: Optional[bool] = allow_user_chats
         self.allow_bot_chats: Optional[bool] = allow_bot_chats
         self.allow_group_chats: Optional[bool] = allow_group_chats
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_telegramobject.py` & `python-telegram-bot-raw-20.4/telegram/_telegramobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from contextlib import contextmanager
 from copy import deepcopy
 from itertools import chain
 from types import MappingProxyType
 from typing import (
     TYPE_CHECKING,
     Any,
+    ClassVar,
     Dict,
     Iterator,
     List,
     Mapping,
     Optional,
     Set,
     Tuple,
@@ -88,21 +89,21 @@
 
     """
 
     __slots__ = ("_id_attrs", "_bot", "_frozen", "api_kwargs")
 
     # Used to cache the names of the parameters of the __init__ method of the class
     # Must be a private attribute to avoid name clashes between subclasses
-    __INIT_PARAMS: Set[str] = set()
+    __INIT_PARAMS: ClassVar[Set[str]] = set()
     # Used to check if __INIT_PARAMS has been set for the current class. Unfortunately, we can't
     # just check if `__INIT_PARAMS is None`, since subclasses use the parent class' __INIT_PARAMS
     # unless it's overridden
     __INIT_PARAMS_CHECK: Optional[Type["TelegramObject"]] = None
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         # Setting _frozen to `False` here means that classes without arguments still need to
         # implement __init__. However, with `True` would mean increased usage of
         # `with self._unfrozen()` in the `__init__` of subclasses and we have fewer empty
         # classes than classes with arguments.
         self._frozen: bool = False
         self._id_attrs: Tuple[object, ...] = ()
         self._bot: Optional["Bot"] = None
@@ -442,15 +443,18 @@
             The Telegram object.
 
         """
         return cls._de_json(data=data, bot=bot)
 
     @classmethod
     def _de_json(
-        cls: Type[Tele_co], data: Optional[JSONDict], bot: "Bot", api_kwargs: JSONDict = None
+        cls: Type[Tele_co],
+        data: Optional[JSONDict],
+        bot: "Bot",
+        api_kwargs: Optional[JSONDict] = None,
     ) -> Optional[Tele_co]:
         if data is None:
             return None
 
         # try-except is significantly faster in case we already have a correct argument set
         try:
             obj = cls(**data, api_kwargs=api_kwargs)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_update.py` & `python-telegram-bot-raw-20.4/telegram/_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Update."""
 
-from typing import TYPE_CHECKING, ClassVar, List, Optional
+from typing import TYPE_CHECKING, Final, List, Optional
 
 from telegram import constants
 from telegram._callbackquery import CallbackQuery
 from telegram._chatjoinrequest import ChatJoinRequest
 from telegram._chatmemberupdated import ChatMemberUpdated
 from telegram._choseninlineresult import ChosenInlineResult
 from telegram._inline.inlinequery import InlineQuery
@@ -167,94 +167,94 @@
         "_effective_chat",
         "_effective_message",
         "my_chat_member",
         "chat_member",
         "chat_join_request",
     )
 
-    MESSAGE: ClassVar[str] = constants.UpdateType.MESSAGE
+    MESSAGE: Final[str] = constants.UpdateType.MESSAGE
     """:const:`telegram.constants.UpdateType.MESSAGE`
 
     .. versionadded:: 13.5"""
-    EDITED_MESSAGE: ClassVar[str] = constants.UpdateType.EDITED_MESSAGE
+    EDITED_MESSAGE: Final[str] = constants.UpdateType.EDITED_MESSAGE
     """:const:`telegram.constants.UpdateType.EDITED_MESSAGE`
 
     .. versionadded:: 13.5"""
-    CHANNEL_POST: ClassVar[str] = constants.UpdateType.CHANNEL_POST
+    CHANNEL_POST: Final[str] = constants.UpdateType.CHANNEL_POST
     """:const:`telegram.constants.UpdateType.CHANNEL_POST`
 
     .. versionadded:: 13.5"""
-    EDITED_CHANNEL_POST: ClassVar[str] = constants.UpdateType.EDITED_CHANNEL_POST
+    EDITED_CHANNEL_POST: Final[str] = constants.UpdateType.EDITED_CHANNEL_POST
     """:const:`telegram.constants.UpdateType.EDITED_CHANNEL_POST`
 
     .. versionadded:: 13.5"""
-    INLINE_QUERY: ClassVar[str] = constants.UpdateType.INLINE_QUERY
+    INLINE_QUERY: Final[str] = constants.UpdateType.INLINE_QUERY
     """:const:`telegram.constants.UpdateType.INLINE_QUERY`
 
     .. versionadded:: 13.5"""
-    CHOSEN_INLINE_RESULT: ClassVar[str] = constants.UpdateType.CHOSEN_INLINE_RESULT
+    CHOSEN_INLINE_RESULT: Final[str] = constants.UpdateType.CHOSEN_INLINE_RESULT
     """:const:`telegram.constants.UpdateType.CHOSEN_INLINE_RESULT`
 
     .. versionadded:: 13.5"""
-    CALLBACK_QUERY: ClassVar[str] = constants.UpdateType.CALLBACK_QUERY
+    CALLBACK_QUERY: Final[str] = constants.UpdateType.CALLBACK_QUERY
     """:const:`telegram.constants.UpdateType.CALLBACK_QUERY`
 
     .. versionadded:: 13.5"""
-    SHIPPING_QUERY: ClassVar[str] = constants.UpdateType.SHIPPING_QUERY
+    SHIPPING_QUERY: Final[str] = constants.UpdateType.SHIPPING_QUERY
     """:const:`telegram.constants.UpdateType.SHIPPING_QUERY`
 
     .. versionadded:: 13.5"""
-    PRE_CHECKOUT_QUERY: ClassVar[str] = constants.UpdateType.PRE_CHECKOUT_QUERY
+    PRE_CHECKOUT_QUERY: Final[str] = constants.UpdateType.PRE_CHECKOUT_QUERY
     """:const:`telegram.constants.UpdateType.PRE_CHECKOUT_QUERY`
 
     .. versionadded:: 13.5"""
-    POLL: ClassVar[str] = constants.UpdateType.POLL
+    POLL: Final[str] = constants.UpdateType.POLL
     """:const:`telegram.constants.UpdateType.POLL`
 
     .. versionadded:: 13.5"""
-    POLL_ANSWER: ClassVar[str] = constants.UpdateType.POLL_ANSWER
+    POLL_ANSWER: Final[str] = constants.UpdateType.POLL_ANSWER
     """:const:`telegram.constants.UpdateType.POLL_ANSWER`
 
     .. versionadded:: 13.5"""
-    MY_CHAT_MEMBER: ClassVar[str] = constants.UpdateType.MY_CHAT_MEMBER
+    MY_CHAT_MEMBER: Final[str] = constants.UpdateType.MY_CHAT_MEMBER
     """:const:`telegram.constants.UpdateType.MY_CHAT_MEMBER`
 
     .. versionadded:: 13.5"""
-    CHAT_MEMBER: ClassVar[str] = constants.UpdateType.CHAT_MEMBER
+    CHAT_MEMBER: Final[str] = constants.UpdateType.CHAT_MEMBER
     """:const:`telegram.constants.UpdateType.CHAT_MEMBER`
 
     .. versionadded:: 13.5"""
-    CHAT_JOIN_REQUEST = constants.UpdateType.CHAT_JOIN_REQUEST
+    CHAT_JOIN_REQUEST: Final[str] = constants.UpdateType.CHAT_JOIN_REQUEST
     """:const:`telegram.constants.UpdateType.CHAT_JOIN_REQUEST`
 
     .. versionadded:: 13.8"""
-    ALL_TYPES: ClassVar[List[str]] = list(constants.UpdateType)
+    ALL_TYPES: Final[List[str]] = list(constants.UpdateType)
     """List[:obj:`str`]: A list of all available update types.
 
     .. versionadded:: 13.5"""
 
     def __init__(
         self,
         update_id: int,
-        message: Message = None,
-        edited_message: Message = None,
-        channel_post: Message = None,
-        edited_channel_post: Message = None,
-        inline_query: InlineQuery = None,
-        chosen_inline_result: ChosenInlineResult = None,
-        callback_query: CallbackQuery = None,
-        shipping_query: ShippingQuery = None,
-        pre_checkout_query: PreCheckoutQuery = None,
-        poll: Poll = None,
-        poll_answer: PollAnswer = None,
-        my_chat_member: ChatMemberUpdated = None,
-        chat_member: ChatMemberUpdated = None,
-        chat_join_request: ChatJoinRequest = None,
+        message: Optional[Message] = None,
+        edited_message: Optional[Message] = None,
+        channel_post: Optional[Message] = None,
+        edited_channel_post: Optional[Message] = None,
+        inline_query: Optional[InlineQuery] = None,
+        chosen_inline_result: Optional[ChosenInlineResult] = None,
+        callback_query: Optional[CallbackQuery] = None,
+        shipping_query: Optional[ShippingQuery] = None,
+        pre_checkout_query: Optional[PreCheckoutQuery] = None,
+        poll: Optional[Poll] = None,
+        poll_answer: Optional[PollAnswer] = None,
+        my_chat_member: Optional[ChatMemberUpdated] = None,
+        chat_member: Optional[ChatMemberUpdated] = None,
+        chat_join_request: Optional[ChatJoinRequest] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.update_id: int = update_id
         # Optionals
         self.message: Optional[Message] = message
         self.edited_message: Optional[Message] = edited_message
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_userprofilephotos.py` & `python-telegram-bot-raw-20.4/telegram/_userprofilephotos.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     __slots__ = ("photos", "total_count")
 
     def __init__(
         self,
         total_count: int,
         photos: Sequence[Sequence[PhotoSize]],
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.total_count: int = total_count
         self.photos: Tuple[Tuple[PhotoSize, ...], ...] = tuple(tuple(sizes) for sizes in photos)
 
         self._id_attrs = (self.total_count, self.photos)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/argumentparsing.py` & `python-telegram-bot-raw-20.4/telegram/_utils/argumentparsing.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/datetime.py` & `python-telegram-bot-raw-20.4/telegram/_utils/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     if tzinfo is DTM_UTC:
         return datetime.replace(tzinfo=DTM_UTC)
     return tzinfo.localize(datetime)  # type: ignore[attr-defined]
 
 
 def to_float_timestamp(
     time_object: Union[int, float, dtm.timedelta, dtm.datetime, dtm.time],
-    reference_timestamp: float = None,
-    tzinfo: dtm.tzinfo = None,
+    reference_timestamp: Optional[float] = None,
+    tzinfo: Optional[dtm.tzinfo] = None,
 ) -> float:
     """
     Converts a given time object to a float POSIX timestamp.
     Used to convert different time specifications to a common format. The time object
     can be relative (i.e. indicate a time increment, or a time of day) or absolute.
     Objects from the :class:`datetime` module that are timezone-naive will be assumed
     to be in UTC, if ``bot`` is not passed or ``bot.defaults`` is :obj:`None`.
@@ -145,16 +145,16 @@
         return _datetime_to_float_timestamp(time_object)
 
     raise TypeError(f"Unable to convert {type(time_object).__name__} object to timestamp")
 
 
 def to_timestamp(
     dt_obj: Union[int, float, dtm.timedelta, dtm.datetime, dtm.time, None],
-    reference_timestamp: float = None,
-    tzinfo: dtm.tzinfo = None,
+    reference_timestamp: Optional[float] = None,
+    tzinfo: Optional[dtm.tzinfo] = None,
 ) -> Optional[int]:
     """
     Wrapper over :func:`to_float_timestamp` which returns an integer (the float value truncated
     down to the nearest integer).
 
     See the documentation for :func:`to_float_timestamp` for more details.
     """
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/defaultvalue.py` & `python-telegram-bot-raw-20.4/telegram/_utils/defaultvalue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/enum.py` & `python-telegram-bot-raw-20.4/telegram/_utils/enum.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/files.py` & `python-telegram-bot-raw-20.4/telegram/_utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,16 @@
         return path.is_file()
     except Exception:
         return False
 
 
 def parse_file_input(  # pylint: disable=too-many-return-statements
     file_input: Union[FileInput, "TelegramObject"],
-    tg_type: Type["TelegramObject"] = None,
-    filename: str = None,
+    tg_type: Optional[Type["TelegramObject"]] = None,
+    filename: Optional[str] = None,
     attach: bool = False,
     local_mode: bool = False,
 ) -> Union[str, "InputFile", Any]:
     """
     Parses input for sending files:
 
     * For string input, if the input is an absolute path of a local file:
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/logging.py` & `python-telegram-bot-raw-20.4/telegram/_utils/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 
 Warning:
     Contents of this module are intended to be used internally by the library and *not* by the
     user. Changes to this module are not considered breaking changes and may not be documented in
     the changelog.
 """
 import logging
+from typing import Optional
 
 
-def get_logger(file_name: str, class_name: str = None) -> logging.Logger:
+def get_logger(file_name: str, class_name: Optional[str] = None) -> logging.Logger:
     """Returns a logger with an appropriate name.
     Use as follows::
 
         logger = get_logger(__name__)
 
     If for example `__name__` is `telegram.ext._updater`, the logger will be named
     `telegram.ext.Updater`. If `class_name` is passed, this will result in
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/markup.py` & `python-telegram-bot-raw-20.4/telegram/_utils/markup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/types.py` & `python-telegram-bot-raw-20.4/telegram/_utils/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,26 @@
 
 Warning:
     Contents of this module are intended to be used internally by the library and *not* by the
     user. Changes to this module are not considered breaking changes and may not be documented in
     the changelog.
 """
 from pathlib import Path
-from typing import IO, TYPE_CHECKING, Any, Collection, Dict, Optional, Tuple, TypeVar, Union
+from typing import (
+    IO,
+    TYPE_CHECKING,
+    Any,
+    Collection,
+    Dict,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 if TYPE_CHECKING:
     from telegram import (
         ForceReply,
         InlineKeyboardMarkup,
         InputFile,
         ReplyKeyboardMarkup,
@@ -71,7 +82,16 @@
 .. versionadded:: 20.0
 """
 
 FieldTuple = Tuple[str, bytes, str]
 """Alias for return type of `InputFile.field_tuple`."""
 UploadFileDict = Dict[str, FieldTuple]
 """Dictionary containing file data to be uploaded to the API."""
+
+HTTPVersion = Literal["1.1", "2.0"]
+"""Allowed HTTP versions.
+
+.. versionadded:: 20.4"""
+
+CorrectOptionID = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+
+MarkdownVersion = Literal[1, 2]
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/warnings.py` & `python-telegram-bot-raw-20.4/telegram/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_utils/warnings_transition.py` & `python-telegram-bot-raw-20.4/telegram/_utils/warnings_transition.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/_version.py` & `python-telegram-bot-raw-20.4/telegram/_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 # pylint: disable=missing-module-docstring
-from typing import NamedTuple
+from typing import Final, NamedTuple
 
 __all__ = ("__version__", "__version_info__", "__bot_api_version__", "__bot_api_version_info__")
 
 
 class Version(NamedTuple):
     """Copies the behavior of sys.version_info.
     serial is always 0 for stable releases.
@@ -46,18 +46,22 @@
             version = f"{version}.{self.micro}"
         if self.releaselevel != "final":
             version = f"{version}{self._rl_shorthand()}{self.serial}"
 
         return version
 
 
-__version_info__ = Version(major=20, minor=3, micro=0, releaselevel="final", serial=0)
-__version__ = str(__version_info__)
+__version_info__: Final[Version] = Version(
+    major=20, minor=4, micro=0, releaselevel="final", serial=0
+)
+__version__: Final[str] = str(__version_info__)
 
 # # SETUP.PY MARKER
 # Lines above this line will be `exec`-cuted in setup.py. Make sure that this only contains
 # std-lib imports!
 
 from telegram import constants  # noqa: E402  # pylint: disable=wrong-import-position
 
-__bot_api_version__ = constants.BOT_API_VERSION
-__bot_api_version_info__ = constants.BOT_API_VERSION_INFO
+__bot_api_version__: Final[str] = constants.BOT_API_VERSION
+__bot_api_version_info__: Final[
+    constants._BotAPIVersion
+] = constants.BOT_API_VERSION_INFO  # pylint: disable=protected-access
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_videochat.py` & `python-telegram-bot-raw-20.4/telegram/_videochat.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     .. versionadded:: 13.4
     .. versionchanged:: 20.0
         This class was renamed from ``VoiceChatStarted`` in accordance to Bot API 6.0.
     """
 
     __slots__ = ()
 
-    def __init__(self, *, api_kwargs: JSONDict = None) -> None:
+    def __init__(self, *, api_kwargs: Optional[JSONDict] = None) -> None:
         super().__init__(api_kwargs=api_kwargs)
 
         self._freeze()
 
 
 class VideoChatEnded(TelegramObject):
     """
@@ -71,15 +71,15 @@
 
     __slots__ = ("duration",)
 
     def __init__(
         self,
         duration: int,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> None:
         super().__init__(api_kwargs=api_kwargs)
         self.duration: int = duration
         self._id_attrs = (self.duration,)
 
         self._freeze()
 
@@ -111,15 +111,15 @@
 
     __slots__ = ("users",)
 
     def __init__(
         self,
         users: Sequence[User],
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> None:
         super().__init__(api_kwargs=api_kwargs)
         self.users: Tuple[User, ...] = parse_sequence_arg(users)
         self._id_attrs = (self.users,)
 
         self._freeze()
 
@@ -163,15 +163,15 @@
 
     __slots__ = ("start_date",)
 
     def __init__(
         self,
         start_date: dtm.datetime,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ) -> None:
         super().__init__(api_kwargs=api_kwargs)
         self.start_date: dtm.datetime = start_date
 
         self._id_attrs = (self.start_date,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_webappdata.py` & `python-telegram-bot-raw-20.4/telegram/_webappdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram WebAppData."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class WebAppData(TelegramObject):
     """Contains data sent from a `Web App <https://core.telegram.org/bots/webapps>`_ to the bot.
 
@@ -47,15 +49,15 @@
 
             Warning:
                 Be aware that a bad client can send arbitrary data in this field.
     """
 
     __slots__ = ("data", "button_text")
 
-    def __init__(self, data: str, button_text: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, data: str, button_text: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.data: str = data
         self.button_text: str = button_text
 
         self._id_attrs = (self.data, self.button_text)
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_webappinfo.py` & `python-telegram-bot-raw-20.4/telegram/_webappinfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Web App Info."""
 
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class WebAppInfo(TelegramObject):
     """
     This object contains information about a `Web App <https://core.telegram.org/bots/webapps>`_.
@@ -43,15 +45,15 @@
         url (:obj:`str`): An HTTPS URL of a Web App to be opened with additional data as specified
             in `Initializing Web Apps \
             <https://core.telegram.org/bots/webapps#initializing-web-apps>`_.
     """
 
     __slots__ = ("url",)
 
-    def __init__(self, url: str, *, api_kwargs: JSONDict = None):
+    def __init__(self, url: str, *, api_kwargs: Optional[JSONDict] = None):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.url: str = url
 
         self._id_attrs = (self.url,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_webhookinfo.py` & `python-telegram-bot-raw-20.4/telegram/_webhookinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,22 +119,22 @@
     )
 
     def __init__(
         self,
         url: str,
         has_custom_certificate: bool,
         pending_update_count: int,
-        last_error_date: int = None,
-        last_error_message: str = None,
-        max_connections: int = None,
-        allowed_updates: Sequence[str] = None,
-        ip_address: str = None,
-        last_synchronization_error_date: int = None,
+        last_error_date: Optional[int] = None,
+        last_error_message: Optional[str] = None,
+        max_connections: Optional[int] = None,
+        allowed_updates: Optional[Sequence[str]] = None,
+        ip_address: Optional[str] = None,
+        last_synchronization_error_date: Optional[int] = None,
         *,
-        api_kwargs: JSONDict = None,
+        api_kwargs: Optional[JSONDict] = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.url: str = url
         self.has_custom_certificate: bool = has_custom_certificate
         self.pending_update_count: int = pending_update_count
```

### Comparing `python-telegram-bot-raw-20.3/telegram/_writeaccessallowed.py` & `python-telegram-bot-raw-20.4/telegram/_writeaccessallowed.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,12 +40,14 @@
 
             .. versionadded:: 20.3
 
     """
 
     __slots__ = ("web_app_name",)
 
-    def __init__(self, web_app_name: str = None, *, api_kwargs: JSONDict = None):
+    def __init__(
+        self, web_app_name: Optional[str] = None, *, api_kwargs: Optional[JSONDict] = None
+    ):
         super().__init__(api_kwargs=api_kwargs)
         self.web_app_name: Optional[str] = web_app_name
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.3/telegram/constants.py` & `python-telegram-bot-raw-20.4/telegram/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     "StickerType",
     "WebhookLimit",
     "UpdateType",
     "UserProfilePhotosLimit",
 ]
 
 import sys
-from typing import List, NamedTuple
+from typing import Final, List, NamedTuple
 
 from telegram._utils.enum import IntEnum, StringEnum
 
 
 class _BotAPIVersion(NamedTuple):
     """Similar behavior to sys.version_info.
     So far TG has only published X.Y releases. We can add X.Y.Z(a(S)) if needed.
@@ -112,27 +112,27 @@
 #: :class:`typing.NamedTuple`: A tuple containing the two components of the version number:
 # ``major`` and ``minor``. Both values are integers.
 #: The components can also be accessed by name, so ``BOT_API_VERSION_INFO[0]`` is equivalent
 #: to ``BOT_API_VERSION_INFO.major`` and so on. Also available as
 #: :data:`telegram.__bot_api_version_info__`.
 #:
 #: .. versionadded:: 20.0
-BOT_API_VERSION_INFO = _BotAPIVersion(major=6, minor=7)
+BOT_API_VERSION_INFO: Final[_BotAPIVersion] = _BotAPIVersion(major=6, minor=7)
 #: :obj:`str`: Telegram Bot API
 #: version supported by this version of `python-telegram-bot`. Also available as
 #: :data:`telegram.__bot_api_version__`.
 #:
 #: .. versionadded:: 13.4
-BOT_API_VERSION = str(BOT_API_VERSION_INFO)
+BOT_API_VERSION: Final[str] = str(BOT_API_VERSION_INFO)
 
 # constants above this line are tested
 
 #: List[:obj:`int`]: Ports supported by
 #:  :paramref:`telegram.Bot.set_webhook.url`.
-SUPPORTED_WEBHOOK_PORTS: List[int] = [443, 80, 88, 8443]
+SUPPORTED_WEBHOOK_PORTS: Final[List[int]] = [443, 80, 88, 8443]
 
 
 class BotCommandLimit(IntEnum):
     """This enum contains limitations for :class:`telegram.BotCommand` and
     :meth:`telegram.Bot.set_my_commands`.
     The enum members of this enumeration are instances of :class:`int` and can be treated as such.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/error.py` & `python-telegram-bot-raw-20.4/telegram/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "NetworkError",
     "PassportDecryptionError",
     "RetryAfter",
     "TelegramError",
     "TimedOut",
 )
 
-from typing import Tuple, Union
+from typing import Optional, Tuple, Union
 
 
 def _lstrip_str(in_s: str, lstr: str) -> str:
     """
     Args:
         in_s (:obj:`str`): in string
         lstr (:obj:`str`): substr to strip from left side
@@ -107,15 +107,15 @@
         message (:obj:`str`, optional): Any additional information about the exception.
 
             .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, message: str = None) -> None:
+    def __init__(self, message: Optional[str] = None) -> None:
         super().__init__("Invalid token" if message is None else message)
 
 
 class NetworkError(TelegramError):
     """Base class for exceptions due to networking errors.
 
     Examples:
@@ -138,15 +138,15 @@
         message (:obj:`str`, optional): Any additional information about the exception.
 
             .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    def __init__(self, message: str = None) -> None:
+    def __init__(self, message: Optional[str] = None) -> None:
         super().__init__(message or "Timed out")
 
 
 class ChatMigrated(TelegramError):
     """
     Raised when the requested group chat migrated to supergroup and has a new chat id.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/helpers.py` & `python-telegram-bot-raw-20.4/telegram/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,24 @@
     "mention_markdown",
 )
 
 import re
 from html import escape
 from typing import TYPE_CHECKING, Optional, Union
 
+from telegram._utils.types import MarkdownVersion
 from telegram.constants import MessageType
 
 if TYPE_CHECKING:
     from telegram import Message, Update
 
 
-def escape_markdown(text: str, version: int = 1, entity_type: str = None) -> str:
+def escape_markdown(
+    text: str, version: MarkdownVersion = 1, entity_type: Optional[str] = None
+) -> str:
     """Helper function to escape telegram markup symbols.
 
     .. versionchanged:: 20.3
         Custom emoji entity escaping is now supported.
 
     Args:
         text (:obj:`str`): The text.
@@ -84,15 +87,15 @@
 
     Returns:
         :obj:`str`: The inline mention for the user as HTML.
     """
     return f'<a href="tg://user?id={user_id}">{escape(name)}</a>'
 
 
-def mention_markdown(user_id: Union[int, str], name: str, version: int = 1) -> str:
+def mention_markdown(user_id: Union[int, str], name: str, version: MarkdownVersion = 1) -> str:
     """
     Helper function to create a user mention in Markdown syntax.
 
     Args:
         user_id (:obj:`int`): The user's id which you want to mention.
         name (:obj:`str`): The name the mention is showing.
         version (:obj:`int` | :obj:`str`): Use to specify the version of Telegram's Markdown.
@@ -136,15 +139,17 @@
     for message_type in MessageType:
         if message[message_type]:
             return message_type
 
     return None
 
 
-def create_deep_linked_url(bot_username: str, payload: str = None, group: bool = False) -> str:
+def create_deep_linked_url(
+    bot_username: str, payload: Optional[str] = None, group: bool = False
+) -> str:
     """
     Creates a deep-linked URL for this :paramref:`~create_deep_linked_url.bot_username` with the
     specified :paramref:`~create_deep_linked_url.payload`. See
     https://core.telegram.org/bots/features#deep-linking to learn more.
 
     The :paramref:`~create_deep_linked_url.payload` may consist of the following characters:
     ``A-Z, a-z, 0-9, _, -``
```

### Comparing `python-telegram-bot-raw-20.3/telegram/request/__init__.py` & `python-telegram-bot-raw-20.4/telegram/request/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.3/telegram/request/_baserequest.py` & `python-telegram-bot-raw-20.4/telegram/request/_baserequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an abstract class to make POST and GET requests."""
 import abc
-import asyncio
 import json
 from http import HTTPStatus
 from types import TracebackType
-from typing import AsyncContextManager, ClassVar, List, Optional, Tuple, Type, TypeVar, Union
+from typing import AsyncContextManager, Final, List, Optional, Tuple, Type, TypeVar, Union, final
 
 from telegram._utils.defaultvalue import DEFAULT_NONE as _DEFAULT_NONE
 from telegram._utils.defaultvalue import DefaultValue
 from telegram._utils.logging import get_logger
 from telegram._utils.types import JSONDict, ODVInput
 from telegram._version import __version__ as ptb_ver
 from telegram.error import (
@@ -80,18 +79,18 @@
         :wiki:`Builder Pattern <Builder-Pattern>`
 
     .. versionadded:: 20.0
     """
 
     __slots__ = ()
 
-    USER_AGENT: ClassVar[str] = f"python-telegram-bot v{ptb_ver} (https://python-telegram-bot.org)"
+    USER_AGENT: Final[str] = f"python-telegram-bot v{ptb_ver} (https://python-telegram-bot.org)"
     """:obj:`str`: A description that can be used as user agent for requests made to the Bot API.
     """
-    DEFAULT_NONE: ClassVar[DefaultValue[None]] = _DEFAULT_NONE
+    DEFAULT_NONE: Final[DefaultValue[None]] = _DEFAULT_NONE
     """:class:`object`: A special object that indicates that an argument of a function was not
     explicitly passed. Used for the timeout parameters of :meth:`post` and :meth:`do_request`.
 
     Example:
         When calling ``request.post(url)``, ``request`` should use the default timeouts set on
         initialization. When calling ``request.post(url, connect_timeout=5, read_timeout=None)``,
         ``request`` should use ``5`` for the connect timeout and :obj:`None` for the read timeout.
@@ -121,18 +120,19 @@
     async def initialize(self) -> None:
         """Initialize resources used by this class. Must be implemented by a subclass."""
 
     @abc.abstractmethod
     async def shutdown(self) -> None:
         """Stop & clear resources used by this class. Must be implemented by a subclass."""
 
+    @final
     async def post(
         self,
         url: str,
-        request_data: RequestData = None,
+        request_data: Optional[RequestData] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
     ) -> Union[JSONDict, List[JSONDict], bool]:
         """Makes a request to the Bot API handles the return code and parses the answer.
 
@@ -175,14 +175,15 @@
             pool_timeout=pool_timeout,
         )
         json_data = self.parse_json_payload(result)
         # For successful requests, the results are in the 'result' entry
         # see https://core.telegram.org/bots/api#making-requests
         return json_data["result"]
 
+    @final
     async def retrieve(
         self,
         url: str,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -225,15 +226,15 @@
             pool_timeout=pool_timeout,
         )
 
     async def _request_wrapper(
         self,
         url: str,
         method: str,
-        request_data: RequestData = None,
+        request_data: Optional[RequestData] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
     ) -> bytes:
         """Wraps the real implementation request method.
 
@@ -279,22 +280,18 @@
                 method=method,
                 request_data=request_data,
                 read_timeout=read_timeout,
                 write_timeout=write_timeout,
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
             )
-        except asyncio.CancelledError as exc:
-            # TODO: in py3.8+, CancelledError is a subclass of BaseException, so we can drop this
-            #  clause when we drop py3.7
-            raise exc
         except TelegramError as exc:
             raise exc
         except Exception as exc:
-            raise NetworkError(f"Unknown error in HTTP implementation: {repr(exc)}") from exc
+            raise NetworkError(f"Unknown error in HTTP implementation: {exc!r}") from exc
 
         if HTTPStatus.OK <= code <= 299:
             # 200-299 range are HTTP success statuses
             return payload
 
         response_data = self.parse_json_payload(payload)
 
@@ -358,15 +355,15 @@
             raise TelegramError("Invalid server response") from exc
 
     @abc.abstractmethod
     async def do_request(
         self,
         url: str,
         method: str,
-        request_data: RequestData = None,
+        request_data: Optional[RequestData] = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
     ) -> Tuple[int, bytes]:
         """Makes a request to the Bot API. Must be implemented by a subclass.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/request/_httpxrequest.py` & `python-telegram-bot-raw-20.4/telegram/request/_httpxrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """This module contains methods to make POST and GET requests using the httpx library."""
 from typing import Optional, Tuple
 
 import httpx
 
 from telegram._utils.defaultvalue import DefaultValue
 from telegram._utils.logging import get_logger
-from telegram._utils.types import ODVInput
+from telegram._utils.types import HTTPVersion, ODVInput
 from telegram.error import NetworkError, TimedOut
 from telegram.request._baserequest import BaseRequest
 from telegram.request._requestdata import RequestData
 
 # Note to future devs:
 # Proxies are currently only tested manually. The httpx development docs have a nice guide on that:
 # https://www.python-httpx.org/contributing/#development-proxy-setup (also saved on archive.org)
@@ -52,15 +52,15 @@
         proxy_url (:obj:`str`, optional): The URL to the proxy server. For example
             ``'http://127.0.0.1:3128'`` or ``'socks5://127.0.0.1:3128'``. Defaults to :obj:`None`.
 
             Note:
                 * The proxy URL can also be set via the environment variables ``HTTPS_PROXY`` or
                   ``ALL_PROXY``. See `the docs of httpx`_ for more info.
                 * For Socks5 support, additional dependencies are required. Make sure to install
-                  PTB via :command:`pip install python-telegram-bot[socks]` in this case.
+                  PTB via :command:`pip install "python-telegram-bot[socks]"` in this case.
                 * Socks5 proxies can not be set via environment variables.
 
             .. _the docs of httpx: https://www.python-httpx.org/environment_variables/#proxies
         read_timeout (:obj:`float` | :obj:`None`, optional): If passed, specifies the maximum
             amount of time (in seconds) to wait for a response from Telegram's server.
             This value is used unless a different value is passed to :meth:`do_request`.
             Defaults to ``5``.
@@ -92,20 +92,20 @@
     """
 
     __slots__ = ("_client", "_client_kwargs", "_http_version")
 
     def __init__(
         self,
         connection_pool_size: int = 1,
-        proxy_url: str = None,
+        proxy_url: Optional[str] = None,
         read_timeout: Optional[float] = 5.0,
         write_timeout: Optional[float] = 5.0,
         connect_timeout: Optional[float] = 5.0,
         pool_timeout: Optional[float] = 1.0,
-        http_version: str = "1.1",
+        http_version: HTTPVersion = "1.1",
     ):
         self._http_version = http_version
         timeout = httpx.Timeout(
             connect=connect_timeout,
             read=read_timeout,
             write=write_timeout,
             pool=pool_timeout,
@@ -135,19 +135,19 @@
         except ImportError as exc:
             if "httpx[http2]" not in str(exc) and "httpx[socks]" not in str(exc):
                 raise exc
 
             if "httpx[socks]" in str(exc):
                 raise RuntimeError(
                     "To use Socks5 proxies, PTB must be installed via `pip install "
-                    "python-telegram-bot[socks]`."
+                    '"python-telegram-bot[socks]"`.'
                 ) from exc
             raise RuntimeError(
                 "To use HTTP/2, PTB must be installed via `pip install "
-                "python-telegram-bot[http2]`."
+                '"python-telegram-bot[http2]"`.'
             ) from exc
 
     @property
     def http_version(self) -> str:
         """
         :obj:`str`: Used HTTP version, see :paramref:`http_version`.
 
@@ -171,15 +171,15 @@
 
         await self._client.aclose()
 
     async def do_request(
         self,
         url: str,
         method: str,
-        request_data: RequestData = None,
+        request_data: Optional[RequestData] = None,
         read_timeout: ODVInput[float] = BaseRequest.DEFAULT_NONE,
         write_timeout: ODVInput[float] = BaseRequest.DEFAULT_NONE,
         connect_timeout: ODVInput[float] = BaseRequest.DEFAULT_NONE,
         pool_timeout: ODVInput[float] = BaseRequest.DEFAULT_NONE,
     ) -> Tuple[int, bytes]:
         """See :meth:`BaseRequest.do_request`."""
         if self._client.is_closed:
```

### Comparing `python-telegram-bot-raw-20.3/telegram/request/_requestdata.py` & `python-telegram-bot-raw-20.4/telegram/request/_requestdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,40 +14,41 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser Public License
 #  along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains a class that holds the parameters of a request to the Bot API."""
 import json
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union, final
 from urllib.parse import urlencode
 
 from telegram._utils.types import UploadFileDict
 from telegram.request._requestparameter import RequestParameter
 
 
+@final
 class RequestData:
     """Instances of this class collect the data needed for one request to the Bot API, including
     all parameters and files to be sent along with the request.
 
     .. versionadded:: 20.0
 
     Warning:
-        How exactly instances of this will are created should be considered an implementation
-        detail and not part of PTBs public API. Users should exclusively rely on the documented
+        How exactly instances of this are created should be considered an implementation detail
+        and not part of PTBs public API. Users should exclusively rely on the documented
         attributes, properties and methods.
 
     Attributes:
         contains_files (:obj:`bool`): Whether this object contains files to be uploaded via
             ``multipart/form-data``.
     """
 
     __slots__ = ("_parameters", "contains_files")
 
-    def __init__(self, parameters: List[RequestParameter] = None):
+    def __init__(self, parameters: Optional[List[RequestParameter]] = None):
         self._parameters: List[RequestParameter] = parameters or []
         self.contains_files: bool = any(param.input_files for param in self._parameters)
 
     @property
     def parameters(self) -> Dict[str, Union[str, int, List[Any], Dict[Any, Any]]]:
         """Gives the parameters as mapping of parameter name to the parameter value, which can be
         a single object of type :obj:`int`, :obj:`float`, :obj:`str` or :obj:`bool` or any
@@ -72,26 +73,26 @@
         """
         return {
             param.name: param.json_value
             for param in self._parameters
             if param.json_value is not None
         }
 
-    def url_encoded_parameters(self, encode_kwargs: Dict[str, Any] = None) -> str:
+    def url_encoded_parameters(self, encode_kwargs: Optional[Dict[str, Any]] = None) -> str:
         """Encodes the parameters with :func:`urllib.parse.urlencode`.
 
         Args:
             encode_kwargs (Dict[:obj:`str`, any], optional): Additional keyword arguments to pass
                 along to :func:`urllib.parse.urlencode`.
         """
         if encode_kwargs:
             return urlencode(self.json_parameters, **encode_kwargs)
         return urlencode(self.json_parameters)
 
-    def parametrized_url(self, url: str, encode_kwargs: Dict[str, Any] = None) -> str:
+    def parametrized_url(self, url: str, encode_kwargs: Optional[Dict[str, Any]] = None) -> str:
         """Shortcut for attaching the return value of :meth:`url_encoded_parameters` to the
         :paramref:`url`.
 
         Args:
             url (:obj:`str`): The URL the parameters will be attached to.
             encode_kwargs (Dict[:obj:`str`, any], optional): Additional keyword arguments to pass
                 along to :func:`urllib.parse.urlencode`.
```

### Comparing `python-telegram-bot-raw-20.3/telegram/request/_requestparameter.py` & `python-telegram-bot-raw-20.4/telegram/request/_requestparameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 #
 #  You should have received a copy of the GNU Lesser Public License
 #  along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains a class that describes a single parameter of a request to the Bot API."""
 import json
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, Optional, Sequence, Tuple
+from typing import List, Optional, Sequence, Tuple, final
 
 from telegram._files.inputfile import InputFile
 from telegram._files.inputmedia import InputMedia
 from telegram._files.inputsticker import InputSticker
 from telegram._telegramobject import TelegramObject
 from telegram._utils.datetime import to_timestamp
 from telegram._utils.enum import StringEnum
 from telegram._utils.types import UploadFileDict
 
 
+@final
 @dataclass(repr=True, eq=False, order=False, frozen=True)
 class RequestParameter:
     """Instances of this class represent a single parameter to be sent along with a request to
     the Bot API.
 
     .. versionadded:: 20.0
```

### Comparing `python-telegram-bot-raw-20.3/telegram/warnings.py` & `python-telegram-bot-raw-20.4/telegram/warnings.py`

 * *Files identical despite different names*

