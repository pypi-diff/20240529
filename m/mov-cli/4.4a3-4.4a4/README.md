# Comparing `tmp/mov_cli-4.4a3.tar.gz` & `tmp/mov_cli-4.4a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.4a3.tar", last modified: Fri May 17 20:50:00 2024, max compression
+gzip compressed data, was "mov_cli-4.4a4.tar", last modified: Wed May 29 20:59:15 2024, max compression
```

## Comparing `mov_cli-4.4a3.tar` & `mov_cli-4.4a4.tar`

### file list

```diff
@@ -1,75 +1,82 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.135967 mov_cli-4.4a3/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.122634 mov_cli-4.4a3/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      469 2024-05-16 17:10:47.000000 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a3/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a3/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a3/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-17 20:50:00.135967 mov_cli-4.4a3/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5970 2024-05-16 17:10:47.000000 mov_cli-4.4a3/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1545 2024-05-16 17:10:47.000000 mov_cli-4.4a3/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-16 17:10:56.000000 mov_cli-4.4a3/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.129301 mov_cli-4.4a3/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a3/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6199 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a3/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2455 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2099 2024-05-16 21:27:57.000000 mov_cli-4.4a3/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a3/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      225 2024-05-16 17:09:32.000000 mov_cli-4.4a3/mov_cli/cli/random_tips.json
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1096 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7063 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1318 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     9115 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      640 2024-05-17 20:46:10.000000 mov_cli-4.4a3/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.129301 mov_cli-4.4a3/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a3/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a3/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a3/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       67 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3010 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1972 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/metadata.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      355 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/quality.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/iina.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1891 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/syncplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3638 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a3/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a3/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      707 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a3/mov_cli/utils/paths.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1133 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a3/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4752 2024-05-16 21:28:20.000000 mov_cli-4.4a3/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3576 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1460 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      244 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1801 2024-05-16 17:10:43.000000 mov_cli-4.4a3/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a3/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a3/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-17 20:50:00.135967 mov_cli-4.4a3/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.109878 mov_cli-4.4a4/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.099878 mov_cli-4.4a4/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.099878 mov_cli-4.4a4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      469 2024-05-16 17:10:47.000000 mov_cli-4.4a4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a4/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a4/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.099878 mov_cli-4.4a4/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a4/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a4/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a4/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a4/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      297 2024-05-29 20:59:05.000000 mov_cli-4.4a4/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-29 20:59:15.109878 mov_cli-4.4a4/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5970 2024-05-16 17:10:47.000000 mov_cli-4.4a4/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1545 2024-05-16 17:10:47.000000 mov_cli-4.4a4/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.099878 mov_cli-4.4a4/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      157 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3102 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/cache.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.103211 mov_cli-4.4a4/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a4/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5643 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a4/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2455 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2099 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3722 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a4/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      225 2024-05-16 17:09:32.000000 mov_cli-4.4a4/mov_cli/cli/random_tips.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1101 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7063 2024-05-29 20:59:05.000000 mov_cli-4.4a4/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1290 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    10017 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      912 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2197 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3677 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.103211 mov_cli-4.4a4/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a4/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a4/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a4/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.103211 mov_cli-4.4a4/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       67 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3010 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1972 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/media/metadata.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      355 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/media/quality.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      157 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/players/iina.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1936 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1362 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/players/mpv_tty.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3638 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a4/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1831 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      117 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      707 2024-05-16 17:10:43.000000 mov_cli-4.4a4/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      379 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/ip.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2238 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1125 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a4/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4752 2024-05-16 21:28:20.000000 mov_cli-4.4a4/mov_cli/utils/scraper/the_movie_db.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/mov_cli/utils/subtitles/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       61 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/subtitles/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    31113 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/subtitles/iso_639.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      832 2024-05-29 20:58:02.000000 mov_cli-4.4a4/mov_cli/utils/subtitles/lang.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3576 2024-05-27 19:43:48.000000 mov_cli-4.4a4/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1629 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      244 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-29 20:59:15.000000 mov_cli-4.4a4/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1833 2024-05-29 20:59:05.000000 mov_cli-4.4a4/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a4/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 20:59:15.106544 mov_cli-4.4a4/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a4/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-29 20:59:15.109878 mov_cli-4.4a4/setup.cfg
```

### Comparing `mov_cli-4.4a3/.github/workflows/pypi.yml` & `mov_cli-4.4a4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/.github/workflows/ruff.yml` & `mov_cli-4.4a4/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/LICENSE` & `mov_cli-4.4a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/PKG-INFO` & `mov_cli-4.4a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a3
+Version: 4.4a4
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a3 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a4 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.4a3/README.md` & `mov_cli-4.4a4/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/disclaimer.md` & `mov_cli-4.4a4/disclaimer.md`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/__main__.py` & `mov_cli-4.4a4/mov_cli/cli/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 if TYPE_CHECKING:
     ...
 
 import typer
 import logging
 from pathlib import Path
-from devgoldyutils import Colours
 
 from .play import play
 from .search import search
 from .ui import welcome_msg
 from .episode import handle_episode
 from .plugins import show_all_plugins
 from .scraper import select_scraper, use_scraper, scrape, steal_scraper_args
 from .configuration import open_config_file, set_cli_config
 
 from ..config import Config
 from ..download import Download
 from ..media import MetadataType
 from ..logger import mov_cli_logger
 from ..http_client import HTTPClient
+from ..utils import hide_ip
 
 __all__ = ("mov_cli",)
 
 uwu_app = typer.Typer(pretty_exceptions_enable = False) # NOTE: goldy has an uwu complex.
 
 def mov_cli(
     query: Optional[List[str]] = typer.Argument(None, help = "A film, tv show or anime you would like to Query."), 
@@ -127,38 +127,21 @@
                 f"The scraper '{chosen_scraper.__class__.__name__}' couldn't find{episode_details_string} '{choice.title}'! " \
                     "Don't report this to mov-cli, report this to the plugin itself."
             )
             return False
 
         if download:
             dl = Download(config)
-            mov_cli_logger.debug(f"Downloading from this url -> '{media.url}'")
+
+            mov_cli_logger.debug(f"Downloading from this url -> '{hide_ip(media.url, config)}'")
 
             popen = dl.download(media)
             
             if popen:
                 popen.wait()
 
         else:
-            option = play(media, choice, chosen_scraper, chosen_episode, config)
-
-            if option == "search":
-                query = input(Colours.BLUE.apply("  Enter Query: "))
-
-                mov_cli(
-                    query = [query], 
-                    debug = debug, 
-                    player = player, 
-                    scraper = scraper, 
-                    fzf = fzf,
-                    episode = None,
-                    auto_select = None,
-
-                    version = False,
-                    edit = False,
-                    download = False,
-                    list_plugins = False
-                )
+            play(media, choice, chosen_scraper, chosen_episode, config)
 
 def app():
     uwu_app.command()(mov_cli)
     uwu_app()
```

