# Comparing `tmp/dry_scraper-0.1.8.8.tar.gz` & `tmp/dry_scraper-0.1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.8.8.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.8.9.tar", max compression
```

## Comparing `dry_scraper-0.1.8.8.tar` & `dry_scraper-0.1.8.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.8/LICENSE
--rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.8/README.md
--rw-r--r--   0        0        0      550 2023-07-07 00:19:41.025172 dry_scraper-0.1.8.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.8/src/dry_scraper/__init__.py
--rw-r--r--   0        0        0     2432 2023-07-04 01:45:24.304507 dry_scraper-0.1.8.8/src/dry_scraper/data_source.py
--rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.8/src/dry_scraper/nhl/__init__.py
--rw-r--r--   0        0        0    29866 2023-07-05 22:33:14.060482 dry_scraper-0.1.8.8/src/dry_scraper/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0     2103 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/base_model.py
--rw-r--r--   0        0        0      688 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0     1044 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     6823 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    14863 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1874 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     2273 2023-07-04 02:50:05.226525 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     2186 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.8/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.8.8/src/dry_scraper/teams.py
--rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.9/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.8.9/README.md
+-rw-r--r--   0        0        0      573 2023-07-07 21:59:34.473102 dry_scraper-0.1.8.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.9/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     4194 2023-07-07 23:38:33.946979 dry_scraper-0.1.8.9/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.8.9/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    32334 2023-07-08 13:27:11.970718 dry_scraper-0.1.8.9/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0     2137 2023-07-07 02:10:27.021791 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/base_model.py
+-rw-r--r--   0        0        0      688 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0     1044 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     6823 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    14970 2023-07-07 01:29:49.641673 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1874 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     2239 2023-07-07 01:11:03.049373 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     2186 2023-07-04 23:28:22.477674 dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.8.9/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30696 2023-07-07 02:09:42.154876 dry_scraper-0.1.8.9/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 dry_scraper-0.1.8.9/PKG-INFO
```

### Comparing `dry_scraper-0.1.8.8/LICENSE` & `dry_scraper-0.1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/README.md` & `dry_scraper-0.1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/pyproject.toml` & `dry_scraper-0.1.8.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "dry-scraper"
-version = "0.1.8.8"
+version = "0.1.8.9"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.11.1"
 pandas = "^2.0.3"
 requests = "^2.28.1"
 pydantic = "^1.10.11"
 uuid = "^1.30"
 fastapi = "^0.99.0"
+sqlalchemy = "^2.0.18"
 
 
 [tool.poetry.dev-dependencies]
 sphinx = "^7.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/nhl_api_sources.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/nhl_api_sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
+import pandas as pd
+import pydantic
 import re
+import requests
 from abc import ABC
 from datetime import datetime
 from typing import ClassVar, TypeVar, Self, Any
+from sqlalchemy import Select, select, Engine
+from sqlalchemy.orm import Session
 
-import pandas as pd
-import pydantic
-import requests
 
 from dry_scraper.nhl.pydantic_models import (
     nhl_schedule_api_source,
     nhl_teams_api_source,
     nhl_divisions_api_source,
     nhl_conferences_api_source,
     nhl_game_live_feed_api_source,
 )
-from dry_scraper.data_source import DataSource
+from dry_scraper.data_source import DataSource, CachedDataSource
 
 DataModel = TypeVar("DataModel", bound=pydantic.BaseModel)
 
 
 class NhlApiSource(DataSource, ABC):
     """
     Abstract subclass of DataSource that represents a request and result from NHL API.
@@ -29,14 +31,16 @@
 
     Attributes
     ----------
     _url_stub : ClassVar[str]
         partial URL location of data source
     _extension : ClassVar[str]
         file extension to be used when writing the raw data source to disk e.g. json, HTM
+    _db_engine : Engine
+        SQLAlchemy database engine object for caching data fetch results
     _pyd_model : DataModel
         pydantic model class describing the response
     _url : str
         fully qualified URL location of data source, completed on instantiation
     _query : dict
         dict representation of API query
     _content : str
@@ -46,14 +50,15 @@
 
     """
 
     _url_stub: ClassVar[str] = "https://statsapi.web.nhl.com/api/v1"
     _extension: ClassVar[str] = "json"
     _content_pyd: DataModel = None
     _pyd_model: DataModel
+    _db_engine: Engine
     _url: str
     _query: dict
     _content: str
 
     @property
     def query(self) -> dict | None:
         return getattr(self, "_query", None)
@@ -73,22 +78,56 @@
     def parse_to_pyd(self) -> Self:
         """
         Parse content into a Pydantic model and store result in self.content_pyd
         """
         self._content_pyd = self.pyd_model.parse_raw(self.content)
         return self
 
