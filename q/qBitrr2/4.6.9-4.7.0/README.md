# Comparing `tmp/qbitrr2-4.6.9.tar.gz` & `tmp/qbitrr2-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.6.9.tar", last modified: Fri May 17 10:59:06 2024, max compression
+gzip compressed data, was "qbitrr2-4.7.0.tar", last modified: Wed May 29 12:58:38 2024, max compression
```

## Comparing `qbitrr2-4.6.9.tar` & `qbitrr2-4.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.843455 qbitrr2-4.6.9/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   225987 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26629 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:59:06.847455 qbitrr2-4.6.9/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 10:59:06.000000 qbitrr2-4.6.9/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-17 10:59:06.851455 qbitrr2-4.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:59:02.000000 qbitrr2-4.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.663204 qbitrr2-4.7.0/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   232066 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27032 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.663204 qbitrr2-4.7.0/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/setup.py
```

### Comparing `qbitrr2-4.6.9/LICENSE` & `qbitrr2-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/PKG-INFO` & `qbitrr2-4.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.9
+Version: 4.7.0
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -36,15 +36,15 @@
 Requires-Dist: jaraco.docker==2.0
 Requires-Dist: packaging==22.0
 Requires-Dist: pathos==0.2.8
 Requires-Dist: peewee==3.14.7
 Requires-Dist: ping3==3.0.2
 Requires-Dist: pyarr==5.2.0
 Requires-Dist: qbittorrent-api==2023.7.52
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: tomlkit==0.7.2
 Provides-Extra: dev
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: isort==5.10.1; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
```

### Comparing `qbitrr2-4.6.9/README.md` & `qbitrr2-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/pyproject.toml` & `qbitrr2-4.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.6.9"
+version = "4.7.0"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.6.9/qBitrr/arss.py` & `qbitrr2-4.7.0/qBitrr/arss.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import logging
 import pathlib
 import re
 import shutil
 import sys
 import time
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor
 from copy import copy
 from datetime import datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Callable, Iterable, Iterator, NoReturn
 
 import ffmpeg
 import pathos
 import qbittorrentapi
@@ -89,27 +88,25 @@
             raise OSError(
                 f"Group '{self._name}' is trying to manage Arr instance: "
                 f"'{self.uri}' which has already been registered."
             )
         self.category = CONFIG.get(f"{name}.Category", fallback=self._name)
         self.manager = manager
         self._LOG_LEVEL = self.manager.qbit_manager.logger.level
+        self.logger = logging.getLogger(f"qBitrr.{self._name}")
         if ENABLE_LOGS:
             LOGS_FOLDER = HOME_PATH.joinpath("logs")
             LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
             LOGS_FOLDER.chmod(mode=0o777)
             logfile = LOGS_FOLDER.joinpath(self._name + ".log")
             if pathlib.Path(logfile).is_file():
                 logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
                 logfile.rename(logold)
             fh = logging.FileHandler(logfile)
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
             self.logger.addHandler(fh)
-        else:
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
         run_logs(self.logger)
         self.completed_folder = pathlib.Path(COMPLETED_DOWNLOAD_FOLDER).joinpath(self.category)
         if not self.completed_folder.exists() and not SEARCH_ONLY:
             try:
                 self.completed_folder.mkdir(parents=True, exist_ok=True)
                 self.completed_folder.chmod(mode=0o777)
             except BaseException:
@@ -300,14 +297,25 @@
         try:
             version_info = self.client.get_update()
             self.version = version_parser.parse(version_info[0].get("version"))
             self.logger.debug("%s version: %s", self._name, self.version.__str__())
         except Exception:
             self.logger.debug("Failed to get version")
 
+        self.use_temp_for_missing = CONFIG.get(
+            f"{name}.EntrySearch.UseTempForMissing", fallback=False
+        )
+        self.main_quality_profile = CONFIG.get(f"{self._name}.EntrySearch.MainQualityProfile")
+        self.temp_quality_profile = CONFIG.get(f"{self._name}.EntrySearch.TempQualityProfile")
+        if self.use_temp_for_missing:
+            (
+                self.main_quality_profile_id,
+                self.temp_quality_profile_id,
+            ) = self.parse_quality_profiles()
+
         if self.rss_sync_timer > 0:
             self.rss_sync_timer_last_checked = datetime(1970, 1, 1)
         else:
             self.rss_sync_timer_last_checked = None
         if self.refresh_downloads_timer > 0:
             self.refresh_downloads_timer_last_checked = datetime(1970, 1, 1)
         else:
