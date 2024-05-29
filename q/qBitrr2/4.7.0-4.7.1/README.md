# Comparing `tmp/qbitrr2-4.7.0.tar.gz` & `tmp/qbitrr2-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.7.0.tar", last modified: Wed May 29 12:58:38 2024, max compression
+gzip compressed data, was "qbitrr2-4.7.1.tar", last modified: Wed May 29 15:13:39 2024, max compression
```

## Comparing `qbitrr2-4.7.0.tar` & `qbitrr2-4.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.663204 qbitrr2-4.7.0/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   232066 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27032 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:58:38.663204 qbitrr2-4.7.0/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 12:58:38.000000 qbitrr2-4.7.0/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 12:58:38.667204 qbitrr2-4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:58:32.000000 qbitrr2-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:39.092072 qbitrr2-4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 15:13:39.092072 qbitrr2-4.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:39.092072 qbitrr2-4.7.1/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   232099 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27032 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:39.092072 qbitrr2-4.7.1/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 15:13:39.000000 qbitrr2-4.7.1/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 15:13:39.096072 qbitrr2-4.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:13:34.000000 qbitrr2-4.7.1/setup.py
```

### Comparing `qbitrr2-4.7.0/LICENSE` & `qbitrr2-4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/PKG-INFO` & `qbitrr2-4.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.7.0
+Version: 4.7.1
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -111,14 +111,15 @@
 - **Radarr v4 and v5 support**
 - Monitor Arr's to trigger missing episode searches.
 - Searches Radarr missing movies based on Minimum Availability
 - Customizable searching by series or singular episodes
 - Optionally searches year by year is ascending or descending order (config option available)
 - Search for CF Score unmet and cancel torrents base on CF Score or Quality unmet search
 - Set minimum free space in download directory and pause torrent downloads accordingly
+- Change quality profile temporarily for missing items until found
 
 ## Tested with
 
 Some things to know before using it.
 
 - qBittorrent >= 4.5.x
 - [Sonarr](https://github.com/Sonarr/Sonarr) and [Radarr](https://github.com/Radarr/Radarr) both setup to add tags to all downloads.
```

### Comparing `qbitrr2-4.7.0/README.md` & `qbitrr2-4.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 - **Radarr v4 and v5 support**
 - Monitor Arr's to trigger missing episode searches.
 - Searches Radarr missing movies based on Minimum Availability
 - Customizable searching by series or singular episodes
 - Optionally searches year by year is ascending or descending order (config option available)
 - Search for CF Score unmet and cancel torrents base on CF Score or Quality unmet search
 - Set minimum free space in download directory and pause torrent downloads accordingly
+- Change quality profile temporarily for missing items until found
 
 ## Tested with
 
 Some things to know before using it.
 
 - qBittorrent >= 4.5.x
 - [Sonarr](https://github.com/Sonarr/Sonarr) and [Radarr](https://github.com/Radarr/Radarr) both setup to add tags to all downloads.
```

### Comparing `qbitrr2-4.7.0/pyproject.toml` & `qbitrr2-4.7.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.7.0"
+version = "4.7.1"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.7.0/qBitrr/arss.py` & `qbitrr2-4.7.1/qBitrr/arss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1200,14 +1200,15 @@
         elif self.type == "sonarr" and not self.series_search:
             episodelist = self.db_get_files_episodes()
             for episodes in episodelist:
                 yield episodes[0], episodes[1], episodes[2], False, len(episodelist)
         elif self.type == "radarr":
             movielist = self.db_get_files_movies()
             for movies in movielist:
+                self.logger.trace("Movielist")
                 yield movies[0], movies[1], movies[2], False, len(movielist)
 
     def db_maybe_reset_entry_searched_state(self):
         if self.type == "sonarr":
             self.db_reset__series_searched_state()
             self.db_reset__episode_searched_state()
         elif self.type == "radarr":
@@ -2523,15 +2524,15 @@
 
                 if self.minimum_availability_check(db_entry) and db_entry["monitored"] == True:
                     title = db_entry["title"]
                     monitored = db_entry["monitored"]
                     tmdbId = db_entry["tmdbId"]
                     year = db_entry["year"]
                     entryId = db_entry["id"]
-                    movieFileId = 1 if "movieFileId" in db_entry else 0
+                    movieFileId = db_entry["movieFileId"]
                     qualityMet = not QualityUnmet if db_entry["hasFile"] else False
                     customFormatMet = customFormat > minCustomFormat
 
                     if not db_entry["hasFile"]:
                         reason = "Missing"
                     elif self.quality_unmet_search and QualityUnmet:
                         reason = "Quality"
```

### Comparing `qbitrr2-4.7.0/qBitrr/config.py` & `qbitrr2-4.7.1/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/env_config.py` & `qbitrr2-4.7.1/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/errors.py` & `qbitrr2-4.7.1/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/ffprobe.py` & `qbitrr2-4.7.1/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/gen_config.py` & `qbitrr2-4.7.1/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/home_path.py` & `qbitrr2-4.7.1/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/logger.py` & `qbitrr2-4.7.1/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/main.py` & `qbitrr2-4.7.1/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/tables.py` & `qbitrr2-4.7.1/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr/utils.py` & `qbitrr2-4.7.1/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.7.1/qBitrr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.7.0
+Version: 4.7.1
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
@@ -111,14 +111,15 @@
 - **Radarr v4 and v5 support**
 - Monitor Arr's to trigger missing episode searches.
 - Searches Radarr missing movies based on Minimum Availability
 - Customizable searching by series or singular episodes
 - Optionally searches year by year is ascending or descending order (config option available)
 - Search for CF Score unmet and cancel torrents base on CF Score or Quality unmet search
 - Set minimum free space in download directory and pause torrent downloads accordingly
+- Change quality profile temporarily for missing items until found
 
 ## Tested with
 
 Some things to know before using it.
 
 - qBittorrent >= 4.5.x
 - [Sonarr](https://github.com/Sonarr/Sonarr) and [Radarr](https://github.com/Radarr/Radarr) both setup to add tags to all downloads.
```

### Comparing `qbitrr2-4.7.0/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.7.1/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.0/setup.cfg` & `qbitrr2-4.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.7.0
+version = 4.7.1
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

