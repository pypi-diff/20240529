# Comparing `tmp/plyball-2.2.72.tar.gz` & `tmp/plyball-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.2.72.tar", max compression
+gzip compressed data, was "plyball-2.3.0.tar", max compression
```

## Comparing `plyball-2.2.72.tar` & `plyball-2.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2024-05-20 15:24:21.366633 plyball-2.2.72/LICENSE.txt
--rw-r--r--   0        0        0      819 2024-05-20 15:24:21.366633 plyball-2.2.72/README.md
--rw-r--r--   0        0        0       22 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/__init__.py
--rw-r--r--   0        0        0       48 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/baseballreference/__init__.py
--rw-r--r--   0        0        0     9610 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/baseballreference/baseballreference.py
--rw-r--r--   0        0        0       33 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/fangraphs/__init__.py
--rw-r--r--   0        0        0    15578 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/fangraphs/fangraphs.py
--rw-r--r--   0        0        0       26 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/lahman/__init__.py
--rw-r--r--   0        0        0    10203 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/lahman/lahman.py
--rw-r--r--   0        0        0     6013 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/mlb/__init__.py
--rw-r--r--   0        0        0       28 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/ottoneu/__init__.py
--rw-r--r--   0        0        0    13950 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/ottoneu/ottoneu.py
--rw-r--r--   0        0        0        0 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/pipeline/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/pipeline/evaluation.py
--rw-r--r--   0        0        0     3517 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/player_id_lookup.py
--rw-r--r--   0        0        0      268 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/player_map.py
--rw-r--r--   0        0        0       35 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/retrosheet/__init__.py
--rw-r--r--   0        0        0     8085 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/retrosheet/retrosheet.py
--rw-r--r--   0        0        0       30 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/statcast/__init__.py
--rw-r--r--   0        0        0    14792 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/statcast/statcast.py
--rw-r--r--   0        0        0     4433 2024-05-20 15:24:21.366633 plyball-2.2.72/plyball/utils.py
--rw-r--r--   0        0        0     2907 2024-05-20 15:24:31.946653 plyball-2.2.72/pyproject.toml
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 plyball-2.2.72/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 12:23:09.413401 plyball-2.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-05-29 12:23:09.413401 plyball-2.3.0/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9626 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15578 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6098 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13950 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/utils.py
+-rw-r--r--   0        0        0     2974 2024-05-29 12:23:20.445293 plyball-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 plyball-2.3.0/PKG-INFO
```

### Comparing `plyball-2.2.72/LICENSE.txt` & `plyball-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/README.md` & `plyball-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/baseballreference/baseballreference.py` & `plyball-2.3.0/plyball/baseballreference/baseballreference.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         if data['Streak'].count() > 0:
             data['Streak2'] = data['Streak'].str.len()
             data.loc[data['Streak'].str[0] == '-', 'Streak2'] = -data['Streak2']
             data['Streak'] = data['Streak2']
             data = data.drop('Streak2', 1)
         return data
 
-    def schedule_and_record(self, season: int, team: str):
+    def schedule_and_record(self, season: int, team: str) -> pd.DataFrame:
         """
         Get a teams schedule and record from Baseball Reference
 
         :param season: Season Year
         :param team: Team Initials
         :return: DataFrame
         """
```

### Comparing `plyball-2.2.72/plyball/fangraphs/fangraphs.py` & `plyball-2.3.0/plyball/fangraphs/fangraphs.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/lahman/lahman.py` & `plyball-2.3.0/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/mlb/__init__.py` & `plyball-2.3.0/plyball/mlb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime as dt
 import logging
 from typing import List, Dict
 