@@ -2143,14 +2151,48 @@
                         )
                     ):
                         searched = True
                         self.model_queue.update(Completed=True).where(
                             self.model_queue.EntryId == episode["id"]
                         ).execute()
 
+                    if self.use_temp_for_missing:
+                        if (
+                            searched
+                            and db_entry["qualityProfileId"] == self.temp_quality_profile_id
+                        ):
+                            data: JsonObject = {"qualityProfileId": self.main_quality_profile_id}
+                            self.logger.debug(
+                                "Updating quality profile for %s to %s",
+                                db_entry["title"],
+                                self.temp_quality_profile,
+                            )
+                        elif (
+                            not searched
+                            and db_entry["qualityProfileId"] == self.main_quality_profile_id
+                        ):
+                            data: JsonObject = {"qualityProfileId": self.temp_quality_profile_id}
+                            self.logger.debug(
+                                "Updating quality profile for %s to %s",
+                                db_entry["title"],
+                                self.temp_quality_profile,
+                            )
+                        completed = True
+                        while completed:
+                            completed = False
+                            try:
+                                self.client.upd_episode(episode["id"], data)
+                            except (
+                                requests.exceptions.ChunkedEncodingError,
+                                requests.exceptions.ContentDecodingError,
+                                requests.exceptions.ConnectionError,
+                                JSONDecodeError,
+                            ) as e:
+                                completed = True
+
                     if episode["monitored"] == True:
                         EntryId = episode["id"]
 
                         SeriesTitle = episode.get("series", {}).get("title")
                         SeasonNumber = episode["seasonNumber"]
                         Title = episode["title"]
                         SeriesId = episode["seriesId"]
@@ -2307,14 +2349,48 @@
                                 episodeFileCount = episodeFileCount + statistics.get(
                                     "episodeFileCount"
                                 )
                         if self.search_specials:
                             searched = totalEpisodeCount == episodeFileCount
                         else:
                             searched = (episodeCount + monitoredEpisodeCount) == episodeFileCount