### Comparing `mov_cli-4.4a3/mov_cli/cli/configuration.py` & `mov_cli-4.4a4/mov_cli/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/episode.py` & `mov_cli-4.4a4/mov_cli/cli/episode.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/play.py` & `mov_cli-4.4a4/mov_cli/cli/play.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from devgoldyutils import Colours
 
 from .scraper import scrape
 from .episode import handle_episode
 from .watch_options import watch_options
 
 from ..media import MetadataType
-from ..utils import what_platform
+from ..utils import what_platform, hide_ip
 from ..logger import mov_cli_logger
 
 def play(media: Media, metadata: Metadata, scraper: Scraper, episode: EpisodeSelector, config: Config) -> Optional[Literal["search"]]:
     platform = what_platform()
 
     chosen_player = config.player
 
@@ -33,15 +33,15 @@
 
         episode_details_string = f"episode {episode_string} in season {season_string} of " if episode.season > 1 else f"episode {episode_string} of "
 
     mov_cli_logger.info(
         f"Playing {episode_details_string}'{Colours.BLUE.apply(media.title)}' " \
             f"with {chosen_player.display_name}..."
     )
-    mov_cli_logger.debug(f"Streaming with this url -> '{media.url}'")
+    mov_cli_logger.debug(f"Streaming with this url -> '{hide_ip(media.url, config)}'")
 
     try:
         popen = chosen_player.play(media)
     except FileNotFoundError as e:
         mov_cli_logger.error(
             f"The player '{chosen_player.display_name}' was not found! " \
                 f"Are you sure you have it installed? Are you sure it's in path? \nError: {e}"
@@ -52,57 +52,54 @@
         mov_cli_logger.error(
             f"The player '{chosen_player.display_name}' is not supported on this platform ({platform}). " \
             "We recommend VLC for iOS, IINA for MacOS and MPV for every other platform."
         )
 
         return None
 
-    option = watch_options(popen, chosen_player, platform, media, config.fzf_enabled)
+    if config.watch_options:
+        option = watch_options(popen, chosen_player, platform, media, config.fzf_enabled)
 
-    if option == "search":
-        popen.kill()
-        return option
+        if option == "next" or option == "previous":
+            popen.kill()
 
-    elif option == "next" or option == "previous":
-        popen.kill()
+            media_episodes = scraper.scrape_episodes(metadata)
 
-        media_episodes = scraper.scrape_episodes(metadata)
+            if option == "next":
+                episode.episode += 1
+            else:
+                episode.episode -= 1
 
-        if option == "next":
-            episode.episode += 1
-        else:
-            episode.episode -= 1
+            season_episode_count = media_episodes.get(episode.season)
 
-        season_episode_count = media_episodes.get(episode.season)
+            if season_episode_count is None:
+                mov_cli_logger.info("No more episodes :(")
+                return None
 
-        if season_episode_count is None:
-            mov_cli_logger.info("No more episodes :(")
-            return None
+            result = __handle_next_season(episode, season_episode_count, media_episodes)
 
-        result = __handle_next_season(episode, season_episode_count, media_episodes)
+            if result is False:
+                mov_cli_logger.info("No more episodes :(")
+                return None
 
-        if result is False:
-            mov_cli_logger.info("No more episodes :(")
-            return None
+            media = scrape(metadata, episode, scraper)
 
-        media = scrape(metadata, episode, scraper)
+            return play(media, metadata, scraper, episode, config)
 
-        return play(media, metadata, scraper, episode, config)
+        elif option == "select":
+            popen.kill()
 
-    elif option == "select":
-        popen.kill()
+            episode = handle_episode(None, scraper, metadata, config.fzf_enabled)
 
-        episode = handle_episode(None, scraper, metadata, config.fzf_enabled)
+            if episode is None:
+                return None
 
-        if episode is None:
-            return None
+            media = scrape(metadata, episode, scraper)
 
-        media = scrape(metadata, episode, scraper)
-
-        return play(media, metadata, scraper, episode, config)
+            return play(media, metadata, scraper, episode, config)
 
     popen.wait()
 
     return None
 
 def __handle_next_season(episode: EpisodeSelector, season_episode_count: int, media_episodes: dict) -> bool:
```

### Comparing `mov_cli-4.4a3/mov_cli/cli/plugins.py` & `mov_cli-4.4a4/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/scraper.py` & `mov_cli-4.4a4/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/search.py` & `mov_cli-4.4a4/mov_cli/cli/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .ui import prompt
 from .auto_select import auto_select_choice
 from .plugins import handle_internal_plugin_error
 
 from ..logger import mov_cli_logger
 
-def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool, limit: int = 20) -> Optional[Metadata]:
+def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool, limit: Optional[int]) -> Optional[Metadata]:
     choice = None
 
     mov_cli_logger.info(f"Searching for '{Colours.ORANGE.apply(query)}'...")
 
     try:
         search_results = scraper.search(query, limit)
     except Exception as e:
