# Comparing `tmp/discoger-2.0.3.tar.gz` & `tmp/discoger-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-2.0.3.tar", last modified: Sat Jul  8 20:35:22 2023, max compression
+gzip compressed data, was "discoger-2.1.0.tar", last modified: Sun Jul  9 20:42:20 2023, max compression
```

## Comparing `discoger-2.0.3.tar` & `discoger-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:35:22.272163 discoger-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 20:35:04.000000 discoger-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 20:35:22.272163 discoger-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-08 20:35:04.000000 discoger-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:35:22.272163 discoger-2.0.3/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:35:04.000000 discoger-2.0.3/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-08 20:35:04.000000 discoger-2.0.3/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-08 20:35:04.000000 discoger-2.0.3/discoger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-08 20:35:04.000000 discoger-2.0.3/discoger/scrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-08 20:35:04.000000 discoger-2.0.3/discoger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:35:22.272163 discoger-2.0.3/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 20:35:22.000000 discoger-2.0.3/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-08 20:35:22.000000 discoger-2.0.3/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:35:22.000000 discoger-2.0.3/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 20:35:22.000000 discoger-2.0.3/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-08 20:35:22.000000 discoger-2.0.3/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-08 20:35:22.272163 discoger-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-08 20:35:04.000000 discoger-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:42:20.871458 discoger-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 20:42:06.000000 discoger-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-09 20:42:20.871458 discoger-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-09 20:42:06.000000 discoger-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:42:20.871458 discoger-2.1.0/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:42:06.000000 discoger-2.1.0/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-09 20:42:06.000000 discoger-2.1.0/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10659 2023-07-09 20:42:06.000000 discoger-2.1.0/discoger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-09 20:42:06.000000 discoger-2.1.0/discoger/scrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-09 20:42:06.000000 discoger-2.1.0/discoger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:42:20.871458 discoger-2.1.0/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-09 20:42:20.000000 discoger-2.1.0/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-09 20:42:20.000000 discoger-2.1.0/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:42:20.000000 discoger-2.1.0/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 20:42:20.000000 discoger-2.1.0/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 20:42:20.000000 discoger-2.1.0/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 20:42:20.871458 discoger-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-09 20:42:06.000000 discoger-2.1.0/setup.py
```

### Comparing `discoger-2.0.3/LICENSE` & `discoger-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-2.0.3/PKG-INFO` & `discoger-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.3
+Version: 2.1.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.1.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.3/README.md` & `discoger-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `discoger-2.0.3/discoger/client.py` & `discoger-2.1.0/discoger/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -166,14 +166,53 @@
             db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
             db["release_list"].pop(int(id_item))
             db.save()
             self.bot.send_message(
                 chat_id, "%s is deleted in following list" % (id_item)
             )
 
+        @self.bot.message_handler(commands=["wantlist"])
+        def wantlist(message):
+            chat_id = message.chat.id
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+            if db.get("wantlist_user"):
+                message.text = db.get("wantlist_user")
+                message.chat.id = chat_id
+                process_wantlist(message)
+            else:
+                msg = "Give your discogs username for checking your wantlist?"
+                answer = self.bot.reply_to(message, msg)
+                self.bot.register_next_step_handler(answer, process_wantlist)
+
+        def process_wantlist(message):
+            chat_id = message.chat.id
+            username = message.text
+            db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
+            try:
+                user_info = self.d.user(username)
+                for i in user_info.wantlist:
+                    release_info = self.d.release(i.id)
+                    if not db.search("release_list[?release_id=='%s']" % (i.id)):
+                        release = scrap.DiscogerInfo(release_info.url, self.d, str(i.id))
+                        db["release_list"].append(release.release_info)
+                        db.save()
+                        logging.info("Item %s added in following list" % (i.id))
+                    else:
+                        logging.info("Item %s already in your following list" % (i.id))
+                self.bot.send_message(
+                    chat_id, "Your wantlist is synchronized"
+                )
+                if not db.get("wantlist_user"):
+                    db["wantlist_user"] = username
+            except discogs_client.exceptions.DiscogsAPIError as e:
+                self.bot.send_message(
+                    chat_id, "Error, %s" % e
+                )
+
+
         def check_discogs(chat_id=None):
             if chat_id:
                 logging.info("Check user list %s" % (chat_id))
                 db = YamlDB(filename="%s/%s.yaml" % (self.database_dir, chat_id))
                 utils.scrap_data(self, chat_id, db)
             else:
                 logging.info("Check all list")
```

### Comparing `discoger-2.0.3/discoger/scrap.py` & `discoger-2.1.0/discoger/scrap.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.3/discoger/utils.py` & `discoger-2.1.0/discoger/utils.py`

 * *Files identical despite different names*

### Comparing `discoger-2.0.3/discoger.egg-info/PKG-INFO` & `discoger-2.1.0/discoger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 2.0.3
+Version: 2.1.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/2.0.3.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/2.1.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-2.0.3/setup.py` & `discoger-2.1.0/setup.py`

 * *Files identical despite different names*