+import pandas as pd
+
 import requests
 
 base_url = 'https://statsapi.mlb.com/api/v1/'
 
 urls = {
     'schedule_by_day': base_url + "schedule/games/?sportId=1&date={run_date}",
     'line_ups': base_url + 'schedule?gamePk={game_pk}&language=en&hydrate=lineups,probablePitcher(note)',
@@ -25,15 +27,15 @@
     Class for MLBStats
 
     """
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self.logger.info('MLBStats Initialized')
 
-    def get_game_lineups(self, game_pk):
+    def get_game_lineups(self, game_pk) -> pd.DataFrame:
         """
         Get Lineups for Today's Games
 
         :return:
         """
         self.logger.info('Getting Lineups|{}'.format(urls['line_ups'].format(game_pk=game_pk)))
         lineups = []
@@ -69,15 +71,15 @@
                                 "batting_order": i + 1,
                                 "team":          {
                                         "team_id":   data["dates"][0]["games"][0]["teams"][team]["team"]["id"],
                                         "team_name": data["dates"][0]["games"][0]["teams"][team]["team"]["name"],
                                 }
                         }
                         lineups.append(player)
-                return lineups
+                return pd.DataFrame(lineups)
             else:
 
                 raise Exception(f"Error retrieving the projected lineup for Game ID: {game_pk}")
 
         else:
             raise Exception(f"Error retrieving the projected lineup for Game ID: {game_pk}")
 
@@ -87,15 +89,15 @@
         Process game data
 
         :param game_data:
         :return:
         """
         pass
 
-    def get_lineups_by_day(self, run_date: dt.datetime):
+    def get_lineups_by_day(self, run_date: dt.datetime) -> pd.DataFrame:
         """
         Get Schedule by Day
 
         :param run_date:
         :return:
         """
         self.logger.info('Getting Lineups|{}'.format(urls['schedule_by_day'].format(run_date=run_date)))
@@ -110,15 +112,15 @@
             data = response.json()
 
             # Check if the game data is available
             for date in data["dates"]:
                 for game in date["games"]:
                     return self.get_game_lineups(game["gamePk"])
 
-    def get_game_boxscore(self, game_pk) -> List[Dict]:
+    def get_game_boxscore(self, game_pk) -> pd.DataFrame:
         """
         Get Game Logs
 
         :param game_pk:
         :return:
         """
         self.logger.info('Getting Game Logs|{}'.format(urls['game'].format(run_date=game_pk)))
@@ -138,15 +140,15 @@
 
                 return game
             else:
                 raise Exception(f"Error retrieving the game data for Game ID: {game_pk}")
         else:
             raise Exception(f"Error retrieving the game data for Game ID: {game_pk}")
 
-    def get_schedule(self, start_date: dt.datetime, end_date: dt.datetime) -> List[Dict]:
+    def get_schedule(self, start_date: dt.datetime, end_date: dt.datetime) -> pd.DataFrame:
         """
         Get Schedule
 
         :return:
         """
         self.logger.info('Getting Schedule|{}'.format(urls['schedule']))
         games = []
@@ -163,10 +165,10 @@
             data = response.json()
 
             # Check if the game data is available
             for date in data["dates"]:
                 for game in date["games"]:
                     games.append(game)
 
-            return games
+            return pd.DataFrame(games)
         else:
             raise Exception(f"Error retrieving the schedule")
```

### Comparing `plyball-2.2.72/plyball/ottoneu/ottoneu.py` & `plyball-2.3.0/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/pipeline/evaluation.py` & `plyball-2.3.0/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/player_id_lookup.py` & `plyball-2.3.0/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/retrosheet/retrosheet.py` & `plyball-2.3.0/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/statcast/statcast.py` & `plyball-2.3.0/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/plyball/utils.py` & `plyball-2.3.0/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.2.72/pyproject.toml` & `plyball-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plyball"
-version = "2.2.72"
+version = "2.3.0"
 description = ""
 authors = ["W. Aaron Morris <waaronmorris@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 alabaster = "0.7.13"
@@ -104,17 +104,18 @@
 autoescape = true
 
 [tool.semantic_release.commit_author]
 env = "GIT_COMMIT_AUTHOR"
 default = "semantic-release <semantic-release>"
 
 [tool.semantic_release.commit_parser_options]
-allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test"]
-minor_tags = ["feat"]
-patch_tags = ["fix", "perf"]
+allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test", "major", "minor", "patch"]
+major_tags = ["major"]
+minor_tags = ["feat", "minor"]
+patch_tags = ["fix", "perf", "patch"]
 default_bump_level = 0
 
 [tool.semantic_release.remote]
 name = "origin"
 type = "github"
 ignore_token_for_push = false
 insecure = false
```

### Comparing `plyball-2.2.72/PKG-INFO` & `plyball-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.2.72
+Version: 2.3.0
 Summary: 
 Author: W. Aaron Morris
 Author-email: waaronmorris@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