```

### Comparing `mov_cli-4.4a3/mov_cli/cli/ui.py` & `mov_cli-4.4a4/mov_cli/cli/ui.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/cli/watch_options.py` & `mov_cli-4.4a4/mov_cli/cli/watch_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 def watch_options(
     popen: Popen, 
     player: Player, 
     platform: SUPPORTED_PLATFORMS, 
     media: Media, 
     fzf_enabled: bool
-) -> Optional[Literal["search", "next", "previous", "select"]]:
+) -> Optional[Literal["next", "previous", "select"]]:
     options = [
-        "search",
         "replay",
         "quit"
     ]
 
     if isinstance(media, Multi):
         options.insert(0, "next")
         options.insert(1, "previous")
```

### Comparing `mov_cli-4.4a3/mov_cli/config.py` & `mov_cli-4.4a4/mov_cli/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 import toml
 import shutil
 from pathlib import Path
 from decouple import AutoConfig
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
-from . import players, utils
-from .logger import mov_cli_logger
-from .utils import get_appdata_directory
+from . import players
 from .media import Quality
+from .logger import mov_cli_logger
+from .utils import get_appdata_directory, what_platform
+from .utils.subtitles import Lang, lang_exists
 
 __all__ = ("Config",)
 
 @final
 class ConfigUIData(TypedDict):
     fzf: bool
 
