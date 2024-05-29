# Comparing `tmp/ossapi-4.0.0.tar.gz` & `tmp/ossapi-4.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-4.0.0.tar", last modified: Wed May 29 18:01:31 2024, max compression
+gzip compressed data, was "ossapi-4.0.0b1.tar", last modified: Fri Apr 19 01:49:42 2024, max compression
```

## Comparing `ossapi-4.0.0.tar` & `ossapi-4.0.0b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-05-29 18:01:31.440434 ossapi-4.0.0/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-4.0.0/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10695 2024-05-29 18:01:31.440204 ossapi-4.0.0/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)    10039 2024-04-17 01:30:55.000000 ossapi-4.0.0/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-05-29 18:01:31.438312 ossapi-4.0.0/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     6151 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      917 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    18069 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2024-04-19 01:42:59.000000 ossapi-4.0.0/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    40041 2024-04-30 17:10:08.000000 ossapi-4.0.0/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    15363 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)   100523 2024-04-30 17:10:09.000000 ossapi-4.0.0/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)   102738 2024-04-30 17:10:09.000000 ossapi-4.0.0/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     3681 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)    11087 2024-04-19 01:43:42.000000 ossapi-4.0.0/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-05-29 18:01:31.439880 ossapi-4.0.0/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10695 2024-05-29 18:01:31.000000 ossapi-4.0.0/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      442 2024-05-29 18:01:31.000000 ossapi-4.0.0/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2024-05-29 18:01:31.000000 ossapi-4.0.0/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2024-05-29 18:01:31.000000 ossapi-4.0.0/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2024-05-29 18:01:31.000000 ossapi-4.0.0/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      638 2024-05-29 18:01:01.000000 ossapi-4.0.0/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2024-05-29 18:01:31.440474 ossapi-4.0.0/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-05-29 18:01:31.439684 ossapi-4.0.0/tests/
--rw-r--r--   0 tybug      (501) staff       (20)      524 2024-04-19 01:43:42.000000 ossapi-4.0.0/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)    11434 2024-04-19 01:43:42.000000 ossapi-4.0.0/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4028 2024-04-19 01:43:42.000000 ossapi-4.0.0/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1140 2024-04-19 01:43:42.000000 ossapi-4.0.0/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.008122 ossapi-4.0.0b1/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-4.0.0b1/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10697 2024-04-19 01:49:42.007824 ossapi-4.0.0b1/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)    10039 2024-04-17 01:30:55.000000 ossapi-4.0.0b1/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.005907 ossapi-4.0.0b1/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     6151 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      917 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    18069 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2024-04-19 01:42:59.000000 ossapi-4.0.0b1/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    39778 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    15363 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    99648 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)   102924 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     3681 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11087 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.007466 ossapi-4.0.0b1/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10697 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      442 2024-04-19 01:49:42.000000 ossapi-4.0.0b1/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2024-04-19 01:49:41.000000 ossapi-4.0.0b1/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      643 2024-04-19 01:47:53.000000 ossapi-4.0.0b1/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2024-04-19 01:49:42.008162 ossapi-4.0.0b1/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-19 01:49:42.007258 ossapi-4.0.0b1/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)      524 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11434 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4028 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1140 2024-04-19 01:43:42.000000 ossapi-4.0.0b1/tests/test_v1.py
```

### Comparing `ossapi-4.0.0/LICENSE` & `ossapi-4.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/PKG-INFO` & `ossapi-4.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 4.0.0
+Version: 4.0.0b1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/tybug/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-4.0.0/README.md` & `ossapi-4.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/__init__.py` & `ossapi-4.0.0b1/ossapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/encoder.py` & `ossapi-4.0.0b1/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/enums.py` & `ossapi-4.0.0b1/ossapi/enums.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/mod.py` & `ossapi-4.0.0b1/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/models.py` & `ossapi-4.0.0b1/ossapi/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,25 +432,22 @@
         return self._api.download_score(self.mode, self.id)
 
 
 class BeatmapUserScore(Model):
     position: int
     score: Score
 
-class _NonLegacyBeatmapUserScore(Model):
-    position: int
-    score: _NonLegacyScore
 
 class BeatmapUserScores(Model):
     scores: List[Score]
 
 
 class BeatmapScores(Model):
     scores: List[Score]
-    user_score: Optional[BeatmapUserScore] = Field(name="userScore")
+    userScore: Optional[BeatmapUserScore]
 
 
 class CommentableMeta(Model):
     # title is the only attribute returned for deleted commentables.
     id: Optional[int]
     title: str
     type: Optional[str]
@@ -1436,15 +1433,15 @@
 # ==================
 # Provisional Models
 # ==================
 
 
 class _NonLegacyBeatmapScores(Model):
     scores: List[_NonLegacyScore]
-    user_score: Optional[_NonLegacyBeatmapUserScore] = Field(name="userScore")
+    userScore: Optional[BeatmapUserScore]
 
 
 class _NonLegacyMod(BaseModel):
     # returned in a new format. e.g.:
     # "mods": [
     #      {
     #          "acronym": "HR"