+    def cache_content(self) -> Self:
+        """
+        If a SQLAlchemy database engine is present, store the fetched content for later re-use
+        """
+        cache_record = CachedDataSource(
+            url=self.url, query=str(self.query), content=self.content
+        )
+        with Session(self.db_engine) as session:
+            session.add(cache_record)
+            session.commit()
+        return self
+
+    def retrieve_cached_content(self) -> Self:
+        """
+        If a SQLAlchemy database engine is present, attempt to retrieve the cached content and store it in self.content
+        instead of querying the API
+        """
+        with Session(self.db_engine) as session:
+            select_statement: Select = select(CachedDataSource).where(
+                CachedDataSource.url == self.url,
+                CachedDataSource.query == str(self.query),
+            )
+            result: CachedDataSource = session.scalars(select_statement).first()
+        if result:
+            self.content = result.content
+        return self
+
     def fetch_content(self) -> Self:
         """
-        Query NHL API endpoint at self.url and store response in self.content
+        If SQLAlchemy engine is present, attempt to retrieve a cached version of the content.
+        Otherwise, query NHL API endpoint at self.url and store response in self.content
         """
+        if self.db_engine:
+            self.retrieve_cached_content()
+            if self.content:
+                return self
         try:
             response = requests.get(self.url, self.query)
             response.raise_for_status()
             self.content = response.text
+            if self.db_engine:
+                self.cache_content()
         except requests.exceptions.HTTPError as errh:
             print(errh)
         except requests.exceptions.ConnectionError as errc:
             print(errc)
         except requests.exceptions.Timeout as errt:
             print(errt)
         except requests.exceptions.RequestException as err:
@@ -103,14 +142,16 @@
 
     ...
 
     Attributes
     ----------
     _pyd_model : DataModel
         pydantic model class describing the response
+    _db_engine : Engine
+        SQLAlchemy database engine object for caching data fetch results
     _date : str
         single date for the season_query (e.g. 2021-03-17)
     _start_date : str
         start date for a date range season_query
     _end_date : str
         end date for  date range season_query
     _season : str
@@ -128,14 +169,15 @@
         'broadcasts' shows broadcast information, 'linescore' shows the line score,
         'tickets' shows ticketing information
         all options listed here: https://statsapi.web.nhl.com/api/v1/expands
 
     """
 
     _pyd_model: DataModel = nhl_schedule_api_source.Schedule
+    _db_engine: Engine
     _date: str
     _start_date: str
     _end_date: str
     _season: str
     _team_id: str
     _game_type: str
     _expand: str
@@ -145,22 +187,24 @@
         date=None,
         start_date=None,
         end_date=None,
         season=None,
         team_id=None,
         game_type=None,
         expand=None,
+        db_engine=None,
     ):
         self.date = date
         self.start_date = start_date
         self.end_date = end_date
         self.season = season
         self.team_id = team_id
         self.game_type = game_type
         self.expand = expand
+        self.db_engine = db_engine
         self.url = f"{self.url_stub}/schedule"
         query = {}
         if date:
             query["date"] = self.date
         if start_date:
             query["startDate"] = self.start_date
         if end_date:
@@ -336,18 +380,20 @@
     Attributes
     ----------
     _team_id : int
         team id number for the NHL API query
     """
 
     _pyd_model: DataModel = nhl_teams_api_source.Teams
+    _db_engine: Engine
     _team_id: str
 
-    def __init__(self, team_id="") -> None:
+    def __init__(self, team_id="", db_engine=None) -> None:
         self.team_id = team_id
+        self.db_engine = db_engine
         self.url = f"{self.url_stub}" "/teams/" f"{self.team_id}"
 
     @property
     def team_id(self) -> str:
         return self._team_id
 
     @team_id.setter
@@ -389,17 +435,18 @@
     _division_id : int
         division id number for the NHL API query
     """
 
     _pyd_model: DataModel = nhl_divisions_api_source.Divisions
     _division_id: str
 
-    def __init__(self, division_id="") -> None:
+    def __init__(self, division_id="", db_engine=None) -> None:
         self.division_id = division_id
         self.url = f"{self.url_stub}" "/divisions/" f"{self.division_id}"
+        self.db_engine = db_engine
 
     @property
     def division_id(self) -> str:
         return self._division_id
 
     @division_id.setter
     def division_id(self, value: str | int) -> None:
@@ -417,17 +464,18 @@
     _conference_id : int
         conference id number for the NHL API query
     """
 
     _pyd_model: DataModel = nhl_conferences_api_source.Conferences
     _conference_id: str
 