@@ -44,26 +45,34 @@
     yt_dlp: bool
 
 @final
 class ConfigQualityData(TypedDict):
     resolution: int
 
 @final
+class ConfigSubtitleData(TypedDict):
+    language: str
+
+@final
 class ConfigData(TypedDict):
     version: int
     debug: bool
     player: str
     editor: str
     parser: SupportedParsersT
+    skip_update_checker: bool
+    hide_ip: bool
     ui: ConfigUIData
     http: ConfigHTTPData
     downloads: ConfigDownloadsData
     scrapers: ScrapersConfigT | Dict[str, str]
     plugins: Dict[str, str]
     quality: ConfigQualityData | str
+    watch_options: bool
+    subtitle: ConfigSubtitleData
 
 HttpHeadersData = TypedDict(
     "HttpHeadersData", 
     {
         "User-Agent": NotRequired[str],
         "Accept-Language": NotRequired[str],
         "Accept": NotRequired[str]
@@ -99,24 +108,26 @@
         return self.data.get("version", 1)
 
     @property
     def player(self) -> Player:
         """Returns the player class that was configured in the config. Defaults to MPV."""
         value = self.data.get("player", "mpv")
 
-        platform = utils.what_platform()
+        platform = what_platform()
 
         if value.lower() == "mpv":
             return players.MPV(platform, self)
         elif value.lower() == "vlc":
             return players.VLC(platform, self)
         elif value.lower() == "syncplay":
             return players.SyncPlay(platform, self)
         elif value.lower() == "iina":
             return players.IINA(platform, self)
+        elif value.lower() in ["tty", "mpv-tty"]:
+            return players.MPV_TTY(platform, self)
 
         return players.CustomPlayer(value)
 
     @property
     def plugins(self) -> Dict[str, str]:
         return self.data.get("plugins", {"test": "mov-cli-test"})
 
@@ -149,14 +160,18 @@
         return self.data.get("editor", None)
 
     @property
     def skip_update_checker(self) -> bool:
         return self.data.get("skip_update_checker", False)
 
     @property
+    def hide_ip(self) -> bool:
+        return self.data.get("hide_ip", True)
+
+    @property
     def default_scraper(self) -> Optional[str]:
         """Returns the scraper that should be used to scrape by default."""
         return self.data.get("scrapers", {}).get("default", None)
 
     @property
     def fzf_enabled(self) -> bool:
         """Returns whether fzf is allowed to be used. Defaults to True of fzf is available."""
@@ -204,14 +219,19 @@
                 proxy = f"{scheme}://{ip}:{port}"
 
             return {"all://": proxy}
         else:
             return None
 
     @property
+    def http_timeout(self) -> int:
+        """Returns the http timeout delay that should be set."""
+        return self.data.get("http", {}).get("timeout", 15)
+
+    @property
     def http_headers(self) -> HttpHeadersData:
         """Returns http headers."""
         default_headers = {
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0",
             "Accept-Language": "en-US,en;q=0.5",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
         }
@@ -237,44 +257,57 @@
 
         resolution_pixel = quality_config.get("resolution")
 
         if resolution_pixel is None or resolution_pixel not in Quality._value2member_map_:
             return Quality.AUTO
 
         return Quality(resolution_pixel)
+    
+    @property
+    def watch_options(self) -> bool:
+        return self.data.get("ui", {}).get("watch_options", True)
+
+    @property
+    def language(self) -> Lang:
+        language = self.data.get("subtitle", {}).get("language", "en")
+
+        if lang_exists(language):
+            return Lang(language)
+    
+        return Lang("en")
 
     def get_env_config(self) -> AutoConfig:
         """Returns python decouple config object for mov-cli's appdata .env file."""
         return AutoConfig(self._env_path)
 
     def __get_config_file(self) -> Path:
         """Function that returns the path to the config file with multi platform support."""
-        platform = utils.what_platform()
+        platform = what_platform()
 
         appdata_folder = get_appdata_directory(platform)
 
         config_path = appdata_folder.joinpath("config.toml")
 
         if not config_path.exists():
             logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
             config_file = open(config_path, "w")
 
-            template_config_path = f"{Path(os.path.split(__file__)[0])}{os.sep}config.template.toml"
+            template_config_path = Path(__file__).parent.joinpath("config.template.toml")
 
             with open(template_config_path, "r") as config_template:
                 config_file.write(config_template.read())
 
             config_file.close()
             logger.info(f"Config created at '{config_path}'.")
 
         return config_path
 
     def __get_env_file(self) -> Path:
         """Function that returns the path to the mov-cli .env file."""
-        platform = utils.what_platform()
+        platform = what_platform()
 
         appdata_folder = get_appdata_directory(platform)
 
         env_file_path = appdata_folder.joinpath(".env")
 
         if not env_file_path.exists():
             logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
```

### Comparing `mov_cli-4.4a3/mov_cli/download.py` & `mov_cli-4.4a4/mov_cli/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
             if media.referrer is not None:
                 args.extend(["--add-header", f"Referer:{media.referrer}"])
 
         else:
             logger.info("Downloading via ffmpeg...")
 
-            args = [ # TODO: Check if url is a m3u8 if not use aria2
+            args = [
                 "ffmpeg",
                 "-n",
                 "-headers",
                 f"Referer: {media.referrer}",
                 "-i",
                 media.url,
             ]
```

### Comparing `mov_cli-4.4a3/mov_cli/errors.py` & `mov_cli-4.4a4/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/http_client.py` & `mov_cli-4.4a4/mov_cli/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     from .config import Config
 
 import httpx
 from devgoldyutils import LoggerAdapter, Colours
 
 from . import errors
 from .logger import mov_cli_logger
+from .utils import hide_ip
 
 __all__ = ("HTTPClient",)
 
 class SiteMaybeBlocked(errors.MovCliException):
     """Raises there's a connection error during a get request."""
     def __init__(self, url: str, error: httpx.ConnectError) -> None:
         super().__init__(
@@ -26,30 +27,30 @@
 class HTTPClient():
     def __init__(self, config: Config) -> None:
         """A base class for building scrapers from."""
         self.config = config
         self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
 
         self.__httpx_client = httpx.Client(
-            timeout = 15.0,
+            timeout = config.http_timeout, 
             cookies = None
         )
-
+        
         super().__init__()
 
     def get(
         self, 
         url: str, 
         headers: dict = {}, 
         include_default_headers: bool = True, 
         redirect: bool = False, 
         **kwargs
     ) -> Response:
         """Performs a GET request and returns httpx.Response."""
-        self.logger.debug(Colours.GREEN.apply("GET") + f" -> {url}")
+        self.logger.debug(Colours.GREEN.apply("GET") + f" -> {hide_ip(url, self.config)}")
 
         if include_default_headers is True:
             if headers.get("Referer") is None:
                 headers.update({"Referer": url})
                 
             headers.update(self.config.http_headers)
 
@@ -59,20 +60,21 @@
                 headers = headers, 
                 follow_redirects = redirect, 
                 **kwargs
             )
 
             if response.is_error:
                 self.logger.debug(
-                    f"GET Request to '{response.url}' failed! ({response})"
+                    f"GET Request to '{response.url}' {Colours.RED.apply('failed!')} ({response})"
                 )
 
             return response
 
         except httpx.ConnectError as e:
+            # TODO: I think this needs improving. I see people are getting certificate errors that aren't being caught here.
             if "[SSL: CERTIFICATE_VERIFY_FAILED]" in str(e):
                 raise SiteMaybeBlocked(url, e)
 
             raise e
 
     def post(
         self, 
@@ -81,15 +83,15 @@
         json: dict = {}, 
         headers: dict = {}, 
         include_default_headers: bool = True, 
         redirect: bool = False, 
         **kwargs
     ) -> Response:
         """Performs a POST request and returns httpx.Response."""
-        self.logger.debug(Colours.GREEN.apply("POST") + f" -> {url}")
+        self.logger.debug(Colours.GREEN.apply("POST") + f" -> {hide_ip(url, self.config)}")
 
         if include_default_headers is True:
             if headers.get("Referer") is None:
                 headers.update({"Referer": url})
 
             headers.update(self.config.http_headers)
```

### Comparing `mov_cli-4.4a3/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.4a4/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/iterfzf/__init__.py` & `mov_cli-4.4a4/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/media/media.py` & `mov_cli-4.4a4/mov_cli/media/media.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/media/metadata.py` & `mov_cli-4.4a4/mov_cli/media/metadata.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/players/custom_player.py` & `mov_cli-4.4a4/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/players/iina.py` & `mov_cli-4.4a4/mov_cli/players/iina.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/players/mpv.py` & `mov_cli-4.4a4/mov_cli/players/mpv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Optional
-    from ..media import Media
+
     from .. import Config
+    from ..media import Media
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import subprocess
 from devgoldyutils import Colours
 
 from .player import Player
+from ..media.quality import Quality
 
 __all__ = ("MPV",)
 
 class MPV(Player):
     def __init__(self, platform: SUPPORTED_PLATFORMS, config: Config, **kwargs) -> None:
         self.platform = platform
         self.config = config
@@ -50,13 +52,13 @@
 
             if media.audio_url is not None:
                 args.append(f"--audio-file={media.audio_url}")
 
             if media.subtitles is not None:
                 args.append(f"--sub-file={media.subtitles}")
 
-            if self.config.resolution is not None:
+            if not self.config.resolution == Quality.AUTO:
                 args.append(f"--hls-bitrate={self.config.resolution.value}") # NOTE: This only works when the file is a m3u8
 
             return subprocess.Popen(args)
 
         return None
```

### Comparing `mov_cli-4.4a3/mov_cli/players/player.py` & `mov_cli-4.4a4/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/players/syncplay.py` & `mov_cli-4.4a4/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/players/vlc.py` & `mov_cli-4.4a4/mov_cli/players/vlc.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/plugins.py` & `mov_cli-4.4a4/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/scraper.py` & `mov_cli-4.4a4/mov_cli/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 
 __all__ = (
     "Scraper",
 )
 
 class Scraper(ABC):
     """A base class for building scrapers from."""
-    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
+    def __init__(
+            self, 
+            config: Config, 
+            http_client: HTTPClient, 
+            options: Optional[ScraperOptionsT] = None
+        ) -> None:
+
         self.config = config
         self.http_client = http_client
         self.options = options or {}
 
         self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
 
         super().__init__()
@@ -45,11 +51,10 @@
     def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Optional[Multi | Single]:
         """
         Where your scraping for the media should be performed. 
         Should return or yield an instance of Media.
         """
         ...
 
-    @abstractmethod
     def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
         """Returns episode count for each season in that Movie/Series."""
-        ...
+        return {None: 1}
```

### Comparing `mov_cli-4.4a3/mov_cli/utils/episode_selector.py` & `mov_cli-4.4a4/mov_cli/utils/episode_selector.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/utils/paths.py` & `mov_cli-4.4a4/mov_cli/utils/paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,30 +38,34 @@
 
     appdata_dir = appdata_dir.joinpath("mov-cli")
     appdata_dir.mkdir(exist_ok = True)
 
     return appdata_dir
 
 def get_temp_directory(platform: SUPPORTED_PLATFORMS) -> Path:
-    """Returns the temporary directory where mov-cli dumps stuff. Files stored here WILL get cleared/deleted."""
+    """
+    Returns the temporary directory where mov-cli can dump stuff. 
+    Files stored here WILL get cleared / deleted automatically by the operating system.
+    """
     temp_directory = None
 
     if platform == "Windows":
         temp_directory = Path(os.getenv("TEMP"))
 
     elif platform == "Darwin": # NOTE: Path maybe incorrect
         temp_directory = Path(os.getenv("TMPDIR"))
 
-    elif platform == "iOS":
-        # TODO: Temp directory for "iSH".
-        ...
+    elif platform == "Linux" and platform == "iOS":
+        linux_temp_dir = os.getenv("TMPDIR") # Respect the TMPDIR environment variable on Linux: https://unix.stackexchange.com/a/362107
 
-    elif platform == "Linux":
-        temp_directory = Path("/tmp")
+        if linux_temp_dir is None:
+            linux_temp_dir = "/tmp"
+
+        temp_directory = Path(linux_temp_dir)
 
     elif platform == "Android":
         temp_directory = Path("$PREFIX/tmp")
 
-    temp_directory = temp_directory.joinpath("mov-cli")
+    temp_directory = temp_directory.joinpath("mov-cli-temp")
     temp_directory.mkdir(exist_ok = True)
 
     return temp_directory
```

### Comparing `mov_cli-4.4a3/mov_cli/utils/platform.py` & `mov_cli-4.4a4/mov_cli/utils/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
         with open("/etc/os-release", "r") as f:
             os_release = csv.reader(f, delimiter="=")
             for row in os_release:
                 if row:
                     RELEASE_DATA[row[0]] = row[1]
 
         return RELEASE_DATA["ID"]    
-        
+
     return None
```

### Comparing `mov_cli-4.4a3/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.4a4/mov_cli/utils/scraper/the_movie_db.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli/utils/version.py` & `mov_cli-4.4a4/mov_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a3/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.4a4/mov_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a3
+Version: 4.4a4
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a3 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a4 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov_cli-4.4a3/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.4a4/mov_cli.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ruff.toml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/pypi.yml
 .github/workflows/ruff.yml
 mov_cli/__init__.py
+mov_cli/cache.py
 mov_cli/config.py
 mov_cli/config.template.toml
 mov_cli/download.py
 mov_cli/errors.py
 mov_cli/http_client.py
 mov_cli/logger.py
 mov_cli/plugins.py
@@ -43,18 +44,23 @@
 mov_cli/media/media.py
 mov_cli/media/metadata.py
 mov_cli/media/quality.py
 mov_cli/players/__init__.py
 mov_cli/players/custom_player.py
 mov_cli/players/iina.py
 mov_cli/players/mpv.py
+mov_cli/players/mpv_tty.py
 mov_cli/players/player.py
 mov_cli/players/syncplay.py
 mov_cli/players/vlc.py
 mov_cli/utils/__init__.py
 mov_cli/utils/episode_selector.py
+mov_cli/utils/ip.py
 mov_cli/utils/paths.py
 mov_cli/utils/platform.py
 mov_cli/utils/version.py
 mov_cli/utils/scraper/__init__.py
 mov_cli/utils/scraper/the_movie_db.py
+mov_cli/utils/subtitles/__init__.py
+mov_cli/utils/subtitles/iso_639.json
+mov_cli/utils/subtitles/lang.py
 scripts/test_cli.py
```

### Comparing `mov_cli-4.4a3/pyproject.toml` & `mov_cli-4.4a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["mov_cli*"]
 
 [tool.setuptools.package-data]
-"mov_cli" = ["config.template.toml", "cli/random_tips.json"]
+"mov_cli" = ["config.template.toml", "cli/random_tips.json", "utils/subtitles/iso_639.json"]
 
 [project.scripts]
 mov-cli = "mov_cli.cli.__main__:app"
```