+                        if self.use_temp_for_missing:
+                            if (
+                                searched
+                                and db_entry["qualityProfileId"] == self.temp_quality_profile_id
+                            ):
+                                db_entry["qualityProfileId"] = self.main_quality_profile_id
+                                self.logger.debug(
+                                    "Updating quality profile for %s to %s",
+                                    db_entry["title"],
+                                    self.temp_quality_profile,
+                                )
+                            elif (
+                                not searched
+                                and db_entry["qualityProfileId"] == self.main_quality_profile_id
+                            ):
+                                db_entry["qualityProfileId"] = self.temp_quality_profile_id
+                                self.logger.debug(
+                                    "Updating quality profile for %s to %s",
+                                    db_entry["title"],
+                                    self.temp_quality_profile,
+                                )
+                            completed = True
+                            while completed:
+                                completed = False
+                                try:
+                                    self.client.upd_series(db_entry)
+                                except (
+                                    requests.exceptions.ChunkedEncodingError,
+                                    requests.exceptions.ContentDecodingError,
+                                    requests.exceptions.ConnectionError,
+                                    JSONDecodeError,
+                                ) as e:
+                                    completed = True
+
                         Title = seriesMetadata.get("title")
                         Monitored = db_entry["monitored"]
 
                         to_update = {
                             self.series_file_model.Monitored: Monitored,
                             self.series_file_model.Title: Title,
                             self.series_file_model.MinCustomFormatScore: minCustomFormat,
@@ -2375,14 +2451,15 @@
                                     customFormat = self.client.get_movie_file(
                                         db_entry["movieFile"]["id"]
                                     )["customFormatScore"]
                                 else:
                                     customFormat = 0
                             else:
                                 customFormat = 0
+
                         else:
                             minCustomFormat = self.client.get_quality_profile(
                                 db_entry["qualityProfileId"]
                             )["minFormatScore"]
                             if db_entry["hasFile"]:
                                 customFormat = self.client.get_movie_file(
                                     db_entry["movieFile"]["id"]
@@ -2409,14 +2486,45 @@
                     and not (self.custom_format_unmet_search and customFormat < minCustomFormat)
                 ):
                     searched = True
                     self.model_queue.update(Completed=True).where(
                         self.model_queue.EntryId == db_entry["id"]
                     ).execute()
 
+                if self.use_temp_for_missing:
+                    if searched and db_entry["qualityProfileId"] == self.temp_quality_profile_id:
+                        db_entry["qualityProfileId"] = self.main_quality_profile_id
+                        self.logger.debug(
+                            "Updating quality profile for %s to %s",
+                            db_entry["title"],
+                            self.temp_quality_profile,
+                        )
+                    elif (
+                        not searched
+                        and db_entry["qualityProfileId"] == self.main_quality_profile_id
+                    ):
+                        db_entry["qualityProfileId"] = self.temp_quality_profile_id
+                        self.logger.debug(
+                            "Updating quality profile for %s to %s",
+                            db_entry["title"],
+                            self.temp_quality_profile,
+                        )
+                    completed = True
+                    while completed:
+                        completed = False
+                        try:
+                            self.client.upd_movie(db_entry)
+                        except (
+                            requests.exceptions.ChunkedEncodingError,
+                            requests.exceptions.ContentDecodingError,
+                            requests.exceptions.ConnectionError,
+                            JSONDecodeError,
+                        ) as e:
+                            completed = True
+
                 if self.minimum_availability_check(db_entry) and db_entry["monitored"] == True:
                     title = db_entry["title"]
                     monitored = db_entry["monitored"]
                     tmdbId = db_entry["tmdbId"]
                     year = db_entry["year"]
                     entryId = db_entry["id"]
                     movieFileId = 1 if "movieFileId" in db_entry else 0
@@ -3865,15 +3973,20 @@
         if "qBitrr-ignored" in torrent.tags:
             torrent.remove_tags(
                 [
                     "qBitrr-allowed_seeding",
                     "qBitrr-free_space_paused",
                 ]
             )
-        if self.custom_format_unmet_search and self.custom_format_unmet_check(torrent):
+        if (
+            self.custom_format_unmet_search
+            and self.custom_format_unmet_check(torrent)
+            and "qBitrr-ignored" not in torrent.tags
+            and "qBitrr-free_space_paused" not in torrent.tags
+        ):
             self._process_single_torrent_delete_cfunmet(torrent)
         elif remove_torrent and not leave_alone and torrent.amount_left == 0:
             self._process_single_torrent_delete_ratio_seed(torrent)
         elif torrent.category == FAILED_CATEGORY:
             # Bypass everything if manually marked as failed
             self._process_single_torrent_failed_cat(torrent)
         elif torrent.category == RECHECK_CATEGORY:
@@ -3903,14 +4016,16 @@
             # stall after being resumed from a paused state).
             self._process_single_torrent_added_to_ignore_cache(torrent)
         elif torrent.state_enum == TorrentStates.QUEUED_UPLOAD:
             self._process_single_torrent_queued_upload(torrent, leave_alone)
         elif (
             torrent.progress >= self.maximum_deletable_percentage
             and self.is_complete_state(torrent) is False
+            and "qBitrr-ignored" not in torrent.tags
+            and "qBitrr-free_space_paused" not in torrent.tags
         ) and torrent.hash in self.cleaned_torrents:
             self._process_single_torrent_percentage_threshold(torrent, maximum_eta)
         # Resume monitored downloads which have been paused.
         elif (
             torrent.state_enum == TorrentStates.PAUSED_DOWNLOAD
             and torrent.amount_left != 0
             and "qBitrr-free_space_paused" not in torrent.tags
@@ -3957,29 +4072,31 @@
             torrent.state_enum != TorrentStates.PAUSED_DOWNLOAD
             and torrent.state_enum.is_downloading
             and self.recently_queue.get(torrent.hash, torrent.added_on)
             < time_now - self.ignore_torrents_younger_than
             and 0 < maximum_eta < torrent.eta
             and not self.do_not_remove_slow
             and "qBitrr-ignored" not in torrent.tags
+            and "qBitrr-free_space_paused" not in torrent.tags
         ):
             self._process_single_torrent_delete_slow(torrent)
         # Process uncompleted torrents
         elif torrent.state_enum.is_downloading:
             # If a torrent availability hasn't reached 100% or more within the configurable
             # "IgnoreTorrentsYoungerThan" variable, mark it for deletion.
-            self.logger.trace("Torrent availability: %s[%s]", torrent.name, torrent.availability)
             if (
                 (
                     self.recently_queue.get(torrent.hash, torrent.added_on)
                     < time_now - self.ignore_torrents_younger_than
                     and torrent.availability < 1
                 )
                 and torrent.hash in self.cleaned_torrents
+                and self.is_downloading_state(torrent)
                 and "qBitrr-ignored" not in torrent.tags
+                and "qBitrr-free_space_paused" not in torrent.tags
             ):
                 self._process_single_torrent_stalled_torrent(torrent, "Unavailable")
             else:
                 if torrent.hash in self.cleaned_torrents:
                     self._process_single_torrent_already_cleaned_up(torrent)
                     return
                 # A downloading torrent is not stalled, parse its contents.
@@ -4225,38 +4342,45 @@
                             e = entry.get("downloadId")
                             _path_filter.add((e, pathlib.Path(output_path).joinpath(title)))
                             # self.downloads_with_bad_error_message_blocklist.add(e)
             if len(_path_filter):
                 self.needs_cleanup = True
             self.files_to_explicitly_delete = iter(_path_filter.copy())
 
-    def force_grab(self):
-        return  # TODO: This may not be needed, pending more testing before it is enabled
-        _temp = self.get_queue()
-        _temp = filter(
-            lambda x: x.get("status") == "delay",
-            _temp,
-        )
-        ids = set()
-        for entry in _temp:
-            if id_ := entry.get("id"):
-                ids.add(id_)
-                self.logger.notice("Attempting to force grab: %s =  %s", id_, entry.get("title"))
-        if ids:
-            with ThreadPoolExecutor(max_workers=16) as executor:
-                executor.map(self._force_grab, ids)
-
-    def _force_grab(self, id_):
-        try:
-            path = f"queue/grab/{id_}"
-            res = self.client._post(path, self.client.ver_uri)
-            self.logger.trace("Successful Grab: %s", id_)
-            return res
-        except Exception:
-            self.logger.error("Exception when trying to force grab - %s", id_)
+    def parse_quality_profiles(self) -> tuple[int, int]:
+        main_quality_profile_id = 0
+        temp_quality_profile_id = 0
+        completed = True
+        while completed:
+            completed = False
+            try:
+                profiles = self.client.get_quality_profile()
+            except (
+                requests.exceptions.ChunkedEncodingError,
+                requests.exceptions.ContentDecodingError,
+                requests.exceptions.ConnectionError,
+                JSONDecodeError,
+            ) as e:
+                completed = True
+        for p in profiles:
+            if p["name"] == self.main_quality_profile:
+                main_quality_profile_id = p["id"]
+                self.logger.trace(
+                    "Quality profile %s:%s",
+                    self.main_quality_profile,
+                    main_quality_profile_id,
+                )
+            if p["name"] == self.temp_quality_profile:
+                temp_quality_profile_id = p["id"]
+                self.logger.trace(
+                    "Quality profile %s:%s",
+                    self.temp_quality_profile,
+                    temp_quality_profile_id,
+                )
+        return (main_quality_profile_id, temp_quality_profile_id)
 
     def register_search_mode(self):
         if self.search_setup_completed:
             return
         if self.search_missing is False:
             self.search_setup_completed = True
             return
@@ -4455,27 +4579,24 @@
                         self.search_current_year,
                     )
                 try:
                     self.db_maybe_reset_entry_searched_state()
                     self.refresh_download_queue()
                     self.db_update()
                     self.run_request_search()
