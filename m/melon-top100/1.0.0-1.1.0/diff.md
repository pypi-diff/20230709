# Comparing `tmp/melon_top100-1.0.0.tar.gz` & `tmp/melon_top100-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_top100-1.0.0.tar", last modified: Tue Apr 19 07:26:30 2022, max compression
+gzip compressed data, was "melon_top100-1.1.0.tar", last modified: Sun Jul  9 13:03:50 2023, max compression
```

## Comparing `melon_top100-1.0.0.tar` & `melon_top100-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 sd         (501) staff       (20)        0 2022-04-19 07:26:30.862292 melon_top100-1.0.0/
--rw-r--r--   0 sd         (501) staff       (20)        0 2022-04-19 01:36:39.000000 melon_top100-1.0.0/LICENSE
--rw-r--r--   0 sd         (501) staff       (20)     1073 2022-04-19 07:26:30.862185 melon_top100-1.0.0/PKG-INFO
--rw-r--r--   0 sd         (501) staff       (20)      567 2022-04-19 07:18:47.000000 melon_top100-1.0.0/README.md
-drwxr-xr-x   0 sd         (501) staff       (20)        0 2022-04-19 07:26:30.861404 melon_top100-1.0.0/melon_top100/
--rw-r--r--   0 sd         (501) staff       (20)     1441 2022-04-19 07:14:40.000000 melon_top100-1.0.0/melon_top100/__init__.py
-drwxr-xr-x   0 sd         (501) staff       (20)        0 2022-04-19 07:26:30.862023 melon_top100-1.0.0/melon_top100.egg-info/
--rw-r--r--   0 sd         (501) staff       (20)     1073 2022-04-19 07:26:30.000000 melon_top100-1.0.0/melon_top100.egg-info/PKG-INFO
--rw-r--r--   0 sd         (501) staff       (20)      230 2022-04-19 07:26:30.000000 melon_top100-1.0.0/melon_top100.egg-info/SOURCES.txt
--rw-r--r--   0 sd         (501) staff       (20)        1 2022-04-19 07:26:30.000000 melon_top100-1.0.0/melon_top100.egg-info/dependency_links.txt
--rw-r--r--   0 sd         (501) staff       (20)       24 2022-04-19 07:26:30.000000 melon_top100-1.0.0/melon_top100.egg-info/requires.txt
--rw-r--r--   0 sd         (501) staff       (20)       13 2022-04-19 07:26:30.000000 melon_top100-1.0.0/melon_top100.egg-info/top_level.txt
--rw-r--r--   0 sd         (501) staff       (20)       38 2022-04-19 07:26:30.862330 melon_top100-1.0.0/setup.cfg
--rw-r--r--   0 sd         (501) staff       (20)      716 2022-04-19 07:26:16.000000 melon_top100-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:03:50.358955 melon_top100-1.1.0/
+-rw-rw-rw-   0        0        0     1099 2023-07-03 10:18:13.000000 melon_top100-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1518 2023-07-09 13:03:50.357954 melon_top100-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-07-09 13:01:39.000000 melon_top100-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 13:03:50.344441 melon_top100-1.1.0/melon_top100/
+-rw-rw-rw-   0        0        0       44 2023-07-03 10:47:56.000000 melon_top100-1.1.0/melon_top100/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-03 10:48:08.000000 melon_top100-1.1.0/melon_top100/melon.py
+drwxrwxrwx   0        0        0        0 2023-07-09 13:03:50.356953 melon_top100-1.1.0/melon_top100.egg-info/
+-rw-rw-rw-   0        0        0     1518 2023-07-09 13:03:50.000000 melon_top100-1.1.0/melon_top100.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-09 13:03:50.000000 melon_top100-1.1.0/melon_top100.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 13:03:50.000000 melon_top100-1.1.0/melon_top100.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 13:03:50.000000 melon_top100-1.1.0/melon_top100.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-09 13:03:50.000000 melon_top100-1.1.0/melon_top100.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-07-09 12:54:35.000000 melon_top100-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 13:03:50.358955 melon_top100-1.1.0/setup.cfg
```

### Comparing `melon_top100-1.0.0/melon_top100/__init__.py` & `melon_top100-1.1.0/melon_top100/melon.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import requests
-from bs4 import BeautifulSoup
-
-headers = {
-    "User-Agent": (
-        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_3) "
-        "AppleWebKit/537.36 (KHTML, like Gecko) "
-        "Chrome/72.0.3626.121 Safari/537.36"
-    ),
-}
-
-def get_songs():
-    res = requests.get("http://www.melon.com/chart/index.htm", headers=headers)
-    res.raise_for_status()
-    html = res.text
-    soup = BeautifulSoup(html, "html.parser")  # HTML Parser
-    tr_tag_list = soup.select(".d_song_list tbody tr")
-
-    song_list = []
-
-    for rank, tr_tag in enumerate(tr_tag_list, 1):
-        song_no = tr_tag["data-song-no"]
-        song_tag = tr_tag.select_one("a[href*=playSong]")
-        album_tag = tr_tag.select_one(".wrap_song_info a[href*=goAlbumDetail]")
-        artist_tag = tr_tag.select_one("a[href*=goArtistDetail]")
-
-        song = {
-            "song_no": song_no,
-            "title": song_tag.text,
-            "album": album_tag.text,
-            "artist": artist_tag.text,
-        }
-        song_list.append(song)
-
-    return song_list
-
-
-def get_like_count(song_no_list):
-    api_url = "https://www.melon.com/commonlike/getSongLike.json"
-    params = {"contsIds": song_no_list}
-    res = requests.get(api_url, params=params, headers=headers)
-    res.raise_for_status()
-    response = res.json()
-    like_list = response["contsLike"]
-    like_dict = {str(song["CONTSID"]): song["SUMMCNT"] for song in like_list}
-    return like_dict
+import requests
+from bs4 import BeautifulSoup
+
+headers = {
+    "User-Agent": (
+        "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_3) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) "
+        "Chrome/72.0.3626.121 Safari/537.36"
+    ),
+}
+
+def get_songs():
+    res = requests.get("http://www.melon.com/chart/index.htm", headers=headers)
+    res.raise_for_status()
+    html = res.text
+    soup = BeautifulSoup(html, "html.parser")  # HTML Parser
+    tr_tag_list = soup.select(".d_song_list tbody tr")
+
+    song_list = []
+
+    for rank, tr_tag in enumerate(tr_tag_list, 1):
+        song_no = tr_tag["data-song-no"]
+        song_tag = tr_tag.select_one("a[href*=playSong]")
+        album_tag = tr_tag.select_one(".wrap_song_info a[href*=goAlbumDetail]")
+        artist_tag = tr_tag.select_one("a[href*=goArtistDetail]")
+
+        song = {
+            "song_no": song_no,
+            "title": song_tag.text,
+            "album": album_tag.text,
+            "artist": artist_tag.text,
+        }
+        song_list.append(song)
+
+    return song_list
+
+
+def get_like_count(song_no_list):
+    api_url = "https://www.melon.com/commonlike/getSongLike.json"
+    params = {"contsIds": song_no_list}
+    res = requests.get(api_url, params=params, headers=headers)
+    res.raise_for_status()
+    response = res.json()
+    like_list = response["contsLike"]
+    like_dict = {str(song["CONTSID"]): song["SUMMCNT"] for song in like_list}
+    return like_dict
```