-    def __init__(self, conference_id=""):  # -> Self:
+    def __init__(self, conference_id="", db_engine=None):  # -> Self:
         self.conference_id = conference_id
         self.url = f"{self.url_stub}" "/conferences/" f"{self.conference_id}"
+        self.db_engine = db_engine
 
     @property
     def conference_id(self) -> str:
         return self._conference_id
 
     @conference_id.setter
     def conference_id(self, value: str | int) -> None:
@@ -447,17 +495,20 @@
     _gamePk : str
         6 character representation of NHL game in a season (e.g. 020462)
     """
 
     _season: str
     _gamePk: str
 
-    def __init__(self, season: str | int, gamePk: str | int) -> None:
+    def __init__(
+        self, season: str | int, gamePk: str | int, db_engine: Engine | None = None
+    ) -> None:
         self.season = season
         self.gamePk = gamePk
+        self.db_engine = db_engine
 
     @property
     def season(self) -> str:
         return self._season
 
     @season.setter
     def season(self, value: int | str) -> None:
@@ -482,16 +533,18 @@
     ----------
     _pyd_model : DataModel
         pydantic model class describing the response
     """
 
     _pyd_model: DataModel = nhl_game_live_feed_api_source.BoxScore
 
-    def __init__(self, season: str | int, gamePk: str | int) -> None:
-        super().__init__(season, gamePk)
+    def __init__(
+        self, season: str | int, gamePk: str | int, db_engine: Engine | None = None
+    ) -> None:
+        super().__init__(season, gamePk, db_engine)
         self.url = (
             f"{self.url_stub}"
             "/game/"
             f"{self.season[:4]}"
             "0"
             f"{self.gamePk}"
             "/boxscore"
@@ -508,16 +561,18 @@
     ----------
     _pyd_model : DataModel
         pydantic model class describing the response
     """
 
     _pyd_model: DataModel = nhl_game_live_feed_api_source.LineScore
 
-    def __init__(self, season: str | int, gamePk: str | int) -> None:
-        super().__init__(season, gamePk)
+    def __init__(
+        self, season: str | int, gamePk: str | int, db_engine: Engine | None = None
+    ) -> None:
+        super().__init__(season, gamePk, db_engine)
         self.url = (
             f"{self.url_stub}"
             "/game/"
             f"{self.season[:4]}"
             "0"
             f"{self.gamePk}"
             "/linescore"
@@ -559,16 +614,18 @@
     ----------
     _pyd_model : DataModel
         pydantic model class describing the response
     """
 
     _pyd_model: DataModel = nhl_game_live_feed_api_source.LiveFeed
 
-    def __init__(self, season: str | int, gamePk: str | int) -> None:
-        super().__init__(season, gamePk)
+    def __init__(
+        self, season: str | int, gamePk: str | int, db_engine: Engine | None = None
+    ) -> None:
+        super().__init__(season, gamePk, db_engine)
         self.url = (
             f"{self.url_stub}"
             "/game/"
             f"{self.season[:4]}"
             "0"
             f"{self.gamePk}"
             "/feed/live"
@@ -779,21 +836,23 @@
         )
         home_line_score_goal_differential = (
             self.content_pyd.live_data.line_score.teams.home.goals
             - self.content_pyd.live_data.line_score.teams.away.goals
         )
         start = self.content_pyd.game_data.date_time.date_time
         end = self.content_pyd.game_data.date_time.end_date_time
+        venue = self.content_pyd.game_data.venue
         for home, team_stats, oppo_stats, team_info, oppo_info in [
             (True, home_stats, away_stats, home_team_info, away_team_info),
             (False, away_stats, home_stats, away_team_info, home_team_info),
         ]:
-            team_dict = {
+            team_stats_dict = {
                 "season": int(self.season),
-                "gamePk": int(self.gamePk),
+                "game_pk": int(self.gamePk),
+                "game_type": self.content_pyd.game_data.game.type,
                 "start_date_time": datetime.min if start is None else start,
                 "end_date_time": datetime.min if end is None else end,
                 "team_id": int(team_info.id),
                 "team_franchise_id": int(team_info.franchise_id),
                 "team_name": str(team_info.name),
                 "team_tricode": str(team_info.tricode),
                 "oppo_id": int(oppo_info.id),
@@ -808,15 +867,15 @@
                     team_stats.power_play_percentage, float
                 ),
                 "team_power_play_goals": not_none(team_stats.power_play_goals, int),
                 "team_power_play_opportunities": not_none(
                     team_stats.power_play_opportunities, int
                 ),
                 "team_face_off_win_percentage": not_none(
-                    team_stats.face_off_win_percentage, float
+                    team_stats.power_play_percentage, float
                 ),
                 "team_blocked_shots": not_none(team_stats.blocked, int),
                 "team_takeaways": not_none(team_stats.takeaways, int),
                 "team_giveaways": not_none(team_stats.giveaways, int),
                 "team_hits": not_none(team_stats.hits, int),
                 "oppo_goals": not_none(oppo_stats.goals, int),
                 "oppo_penalty_minutes": not_none(oppo_stats.pim, int),
@@ -838,16 +897,18 @@
                 "team_goal_differential": int(team_stats.goals) - int(oppo_stats.goals),
                 "team_decision": determine_team_decision(
                     home_line_score_goal_differential
                     if home
                     else -home_line_score_goal_differential,
                     self.content_pyd.live_data.line_score.current_period_ordinal,
                 ),
+                "venue_id": None if venue is None else not_none(venue.id, int),
+                "venue_name": None if venue is None else not_none(venue.name, str),
             }
             team_stats_df.loc[
                 f"{self.gamePk} Home" if home else f"{self.gamePk} Away"
-            ] = team_dict
+            ] = team_stats_dict
         return team_stats_df
 
 
 def not_none(value: Any, type_function: type) -> Any:
     return type_function(value) if value is not None else None