@@ -1517,10 +1514,7 @@
     beatmapset: Optional[BeatmapsetCompact]
     rank_country: Optional[int]
     rank_global: Optional[int]
     weight: Optional[Weight]
     _user: Optional[UserCompact] = Field(name="user")
     match: Optional[ScoreMatchInfo]
     type: str
-
-    def user(self) -> Union[UserCompact, User]:
-        return self._fk_user(self.user_id, existing=self._user)
```

### Comparing `ossapi-4.0.0/ossapi/ossapi.py` & `ossapi-4.0.0b1/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/ossapiv2.py` & `ossapi-4.0.0b1/ossapi/ossapiv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1137,39 +1137,31 @@
     # ---------------
 
     @request(Scope.PUBLIC, category="beatmap packs")
     def beatmap_packs(
         self,
         type: Optional[BeatmapPackTypeT] = None,
         cursor_string: Optional[str] = None,
-        legacy_only: Optional[bool] = None,
     ) -> BeatmapPacks:
         """
         Get a list of beatmap packs. If you want to retrieve a specific pack,
         see :meth:`beatmap_pack`.
 
         Parameters
         ----------
         cursor_string
             Cursor for pagination.
-        legacy_only
-            Whether to exclude lazer scores for user completion data. Defaults
-            to False.
 
         Notes
         -----
         Implements the `Beatmap Packs
         <https://osu.ppy.sh/docs/index.html#get-beatmap-packs>`__
         endpoint.
         """
-        params = {
-            "type": type,
-            "cursor_string": cursor_string,
-            "legacy_only": None if legacy_only is None else int(legacy_only),
-        }
+        params = {"type": type, "cursor_string": cursor_string}
         return self._get(BeatmapPacks, "/beatmaps/packs", params)
 
     @request(Scope.PUBLIC, category="beatmap packs")
     def beatmap_pack(self, pack: str) -> BeatmapPack:
         """
         Get a beatmap pack. If you want to retrieve a list of beatmap packs, see
         see :meth:`beatmap_packs`.
@@ -1189,15 +1181,14 @@
     def beatmap_user_score(
         self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
-        legacy_only: Optional[bool] = None,
     ) -> BeatmapUserScore:
         """
         Get a user's best score on a beatmap. If you want to retrieve all
         scores, see :meth:`beatmap_user_scores`.
 
         Parameters
         ----------
@@ -1205,66 +1196,54 @@
             The beatmap the score was set on.
         user_id
             The user who set the score.
         mode
             The mode the scores were set on.
         mods
             The mods the score was set with.
-        legacy_only
-            Whether to exclude lazer scores. Defaults to False.
 
         Notes
         -----
         Implements the `User Beatmap Score
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-score>`__
         endpoint.
         """
-        params = {
-            "mode": mode,
-            "mods": mods,
-            "legacy_only": None if legacy_only is None else int(legacy_only),
-        }
+        params = {"mode": mode, "mods": mods}
         return self._get(
             BeatmapUserScore, f"/beatmaps/{beatmap_id}/scores/users/{user_id}", params
         )
 
     @request(Scope.PUBLIC, category="beatmaps")
     def beatmap_user_scores(
         self,
         beatmap_id: BeatmapIdT,
         user_id: UserIdT,
         *,
         mode: Optional[GameModeT] = None,
-        legacy_only: Optional[bool] = None,
     ) -> List[Score]:
         """
         Get all of a user's scores on a beatmap. If you only want the top user
         score, see :meth:`beatmap_user_score`.
 
         Parameters
         ----------
         beatmap_id
             The beatmap the scores were set on.
         user_id
             The user who set the scores.
         mode
             The mode the scores were set on.
-        legacy_only
-            Whether to exclude lazer scores. Defaults to False.
 
         Notes
         -----
         Implements to `User Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-a-user-beatmap-scores>`__
         endpoint.
         """
-        params = {
-            "mode": mode,
-            "legacy_only": None if legacy_only is None else int(legacy_only),
-        }
+        params = {"mode": mode}
         scores = self._get(
             BeatmapUserScores,
             f"/beatmaps/{beatmap_id}/scores/users/{user_id}/all",
             params,
         )
         return scores.scores
 
@@ -1273,15 +1252,14 @@
         self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
         type: Optional[RankingTypeT] = None,
         limit: Optional[int] = None,
-        legacy_only: Optional[bool] = None,
     ) -> BeatmapScores:
         """
         Get the top scores of a beatmap.
 
         Parameters
         ----------
         beatmap_id
@@ -1291,53 +1269,47 @@
         mods
             Get the top scores set with exactly these mods, if passed.
         type
             How to order the scores. Defaults to ordering by score.
         limit
             How many results to return. Defaults to 50. Must be between 1 and
             100.