-                    self.force_grab()
                     try:
                         if self.search_by_year:
                             if years.index(self.search_current_year) != years_count - 1:
                                 years_index += 1
                                 self.search_current_year = years[years_index]
                             elif datetime.now() >= (timer + loop_timer):
                                 self.refresh_download_queue()
-                                self.force_grab()
                                 raise RestartLoopException
                         elif datetime.now() >= (timer + loop_timer):
                             self.refresh_download_queue()
-                            self.force_grab()
                             raise RestartLoopException
                         if not searched:
                             for (
                                 entry,
                                 todays,
                                 limit_bypass,
                                 series_search,
@@ -4683,27 +4804,25 @@
         self.ignore_torrents_younger_than = CONFIG.get(
             "Settings.IgnoreTorrentsYoungerThan", fallback=600
         )
         self.timed_ignore_cache = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
         self.timed_skip = ExpiringSet(max_age_seconds=self.ignore_torrents_younger_than)
         self.tracker_delay = ExpiringSet(max_age_seconds=600)
         self._LOG_LEVEL = self.manager.qbit_manager.logger.level
+        self.logger = logging.getLogger(f"qBitrr.{self._name}")
         if ENABLE_LOGS:
             LOGS_FOLDER = HOME_PATH.joinpath("logs")
             LOGS_FOLDER.mkdir(parents=True, exist_ok=True)
             LOGS_FOLDER.chmod(mode=0o777)
             logfile = LOGS_FOLDER.joinpath(self._name + ".log")
             if pathlib.Path(logfile).is_file():
                 logold = LOGS_FOLDER.joinpath(self._name + ".log.old")
                 logfile.rename(logold)
             fh = logging.FileHandler(logfile)
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
             self.logger.addHandler(fh)
-        else:
-            self.logger = logging.getLogger(f"qBitrr.{self._name}")
         run_logs(self.logger)
         self.search_missing = False
         self.session = None
         self.logger.hnotice("Starting %s monitor", self._name)
 
     def _process_errored(self):
         # Recheck all torrents marked for rechecking.
@@ -4924,14 +5043,15 @@
                             sort="added_on",
                             reverse=False,
                         )
                     except qbittorrentapi.exceptions.APIError:
                         completed = True
                 torrents = [t for t in torrents if hasattr(t, "category")]
                 torrents = [t for t in torrents if t.category in self.categories]
