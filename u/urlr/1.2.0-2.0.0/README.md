# Comparing `tmp/urlr-1.2.0.tar.gz` & `tmp/urlr-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlr-1.2.0.tar", last modified: Thu May  2 18:44:43 2024, max compression
+gzip compressed data, was "urlr-2.0.0.tar", last modified: Wed May 29 19:46:34 2024, max compression
```

## Comparing `urlr-1.2.0.tar` & `urlr-2.0.0.tar`

### file list

```diff
@@ -1,63 +1,73 @@
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.535401 urlr-1.2.0/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-05-02 18:44:43.535401 urlr-1.2.0/PKG-INFO
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4037 2024-05-02 18:42:46.000000 urlr-1.2.0/README.md
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1875 2024-05-02 18:42:46.000000 urlr-1.2.0/pyproject.toml
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       69 2024-05-02 18:44:43.535401 urlr-1.2.0/setup.cfg
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1200 2024-05-02 18:42:46.000000 urlr-1.2.0/setup.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.531401 urlr-1.2.0/test/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1494 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1544 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification401_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      771 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1480 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_authentification_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1596 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1571 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder200_response_folders_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      701 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1354 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_folder_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      696 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_link_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1610 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1481 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1624 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_reduce_link_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1399 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1390 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      699 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1499 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_stats_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1549 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1510 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team200_response_teams_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      685 2024-02-13 12:53:10.000000 urlr-1.2.0/test/test_team_api.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.532401 urlr-1.2.0/urlr/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1953 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/__init__.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.533401 urlr-1.2.0/urlr/api/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      268 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/api/__init__.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11979 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/authentification_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11576 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/folder_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11812 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/link_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11697 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/stats_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9942 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api/team_api.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    26250 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/api_client.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      652 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/api_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    14738 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/configuration.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     5940 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/exceptions.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.534401 urlr-1.2.0/urlr/models/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1279 2024-02-13 12:53:10.000000 urlr-1.2.0/urlr/models/__init__.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2523 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2624 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification401_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2699 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/authentification_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3000 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2701 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder200_response_folders_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2499 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/folder_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3399 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2840 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3758 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/reduce_link_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2708 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2561 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats400_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3386 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/stats_request.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2958 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/team200_response.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2681 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/models/team200_response_teams_inner.py
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 07:55:59.000000 urlr-1.2.0/urlr/py.typed
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9366 2024-05-02 18:42:46.000000 urlr-1.2.0/urlr/rest.py
-drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-02 18:44:43.534401 urlr-1.2.0/urlr.egg-info/
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      409 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/PKG-INFO
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1617 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/SOURCES.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        1 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/dependency_links.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       76 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/requires.txt
--rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        5 2024-05-02 18:44:43.000000 urlr-1.2.0/urlr.egg-info/top_level.txt
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.795398 urlr-2.0.0/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      796 2024-05-29 19:46:34.795398 urlr-2.0.0/PKG-INFO
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4732 2024-05-29 19:45:57.000000 urlr-2.0.0/README.md
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1875 2024-05-29 19:45:57.000000 urlr-2.0.0/pyproject.toml
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       69 2024-05-29 19:46:34.795398 urlr-2.0.0/setup.cfg
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1894 2024-05-29 19:45:57.000000 urlr-2.0.0/setup.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.790398 urlr-2.0.0/test/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1219 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_access_tokens_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1851 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_access_token200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1865 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_access_token401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1863 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_access_token_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2232 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_link201_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1816 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_link429_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1816 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_link500_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1996 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_create_link_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1023 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_folders_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1996 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_folders200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1962 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_folders200_response_folders_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1727 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_link200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1780 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_link401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1780 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_link404_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1780 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_link422_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1833 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_statistics200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1961 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_statistics_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1949 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_teams200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1901 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_get_teams200_response_teams_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1124 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_links_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1882 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_refresh_access_token401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1823 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_refresh_access_token_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1049 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_statistics_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     1007 2024-05-29 19:45:57.000000 urlr-2.0.0/test/test_teams_api.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.791398 urlr-2.0.0/urlr/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2731 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/__init__.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.792398 urlr-2.0.0/urlr/api/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      277 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/__init__.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    23381 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/access_tokens_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    11478 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/folders_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    22616 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/links_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    12658 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/statistics_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    10483 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api/teams_api.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    26557 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/api_client.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      652 2024-02-13 12:53:10.000000 urlr-2.0.0/urlr/api_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)    15051 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/configuration.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     6247 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/exceptions.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.794398 urlr-2.0.0/urlr/models/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2048 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/__init__.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3087 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_access_token200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2935 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_access_token401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2952 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_access_token_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4101 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_link201_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3079 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_link429_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3079 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_link500_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     4076 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/create_link_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3340 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_folders200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3017 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_folders200_response_folders_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2831 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_link200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3067 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_link401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3067 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_link404_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3067 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_link422_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3175 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_statistics200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3422 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_statistics_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     3298 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_teams200_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2997 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/get_teams200_response_teams_inner.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2939 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/refresh_access_token401_response.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2871 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/models/refresh_access_token_request.py
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-02-13 07:55:59.000000 urlr-2.0.0/urlr/py.typed
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     9673 2024-05-29 19:45:57.000000 urlr-2.0.0/urlr/rest.py
+drwxr-xr-x   0 hugoposnic  (1000) hugoposnic  (1000)        0 2024-05-29 19:46:34.795398 urlr-2.0.0/urlr.egg-info/
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)      796 2024-05-29 19:46:34.000000 urlr-2.0.0/urlr.egg-info/PKG-INFO
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)     2135 2024-05-29 19:46:34.000000 urlr-2.0.0/urlr.egg-info/SOURCES.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        1 2024-05-29 19:46:34.000000 urlr-2.0.0/urlr.egg-info/dependency_links.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)       76 2024-05-29 19:46:34.000000 urlr-2.0.0/urlr.egg-info/requires.txt
+-rw-r--r--   0 hugoposnic  (1000) hugoposnic  (1000)        5 2024-05-29 19:46:34.000000 urlr-2.0.0/urlr.egg-info/top_level.txt
```

### Comparing `urlr-1.2.0/pyproject.toml` & `urlr-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "urlr"
-version = "1.2.0"
+version = "2.0.0"
 description = "Python client for URLR"
 authors = ["URLR <contact@urlr.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/urlr/urlr-python"
 keywords = ["link shortener", "api", "sdk", "client"]
 include = ["urlr/py.typed"]
```

### Comparing `urlr-1.2.0/test/test_folder200_response.py` & `urlr-2.0.0/test/test_create_link500_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.folder200_response import Folder200Response
+from urlr.models.create_link500_response import CreateLink500Response
 
-class TestFolder200Response(unittest.TestCase):
-    """Folder200Response unit test stubs"""
+class TestCreateLink500Response(unittest.TestCase):
+    """CreateLink500Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Folder200Response:
-        """Test Folder200Response
+    def make_instance(self, include_optional) -> CreateLink500Response:
+        """Test CreateLink500Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Folder200Response`
+        # uncomment below to create an instance of `CreateLink500Response`
         """
-        model = Folder200Response()
+        model = CreateLink500Response()
         if include_optional:
-            return Folder200Response(
-                folders = [
-                    urlr.models.folder_200_response_folders_inner.folder_200_response_folders_inner(
-                        id = 123, 
-                        name = 'folder-campaign-google-ads', )
-                    ]
+            return CreateLink500Response(
+                type = '',
+                title = '',
+                status = 500,
+                detail = ''
             )
         else:
-            return Folder200Response(
+            return CreateLink500Response(
         )
         """
 
-    def testFolder200Response(self):
-        """Test Folder200Response"""
+    def testCreateLink500Response(self):
+        """Test CreateLink500Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_link_api.py` & `urlr-2.0.0/test/test_folders_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.api.link_api import LinkApi
+from urlr.api.folders_api import FoldersApi
 
 
-class TestLinkApi(unittest.TestCase):
-    """LinkApi unit test stubs"""
+class TestFoldersApi(unittest.TestCase):
+    """FoldersApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = LinkApi()
+        self.api = FoldersApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_reduce_link(self) -> None:
-        """Test case for reduce_link
+    def test_get_folders(self) -> None:
+        """Test case for get_folders
 
-        Shorten a link
+        Get folders of team
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_reduce_link200_response.py` & `urlr-2.0.0/test/test_get_link200_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.reduce_link200_response import ReduceLink200Response
+from urlr.models.get_link200_response import GetLink200Response
 
-class TestReduceLink200Response(unittest.TestCase):
-    """ReduceLink200Response unit test stubs"""
+class TestGetLink200Response(unittest.TestCase):
+    """GetLink200Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ReduceLink200Response:
-        """Test ReduceLink200Response
+    def make_instance(self, include_optional) -> GetLink200Response:
+        """Test GetLink200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ReduceLink200Response`
+        # uncomment below to create an instance of `GetLink200Response`
         """
-        model = ReduceLink200Response()
+        model = GetLink200Response()
         if include_optional:
-            return ReduceLink200Response(
-                url = '',
-                expired_at = '',
-                team = 56,
-                folder = 56,
-                url_code = 'xMs5c',
-                domain = 'urlr.me',
-                code = 200
+            return GetLink200Response(
+                id = '436b5d20-e174-4363-94e5-2b3dd4e74b5f'
             )
         else:
-            return ReduceLink200Response(
+            return GetLink200Response(
         )
         """
 
-    def testReduceLink200Response(self):
-        """Test ReduceLink200Response"""
+    def testGetLink200Response(self):
+        """Test GetLink200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_reduce_link400_response.py` & `urlr-2.0.0/test/test_get_link422_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.reduce_link400_response import ReduceLink400Response
+from urlr.models.get_link422_response import GetLink422Response
 
-class TestReduceLink400Response(unittest.TestCase):
-    """ReduceLink400Response unit test stubs"""
+class TestGetLink422Response(unittest.TestCase):
+    """GetLink422Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ReduceLink400Response:
-        """Test ReduceLink400Response
+    def make_instance(self, include_optional) -> GetLink422Response:
+        """Test GetLink422Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ReduceLink400Response`
+        # uncomment below to create an instance of `GetLink422Response`
         """
-        model = ReduceLink400Response()
+        model = GetLink422Response()
         if include_optional:
-            return ReduceLink400Response(
-                code = 401,
-                error = -1,
-                message = ''
+            return GetLink422Response(
+                type = '',
+                title = '',
+                status = 422,
+                detail = ''
             )
         else:
-            return ReduceLink400Response(
+            return GetLink422Response(
         )
         """
 
-    def testReduceLink400Response(self):
-        """Test ReduceLink400Response"""
+    def testGetLink422Response(self):
+        """Test GetLink422Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_reduce_link_request.py` & `urlr-2.0.0/test/test_create_link_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.reduce_link_request import ReduceLinkRequest
+from urlr.models.create_link_request import CreateLinkRequest
 
-class TestReduceLinkRequest(unittest.TestCase):
-    """ReduceLinkRequest unit test stubs"""
+class TestCreateLinkRequest(unittest.TestCase):
+    """CreateLinkRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ReduceLinkRequest:
-        """Test ReduceLinkRequest
+    def make_instance(self, include_optional) -> CreateLinkRequest:
+        """Test CreateLinkRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ReduceLinkRequest`
+        # uncomment below to create an instance of `CreateLinkRequest`
         """
-        model = ReduceLinkRequest()
+        model = CreateLinkRequest()
         if include_optional:
-            return ReduceLinkRequest(
+            return CreateLinkRequest(
                 url = '',
-                team = '',
-                folder = '',
-                code = 'zA9LCSLv1C1ylmgd0-Y2TA5',
+                team_id = '',
+                folder_id = '',
+                code = 'xxxxx',
                 label = '',
                 password = '',
-                expired_at = ''
+                expired_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else:
-            return ReduceLinkRequest(
+            return CreateLinkRequest(
                 url = '',
-                team = '',
+                team_id = '',
         )
         """
 
-    def testReduceLinkRequest(self):
-        """Test ReduceLinkRequest"""
+    def testCreateLinkRequest(self):
+        """Test CreateLinkRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_stats200_response.py` & `urlr-2.0.0/test/test_get_link401_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.stats200_response import Stats200Response
+from urlr.models.get_link401_response import GetLink401Response
 
-class TestStats200Response(unittest.TestCase):
-    """Stats200Response unit test stubs"""
+class TestGetLink401Response(unittest.TestCase):
+    """GetLink401Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Stats200Response:
-        """Test Stats200Response
+    def make_instance(self, include_optional) -> GetLink401Response:
+        """Test GetLink401Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Stats200Response`
+        # uncomment below to create an instance of `GetLink401Response`
         """
-        model = Stats200Response()
+        model = GetLink401Response()
         if include_optional:
-            return Stats200Response(
-                clicks = 32,
-                unique_clicks = 51
+            return GetLink401Response(
+                type = '',
+                title = '',
+                status = 401,
+                detail = ''
             )
         else:
-            return Stats200Response(
+            return GetLink401Response(
         )
         """
 
-    def testStats200Response(self):
-        """Test Stats200Response"""
+    def testGetLink401Response(self):
+        """Test GetLink401Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_stats400_response.py` & `urlr-2.0.0/test/test_create_access_token401_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.stats400_response import Stats400Response
+from urlr.models.create_access_token401_response import CreateAccessToken401Response
 
-class TestStats400Response(unittest.TestCase):
-    """Stats400Response unit test stubs"""
+class TestCreateAccessToken401Response(unittest.TestCase):
+    """CreateAccessToken401Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Stats400Response:
-        """Test Stats400Response
+    def make_instance(self, include_optional) -> CreateAccessToken401Response:
+        """Test CreateAccessToken401Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Stats400Response`
+        # uncomment below to create an instance of `CreateAccessToken401Response`
         """
-        model = Stats400Response()
+        model = CreateAccessToken401Response()
         if include_optional:
-            return Stats400Response(
+            return CreateAccessToken401Response(
                 code = 401,
-                error = -1
+                message = 'Invalid credentials.'
             )
         else:
-            return Stats400Response(
+            return CreateAccessToken401Response(
         )
         """
 
-    def testStats400Response(self):
-        """Test Stats400Response"""
+    def testCreateAccessToken401Response(self):
+        """Test CreateAccessToken401Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_stats_request.py` & `urlr-2.0.0/test/test_refresh_access_token_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.stats_request import StatsRequest
+from urlr.models.refresh_access_token_request import RefreshAccessTokenRequest
 
-class TestStatsRequest(unittest.TestCase):
-    """StatsRequest unit test stubs"""
+class TestRefreshAccessTokenRequest(unittest.TestCase):
+    """RefreshAccessTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> StatsRequest:
-        """Test StatsRequest
+    def make_instance(self, include_optional) -> RefreshAccessTokenRequest:
+        """Test RefreshAccessTokenRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `StatsRequest`
+        # uncomment below to create an instance of `RefreshAccessTokenRequest`
         """
-        model = StatsRequest()
+        model = RefreshAccessTokenRequest()
         if include_optional:
-            return StatsRequest(
-                code = 'zA9LCSLv1C1ylmgd0-Y2TA5',
-                var_from = 'dd/mm/yyyy',
-                to = 'dd/mm/yyyy',
-                include_bots = True
+            return RefreshAccessTokenRequest(
+                refresh_token = ''
             )
         else:
-            return StatsRequest(
-                code = 'zA9LCSLv1C1ylmgd0-Y2TA5',
+            return RefreshAccessTokenRequest(
+                refresh_token = '',
         )
         """
 
-    def testStatsRequest(self):
-        """Test StatsRequest"""
+    def testRefreshAccessTokenRequest(self):
+        """Test RefreshAccessTokenRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/test/test_team200_response.py` & `urlr-2.0.0/test/test_get_teams200_response_teams_inner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from urlr.models.team200_response import Team200Response
+from urlr.models.get_teams200_response_teams_inner import GetTeams200ResponseTeamsInner
 
-class TestTeam200Response(unittest.TestCase):
-    """Team200Response unit test stubs"""
+class TestGetTeams200ResponseTeamsInner(unittest.TestCase):
+    """GetTeams200ResponseTeamsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Team200Response:
-        """Test Team200Response
+    def make_instance(self, include_optional) -> GetTeams200ResponseTeamsInner:
+        """Test GetTeams200ResponseTeamsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Team200Response`
+        # uncomment below to create an instance of `GetTeams200ResponseTeamsInner`
         """
-        model = Team200Response()
+        model = GetTeams200ResponseTeamsInner()
         if include_optional:
-            return Team200Response(
-                teams = [
-                    urlr.models.team_200_response_teams_inner.team_200_response_teams_inner(
-                        id = 131, 
-                        name = 'the best team', )
-                    ]
+            return GetTeams200ResponseTeamsInner(
+                id = 'ffefc6c4-d970-4373-a867-2a69c8be2c89',
+                name = 'the best team'
             )
         else:
-            return Team200Response(
+            return GetTeams200ResponseTeamsInner(
         )
         """
 
-    def testTeam200Response(self):
-        """Test Team200Response"""
+    def testGetTeams200ResponseTeamsInner(self):
+        """Test GetTeams200ResponseTeamsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `urlr-1.2.0/urlr/__init__.py` & `urlr-2.0.0/urlr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.2.0"
+__version__ = "2.0.0"
 
 # import apis into sdk package
-from urlr.api.authentification_api import AuthentificationApi
-from urlr.api.folder_api import FolderApi
-from urlr.api.link_api import LinkApi
-from urlr.api.stats_api import StatsApi
-from urlr.api.team_api import TeamApi
+from urlr.api.access_tokens_api import AccessTokensApi
+from urlr.api.folders_api import FoldersApi
+from urlr.api.links_api import LinksApi
+from urlr.api.statistics_api import StatisticsApi
+from urlr.api.teams_api import TeamsApi
 
 # import ApiClient
 from urlr.api_response import ApiResponse
 from urlr.api_client import ApiClient
 from urlr.configuration import Configuration
 from urlr.exceptions import OpenApiException
 from urlr.exceptions import ApiTypeError
 from urlr.exceptions import ApiValueError
 from urlr.exceptions import ApiKeyError
 from urlr.exceptions import ApiAttributeError
 from urlr.exceptions import ApiException
 
 # import models into sdk package
-from urlr.models.authentification200_response import Authentification200Response
-from urlr.models.authentification401_response import Authentification401Response
-from urlr.models.authentification_request import AuthentificationRequest
-from urlr.models.folder200_response import Folder200Response
-from urlr.models.folder200_response_folders_inner import Folder200ResponseFoldersInner
-from urlr.models.folder_request import FolderRequest
-from urlr.models.reduce_link200_response import ReduceLink200Response
-from urlr.models.reduce_link400_response import ReduceLink400Response
-from urlr.models.reduce_link_request import ReduceLinkRequest
-from urlr.models.stats200_response import Stats200Response
-from urlr.models.stats400_response import Stats400Response
-from urlr.models.stats_request import StatsRequest
-from urlr.models.team200_response import Team200Response
-from urlr.models.team200_response_teams_inner import Team200ResponseTeamsInner
+from urlr.models.create_access_token200_response import CreateAccessToken200Response
+from urlr.models.create_access_token401_response import CreateAccessToken401Response
+from urlr.models.create_access_token_request import CreateAccessTokenRequest
+from urlr.models.create_link201_response import CreateLink201Response
+from urlr.models.create_link429_response import CreateLink429Response
+from urlr.models.create_link500_response import CreateLink500Response
+from urlr.models.create_link_request import CreateLinkRequest
+from urlr.models.get_folders200_response import GetFolders200Response
+from urlr.models.get_folders200_response_folders_inner import GetFolders200ResponseFoldersInner
+from urlr.models.get_link200_response import GetLink200Response
+from urlr.models.get_link401_response import GetLink401Response
+from urlr.models.get_link404_response import GetLink404Response
+from urlr.models.get_link422_response import GetLink422Response
+from urlr.models.get_statistics200_response import GetStatistics200Response
+from urlr.models.get_statistics_request import GetStatisticsRequest
+from urlr.models.get_teams200_response import GetTeams200Response
+from urlr.models.get_teams200_response_teams_inner import GetTeams200ResponseTeamsInner
+from urlr.models.refresh_access_token401_response import RefreshAccessToken401Response
+from urlr.models.refresh_access_token_request import RefreshAccessTokenRequest
```

### Comparing `urlr-1.2.0/urlr/api/authentification_api.py` & `urlr-2.0.0/urlr/api/statistics_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field
 from typing import Optional
 from typing_extensions import Annotated
-from urlr.models.authentification200_response import Authentification200Response
-from urlr.models.authentification_request import AuthentificationRequest
+from urlr.models.get_statistics200_response import GetStatistics200Response
+from urlr.models.get_statistics_request import GetStatisticsRequest
 
 from urlr.api_client import ApiClient, RequestSerialized
 from urlr.api_response import ApiResponse
 from urlr.rest import RESTResponseType
 
 
-class AuthentificationApi:
+class StatisticsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def authentification(
+    def get_statistics(
         self,
-        authentification_request: Annotated[Optional[AuthentificationRequest], Field(description="Your credentials")] = None,
+        get_statistics_request: Annotated[Optional[GetStatisticsRequest], Field(description="Infos to provide to get statistics of a link")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Authentification200Response:
-        """Get an access token
+    ) -> GetStatistics200Response:
+        """Get statistics of a link
 
 
-        :param authentification_request: Your credentials
-        :type authentification_request: AuthentificationRequest
+        :param get_statistics_request: Infos to provide to get statistics of a link
+        :type get_statistics_request: GetStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,59 +81,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._authentification_serialize(
-            authentification_request=authentification_request,
+        _param = self._get_statistics_serialize(
+            get_statistics_request=get_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Authentification200Response",
-            '401': "Authentification401Response",
+            '200': "GetStatistics200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def authentification_with_http_info(
+    def get_statistics_with_http_info(
         self,
-        authentification_request: Annotated[Optional[AuthentificationRequest], Field(description="Your credentials")] = None,
+        get_statistics_request: Annotated[Optional[GetStatisticsRequest], Field(description="Infos to provide to get statistics of a link")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Authentification200Response]:
-        """Get an access token
+    ) -> ApiResponse[GetStatistics200Response]:
+        """Get statistics of a link
 
 
-        :param authentification_request: Your credentials
-        :type authentification_request: AuthentificationRequest
+        :param get_statistics_request: Infos to provide to get statistics of a link
+        :type get_statistics_request: GetStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -148,59 +150,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._authentification_serialize(
-            authentification_request=authentification_request,
+        _param = self._get_statistics_serialize(
+            get_statistics_request=get_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Authentification200Response",
-            '401': "Authentification401Response",
+            '200': "GetStatistics200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def authentification_without_preload_content(
+    def get_statistics_without_preload_content(
         self,
-        authentification_request: Annotated[Optional[AuthentificationRequest], Field(description="Your credentials")] = None,
+        get_statistics_request: Annotated[Optional[GetStatisticsRequest], Field(description="Infos to provide to get statistics of a link")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get an access token
+        """Get statistics of a link
 
 
-        :param authentification_request: Your credentials
-        :type authentification_request: AuthentificationRequest
+        :param get_statistics_request: Infos to provide to get statistics of a link
+        :type get_statistics_request: GetStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -215,36 +219,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._authentification_serialize(
-            authentification_request=authentification_request,
+        _param = self._get_statistics_serialize(
+            get_statistics_request=get_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Authentification200Response",
-            '401': "Authentification401Response",
+            '200': "GetStatistics200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _authentification_serialize(
+    def _get_statistics_serialize(
         self,
-        authentification_request,
+        get_statistics_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -260,22 +266,23 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if authentification_request is not None:
-            _body_params = authentification_request
+        if get_statistics_request is not None:
+            _body_params = get_statistics_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json'
+                'application/json', 
+                'application/problem+json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
@@ -287,19 +294,20 @@
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
+            'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/login_check',
+            resource_path='/statistics',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `urlr-1.2.0/urlr/api/folder_api.py` & `urlr-2.0.0/urlr/api/teams_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,65 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field
-from typing import Optional
-from typing_extensions import Annotated
-from urlr.models.folder200_response import Folder200Response
-from urlr.models.folder_request import FolderRequest
+from urlr.models.get_teams200_response import GetTeams200Response
 
 from urlr.api_client import ApiClient, RequestSerialized
 from urlr.api_response import ApiResponse
 from urlr.rest import RESTResponseType
 
 
-class FolderApi:
+class TeamsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def folder(
+    def get_teams(
         self,
-        folder_request: Annotated[Optional[FolderRequest], Field(description="Infos to provide to get folders of team")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Folder200Response:
-        """Get folders of team
+    ) -> GetTeams200Response:
+        """Get teams of user
 
 
-        :param folder_request: Infos to provide to get folders of team
-        :type folder_request: FolderRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,58 +74,55 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._folder_serialize(
-            folder_request=folder_request,
+        _param = self._get_teams_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Folder200Response",
+            '200': "GetTeams200Response",
+            '401': "GetLink401Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def folder_with_http_info(
+    def get_teams_with_http_info(
         self,
-        folder_request: Annotated[Optional[FolderRequest], Field(description="Infos to provide to get folders of team")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Folder200Response]:
-        """Get folders of team
+    ) -> ApiResponse[GetTeams200Response]:
+        """Get teams of user
 
 
-        :param folder_request: Infos to provide to get folders of team
-        :type folder_request: FolderRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -147,58 +137,55 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._folder_serialize(
-            folder_request=folder_request,
+        _param = self._get_teams_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Folder200Response",
+            '200': "GetTeams200Response",
+            '401': "GetLink401Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def folder_without_preload_content(
+    def get_teams_without_preload_content(
         self,
-        folder_request: Annotated[Optional[FolderRequest], Field(description="Infos to provide to get folders of team")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get folders of team
+        """Get teams of user
 
 
-        :param folder_request: Infos to provide to get folders of team
-        :type folder_request: FolderRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -213,35 +200,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._folder_serialize(
-            folder_request=folder_request,
+        _param = self._get_teams_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Folder200Response",
+            '200': "GetTeams200Response",
+            '401': "GetLink401Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _folder_serialize(
+    def _get_teams_serialize(
         self,
-        folder_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -257,47 +243,33 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if folder_request is not None:
-            _body_params = folder_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json'
+                'application/json', 
+                'application/problem+json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/folder',
+            resource_path='/teams',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `urlr-1.2.0/urlr/api/link_api.py` & `urlr-2.0.0/urlr/api/folders_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field
-from typing import Optional
+from pydantic import Field, StrictStr
 from typing_extensions import Annotated
-from urlr.models.reduce_link200_response import ReduceLink200Response
-from urlr.models.reduce_link_request import ReduceLinkRequest
+from urlr.models.get_folders200_response import GetFolders200Response
 
 from urlr.api_client import ApiClient, RequestSerialized
 from urlr.api_response import ApiResponse
 from urlr.rest import RESTResponseType
 
 
-class LinkApi:
+class FoldersApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def reduce_link(
+    def get_folders(
         self,
-        reduce_link_request: Annotated[Optional[ReduceLinkRequest], Field(description="Info of the link to shorten")] = None,
+        team_id: Annotated[StrictStr, Field(description="Team API ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ReduceLink200Response:
-        """Shorten a link
+    ) -> GetFolders200Response:
+        """Get folders of team
 
 
-        :param reduce_link_request: Info of the link to shorten
-        :type reduce_link_request: ReduceLinkRequest
+        :param team_id: Team API ID (required)
+        :type team_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,59 +79,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._reduce_link_serialize(
-            reduce_link_request=reduce_link_request,
+        _param = self._get_folders_serialize(
+            team_id=team_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ReduceLink200Response",
-            '400': "ReduceLink400Response",
+            '200': "GetFolders200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def reduce_link_with_http_info(
+    def get_folders_with_http_info(
         self,
-        reduce_link_request: Annotated[Optional[ReduceLinkRequest], Field(description="Info of the link to shorten")] = None,
+        team_id: Annotated[StrictStr, Field(description="Team API ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ReduceLink200Response]:
-        """Shorten a link
+    ) -> ApiResponse[GetFolders200Response]:
+        """Get folders of team
 
 
-        :param reduce_link_request: Info of the link to shorten
-        :type reduce_link_request: ReduceLinkRequest
+        :param team_id: Team API ID (required)
+        :type team_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -148,59 +148,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._reduce_link_serialize(
-            reduce_link_request=reduce_link_request,
+        _param = self._get_folders_serialize(
+            team_id=team_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ReduceLink200Response",
-            '400': "ReduceLink400Response",
+            '200': "GetFolders200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def reduce_link_without_preload_content(
+    def get_folders_without_preload_content(
         self,
-        reduce_link_request: Annotated[Optional[ReduceLinkRequest], Field(description="Info of the link to shorten")] = None,
+        team_id: Annotated[StrictStr, Field(description="Team API ID")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Shorten a link
+        """Get folders of team
 
 
-        :param reduce_link_request: Info of the link to shorten
-        :type reduce_link_request: ReduceLinkRequest
+        :param team_id: Team API ID (required)
+        :type team_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -215,36 +217,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._reduce_link_serialize(
-            reduce_link_request=reduce_link_request,
+        _param = self._get_folders_serialize(
+            team_id=team_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ReduceLink200Response",
-            '400': "ReduceLink400Response",
+            '200': "GetFolders200Response",
+            '404': "GetLink404Response",
+            '401': "GetLink401Response",
+            '422': "GetLink422Response",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _reduce_link_serialize(
+    def _get_folders_serialize(
         self,
-        reduce_link_request,
+        team_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -256,51 +260,39 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if team_id is not None:
+            _path_params['team_id'] = team_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if reduce_link_request is not None:
-            _body_params = reduce_link_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json'
+                'application/json', 
+                'application/problem+json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'bearerAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/reduce-link',
+            method='GET',
+            resource_path='/folders/{team_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `urlr-1.2.0/urlr/api_client.py` & `urlr-2.0.0/urlr/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.2.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `urlr-1.2.0/urlr/api_response.py` & `urlr-2.0.0/urlr/api_response.py`

 * *Files identical despite different names*

### Comparing `urlr-1.2.0/urlr/configuration.py` & `urlr-2.0.0/urlr/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -67,15 +67,15 @@
                  access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ) -> None:
         """Constructor
         """
-        self._base_path = "https://urlr.me/api" if host is None else host
+        self._base_path = "https://urlr.me/api/v1" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -375,26 +375,26 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.3\n"\
-               "SDK Package Version: 1.2.0".\
+               "Version of the API: 1.0\n"\
+               "SDK Package Version: 2.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://urlr.me/api",
+                'url': "https://urlr.me/api/v1",
                 'description': "Main API entry point",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `urlr-1.2.0/urlr/exceptions.py` & `urlr-2.0.0/urlr/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `urlr-1.2.0/urlr/models/authentification200_response.py` & `urlr-2.0.0/urlr/models/get_link422_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Authentification200Response(BaseModel):
+class GetLink422Response(BaseModel):
     """
-    Authentification200Response
+    GetLink422Response
     """ # noqa: E501
-    token: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["token"]
+    type: Optional[StrictStr] = None
+    title: Optional[StrictStr] = None
+    status: Optional[StrictInt] = None
+    detail: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "title", "status", "detail"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Authentification200Response from a JSON string"""
+        """Create an instance of GetLink422Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Authentification200Response from a dict"""
+        """Create an instance of GetLink422Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "token": obj.get("token")
+            "type": obj.get("type"),
+            "title": obj.get("title"),
+            "status": obj.get("status"),
+            "detail": obj.get("detail")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/authentification401_response.py` & `urlr-2.0.0/urlr/models/refresh_access_token401_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -19,17 +19,17 @@
 import json
 
 from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Authentification401Response(BaseModel):
+class RefreshAccessToken401Response(BaseModel):
     """
-    Authentification401Response
+    RefreshAccessToken401Response
     """ # noqa: E501
     code: Optional[StrictInt] = None
     message: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["code", "message"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Authentification401Response from a JSON string"""
+        """Create an instance of RefreshAccessToken401Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Authentification401Response from a dict"""
+        """Create an instance of RefreshAccessToken401Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `urlr-1.2.0/urlr/models/authentification_request.py` & `urlr-2.0.0/urlr/models/get_link404_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AuthentificationRequest(BaseModel):
+class GetLink404Response(BaseModel):
     """
-    AuthentificationRequest
+    GetLink404Response
     """ # noqa: E501
-    username: Optional[StrictStr] = Field(default=None, description="Email")
-    password: Optional[StrictStr] = Field(default=None, description="Password")
-    __properties: ClassVar[List[str]] = ["username", "password"]
+    type: Optional[StrictStr] = None
+    title: Optional[StrictStr] = None
+    status: Optional[StrictInt] = None
+    detail: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "title", "status", "detail"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AuthentificationRequest from a JSON string"""
+        """Create an instance of GetLink404Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AuthentificationRequest from a dict"""
+        """Create an instance of GetLink404Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "username": obj.get("username"),
-            "password": obj.get("password")
+            "type": obj.get("type"),
+            "title": obj.get("title"),
+            "status": obj.get("status"),
+            "detail": obj.get("detail")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/folder200_response.py` & `urlr-2.0.0/urlr/models/get_folders200_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from urlr.models.folder200_response_folders_inner import Folder200ResponseFoldersInner
+from urlr.models.get_folders200_response_folders_inner import GetFolders200ResponseFoldersInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Folder200Response(BaseModel):
+class GetFolders200Response(BaseModel):
     """
-    Folder200Response
+    GetFolders200Response
     """ # noqa: E501
-    folders: Optional[List[Folder200ResponseFoldersInner]] = None
+    folders: Optional[List[GetFolders200ResponseFoldersInner]] = None
     __properties: ClassVar[List[str]] = ["folders"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Folder200Response from a JSON string"""
+        """Create an instance of GetFolders200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,20 +77,20 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['folders'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Folder200Response from a dict"""
+        """Create an instance of GetFolders200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "folders": [Folder200ResponseFoldersInner.from_dict(_item) for _item in obj["folders"]] if obj.get("folders") is not None else None
+            "folders": [GetFolders200ResponseFoldersInner.from_dict(_item) for _item in obj["folders"]] if obj.get("folders") is not None else None
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/folder200_response_folders_inner.py` & `urlr-2.0.0/urlr/models/get_folders200_response_folders_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Folder200ResponseFoldersInner(BaseModel):
+class GetFolders200ResponseFoldersInner(BaseModel):
     """
-    Folder200ResponseFoldersInner
+    GetFolders200ResponseFoldersInner
     """ # noqa: E501
-    id: Optional[StrictInt] = Field(default=None, description="Folder ID")
+    id: Optional[StrictStr] = Field(default=None, description="Folder API ID")
     name: Optional[StrictStr] = Field(default=None, description="Folder name")
     __properties: ClassVar[List[str]] = ["id", "name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Folder200ResponseFoldersInner from a JSON string"""
+        """Create an instance of GetFolders200ResponseFoldersInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,15 +70,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Folder200ResponseFoldersInner from a dict"""
+        """Create an instance of GetFolders200ResponseFoldersInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `urlr-1.2.0/urlr/models/folder_request.py` & `urlr-2.0.0/urlr/models/create_access_token401_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FolderRequest(BaseModel):
+class CreateAccessToken401Response(BaseModel):
     """
-    FolderRequest
+    CreateAccessToken401Response
     """ # noqa: E501
-    team: StrictInt = Field(description="Team ID (displayed on dashboard)")
-    __properties: ClassVar[List[str]] = ["team"]
+    code: Optional[StrictInt] = None
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["code", "message"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FolderRequest from a JSON string"""
+        """Create an instance of CreateAccessToken401Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FolderRequest from a dict"""
+        """Create an instance of CreateAccessToken401Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "team": obj.get("team")
+            "code": obj.get("code"),
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/reduce_link200_response.py` & `urlr-2.0.0/urlr/models/get_link401_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ReduceLink200Response(BaseModel):
+class GetLink401Response(BaseModel):
     """
-    ReduceLink200Response
+    GetLink401Response
     """ # noqa: E501
-    url: Optional[StrictStr] = Field(default=None, description="Original URL")
-    expired_at: Optional[StrictStr] = Field(default=None, description="Expiration date")
-    team: Optional[StrictInt] = Field(default=None, description="Team ID (displayed on dashboard)")
-    folder: Optional[StrictInt] = Field(default=None, description="Folder ID (displayed on dashboard)")
-    url_code: Optional[StrictStr] = Field(default=None, description="Short code")
-    domain: Optional[StrictStr] = Field(default=None, description="Domain")
-    code: Optional[StrictInt] = Field(default=None, description="HTTP status code")
-    __properties: ClassVar[List[str]] = ["url", "expired_at", "team", "folder", "url_code", "domain", "code"]
+    type: Optional[StrictStr] = None
+    title: Optional[StrictStr] = None
+    status: Optional[StrictInt] = None
+    detail: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "title", "status", "detail"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -50,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ReduceLink200Response from a JSON string"""
+        """Create an instance of GetLink401Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,26 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ReduceLink200Response from a dict"""
+        """Create an instance of GetLink401Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "url": obj.get("url"),
-            "expired_at": obj.get("expired_at"),
-            "team": obj.get("team"),
-            "folder": obj.get("folder"),
-            "url_code": obj.get("url_code"),
-            "domain": obj.get("domain"),
-            "code": obj.get("code")
+            "type": obj.get("type"),
+            "title": obj.get("title"),
+            "status": obj.get("status"),
+            "detail": obj.get("detail")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/reduce_link400_response.py` & `urlr-2.0.0/urlr/models/get_link200_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ReduceLink400Response(BaseModel):
+class GetLink200Response(BaseModel):
     """
-    ReduceLink400Response
+    GetLink200Response
     """ # noqa: E501
-    code: Optional[StrictInt] = Field(default=None, description="HTTP status code")
-    error: Optional[StrictInt] = Field(default=None, description="Error code")
-    message: Optional[StrictStr] = Field(default=None, description="Message describing the error")
-    __properties: ClassVar[List[str]] = ["code", "error", "message"]
+    id: Optional[StrictStr] = Field(default=None, description="Link API ID")
+    __properties: ClassVar[List[str]] = ["id"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -46,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ReduceLink400Response from a JSON string"""
+        """Create an instance of GetLink200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,22 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ReduceLink400Response from a dict"""
+        """Create an instance of GetLink200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "code": obj.get("code"),
-            "error": obj.get("error"),
-            "message": obj.get("message")
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/reduce_link_request.py` & `urlr-2.0.0/urlr/models/get_statistics_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,42 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ReduceLinkRequest(BaseModel):
+class GetStatisticsRequest(BaseModel):
     """
-    ReduceLinkRequest
+    GetStatisticsRequest
     """ # noqa: E501
-    url: StrictStr = Field(description="URL to shorten")
-    team: StrictStr = Field(description="Team ID (displayed on dashboard)")
-    folder: Optional[StrictStr] = Field(default=None, description="Folder ID (displayed on dashboard)")
-    code: Optional[Annotated[str, Field(strict=True)]] = Field(default=None, description="Custom short code")
-    label: Optional[StrictStr] = Field(default=None, description="Label")
-    password: Optional[StrictStr] = Field(default=None, description="Password")
-    expired_at: Optional[StrictStr] = Field(default=None, description="Expiration date")
-    __properties: ClassVar[List[str]] = ["url", "team", "folder", "code", "label", "password", "expired_at"]
-
-    @field_validator('code')
-    def code_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if value is None:
-            return value
-
-        if not re.match(r"^[a-zA-Z0-9!-]{3,50}$", value):
-            raise ValueError(r"must validate the regular expression /^[a-zA-Z0-9!-]{3,50}$/")
-        return value
+    link_id: Optional[StrictStr] = Field(default=None, description="Link API ID")
+    var_from: Optional[datetime] = Field(default=None, description="Get stats from this date", alias="from")
+    to: Optional[datetime] = Field(default=None, description="Get stats until this date")
+    include_bots: Optional[StrictBool] = Field(default=False, description="Whether include bots or not in statistics")
+    __properties: ClassVar[List[str]] = ["link_id", "from", "to", "include_bots"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -61,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ReduceLinkRequest from a JSON string"""
+        """Create an instance of GetStatisticsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -86,26 +73,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ReduceLinkRequest from a dict"""
+        """Create an instance of GetStatisticsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "url": obj.get("url"),
-            "team": obj.get("team"),
-            "folder": obj.get("folder"),
-            "code": obj.get("code"),
-            "label": obj.get("label"),
-            "password": obj.get("password"),
-            "expired_at": obj.get("expired_at")
+            "link_id": obj.get("link_id"),
+            "from": obj.get("from"),
+            "to": obj.get("to"),
+            "include_bots": obj.get("include_bots") if obj.get("include_bots") is not None else False
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/stats200_response.py` & `urlr-2.0.0/urlr/models/get_statistics200_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Stats200Response(BaseModel):
+class GetStatistics200Response(BaseModel):
     """
-    Stats200Response
+    GetStatistics200Response
     """ # noqa: E501
+    link_id: Optional[StrictStr] = Field(default=None, description="Link API ID")
     clicks: Optional[StrictInt] = Field(default=None, description="Clicks")
-    unique_clicks: Optional[StrictInt] = Field(default=None, description="Unique clicks", alias="uniqueClicks")
-    __properties: ClassVar[List[str]] = ["clicks", "uniqueClicks"]
+    unique_clicks: Optional[StrictInt] = Field(default=None, description="Unique clicks")
+    __properties: ClassVar[List[str]] = ["link_id", "clicks", "unique_clicks"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Stats200Response from a JSON string"""
+        """Create an instance of GetStatistics200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +71,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Stats200Response from a dict"""
+        """Create an instance of GetStatistics200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "link_id": obj.get("link_id"),
             "clicks": obj.get("clicks"),
-            "uniqueClicks": obj.get("uniqueClicks")
+            "unique_clicks": obj.get("unique_clicks")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/stats400_response.py` & `urlr-2.0.0/urlr/models/get_teams200_response_teams_inner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Stats400Response(BaseModel):
+class GetTeams200ResponseTeamsInner(BaseModel):
     """
-    Stats400Response
+    GetTeams200ResponseTeamsInner
     """ # noqa: E501
-    code: Optional[StrictInt] = None
-    error: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["code", "error"]
+    id: Optional[StrictStr] = Field(default=None, description="Team API ID")
+    name: Optional[StrictStr] = Field(default=None, description="Team name")
+    __properties: ClassVar[List[str]] = ["id", "name"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Stats400Response from a JSON string"""
+        """Create an instance of GetTeams200ResponseTeamsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Stats400Response from a dict"""
+        """Create an instance of GetTeams200ResponseTeamsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "code": obj.get("code"),
-            "error": obj.get("error")
+            "id": obj.get("id"),
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/team200_response.py` & `urlr-2.0.0/urlr/models/get_teams200_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from urlr.models.team200_response_teams_inner import Team200ResponseTeamsInner
+from urlr.models.get_teams200_response_teams_inner import GetTeams200ResponseTeamsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Team200Response(BaseModel):
+class GetTeams200Response(BaseModel):
     """
-    Team200Response
+    GetTeams200Response
     """ # noqa: E501
-    teams: Optional[List[Team200ResponseTeamsInner]] = None
+    teams: Optional[List[GetTeams200ResponseTeamsInner]] = None
     __properties: ClassVar[List[str]] = ["teams"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Team200Response from a JSON string"""
+        """Create an instance of GetTeams200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,20 +77,20 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['teams'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Team200Response from a dict"""
+        """Create an instance of GetTeams200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "teams": [Team200ResponseTeamsInner.from_dict(_item) for _item in obj["teams"]] if obj.get("teams") is not None else None
+            "teams": [GetTeams200ResponseTeamsInner.from_dict(_item) for _item in obj["teams"]] if obj.get("teams") is not None else None
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/models/team200_response_teams_inner.py` & `urlr-2.0.0/urlr/models/create_access_token200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Team200ResponseTeamsInner(BaseModel):
+class CreateAccessToken200Response(BaseModel):
     """
-    Team200ResponseTeamsInner
+    CreateAccessToken200Response
     """ # noqa: E501
-    id: Optional[StrictInt] = Field(default=None, description="Team ID")
-    name: Optional[StrictStr] = Field(default=None, description="Team name")
-    __properties: ClassVar[List[str]] = ["id", "name"]
+    token: Optional[StrictStr] = Field(default=None, description="Access token (JWT) valid for 1 hour")
+    refresh_token: Optional[StrictStr] = Field(default=None, description="Refresh token valid for 1 month")
+    __properties: ClassVar[List[str]] = ["token", "refresh_token"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Team200ResponseTeamsInner from a JSON string"""
+        """Create an instance of CreateAccessToken200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Team200ResponseTeamsInner from a dict"""
+        """Create an instance of CreateAccessToken200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name")
+            "token": obj.get("token"),
+            "refresh_token": obj.get("refresh_token")
         })
         return _obj
```

### Comparing `urlr-1.2.0/urlr/rest.py` & `urlr-2.0.0/urlr/rest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
-    Developer API - URLR
+    URLR API Reference
 
-    API powering the features of URLR.
+    API powering the features of URLR.<br><br>Note that in order to facilitate integration, we provide SDKs for various languages at https://github.com/URLR.<br><br>Key API principles:<br>         <ul><li>All dates follow **ISO-8601** format</li><li>Most errors follow **RFC 9457** standard</li><li>All responses are delivered in English</li></ul>
 
-    The version of the OpenAPI document: 0.3
+    The version of the OpenAPI document: 1.0
     Contact: contact@urlr.me
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `urlr-1.2.0/urlr.egg-info/SOURCES.txt` & `urlr-2.0.0/urlr.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-test/test_authentification200_response.py
-test/test_authentification401_response.py
-test/test_authentification_api.py
-test/test_authentification_request.py
-test/test_folder200_response.py
-test/test_folder200_response_folders_inner.py
-test/test_folder_api.py
-test/test_folder_request.py
-test/test_link_api.py
-test/test_reduce_link200_response.py
-test/test_reduce_link400_response.py
-test/test_reduce_link_request.py
-test/test_stats200_response.py
-test/test_stats400_response.py
-test/test_stats_api.py
-test/test_stats_request.py
-test/test_team200_response.py
-test/test_team200_response_teams_inner.py
-test/test_team_api.py
+test/test_access_tokens_api.py
+test/test_create_access_token200_response.py
+test/test_create_access_token401_response.py
+test/test_create_access_token_request.py
+test/test_create_link201_response.py
+test/test_create_link429_response.py
+test/test_create_link500_response.py
+test/test_create_link_request.py
+test/test_folders_api.py
+test/test_get_folders200_response.py
+test/test_get_folders200_response_folders_inner.py
+test/test_get_link200_response.py
+test/test_get_link401_response.py
+test/test_get_link404_response.py
+test/test_get_link422_response.py
+test/test_get_statistics200_response.py
+test/test_get_statistics_request.py
+test/test_get_teams200_response.py
+test/test_get_teams200_response_teams_inner.py
+test/test_links_api.py
+test/test_refresh_access_token401_response.py
+test/test_refresh_access_token_request.py
+test/test_statistics_api.py
+test/test_teams_api.py
 urlr/__init__.py
 urlr/api_client.py
 urlr/api_response.py
 urlr/configuration.py
 urlr/exceptions.py
 urlr/py.typed
 urlr/rest.py
 urlr.egg-info/PKG-INFO
 urlr.egg-info/SOURCES.txt
 urlr.egg-info/dependency_links.txt
 urlr.egg-info/requires.txt
 urlr.egg-info/top_level.txt
 urlr/api/__init__.py
-urlr/api/authentification_api.py
-urlr/api/folder_api.py
-urlr/api/link_api.py
-urlr/api/stats_api.py
-urlr/api/team_api.py
+urlr/api/access_tokens_api.py
+urlr/api/folders_api.py
+urlr/api/links_api.py
+urlr/api/statistics_api.py
+urlr/api/teams_api.py
 urlr/models/__init__.py
-urlr/models/authentification200_response.py
-urlr/models/authentification401_response.py
-urlr/models/authentification_request.py
-urlr/models/folder200_response.py
-urlr/models/folder200_response_folders_inner.py
-urlr/models/folder_request.py
-urlr/models/reduce_link200_response.py
-urlr/models/reduce_link400_response.py
-urlr/models/reduce_link_request.py
-urlr/models/stats200_response.py
-urlr/models/stats400_response.py
-urlr/models/stats_request.py
-urlr/models/team200_response.py
-urlr/models/team200_response_teams_inner.py
+urlr/models/create_access_token200_response.py
+urlr/models/create_access_token401_response.py
+urlr/models/create_access_token_request.py
+urlr/models/create_link201_response.py
+urlr/models/create_link429_response.py
+urlr/models/create_link500_response.py
+urlr/models/create_link_request.py
+urlr/models/get_folders200_response.py
+urlr/models/get_folders200_response_folders_inner.py
+urlr/models/get_link200_response.py
+urlr/models/get_link401_response.py
+urlr/models/get_link404_response.py
+urlr/models/get_link422_response.py
+urlr/models/get_statistics200_response.py
+urlr/models/get_statistics_request.py
+urlr/models/get_teams200_response.py
+urlr/models/get_teams200_response_teams_inner.py
+urlr/models/refresh_access_token401_response.py
+urlr/models/refresh_access_token_request.py
```