-        legacy_only
-            Whether to exclude lazer scores. Defaults to False.
 
         Notes
         -----
         Implements the `Get Beatmap Scores
         <https://osu.ppy.sh/docs/index.html#get-beatmap-scores>`__ endpoint.
         """
-        params = {
-            "mode": mode,
-            "mods": mods,
-            "type": type,
-            "limit": limit,
-            "legacy_only": None if legacy_only is None else int(legacy_only),
-        }
+        params = {"mode": mode, "mods": mods, "type": type, "limit": limit}
         return self._get(BeatmapScores, f"/beatmaps/{beatmap_id}/scores", params)
 
     def _beatmap_scores_non_legacy(
         self,
         beatmap_id: BeatmapIdT,
         *,
         mode: Optional[GameModeT] = None,
         mods: Optional[ModT] = None,
         type: Optional[RankingTypeT] = None,
         limit: Optional[int] = None,
+        legacy_only: Optional[bool] = None,
     ) -> _NonLegacyBeatmapScores:
         """
         This is a provisional method. It may change or disappear in the future.
         Feel free to use it, but don't expect ossapi to maintain backwards
         compatability here.
 
         I'll decide what to do about these provisional methods once the lazer
         migration settles down.
         """
         params = {
             "mode": mode,
             "mods": mods,
             "type": type,
             "limit": limit,
+            "legacy_only": legacy_only,
         }
         return self._get(
             _NonLegacyBeatmapScores, f"/beatmaps/{beatmap_id}/solo-scores", params
         )
 
     @request(Scope.PUBLIC, category="beatmaps")
     def beatmap(
@@ -2738,15 +2710,14 @@
         user_id: UserIdT,
         type: ScoreTypeT,
         *,
         include_fails: Optional[bool] = None,
         mode: Optional[GameModeT] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        legacy_only: Optional[bool] = None,
     ) -> List[Score]:
         """
         Get scores of a user.
 
         user_id
             The user to get scores of.
         type
@@ -2755,29 +2726,33 @@
             Whether to include failed scores.
         mode
             Filter scores by game mode. Defaults to the user's default mode.
         limit
             Maximum number of scores to return.
         offset
             Offset for pagination.
-        legacy_only
-            Whether to exclude lazer scores. Defaults to False.
 
         Notes
         -----
         Implements the `Get User Scores
         <https://osu.ppy.sh/docs/index.html#get-user-scores>`__ endpoint.
         """
+        # `include_fails` is actually a string in the api spec. We'll still
+        # require a bool to be passed, and just do the conversion behind the
+        # scenes.
+        if include_fails is False:
+            include_fails = 0
+        if include_fails is True:
+            include_fails = 1
 
         params = {
-            "include_fails": None if include_fails is None else int(include_fails),
+            "include_fails": include_fails,
             "mode": mode,
             "limit": limit,
             "offset": offset,
-            "legacy_only": None if legacy_only is None else int(legacy_only),
         }
         return self._get(List[Score], f"/users/{user_id}/scores/{type.value}", params)
 
     @request(Scope.PUBLIC, category="users")
     def user_beatmaps(
         self,
         user_id: UserIdT,
```

### Comparing `ossapi-4.0.0/ossapi/ossapiv2_async.py` & `ossapi-4.0.0b1/ossapi/ossapiv2_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -2785,17 +2785,24 @@
             Offset for pagination.
 
         Notes
         -----
         Implements the `Get User Scores
         <https://osu.ppy.sh/docs/index.html#get-user-scores>`__ endpoint.
         """
+        # `include_fails` is actually a string in the api spec. We'll still
+        # require a bool to be passed, and just do the conversion behind the
+        # scenes.
+        if include_fails is False:
+            include_fails = 0
+        if include_fails is True:
+            include_fails = 1
+
         params = {
-            # `include_fails` is actually 0/1 in the api spec, not a bool.
-            "include_fails": None if include_fails is None else int(include_fails),
+            "include_fails": include_fails,
             "mode": mode,
             "limit": limit,
             "offset": offset,
         }
         return await self._get(
             List[Score], f"/users/{user_id}/scores/{type.value}", params
         )
```

### Comparing `ossapi-4.0.0/ossapi/replay.py` & `ossapi-4.0.0b1/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi/utils.py` & `ossapi-4.0.0b1/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/ossapi.egg-info/PKG-INFO` & `ossapi-4.0.0b1/ossapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 4.0.0
+Version: 4.0.0b1
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/tybug/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-4.0.0/pyproject.toml` & `ossapi-4.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "4.0.0"
+version = "4.0.0beta1"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-4.0.0/tests/test_cursor.py` & `ossapi-4.0.0b1/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/tests/test_endpoints.py` & `ossapi-4.0.0b1/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/tests/test_models.py` & `ossapi-4.0.0b1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-4.0.0/tests/test_v1.py` & `ossapi-4.0.0b1/tests/test_v1.py`

 * *Files identical despite different names*

