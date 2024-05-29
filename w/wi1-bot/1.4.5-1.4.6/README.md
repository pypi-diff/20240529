# Comparing `tmp/wi1-bot-1.4.5.tar.gz` & `tmp/wi1-bot-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.4.5.tar", last modified: Tue May 28 02:08:36 2024, max compression
+gzip compressed data, was "wi1-bot-1.4.6.tar", last modified: Wed May 29 03:15:19 2024, max compression
```

## Comparing `wi1-bot-1.4.5.tar` & `wi1-bot-1.4.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:08:36.836720 wi1-bot-1.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.828720 wi1-bot-1.4.5/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 02:08:35.000000 wi1-bot-1.4.5/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/rescan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8729 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-28 02:08:26.000000 wi1-bot-1.4.5/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:08:36.832720 wi1-bot-1.4.5/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 02:08:36.000000 wi1-bot-1.4.5/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.557452 wi1-bot-1.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.557452 wi1-bot-1.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.557452 wi1-bot-1.4.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.557452 wi1-bot-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.557452 wi1-bot-1.4.6/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-29 03:15:18.000000 wi1-bot-1.4.6/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/scripts/rescan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-29 03:15:09.000000 wi1-bot-1.4.6/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:15:19.561452 wi1-bot-1.4.6/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 03:15:19.000000 wi1-bot-1.4.6/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.4.5/.github/workflows/pypi-publish.yml` & `wi1-bot-1.4.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/LICENSE` & `wi1-bot-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/PKG-INFO` & `wi1-bot-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.5
+Version: 1.4.6
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.5/README.md` & `wi1-bot-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/config.yaml.template` & `wi1-bot-1.4.6/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/pyproject.toml` & `wi1-bot-1.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/arr/download.py` & `wi1-bot-1.4.6/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/arr/episode.py` & `wi1-bot-1.4.6/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/arr/movie.py` & `wi1-bot-1.4.6/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/arr/radarr.py` & `wi1-bot-1.4.6/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/arr/sonarr.py` & `wi1-bot-1.4.6/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/config.py` & `wi1-bot-1.4.6/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/discord/bot.py` & `wi1-bot-1.4.6/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.4.6/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.4.6/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/discord/helpers.py` & `wi1-bot-1.4.6/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/push.py` & `wi1-bot-1.4.6/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.4.6/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/scripts/rescan.py` & `wi1-bot-1.4.6/wi1_bot/scripts/rescan.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/scripts/start.py` & `wi1-bot-1.4.6/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.4.6/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.4.6/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.4.6/wi1_bot/transcoder/transcoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,16 @@
                 for line in proc.stdout:
                     ffmpeg_log_file.write(line)
                     last_output = line.strip()
 
             status = proc.wait()
 
             if status != 0:
+                transcode_to.unlink()
+
                 if "Error opening input files" in last_output:
                     self.logger.info(
                         f"file does not exist: {path}, skipping transcoding"
                     )
                     return True
 
                 if "received signal 15" in last_output:
@@ -139,24 +141,23 @@
                 push.send(
                     f"{path.name} has failed to transcode, log: {perm_log_path}",
                     title="transcoding error",
                 )
 
                 return True
 
-        new_path = path.parent / transcode_to.name
-
         if not path.exists():
             self.logger.debug(
                 f"file doesn't exist: {item.path}, deleting transcoded file"
             )
 
             transcode_to.unlink()
             return True
 
+        new_path = path.parent / transcode_to.name
         shutil.move(transcode_to, new_path)
         path.unlink()
 
         self._rescan_content(item, str(new_path))
 
         self.logger.info(f"transcoded: {path.name} -> {new_path.name}")
         # push.send(f"{path.name} -> {new_path.name}", title="file transcoded")
```

### Comparing `wi1-bot-1.4.5/wi1_bot/webhook.py` & `wi1-bot-1.4.6/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.5/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.4.6/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.5
+Version: 1.4.6
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.4.5/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.4.6/wi1_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