```

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/base_model.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import no_type_check, Type, Any
 
 from pydantic import BaseModel, ValidationError, StrBytes, Protocol
 
 
+# noinspection PyMethodParameters
 class BaseModelNoException(BaseModel):
     def __init__(__pydantic_self__, **data: Any) -> None:
         try:
             super(BaseModelNoException, __pydantic_self__).__init__(**data)
         except ValidationError as pve:
             print(
                 f"This is a warning. __init__ failed to validate:\n {json.dumps(data, indent=4)}\n"
```

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,40 +399,44 @@
     "team_id": "int",
     "team_name": "str",
     "team_tricode": "str",
 }
 
 team_stats_df_model = {
     "season": "int",
-    "gamePk": "int",
+    "game_pk": "int",
+    "game_type": "str",
+    "game_date": "datetime64[D]",
     "start_date_time": "datetime64[s]",
     "end_date_time": "datetime64[s]",
+    "venue_id": "int",
+    "venue_name": "str",
     "team_id": "int",
     "team_franchise_id": "int",
     "team_name": "str",
     "team_tricode": "str",
     "oppo_id": "int",
     "oppo_franchise_id": "int",
     "oppo_name": "str",
     "oppo_tricode": "str",
     "team_home": "bool",
     "team_goals": "int",
-    "team_penalty_minutes": "int",
     "team_shots_on_goal": "int",
+    "team_penalty_minutes": "int",
     "team_power_play_percentage": "float",
     "team_power_play_goals": "int",
     "team_power_play_opportunities": "int",
     "team_face_off_win_percentage": "float",
     "team_blocked_shots": "int",
     "team_takeaways": "int",
     "team_giveaways": "int",
     "team_hits": "int",
     "oppo_goals": "int",
-    "oppo_penalty_minutes": "int",
     "oppo_shots_on_goal": "int",
+    "oppo_penalty_minutes": "int",
     "oppo_power_play_percentage": "float",
     "oppo_power_play_goals": "int",
     "oppo_power_play_opportunities": "int",
     "oppo_face_off_win_percentage": "float",
     "oppo_blocked_shots": "int",
     "oppo_takeaways": "int",
     "oppo_giveaways": "int",
```

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
 
 schedule_df_model = {
     "date": "str",
     "season": "int",
     "gamePk": "int",
     "game_type": "str",
-    "game_date": "datetime64[m]",
     "abstract_game_state": "str",
     "coded_game_state": "int",
     "detailed_state": "str",
     "status_code": "int",
     "start_time_tbd": "bool",
     "away_team_id": "int",
     "away_team_name": "str",
```

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.8.9/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/shared.py` & `dry_scraper-0.1.8.9/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.8.8/src/dry_scraper/teams.py` & `dry_scraper-0.1.8.9/src/dry_scraper/teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# noinspection DuplicatedCode
+# noinspection DuplicatedCode,HttpUrlsUsage
 TEAMS = {
     "ANA": {
         "abbreviation": "ANA",
         "active": True,
         "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
         "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1993",
```

### Comparing `dry_scraper-0.1.8.8/PKG-INFO` & `dry_scraper-0.1.8.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.8.8
+Version: 0.1.8.9
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: fastapi (>=0.99.0,<0.100.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: sqlalchemy (>=2.0.18,<3.0.0)
 Requires-Dist: uuid (>=1.30,<2.0)
 Description-Content-Type: text/markdown
 
 # dry_scraper
 
 `dry_scraper` is a framework for retrieving and parsing hockey data into useful forms.
```