+                torrents = [t for t in torrents if "qBitrr-ignored" not in t.tags]
                 if not len(torrents):
                     raise DelayLoopException(length=5, type="no_downloads")
                 if has_internet() is False:
                     self.manager.qbit_manager.should_delay_torrent_scan = True
                     raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="internet")
                 if self.manager.qbit_manager.should_delay_torrent_scan:
                     raise DelayLoopException(length=NO_INTERNET_SLEEP_TIMER, type="delay")
```

### Comparing `qbitrr2-4.6.9/qBitrr/config.py` & `qbitrr2-4.7.0/qBitrr/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "-s",
         "-h",
         "--help",
     ]
 ):
     CONFIG = MyConfig(CONFIG_FILE, config=generate_doc())
     COPIED_TO_NEW_DIR = None
-elif (not CONFIG_FILE.exists()) or (not CONFIG_PATH.exists()):
+elif (not CONFIG_FILE.exists()) and (not CONFIG_PATH.exists()):
     print(f"{file} has not been found")
 
     CONFIG_FILE = _write_config_file(docker=True)
     print(f"'{CONFIG_FILE.name}' has been generated")
     print('Rename it to "config.toml" then edit it and restart the container')
 
     CONFIG_EXISTS = False
```

### Comparing `qbitrr2-4.6.9/qBitrr/env_config.py` & `qbitrr2-4.7.0/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr/errors.py` & `qbitrr2-4.7.0/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr/ffprobe.py` & `qbitrr2-4.7.0/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr/gen_config.py` & `qbitrr2-4.7.0/qBitrr/gen_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,32 @@
     _gen_default_line(
         search_table,
         "Once you have search all files on your specified year range restart the loop and "
         "search again.",
         "SearchAgainOnSearchCompletion",
         True,
     )
