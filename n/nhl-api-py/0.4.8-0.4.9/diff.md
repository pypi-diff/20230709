# Comparing `tmp/nhl_api_py-0.4.8.tar.gz` & `tmp/nhl_api_py-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.4.8.tar", max compression
+gzip compressed data, was "nhl_api_py-0.4.9.tar", max compression
```

## Comparing `nhl_api_py-0.4.8.tar` & `nhl_api_py-0.4.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     4940 2023-06-18 13:41:39.289397 nhl_api_py-0.4.8/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.8/nhlpy/__init__.py
--rw-r--r--   0        0        0      315 2023-06-21 16:19:03.961354 nhl_api_py-0.4.8/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.8/nhlpy/api/core.py
--rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.8/nhlpy/api/games.py
--rw-r--r--   0        0        0    10858 2023-07-09 15:49:13.259021 nhl_api_py-0.4.8/nhlpy/api/helpers.py
--rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.8/nhlpy/api/players.py
--rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.8/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1942 2023-06-18 13:41:39.289397 nhl_api_py-0.4.8/nhlpy/api/standings.py
--rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.8/nhlpy/api/teams.py
--rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.8/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1390 2023-07-09 15:36:17.369020 nhl_api_py-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nhl_api_py-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     4940 2023-06-18 13:41:39.289397 nhl_api_py-0.4.9/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.9/nhlpy/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-09 17:17:13.069033 nhl_api_py-0.4.9/nhlpy/_version.py
+-rw-r--r--   0        0        0      315 2023-06-21 16:19:03.961354 nhl_api_py-0.4.9/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.9/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.9/nhlpy/api/games.py
+-rw-r--r--   0        0        0    10877 2023-07-09 17:16:44.059033 nhl_api_py-0.4.9/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.9/nhlpy/api/players.py
+-rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.9/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1942 2023-06-18 13:41:39.289397 nhl_api_py-0.4.9/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.9/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.9/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1390 2023-07-09 17:17:17.449033 nhl_api_py-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6105 1970-01-01 00:00:00.000000 nhl_api_py-0.4.9/PKG-INFO
```

### Comparing `nhl_api_py-0.4.8/README.md` & `nhl_api_py-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/core.py` & `nhl_api_py-0.4.9/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/games.py` & `nhl_api_py-0.4.9/nhlpy/api/games.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/helpers.py` & `nhl_api_py-0.4.9/nhlpy/api/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
         for event_type in game_data["liveData"]["plays"]["allPlays"]:
             if event_type["result"]["event"] not in ["Shot", "Goal"]:
                 continue
 
             player_id, player_name = (
                 _get_shooter(event_type)
-                if event_type == "Shot"
+                if event_type["result"]["event"] == "Shot"
                 else _get_goal_scorer(event_type)
             )
 
             try:
                 shot = {
                     "game_id": game_id,
                     "season": season,
```

### Comparing `nhl_api_py-0.4.8/nhlpy/api/players.py` & `nhl_api_py-0.4.9/nhlpy/api/players.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/schedule.py` & `nhl_api_py-0.4.9/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/standings.py` & `nhl_api_py-0.4.9/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/api/teams.py` & `nhl_api_py-0.4.9/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/nhlpy/nhl_client.py` & `nhl_api_py-0.4.9/nhlpy/nhl_client.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.4.8/pyproject.toml` & `nhl_api_py-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.4.8"
+version = "0.4.9"
 description = "NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-0.4.8/PKG-INFO` & `nhl_api_py-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.4.8
+Version: 0.4.9
 Summary: NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
```