+    _gen_default_line(
+        search_table,
+        "Main quality profile",
+        "MainQualityProfile",
+        "CHANGE_ME",
+    )
+    _gen_default_line(
+        search_table,
+        "Temp quality profile",
+        "TempQualityProfile",
+        "CHANGE_ME",
+    )
+    _gen_default_line(
+        search_table,
+        "Use Temp profile for missing",
+        "UseTempForMissing",
+        False,
+    )
     if "sonarr" in category.lower():
         _gen_default_line(
             search_table,
             "Search by series instead of by episode (This ignored the QualityUnmetSearch and CustomFormatUnmetSearch setting)",
             "SearchBySeries",
             True,
         )
```

### Comparing `qbitrr2-4.6.9/qBitrr/home_path.py` & `qbitrr2-4.7.0/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr/logger.py` & `qbitrr2-4.7.0/qBitrr/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             levelname=dict(color="red", bold=True),
             name=dict(color="blue", bold=True),
             thread=dict(color="cyan"),
         ),
         reconfigure=True,
     )
     if HAS_RUN is False:
+        HAS_RUN = True
         log_Debugs(logger)
 
 
 def log_Debugs(logger):
     logger.debug("Log Level: %s", CONSOLE_LOGGING_LEVEL_STRING)
     logger.debug("Ping URLs:  %s", PING_URLS)
     logger.debug("Script Config:  FailedCategory=%s", FAILED_CATEGORY)
```

### Comparing `qbitrr2-4.6.9/qBitrr/main.py` & `qbitrr2-4.7.0/qBitrr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,18 @@
 
 def run():
     global CHILD_PROCESSES
     early_exit = process_flags()
     if early_exit is True:
         sys.exit(0)
     logger.info("Starting qBitrr: Version: %s.", patched_version)
-    manager = qBitManager()
+    try:
+        manager = qBitManager()
+    except NameError:
+        sys.exit(0)
     run_logs(logger)
     logger.debug("Environment variables: %r", ENVIRO_CONFIG)
     try:
         if CHILD_PROCESSES := manager.get_child_processes():
             manager.run()
         else:
             logger.warning(
```

### Comparing `qbitrr2-4.6.9/qBitrr/tables.py` & `qbitrr2-4.7.0/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr/utils.py` & `qbitrr2-4.7.0/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.6.9/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.7.0/qBitrr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.6.9
+Version: 4.7.0
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -36,15 +36,15 @@
 Requires-Dist: jaraco.docker==2.0
 Requires-Dist: packaging==22.0
 Requires-Dist: pathos==0.2.8
 Requires-Dist: peewee==3.14.7
 Requires-Dist: ping3==3.0.2
 Requires-Dist: pyarr==5.2.0
 Requires-Dist: qbittorrent-api==2023.7.52
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: tomlkit==0.7.2
 Provides-Extra: dev
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: isort==5.10.1; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pre-commit==3.3.3; extra == "dev"
```

### Comparing `qbitrr2-4.6.9/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.7.0/qBitrr2.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jaraco.docker==2.0
 packaging==22.0
 pathos==0.2.8
 peewee==3.14.7
 ping3==3.0.2
 pyarr==5.2.0
 qbittorrent-api==2023.7.52
-requests==2.31.0
+requests==2.32.0
 tomlkit==0.7.2
 
 [all]
 black==24.3.0
 bump2version==1.0.1
 isort==5.10.1
 pip-tools==7.3.0
```

### Comparing `qbitrr2-4.6.9/setup.cfg` & `qbitrr2-4.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.6.9
+version = 4.7.0
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
@@ -44,15 +44,15 @@
 	jaraco.docker==2.0
 	packaging==22.0
 	pathos==0.2.8
 	peewee==3.14.7
 	ping3==3.0.2
 	pyarr==5.2.0
 	qbittorrent-api==2023.7.52
-	requests==2.31.0
+	requests==2.32.0
 	tomlkit==0.7.2
 python_requires = >=3.8.3,<4
 include_package_data = True
 
 [options.packages.find]
 include = 
 	qBitrr
```

