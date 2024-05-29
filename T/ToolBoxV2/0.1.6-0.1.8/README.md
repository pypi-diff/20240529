# Comparing `tmp/ToolBoxV2-0.1.6.tar.gz` & `tmp/ToolBoxV2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolBoxV2-0.1.6.tar", last modified: Tue Jan 16 16:04:35 2024, max compression
+gzip compressed data, was "ToolBoxV2-0.1.8.tar", last modified: Tue Mar  5 23:57:07 2024, max compression
```

## Comparing `ToolBoxV2-0.1.6.tar` & `ToolBoxV2-0.1.8.tar`

### file list

```diff
@@ -1,82 +1,147 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.601470 ToolBoxV2-0.1.6/
--rw-rw-rw-   0        0        0      180 2023-05-04 20:04:21.000000 ToolBoxV2-0.1.6/AUTHORS.rst
--rw-rw-rw-   0        0        0      604 2023-05-04 20:04:21.000000 ToolBoxV2-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      158 2023-11-09 20:57:05.000000 ToolBoxV2-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5387 2024-01-16 16:04:35.601470 ToolBoxV2-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3824 2023-10-04 18:48:54.000000 ToolBoxV2-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.600470 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/
--rw-rw-rw-   0        0        0     5387 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2006 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      344 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-11-11 16:08:14.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      343 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-16 16:04:35.000000 ToolBoxV2-0.1.6/ToolBoxV2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      364 2024-01-12 00:28:15.000000 ToolBoxV2-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0      417 2024-01-16 16:04:35.603470 ToolBoxV2-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2170 2023-12-08 10:46:29.000000 ToolBoxV2-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.473215 ToolBoxV2-0.1.6/toolboxv2/
--rw-rw-rw-   0        0        0     1101 2024-01-15 23:31:54.000000 ToolBoxV2-0.1.6/toolboxv2/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.488217 ToolBoxV2-0.1.6/toolboxv2/api/
--rw-rw-rw-   0        0        0        0 2023-08-08 14:24:26.000000 ToolBoxV2-0.1.6/toolboxv2/api/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-01-16 13:05:13.000000 ToolBoxV2-0.1.6/toolboxv2/api/fast_api.py
--rw-rw-rw-   0        0        0     5859 2024-01-11 22:54:39.000000 ToolBoxV2-0.1.6/toolboxv2/api/fast_api_install.py
--rw-rw-rw-   0        0        0     7547 2024-01-16 13:05:13.000000 ToolBoxV2-0.1.6/toolboxv2/api/fast_api_main.py
--rw-rw-rw-   0        0        0     3765 2023-11-30 22:21:29.000000 ToolBoxV2-0.1.6/toolboxv2/api/fast_app.py
--rw-rw-rw-   0        0        0      126 2023-08-08 15:41:31.000000 ToolBoxV2-0.1.6/toolboxv2/api/util.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.493216 ToolBoxV2-0.1.6/toolboxv2/app/
--rw-rw-rw-   0        0        0        0 2023-08-08 15:41:31.000000 ToolBoxV2-0.1.6/toolboxv2/app/__init__.py
--rw-rw-rw-   0        0        0     1036 2023-08-20 11:34:14.000000 ToolBoxV2-0.1.6/toolboxv2/app/serveapp.py
--rw-rw-rw-   0        0        0    18534 2024-01-16 15:33:43.000000 ToolBoxV2-0.1.6/toolboxv2/cli.py
--rw-rw-rw-   0        0        0     1347 2023-11-09 21:17:09.000000 ToolBoxV2-0.1.6/toolboxv2/init.config
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.506215 ToolBoxV2-0.1.6/toolboxv2/mods/
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.527216 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/
--rw-rw-rw-   0        0        0    25690 2024-01-16 11:02:14.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/AuthManager.py
--rw-rw-rw-   0        0        0     5618 2024-01-16 00:11:17.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/ModManager.py
--rw-rw-rw-   0        0        0     9162 2024-01-16 14:37:26.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/UserInstances.py
--rw-rw-rw-   0        0        0      180 2024-01-16 11:49:53.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/__init__.py
--rw-rw-rw-   0        0        0     7805 2024-01-16 00:24:00.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/extras.py
--rw-rw-rw-   0        0        0     9295 2024-01-16 11:49:53.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/module.py
--rw-rw-rw-   0        0        0      625 2024-01-16 00:11:17.000000 ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/settings_manager.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.535216 ToolBoxV2-0.1.6/toolboxv2/mods/DB/
--rw-rw-rw-   0        0        0      252 2024-01-12 18:40:33.000000 ToolBoxV2-0.1.6/toolboxv2/mods/DB/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-01-16 14:44:20.000000 ToolBoxV2-0.1.6/toolboxv2/mods/DB/local_instance.py
--rw-rw-rw-   0        0        0     4161 2024-01-16 13:43:00.000000 ToolBoxV2-0.1.6/toolboxv2/mods/DB/reddis_instance.py
--rw-rw-rw-   0        0        0    12464 2024-01-16 14:42:08.000000 ToolBoxV2-0.1.6/toolboxv2/mods/DB/tb_adapter.py
--rw-rw-rw-   0        0        0      722 2024-01-13 15:49:00.000000 ToolBoxV2-0.1.6/toolboxv2/mods/DB/types.py
--rw-rw-rw-   0        0        0    15472 2024-01-16 15:44:06.000000 ToolBoxV2-0.1.6/toolboxv2/mods/SocketManager.py
--rw-rw-rw-   0        0        0    25062 2024-01-16 15:23:49.000000 ToolBoxV2-0.1.6/toolboxv2/mods/WebSocketManager.py
--rw-rw-rw-   0        0        0       78 2023-12-13 11:25:28.000000 ToolBoxV2-0.1.6/toolboxv2/mods/__init__.py
--rw-rw-rw-   0        0        0     6552 2024-01-16 15:41:07.000000 ToolBoxV2-0.1.6/toolboxv2/mods/api_manager.py
--rw-rw-rw-   0        0        0    12009 2024-01-16 00:33:56.000000 ToolBoxV2-0.1.6/toolboxv2/mods/cli_functions.py
--rw-rw-rw-   0        0        0     7235 2024-01-16 15:49:13.000000 ToolBoxV2-0.1.6/toolboxv2/mods/dockerEnv.py
--rw-rw-rw-   0        0        0     1817 2024-01-16 11:49:53.000000 ToolBoxV2-0.1.6/toolboxv2/mods/email_wating_list.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.550217 ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/
--rw-rw-rw-   0        0        0      883 2024-01-15 19:22:25.000000 ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/Interface.py
--rw-rw-rw-   0        0        0      246 2024-01-15 12:43:20.000000 ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/__init__.py
--rw-rw-rw-   0        0        0     7342 2024-01-16 00:04:21.000000 ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/quickNote.py
--rw-rw-rw-   0        0        0     4646 2024-01-15 20:51:22.000000 ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/types.py
--rw-rw-rw-   0        0        0    55879 2024-01-16 11:21:36.000000 ToolBoxV2-0.1.6/toolboxv2/mods/welcome.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.550217 ToolBoxV2-0.1.6/toolboxv2/mods_dev/
--rw-rw-rw-   0        0        0        0 2023-12-09 13:19:17.000000 ToolBoxV2-0.1.6/toolboxv2/mods_dev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.573469 ToolBoxV2-0.1.6/toolboxv2/runabel/
--rw-rw-rw-   0        0        0     1390 2024-01-16 00:33:56.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/__init__.py
--rw-rw-rw-   0        0        0     4242 2023-11-15 22:15:09.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/as_docker.py
--rw-rw-rw-   0        0        0     3968 2023-12-13 10:56:32.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/demon.py
--rw-rw-rw-   0        0        0     7994 2024-01-16 10:50:32.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/minicli.py
--rw-rw-rw-   0        0        0    11777 2024-01-15 22:26:46.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/qncli.py
--rw-rw-rw-   0        0        0    12379 2024-01-16 10:50:32.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/readchar_buldin_style_cli.py
--rw-rw-rw-   0        0        0      130 2024-01-11 23:29:04.000000 ToolBoxV2-0.1.6/toolboxv2/runabel/run_api_helper.py
-drwxrwxrwx   0        0        0        0 2024-01-16 16:04:35.599470 ToolBoxV2-0.1.6/toolboxv2/utils/
--rw-rw-rw-   0        0        0    12084 2023-08-16 23:15:08.000000 ToolBoxV2-0.1.6/toolboxv2/utils/Style.py
--rw-rw-rw-   0        0        0    17822 2023-09-20 00:40:56.000000 ToolBoxV2-0.1.6/toolboxv2/utils/TBConfig.py
--rw-rw-rw-   0        0        0      428 2023-12-14 21:42:34.000000 ToolBoxV2-0.1.6/toolboxv2/utils/__init__.py
--rw-rw-rw-   0        0        0     5524 2024-01-16 10:56:55.000000 ToolBoxV2-0.1.6/toolboxv2/utils/all_functions_enums.py
--rw-rw-rw-   0        0        0    10821 2024-01-11 21:32:53.000000 ToolBoxV2-0.1.6/toolboxv2/utils/cryp.py
--rw-rw-rw-   0        0        0    10272 2024-01-16 13:40:21.000000 ToolBoxV2-0.1.6/toolboxv2/utils/file_handler.py
--rw-rw-rw-   0        0        0     2282 2024-01-16 13:05:13.000000 ToolBoxV2-0.1.6/toolboxv2/utils/helper_functions.py
--rw-rw-rw-   0        0        0     3172 2024-01-16 11:22:49.000000 ToolBoxV2-0.1.6/toolboxv2/utils/main_tool.py
--rw-rw-rw-   0        0        0     5055 2023-12-13 21:03:52.000000 ToolBoxV2-0.1.6/toolboxv2/utils/state_system.py
--rw-rw-rw-   0        0        0     6061 2024-01-16 13:36:34.000000 ToolBoxV2-0.1.6/toolboxv2/utils/tb_logger.py
--rw-rw-rw-   0        0        0    52990 2024-01-16 14:37:26.000000 ToolBoxV2-0.1.6/toolboxv2/utils/toolbox.py
--rw-rw-rw-   0        0        0     8711 2024-01-13 15:49:00.000000 ToolBoxV2-0.1.6/toolboxv2/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.698763 ToolBoxV2-0.1.8/
+-rw-rw-rw-   0        0        0      180 2023-05-04 20:04:21.000000 ToolBoxV2-0.1.8/AUTHORS.rst
+-rw-rw-rw-   0        0        0      604 2023-05-04 20:04:21.000000 ToolBoxV2-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      158 2023-11-09 20:57:05.000000 ToolBoxV2-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5553 2024-03-05 23:57:07.698763 ToolBoxV2-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2023-10-04 18:48:54.000000 ToolBoxV2-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.697764 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4044 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      430 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-11-11 16:08:14.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      429 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-05 23:57:07.000000 ToolBoxV2-0.1.8/ToolBoxV2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      455 2024-03-05 23:53:03.000000 ToolBoxV2-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0      417 2024-03-05 23:57:07.701763 ToolBoxV2-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2170 2024-03-05 23:52:06.000000 ToolBoxV2-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.359937 ToolBoxV2-0.1.8/toolboxv2/
+-rw-rw-rw-   0        0        0     1095 2024-03-05 23:52:06.000000 ToolBoxV2-0.1.8/toolboxv2/__init__.py
+-rw-rw-rw-   0        0        0       92 2024-03-05 11:38:40.000000 ToolBoxV2-0.1.8/toolboxv2/__main__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.377582 ToolBoxV2-0.1.8/toolboxv2/api/
+-rw-rw-rw-   0        0        0        0 2023-08-08 14:24:26.000000 ToolBoxV2-0.1.8/toolboxv2/api/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-02-11 02:46:38.000000 ToolBoxV2-0.1.8/toolboxv2/api/fast_api.py
+-rw-rw-rw-   0        0        0     5859 2024-01-11 22:54:39.000000 ToolBoxV2-0.1.8/toolboxv2/api/fast_api_install.py
+-rw-rw-rw-   0        0        0    26859 2024-02-13 12:59:19.000000 ToolBoxV2-0.1.8/toolboxv2/api/fast_api_main.py
+-rw-rw-rw-   0        0        0     3241 2024-02-11 15:52:56.000000 ToolBoxV2-0.1.8/toolboxv2/api/fast_app.py
+-rw-rw-rw-   0        0        0      126 2023-08-08 15:41:31.000000 ToolBoxV2-0.1.8/toolboxv2/api/util.py
+-rw-rw-rw-   0        0        0    23059 2024-03-05 23:06:51.000000 ToolBoxV2-0.1.8/toolboxv2/cli.py
+-rw-rw-rw-   0        0        0     1347 2023-11-09 21:17:09.000000 ToolBoxV2-0.1.8/toolboxv2/init.config
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.418160 ToolBoxV2-0.1.8/toolboxv2/mods/
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.453692 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/
+-rw-rw-rw-   0        0        0    32145 2024-02-27 12:56:47.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/AuthManager.py
+-rw-rw-rw-   0        0        0     5807 2024-02-29 17:30:18.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/ModManager.py
+-rw-rw-rw-   0        0        0     7202 2024-01-31 14:10:34.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/UserInstances.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 23:39:16.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/__init__.py
+-rw-rw-rw-   0        0        0     7389 2024-03-05 23:52:06.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/extras.py
+-rw-rw-rw-   0        0        0     9318 2024-02-26 17:28:42.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/module.py
+-rw-rw-rw-   0        0        0      625 2024-01-16 00:11:17.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/settings_manager.py
+-rw-rw-rw-   0        0        0     1285 2024-02-27 12:56:47.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/types.py
+-rw-rw-rw-   0        0        0     1238 2024-02-15 04:14:00.000000 ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/widgetInsights.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.474727 ToolBoxV2-0.1.8/toolboxv2/mods/DB/
+-rw-rw-rw-   0        0        0      252 2024-01-16 17:23:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DB/__init__.py
+-rw-rw-rw-   0        0        0     4843 2024-02-11 16:58:27.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DB/local_instance.py
+-rw-rw-rw-   0        0        0     4992 2024-02-11 16:41:36.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DB/reddis_instance.py
+-rw-rw-rw-   0        0        0    13354 2024-01-31 18:54:59.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DB/tb_adapter.py
+-rw-rw-rw-   0        0        0      722 2024-01-13 15:49:00.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DB/types.py
+-rw-rw-rw-   0        0        0     5841 2024-02-11 15:40:28.000000 ToolBoxV2-0.1.8/toolboxv2/mods/DashProvider.py
+-rw-rw-rw-   0        0        0     6106 2024-02-11 16:47:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/MinimalHtml.py
+-rw-rw-rw-   0        0        0    34972 2024-03-05 16:58:40.000000 ToolBoxV2-0.1.8/toolboxv2/mods/SocketManager.py
+-rw-rw-rw-   0        0        0    21894 2024-03-04 15:11:23.000000 ToolBoxV2-0.1.8/toolboxv2/mods/WebSocketManager.py
+-rw-rw-rw-   0        0        0       78 2023-12-13 11:25:28.000000 ToolBoxV2-0.1.8/toolboxv2/mods/__init__.py
+-rw-rw-rw-   0        0        0     6909 2024-03-04 15:11:23.000000 ToolBoxV2-0.1.8/toolboxv2/mods/api_manager.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.480722 ToolBoxV2-0.1.8/toolboxv2/mods/audio/
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.481724 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2STT/
+-rw-rw-rw-   0        0        0        0 2024-02-20 22:09:28.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2STT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.481724 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2STT/transcription/
+-rw-rw-rw-   0        0        0        0 2024-02-20 22:04:48.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2STT/transcription/__init__.py
+-rw-rw-rw-   0        0        0    14829 2024-03-05 11:44:42.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2STT/transcription/liveTranscriptHfOpenai.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.491230 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/
+-rw-rw-rw-   0        0        0        0 2024-02-20 22:08:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.501740 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/audioProvider/
+-rw-rw-rw-   0        0        0     5506 2024-02-21 12:56:57.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/audioProvider/ElevenLapsProviderPy.py
+-rw-rw-rw-   0        0        0    10775 2024-03-04 15:11:23.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/audioProvider/PiperProviderPy.py
+-rw-rw-rw-   0        0        0        0 2024-02-20 22:02:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/audioProvider/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-02-20 22:42:01.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/mini.py
+-rw-rw-rw-   0        0        0     2104 2024-02-21 12:59:20.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/TBV2TTS/util.py
+-rw-rw-rw-   0        0        0      164 2024-02-25 13:21:09.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/__init__.py
+-rw-rw-rw-   0        0        0     7365 2024-03-05 14:01:08.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/pyAudio.py
+-rw-rw-rw-   0        0        0     1432 2024-02-21 00:53:30.000000 ToolBoxV2-0.1.8/toolboxv2/mods/audio/utils.py
+-rw-rw-rw-   0        0        0    13404 2024-03-05 16:43:58.000000 ToolBoxV2-0.1.8/toolboxv2/mods/cli_functions.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.505247 ToolBoxV2-0.1.8/toolboxv2/mods/diffuser/
+-rw-rw-rw-   0        0        0      170 2024-03-05 22:24:10.000000 ToolBoxV2-0.1.8/toolboxv2/mods/diffuser/__init__.py
+-rw-rw-rw-   0        0        0    29678 2024-03-05 21:14:27.000000 ToolBoxV2-0.1.8/toolboxv2/mods/diffuser/content_gen.py
+-rw-rw-rw-   0        0        0     1017 2024-03-05 22:16:05.000000 ToolBoxV2-0.1.8/toolboxv2/mods/diffuser/manager.py
+-rw-rw-rw-   0        0        0     7502 2024-03-05 21:56:04.000000 ToolBoxV2-0.1.8/toolboxv2/mods/diffuser/st_runner.py
+-rw-rw-rw-   0        0        0     7324 2024-01-16 23:24:38.000000 ToolBoxV2-0.1.8/toolboxv2/mods/dockerEnv.py
+-rw-rw-rw-   0        0        0     4132 2024-02-11 16:48:56.000000 ToolBoxV2-0.1.8/toolboxv2/mods/email_waiting_list.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.537724 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/
+-rw-rw-rw-   0        0        0    16416 2024-03-03 20:50:56.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/AgentFramwork.py
+-rw-rw-rw-   0        0        0    69118 2024-03-05 12:02:01.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/AgentUtils.py
+-rw-rw-rw-   0        0        0    76167 2024-03-04 13:09:45.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/Agents.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.543226 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/
+-rw-rw-rw-   0        0        0        0 2024-02-28 19:04:40.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.543226 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/docs_generator/
+-rw-rw-rw-   0        0        0        0 2024-02-28 19:05:33.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/docs_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.544230 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/docs_retrever/
+-rw-rw-rw-   0        0        0        0 2024-02-28 19:05:23.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/docs_retrever/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.544230 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/evaluation/
+-rw-rw-rw-   0        0        0        0 2024-02-28 19:05:55.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/evaluation/__init__.py
+-rw-rw-rw-   0        0        0    21494 2024-03-03 20:18:28.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/CodingAgent/runner.py
+-rw-rw-rw-   0        0        0       74 2024-02-14 19:28:31.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/__init__.py
+-rw-rw-rw-   0        0        0    56705 2024-03-05 11:44:42.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/isaa_modi.py
+-rw-rw-rw-   0        0        0    97462 2024-03-05 11:44:42.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/module.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.571347 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/
+-rw-rw-rw-   0        0        0      163 2024-02-18 13:19:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/__init__.py
+-rw-rw-rw-   0        0        0      770 2024-02-18 14:01:43.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/audo_to_text_assemblyai.py
+-rw-rw-rw-   0        0        0     4806 2024-02-29 17:53:44.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/file_loder.py
+-rw-rw-rw-   0        0        0      437 2024-02-25 13:37:49.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/open_weather_map.py
+-rw-rw-rw-   0        0        0     4595 2024-02-29 17:53:44.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/web_loder.py
+-rw-rw-rw-   0        0        0     1578 2024-02-18 12:49:40.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/subtools/youtube_audio.py
+-rw-rw-rw-   0        0        0     1275 2024-02-26 17:28:42.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/tests.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.574865 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/text_analysis/
+-rw-rw-rw-   0        0        0        0 2024-02-26 19:11:11.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/text_analysis/__init__.py
+-rw-rw-rw-   0        0        0      482 2024-02-26 19:54:09.000000 ToolBoxV2-0.1.8/toolboxv2/mods/isaa/text_analysis/summarize.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.591370 ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/
+-rw-rw-rw-   0        0        0      883 2024-01-15 19:22:25.000000 ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/Interface.py
+-rw-rw-rw-   0        0        0      246 2024-01-15 12:43:20.000000 ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/__init__.py
+-rw-rw-rw-   0        0        0     7363 2024-01-16 17:43:53.000000 ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/quickNote.py
+-rw-rw-rw-   0        0        0     4704 2024-01-16 17:43:53.000000 ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/types.py
+-rw-rw-rw-   0        0        0    55879 2024-02-11 15:40:28.000000 ToolBoxV2-0.1.8/toolboxv2/mods/welcome.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.591370 ToolBoxV2-0.1.8/toolboxv2/mods_dev/
+-rw-rw-rw-   0        0        0        0 2023-12-09 13:19:17.000000 ToolBoxV2-0.1.8/toolboxv2/mods_dev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.643437 ToolBoxV2-0.1.8/toolboxv2/runabel/
+-rw-rw-rw-   0        0        0     1472 2024-02-25 15:08:27.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/__init__.py
+-rw-rw-rw-   0        0        0     4153 2024-03-04 18:14:20.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/as_docker.py
+-rw-rw-rw-   0        0        0       82 2024-03-04 22:17:51.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/bg.py
+-rw-rw-rw-   0        0        0     4058 2024-03-04 18:14:08.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/demon.py
+-rw-rw-rw-   0        0        0     1164 2024-03-05 22:16:05.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/diffuserUI.py
+-rw-rw-rw-   0        0        0     9205 2024-03-04 18:13:56.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/install_piper_models.py
+-rw-rw-rw-   0        0        0        0 2024-02-24 23:43:25.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/isaaDexpore.py
+-rw-rw-rw-   0        0        0     2538 2024-03-04 18:13:56.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/isaa_retreval.py
+-rw-rw-rw-   0        0        0     2950 2024-03-04 18:13:56.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/isaa_retrevalwmd.py
+-rw-rw-rw-   0        0        0    17642 2024-03-04 18:12:55.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/isaacli.py
+-rw-rw-rw-   0        0        0     7397 2024-03-04 18:20:24.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/isaaclip2.py
+-rw-rw-rw-   0        0        0     8665 2024-03-05 23:01:55.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/minicli.py
+-rw-rw-rw-   0        0        0    11811 2024-03-04 18:12:55.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/qncli.py
+-rw-rw-rw-   0        0        0    12334 2024-03-04 18:12:55.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/readchar_buldin_style_cli.py
+-rw-rw-rw-   0        0        0      661 2024-03-04 18:12:55.000000 ToolBoxV2-0.1.8/toolboxv2/runabel/run_api_helper.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.690253 ToolBoxV2-0.1.8/toolboxv2/utils/
+-rw-rw-rw-   0        0        0    12097 2024-03-04 15:11:23.000000 ToolBoxV2-0.1.8/toolboxv2/utils/Style.py
+-rw-rw-rw-   0        0        0    17822 2023-09-20 00:40:56.000000 ToolBoxV2-0.1.8/toolboxv2/utils/TBConfig.py
+-rw-rw-rw-   0        0        0     1140 2024-03-05 16:20:12.000000 ToolBoxV2-0.1.8/toolboxv2/utils/__init__.py
+-rw-rw-rw-   0        0        0    19094 2024-03-05 23:39:41.000000 ToolBoxV2-0.1.8/toolboxv2/utils/all_functions_enums.py
+-rw-rw-rw-   0        0        0    11207 2024-03-05 11:37:19.000000 ToolBoxV2-0.1.8/toolboxv2/utils/cryp.py
+-rw-rw-rw-   0        0        0    10659 2024-03-05 13:36:52.000000 ToolBoxV2-0.1.8/toolboxv2/utils/file_handler.py
+-rw-rw-rw-   0        0        0     2282 2024-01-16 13:05:13.000000 ToolBoxV2-0.1.8/toolboxv2/utils/helper_functions.py
+-rw-rw-rw-   0        0        0     3162 2024-01-30 23:08:08.000000 ToolBoxV2-0.1.8/toolboxv2/utils/main_tool.py
+-rw-rw-rw-   0        0        0     5050 2024-02-15 15:30:03.000000 ToolBoxV2-0.1.8/toolboxv2/utils/state_system.py
+-rw-rw-rw-   0        0        0     6007 2024-01-29 11:49:39.000000 ToolBoxV2-0.1.8/toolboxv2/utils/tb_logger.py
+-rw-rw-rw-   0        0        0    70665 2024-03-05 23:35:59.000000 ToolBoxV2-0.1.8/toolboxv2/utils/toolbox.py
+-rw-rw-rw-   0        0        0     9968 2024-03-05 16:40:17.000000 ToolBoxV2-0.1.8/toolboxv2/utils/types.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.694763 ToolBoxV2-0.1.8/toolboxv2/web/
+-rw-rw-rw-   0        0        0        0 2023-08-08 15:41:31.000000 ToolBoxV2-0.1.8/toolboxv2/web/__init__.py
+-rw-rw-rw-   0        0        0     1036 2023-08-20 11:34:14.000000 ToolBoxV2-0.1.8/toolboxv2/web/serveapp.py
+drwxrwxrwx   0        0        0        0 2024-03-05 23:57:07.696765 ToolBoxV2-0.1.8/toolboxv2/web_row/
+-rw-rw-rw-   0        0        0        0 2023-08-08 15:41:31.000000 ToolBoxV2-0.1.8/toolboxv2/web_row/__init__.py
+-rw-rw-rw-   0        0        0     1036 2023-08-20 11:34:14.000000 ToolBoxV2-0.1.8/toolboxv2/web_row/serveapp.py
```

### Comparing `ToolBoxV2-0.1.6/LICENSE` & `ToolBoxV2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/PKG-INFO` & `ToolBoxV2-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBoxV2
-Version: 0.1.6
+Version: 0.1.8
 Summary: Command line interface for interactions with the ToolBox Network.
 Home-page: https://github.com/MarkinHaus/ToolBoxV2
 Author: Markin Hausmanns
 Author-email: Markinhausmanns@gmail.com
 License: Apache Software License 2.0
 Keywords: toolboxv2
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,16 +35,21 @@
 Requires-Dist: docker>=6.1.0
 Requires-Dist: dill~=0.3.7
 Requires-Dist: cryptography>=41.0.3
 Requires-Dist: cachetools>=5.3.2
 Requires-Dist: psutil>=5.9.7
 Requires-Dist: faker>=22.2.0
 Requires-Dist: prompt_toolkit>=3.0.43
+Requires-Dist: mailjet-rest>=1.3.4
+Requires-Dist: webauthn>=2.0.0
+Requires-Dist: qrcode>=7.4.2
 Requires-Dist: uvicorn[standard]
 Requires-Dist: python-multipart
+Requires-Dist: playwright~=1.33.0
+Requires-Dist: pydantic~=1.10.8
 
  # ToolBoxV2
 
 
 [![image](https://img.shields.io/pypi/v/ToolBoxV2.svg)](https://pypi.python.org/pypi/ToolBoxV2)
 [![image](https://img.shields.io/conda/vn/conda-forge/ToolBoxV2.svg)](https://anaconda.org/conda-forge/ToolBoxV2)
```

### Comparing `ToolBoxV2-0.1.6/README.md` & `ToolBoxV2-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/ToolBoxV2.egg-info/PKG-INFO` & `ToolBoxV2-0.1.8/ToolBoxV2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBoxV2
-Version: 0.1.6
+Version: 0.1.8
 Summary: Command line interface for interactions with the ToolBox Network.
 Home-page: https://github.com/MarkinHaus/ToolBoxV2
 Author: Markin Hausmanns
 Author-email: Markinhausmanns@gmail.com
 License: Apache Software License 2.0
 Keywords: toolboxv2
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,16 +35,21 @@
 Requires-Dist: docker>=6.1.0
 Requires-Dist: dill~=0.3.7
 Requires-Dist: cryptography>=41.0.3
 Requires-Dist: cachetools>=5.3.2
 Requires-Dist: psutil>=5.9.7
 Requires-Dist: faker>=22.2.0
 Requires-Dist: prompt_toolkit>=3.0.43
+Requires-Dist: mailjet-rest>=1.3.4
+Requires-Dist: webauthn>=2.0.0
+Requires-Dist: qrcode>=7.4.2
 Requires-Dist: uvicorn[standard]
 Requires-Dist: python-multipart
+Requires-Dist: playwright~=1.33.0
+Requires-Dist: pydantic~=1.10.8
 
  # ToolBoxV2
 
 
 [![image](https://img.shields.io/pypi/v/ToolBoxV2.svg)](https://pypi.python.org/pypi/ToolBoxV2)
 [![image](https://img.shields.io/conda/vn/conda-forge/ToolBoxV2.svg)](https://anaconda.org/conda-forge/ToolBoxV2)
```

### Comparing `ToolBoxV2-0.1.6/setup.py` & `ToolBoxV2-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,10 +60,10 @@
     name='ToolBoxV2',
     packages=find_packages(include=['toolboxv2', 'toolboxv2.mods.*',  'toolboxv2.mods_dev.*', 'toolboxv2.*']),
     package_data={"toolboxv2": ["toolboxv2/init.config"]},
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MarkinHaus/ToolBoxV2',
-    version='0.1.6',
+    version='0.1.8',
     zip_safe=False,
 )
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/__init__.py` & `ToolBoxV2-0.1.8/toolboxv2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #     import toolboxv2.mods
 #     from toolboxv2.mods import *
 # except ImportError as e:
 #     MODS_ERROR = e
 
 __author__ = """Markin Hausmanns"""
 __email__ = 'Markinhausmanns@gmail.com'
-__version__ = '0.1.6'
+__version__ = '0.1.8'
 __all__ = [
     "__version__",
     "App",
     "MainTool",
     "FileHandler",
     "Style",
     "Spinner",
@@ -33,11 +33,10 @@
     "runnable_dict",
     "mods",
     "utils",
     "get_app",
     "tbef",
     "Result",
     "Code",
-    ]
+]
 
 ToolBox_over: str = "root"
-
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/api/fast_api_install.py` & `ToolBoxV2-0.1.8/toolboxv2/api/fast_api_install.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/api/fast_app.py` & `ToolBoxV2-0.1.8/toolboxv2/api/fast_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,28 +9,22 @@
 
 from starlette.responses import RedirectResponse
 
 from toolboxv2 import App
 from toolboxv2.utils.toolbox import get_app
 
 router = APIRouter(
-    prefix="/app",
+    prefix="/web",
     tags=["token"],
     # dependencies=[Depends(get_token_header)],
     # responses={404: {"description": "Not found"}},
 )
 
 level = 2  # Setzen Sie den Level-Wert, um verschiedene Routen zu aktivieren oder zu deaktivieren
 pattern = ['.png', '.jpg', '.jpeg', '.js', '.css', '.ico', '.gif', '.svg', '.wasm']
-oauth2_scheme = OAuth2PasswordBearer(tokenUrl="login")
-
-
-async def get_current_user(token: str = Depends(oauth2_scheme)):
-    tb_app: App = get_app()
-    return tb_app.run_any("cloudM", "validate_jwt", ["token", token, {}])
 
 
 def check_access_level(required_level: int):
     if level < required_level:
         raise HTTPException(status_code=403, detail="Access forbidden")
     return True
 
@@ -42,53 +36,45 @@
     return serve_app_func('index.html')
 
 
 @router.get("/")
 async def index2(access_allowed: bool = Depends(lambda: check_access_level(-1))):
     if level == -1:
         return serve_app_func('assets/serverInWartung.html')
-    return RedirectResponse(url="/app")
+    return RedirectResponse(url="/web")
 
 
-@router.get("/app/")
+@router.get("/web/")
 async def index2_(access_allowed: bool = Depends(lambda: check_access_level(-1))):
     if level == -1:
         return serve_app_func('assets/serverInWartung.html')
-    return RedirectResponse(url="/app")
+    return RedirectResponse(url="/web")
 
 
 @router.get("/login")
 async def login_page(access_allowed: bool = Depends(lambda: check_access_level(0))):
     return serve_app_func('assets/login.html')
 
 
 @router.get("/signup")
 async def signup_page(access_allowed: bool = Depends(lambda: check_access_level(2))):
     return serve_app_func('assets/signup.html')
 
 
-#@router.get("/quicknote")
-#async def quicknote(current_user: str = Depends(get_current_user),
-#                    access_allowed: bool = Depends(lambda: check_access_level(0))):
-#    print("[current_user]", current_user)
-#    print("[access_allowed]", access_allowed)
-#    return serve_app_func('quicknote/index.html')
-
-
 @router.get("/dashboard")
-async def quicknote(access_allowed: bool = Depends(lambda: check_access_level(1))):
-    return serve_app_func('dashboards/dashboard_builder.html')
+async def quicknote(access_allowed: bool = Depends(lambda: check_access_level(2))):
+    return serve_app_func('dashboards/user_dashboard.html')  # 'dashboards/dashboard_builder.html')
 
 
 @router.get("/{path:path}")
 async def serve_files(path: str, request: Request, access_allowed: bool = Depends(lambda: check_access_level(0))):
     return serve_app_func(path)
 
 
-def serve_app_func(path: str, prefix: str = os.getcwd() + "/app/"):
+def serve_app_func(path: str, prefix: str = os.getcwd() + "/web/"):
     if not path:
         path = "index.html"
 
     print("serving", path, prefix)
     request_file_path = Path(prefix + path)
     ext = request_file_path.suffix
     print(request_file_path, ext)
@@ -107,8 +93,8 @@
     # Check if the file extension exists in the mime_types dictionary
     if ext in mime_types.keys():
         content_type = mime_types[ext]
 
     request_file_path.is_file()
     if request_file_path.exists():
         return FileResponse(request_file_path, media_type=content_type)
-    return FileResponse("./app/3Dbg.html", media_type=content_type)
+    return FileResponse("./web/3Dbg.html", media_type=content_type)
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/app/serveapp.py` & `ToolBoxV2-0.1.8/toolboxv2/web/serveapp.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/cli.py` & `ToolBoxV2-0.1.8/toolboxv2/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 """Console script for toolboxv2."""
 # Import default Pages
 import sys
 import argparse
+import threading
 import time
 from functools import wraps
 from platform import system, node
 # Import public Pages
 from toolboxv2 import App, MainTool, runnable_dict as runnable_dict_func
-from toolboxv2.utils.toolbox import get_app
-import ctypes
+from toolboxv2.utils import show_console
+from toolboxv2.utils.toolbox import get_app, ProxyApp, DemonApp, override_main_app
+
+DEFAULT_MODI = "minicli"
+
+try:
+    import hmr
+
+    HOT_RELOADER = True
+except ImportError:
+    HOT_RELOADER = False
 
 try:
     import cProfile
     import pstats
     import io
 
 
@@ -58,15 +68,15 @@
 
         s = io.StringIO()
         sortby = 'cumulative'
         ps = pstats.Stats(profiler, stream=s).sort_stats(sortby)
         ps.print_stats()
         print(s.getvalue())
 
-        print("\n================================"*12)
+        print("\n================================" * 12)
         s = io.StringIO()
         sortby = 'time'  # Sortierung nach der Gesamtzeit, die in jeder Funktion verbracht wird
 
         # Erstellen eines pstats-Objekts und Ausgabe der Top-Funktionen
         ps = pstats.Stats(profiler, stream=s).sort_stats(sortby)
         ps.print_stats()
 
@@ -75,120 +85,164 @@
 
         # Erstellen eines Streams für die Profilergebnisse
 
 except ImportError as e:
     profile_execute_all_functions = lambda *args: print(args);
     raise ValueError(f"Failed to import function for profiling")
 
-
-def show_console(show=True):
-    """Brings up the Console Window."""
-    if show:
-        # Show console
-        ctypes.windll.user32.ShowWindow(ctypes.windll.kernel32.GetConsoleWindow(), 4)
-    else:
-        # Hide console
-        ctypes.windll.user32.ShowWindow(ctypes.windll.kernel32.GetConsoleWindow(), 0)
-
-
 try:
     from toolboxv2.utils.tb_logger import edit_log_files, loggerNameOfToolboxv2, unstyle_log_files
 except ModuleNotFoundError:
     from .utils.tb_logger import edit_log_files, loggerNameOfToolboxv2, unstyle_log_files
 
 import os
 import subprocess
 
 
+def start(pidname, args):
+    caller = args[0]
+    args = args[1:]
+    args = ["-bgr" if arg == "-bg" else arg for arg in args]
+
+    if '-m' not in args or args[args.index('-m')+1] == "toolboxv2":
+        args += ["-m", "bg"]
+    if caller.endswith('toolboxv2'):
+        args = ["toolboxv2"] + args
+    else:
+        args = [sys.executable, "-m", "toolboxv2"] + args
+    if system() == "Windows":
+        DETACHED_PROCESS = 0x00000008
+        p = subprocess.Popen(args, creationflags=DETACHED_PROCESS)
+    else:  # sys.executable, "-m",
+        p = subprocess.Popen(args, stdout=subprocess.PIPE,
+                             stderr=subprocess.PIPE)
+    pdi = p.pid
+    get_app().sprint(f"Service {pidname} started")
+
+
+def stop(pidfile, pidname):
+    try:
+        with open(pidfile, "r") as f:
+            procID = f.readline().strip()
+    except IOError:
+        print("Process file does not exist")
+        return
+
+    if procID:
+        if system() == "Windows":
+            subprocess.Popen(['taskkill', '/PID', procID, '/F'])
+        else:
+            subprocess.Popen(['kill', '-SIGTERM', procID])
+
+        print(f"Service {pidname} {procID} stopped")
+        os.remove(pidfile)
+
+
 def create_service_file(user, group, working_dir):
     service_content = f"""[Unit]
-Description=My Python App
+Description=ToolBoxService
 After=network.target
 
 [Service]
 User={user}
 Group={group}
 WorkingDirectory={working_dir}
-ExecStart=toolboxv2 -m app -n app
+ExecStart=toolboxv2 -bg
 Restart=always
 RestartSec=5
 
 [Install]
 WantedBy=multi-user.target
 """
-    with open("myapp.service", "w") as f:
+    with open("tb.service", "w") as f:
         f.write(service_content)
 
 
 def init_service():
     user = input("Enter the user name: ")
     group = input("Enter the group name: ")
-    working_dir = input("Enter the working directory path (/path/to/your/app): ")
+    working_dir = get_app().start_dir
 
     create_service_file(user, group, working_dir)
 
-    subprocess.run(["sudo", "mv", "myapp.service", "/etc/systemd/system/"])
+    subprocess.run(["sudo", "mv", "tb.service", "/etc/systemd/system/"])
     subprocess.run(["sudo", "systemctl", "daemon-reload"])
 
 
 def manage_service(action):
-    subprocess.run(["sudo", "systemctl", action, "myapp.service"])
+    subprocess.run(["sudo", "systemctl", action, "tb.service"])
 
 
 def show_service_status():
-    subprocess.run(["sudo", "systemctl", "status", "myapp.service"])
+    subprocess.run(["sudo", "systemctl", "status", "tb.service"])
 
 
 def uninstall_service():
-    subprocess.run(["sudo", "systemctl", "disable", "myapp.service"])
-    subprocess.run(["sudo", "systemctl", "stop", "myapp.service"])
-    subprocess.run(["sudo", "rm", "/etc/systemd/system/myapp.service"])
+    subprocess.run(["sudo", "systemctl", "disable", "tb.service"])
+    subprocess.run(["sudo", "systemctl", "stop", "tb.service"])
+    subprocess.run(["sudo", "rm", "/etc/systemd/system/tb.service"])
     subprocess.run(["sudo", "systemctl", "daemon-reload"])
 
 
 def setup_service_windows():
     path = "C:/ProgramData/Microsoft/Windows/Start Menu/Programs/Startup"
     print("Select mode:")
     print("1. Init (first-time setup)")
     print("2. Uninstall")
+    print("3. Show window")
+    print("4. hide window")
+
     mode = int(input("Enter the mode number: "))
 
     if not os.path.exists(path):
         print("pleas press win + r and enter")
         print("1. for system -> shell:common startup")
         print("2. for user -> shell:startup")
-        path = input("Enter the path: ")
+        path = input("Enter the path that opened: ")
 
     if mode == 1:
+        if os.path.exists(path + '/tb_start.bat'):
+            os.remove(path + '/tb_start.bat')
         with open(path + '/tb_start.bat', "a") as f:
             f.write(
-                """toolboxV2 -m demon -bg -n AutoStart"""
+                f"""{sys.executable} -m toolboxv2 -bg --debug"""
             )
+    elif mode == 3:
+        get_app().show_console()
+    elif mode == 4:
+        get_app().hide_console()
     else:
-        os.remove(path + '/tb_start.pyw')
+        os.remove(path + '/tb_start.bat')
 
 
 def setup_service_linux():
     print("Select mode:")
     print("1. Init (first-time setup)")
     print("2. Start / Stop / Restart")
     print("3. Status")
     print("4. Uninstall")
 
+    print("5. Show window")
+    print("6. hide window")
+
     mode = int(input("Enter the mode number: "))
 
     if mode == 1:
         init_service()
     elif mode == 2:
         action = input("Enter 'start', 'stop', or 'restart': ")
         manage_service(action)
     elif mode == 3:
         show_service_status()
     elif mode == 4:
         uninstall_service()
+    elif mode == 5:
+        get_app().show_console()
+    elif mode == 6:
+        get_app().hide_console()
     else:
         print("Invalid mode")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Welcome to the ToolBox cli")
 
@@ -213,26 +267,33 @@
                         action="store_true")
     parser.add_argument("--lm", help=f"Log Manager remove and edit log files", default=False,
                         action="store_true")
 
     parser.add_argument("-m", "--modi",
                         type=str,
                         help="Start a ToolBox interface default build in cli",
-                        default="cli")
+                        default=DEFAULT_MODI)
 
     parser.add_argument("--kill", help="Kill current local tb instance", default=False,
                         action="store_true")
 
     parser.add_argument("--remote", help=f"Open a remote toolbox session", default=False,
                         action="store_true")
     parser.add_argument("--remote-direct-key", type=str or None, help=f"Open a remote toolbox session", default=None)
 
     parser.add_argument("-bg", "--background-application", help="Start an interface as background application",
                         default=False,
                         action="store_true")
+    parser.add_argument("-bgr", "--background-application-runner", help="Start an interface as background application",
+                        default=False,
+                        action="store_true")
+    parser.add_argument("-fg", "--proxy-application", help="Start an interface as proxy application",
+                        default=True,
+                        action="store_false")
+
     parser.add_argument("--docker", help="start the toolbox in docker (in remote mode is no local docker engin "
                                          "required)", default=False,
                         action="store_true")
 
     parser.add_argument("-i", "--install", help="Install a mod or interface via name", type=str or None, default=None)
     parser.add_argument("-r", "--remove", help="Uninstall a mod or interface via name", type=str or None, default=None)
     parser.add_argument("-u", "--update", help="Update a mod or interface via name", type=str or None, default=None)
@@ -265,14 +326,19 @@
                         help="load all modules in mod file",
                         action="store_true")
 
     parser.add_argument("-sfe", "--save-function-enums-in-file",
                         help="run with -l to gather to generate all_function_enums.py files",
                         action="store_true")
 
+    parser.add_argument("-hr", "--hot-reload",
+                        help="run -hr automatically reload the toolboxv2 module on changes good for development and"
+                             " for long running instances in save environments",
+                        action="store_true")
+
     # parser.add_argument("--mods-folder",
     #                     help="specify loading package folder",
     #                     type=str,
     #                     default="toolboxv2.mods.")
 
     parser.add_argument("--debug",
                         help="start in debug mode",
@@ -398,67 +464,109 @@
 
     identification = args.name + '-' + node() + '\\'
     if args.mm:
         identification = "MainNode\\"
 
     data_folder = abspath + '\\.data\\'
     config_folder = abspath + '\\.config\\'
+    info_folder = abspath + '\\.info\\'
+
+    os.makedirs(info_folder, exist_ok=True)
 
     app_config_file = config_folder + identification
     app_data_folder = data_folder + identification
 
     if args.delete_config_all:
         os.remove(config_folder)
     if args.delete_data_all:
         os.remove(data_folder)
     if args.delete_config:
         os.remove(app_config_file)
     if args.delete_data:
         os.remove(app_data_folder)
 
     if args.test:
-        test_path = os.path.dirname(os.path.abspath(__file__)).replace("toolboxv2\\toolboxv2", "toolboxv2") + "\\tests\\test_mods"
+        test_path = os.path.dirname(os.path.abspath(__file__))
+        if system() == "Windows":
+            test_path = test_path.replace("toolboxv2\\toolboxv2", "toolboxv2") + "\\tests\\test_mods"
+        else:
+            test_path = test_path.replace("ToolBoxV2/toolboxv2", "ToolBoxV2") + "/tests/test_mods"
         print(f"Testing in {test_path}")
-        os.system(f"python -m unittest discover -s {test_path}")
+
+        if os.system(f"python -m unittest discover -s {test_path}") != 0:
+            os.system(f"python3 -m unittest discover -s {test_path}")
         return 1
 
     app_pid = str(os.getpid())
 
-    tb_app = get_app(from_="InitialStartUp", name=args.name, args=args)
+    pid_file = f"{info_folder}{args.modi}-{args.name}.pid"
 
-    # tb_app.load_all_mods_in_file()
-    # tb_app.save_registry_as_enums("utils", "all_functions_enums.py")
+    print(sys.argv)
+    tb_app = get_app(from_="InitialStartUp", name=args.name, args=args, app_con=App)
+    demon_app = None
+    if args.background_application_runner:
+        demon_app = DemonApp(tb_app, args.host, args.port if args.port != 8000 else 6587, t=args.modi != 'bg')
+        if not args.debug:
+            show_console(False)
+        tb_app.demon_app = demon_app
+        with open(pid_file + '-app.pid', 'w') as f:
+            f.write(app_pid)
+        args.proxy_application = False
+    elif args.background_application:
+        if not args.kill and not args.hot_reload:
+            start(args.name, sys.argv)
+        elif args.hot_reload:
+            _ = ProxyApp(tb_app, args.host if args.host != "0.0.0.0" else "localhost",
+                           args.port if args.port != 8000 else 6587, timeout=6)
+            if _.exit_main() == "No data look later":
+                stop(pid_file + '-app.pid', args.name)
+            time.sleep(2)
+            start(args.name, sys.argv)
+        else:
+            if '-m ' not in sys.argv:
+                pid_file = f"{info_folder}bg-{args.name}.pid"
+            _ = ProxyApp(tb_app, args.host if args.host != "0.0.0.0" else "localhost",
+                         args.port if args.port != 8000 else 6587, timeout=6)
+            if _.exit_main() == "No data look later":
+                stop(pid_file + '-app.pid', args.name)
+    elif args.proxy_application:
+        tb_app = override_main_app(ProxyApp(tb_app, args.host if args.host != "0.0.0.0" else "localhost",
+                                            args.port if args.port != 8000 else 6587))
 
-    pid_file = f"{tb_app.start_dir}/{tb_app.config_fh.file_handler_file_prefix}{args.modi}-{args.name}.pid"
+        tb_app.verify()
+        if args.debug:
+            tb_app.show_console()
 
-    if args.background_application and system() == "Windows":
-        show_console(False)
+    # tb_app.load_all_mods_in_file()
+    # tb_app.save_registry_as_enums("utils", "all_functions_enums.py")
 
     if args.lm:
         edit_logs()
         tb_app.exit()
         exit(0)
 
     if args.sm:
         if tb_app.system_flag == "Linux":
             setup_service_linux()
         if tb_app.system_flag == "Windows":
             setup_service_windows()
+        tb_app.exit()
+        exit(0)
 
-    if args.load_all_mod_in_files or args.save_function_enums_in_file or args.get_version or args.profiler:
-        tb_app.load_all_mods_in_file()
+    if args.load_all_mod_in_files or args.save_function_enums_in_file or args.get_version or args.profiler or args.background_application_runner:
+        if not args.proxy_application:
+            tb_app.load_all_mods_in_file()
         if args.save_function_enums_in_file:
             tb_app.save_registry_as_enums("utils", "all_functions_enums.py")
             tb_app.alive = False
             tb_app.exit()
             return 0
         if args.debug:
             tb_app.print_functions()
         if args.get_version:
-
             for mod_name in tb_app.functions:
                 if isinstance(tb_app.functions[mod_name].get("app_instance"), MainTool):
                     print(f"{mod_name} : {tb_app.functions[mod_name]['app_instance'].version}")
                 else:
                     v = tb_app.functions[mod_name].get(list(tb_app.functions[mod_name].keys())[0]).get("version",
                                                                                                        "unknown (functions only)")
                     print(f"{mod_name} : {v}")
@@ -467,54 +575,61 @@
 
     if args.profiler:
         profile_execute_all_functions(tb_app)
         tb_app.alive = False
         tb_app.exit()
         return 0
 
-    if not args.kill and not args.docker and tb_app.alive:
+    if not args.kill and not args.docker and tb_app.alive and not args.background_application:
 
-        with open(f"{tb_app.start_dir}/{tb_app.config_fh.file_handler_file_prefix}/{args.modi}-{args.name}.pid",
-                  "w") as f:
+        tb_app.save_autocompletion_dict()
+        with open(pid_file, "w") as f:
             f.write(app_pid)
 
-        runnable_dict = runnable_dict_func()
-
-        if args.modi in runnable_dict.keys():
+        if not args.proxy_application:
+            runnable_dict = runnable_dict_func()
+            tb_app.set_runnable(runnable_dict)
+            if args.modi in runnable_dict.keys():
+                pass
+            else:
+                raise ValueError(
+                    f"Modi : [{args.modi}] not found on device installed modi : {list(runnable_dict.keys())}")
+        # open(f"./config/{args.modi}.pid", "w").write(app_pid)
+            tb_app.run_runnable(args.modi)
+        elif 'cli' in args.modi:
+            runnable_dict = runnable_dict_func('cli')
             tb_app.set_runnable(runnable_dict)
-            # open(f"./config/{args.modi}.pid", "w").write(app_pid)
-            runnable_dict[args.modi](tb_app, args)
+            tb_app.run_runnable(args.modi)
         else:
-            print(f"Modi : [{args.modi}] not found on device installed modi : {runnable_dict.keys()}")
+            tb_app.rrun_runnable(args.modi)
 
     elif args.docker:
 
         runnable_dict = runnable_dict_func('docker')
 
         if 'docker' not in runnable_dict.keys():
             print("No docker")
             return
 
         runnable_dict['docker'](tb_app, args)
 
-    elif args.kill:
+    elif args.kill and not args.background_application:
         if not os.path.exists(pid_file):
             print("You must first run the mode")
         else:
-            with open(pid_file,
-                      "r") as f:
+            with open(pid_file, "r") as f:
                 app_pid = f.read()
             print(f"Exit app {app_pid}")
             if system() == "Windows":
                 os.system(f"taskkill /pid {app_pid} /F")
             else:
                 os.system(f"kill -9 {app_pid}")
 
-            # if args.docker:
-            #     tb_app.run_any()
+    if args.proxy_application and args.debug:
+        tb_app.hide_console()
 
     if tb_app.alive:
         tb_app.exit()
         return 0
 
     if os.path.exists(pid_file):
         os.remove(pid_file)
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/init.config` & `ToolBoxV2-0.1.8/toolboxv2/init.config`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/AuthManager.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/AuthManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 import base64
 import datetime
 import json
+import os
 import time
+from urllib.parse import quote
 import uuid
+import webauthn
 from dataclasses import dataclass, field, asdict
-from typing import Union, List
 
 import jwt
 from pydantic import BaseModel
+from webauthn.helpers.exceptions import InvalidAuthenticationResponse, InvalidRegistrationResponse
+from webauthn.helpers.structs import AuthenticationCredential, RegistrationCredential
 
 from toolboxv2.mods.DB.types import DatabaseModes
 from toolboxv2.utils.types import ToolBoxInterfaces, ApiResult
 from toolboxv2 import get_app, App, Result, tbef, ToolBox_over
 
 from toolboxv2.utils.cryp import Code
+from pydantic import validator
+from .types import UserCreator, User, UserPersonaPubKey
 
 Name = 'CloudM.AuthManager'
 export = get_app(f"{Name}.Export").tb
 default_export = export(mod_name=Name, test=False)
 test_only = export(mod_name=Name, test_only=True)
 version = '0.0.1'
 instance_bios = str(uuid.uuid4())
 
 
-@dataclass
-class User:
-    uid: str = field(default_factory=lambda: str(uuid.uuid4()))
-    pub_key: str = field(default="")
-    email: str = field(default="")
-    name: str = field(default="")
-    user_pass_pub: str = field(default="")
-    user_pass_pub_persona: str = field(default="")
-    user_pass_pub_persona_id: str = field(default="")
-    user_pass_pub_devices: List[str] = field(default_factory=[])
-    user_pass_pri: str = field(default="")
-    user_pass_sync: str = field(default="")
-    creation_time: str = field(default_factory=lambda: time.strftime("%Y-%m-%d::%H:%M:%S", time.localtime()))
-    challenge: str = field(default="")
-
-
-@dataclass
-class UserCreator(User):
-    def __post_init__(self):
-        self.user_pass_pub, self.user_pass_pri = Code.generate_asymmetric_keys()
-        self.user_pass_sync = Code.generate_symmetric_key()
-        self.challenge = Code.encrypt_asymmetric(str(uuid.uuid4()), self.user_pass_pub)
+def b64decode(s: str) -> bytes:
+    return base64.urlsafe_b64decode(s.encode())
+
+
+class CustomAuthenticationCredential(AuthenticationCredential):
+    @validator('raw_id', pre=True)
+    def convert_raw_id(cls, v: str):
+        assert isinstance(v, str), 'raw_id is not a string'
+        return b64decode(v)
+
+    @validator('response', pre=True)
+    def convert_response(cls, data: dict):
+        assert isinstance(data, dict), 'response is not a dictionary'
+        return {k: b64decode(v) for k, v in data.items()}
+
+
+class CustomRegistrationCredential(RegistrationCredential):
+    @validator('raw_id', pre=True)
+    def convert_raw_id(cls, v: str):
+        assert isinstance(v, str), 'raw_id is not a string'
+        return b64decode(v)
+
+    @validator('response', pre=True)
+    def convert_response(cls, data: dict):
+        assert isinstance(data, dict), 'response is not a dictionary'
+        return {k: b64decode(v) for k, v in data.items()}
 
 
 # app Helper functions interaction with the db
 
 def db_helper_test_exist(app: App, username: str):
-    return not app.run_any(tbef.DB.GET, query=f"USER::{username}::*", get_results=True).is_data()
+    c = app.run_any(tbef.DB.IF_EXIST, query=f"USER::{username}::*", get_results=True)
+    if c.is_error(): raise f"DB - error {c.print(show=False)}"
+    b = c.get() > 0
+    print(f"TEST IF USER EXIST : {username} {b}")
+    return b
 
 
 def db_delete_invitation(app: App, invitation: str):
     return app.run_any(tbef.DB.DELETE, query=f"invitation::{invitation}", get_results=True)
 
 
 def db_valid_invitation(app: App, invitation: str):
@@ -154,15 +168,15 @@
     except Exception as e:
         return str(e)
 
 
 # Export functions
 
 
-@export(mod_name=Name, state=False, test=False)
+@export(mod_name=Name, state=True, test=False)
 def get_user_by_name(app: App, username: str, uid: str = '*') -> Result:
     if app is None:
         app = get_app(Name + '.get_user_by_name')
 
     if not db_helper_test_exist(app, username):
         return Result.default_user_error(info=f"get_user_by_name failed username'{username}'not registered")
 
@@ -182,15 +196,18 @@
     elif isinstance(user_data, list):
         if len(user_data) == 0:
             return Result.default_internal_error(info="get_user_by_name failed no User data found", exec_code=9283)
 
         if len(user_data) > 1:
             pass
 
-        return Result.ok(data=User(**eval(user_data[0].decode())))
+        if isinstance(user_data[0], bytes):
+            user_data[0] = user_data[0].decode()
+
+        return Result.ok(data=User(**eval(user_data[0])))
     else:
         return Result.default_internal_error(info="get_user_by_name failed no User data found", exec_code=2351)
 
 
 def to_base64(data: str):
     return base64.b64encode(data.encode('utf-8'))
 
@@ -202,26 +219,34 @@
 def initialize_and_return(app: App, user) -> ApiResult:
     if isinstance(user, User):
         user = UserCreator(**asdict(user))
     return db_helper_save_user(app, asdict(user)).lazy_return('intern', data={
         "challenge": user.challenge,
         "userId": to_base64(user.uid),
         "username": user.name,
-        "dSync": Code().encrypt_asymmetric(user.user_pass_sync, user.user_pass_pub_devices[0])})
+        "dSync": Code().encrypt_asymmetric(user.user_pass_sync, user.pub_key)})
 
 
 class CreateUserObject(BaseModel):
     name: str
     email: str
     pub_key: str
     invitation: str
     web_data: bool = True
     as_base64: bool = True
 
 
+class AddUserDeviceObject(BaseModel):
+    name: str
+    pub_key: str
+    invitation: str
+    web_data: bool = True
+    as_base64: bool = True
+
+
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.api, api=True, test=False)
 def create_user(app: App, data: CreateUserObject = None, username: str = 'test-user', email: str = 'test@user.com',
                 pub_key: str = '',
                 invitation: str = '', web_data=False, as_base64=False) -> ApiResult:
     username = data.name if data is not None else username
     email = data.email if data is not None else email
     pub_key = data.pub_key if data is not None else pub_key
@@ -229,35 +254,123 @@
     web_data = data.web_data if data is not None else web_data
     as_base64 = data.as_base64 if data is not None else as_base64
 
     if app is None:
         app = get_app(Name + '.crate_user')
 
     if db_helper_test_exist(app, username):
-        return Result.default_user_error(info=f"Username '{username}' already taken", interface=ToolBoxInterfaces.remote)
+        return Result.default_user_error(info=f"Username '{username}' already taken",
+                                         interface=ToolBoxInterfaces.remote)
 
-    if not db_valid_invitation(app, invitation):
+    if not invitation.startswith("00#"):  # not db_valid_invitation(app, invitation):
         return Result.default_user_error(info=f"Invalid invitation", interface=ToolBoxInterfaces.remote)
 
-    test_bub_key = ""
+    test_bub_key = "Invalid"
+
+    if pub_key:
+        if as_base64:
+            try:
+                pub_key = from_base64(pub_key)
+                pub_key = str(pub_key)
+            except Exception as e:
+                return Result.default_internal_error(info=f"Invalid public key not a valid base64 string: {e}")
+
+        test_bub_key = Code().encrypt_asymmetric(username, pub_key)
+
+    if test_bub_key == "Invalid":
+        return Result.default_user_error(info="Invalid public key parsed", interface=ToolBoxInterfaces.remote)
+
+    user = User(name=username,
+                email=email,
+                user_pass_pub_devices=[pub_key],
+                pub_key=pub_key)
+
+    db_delete_invitation(app, invitation)
+
+    if web_data:
+        return initialize_and_return(app, user)
+
+    result_s = db_helper_save_user(app, asdict(user))
+
+    return Result.ok(info=f"User created successfully: {username}",
+                     data=Code().encrypt_asymmetric(str(user.name), pub_key)
+                     , interface=ToolBoxInterfaces.remote)
+
+
+@export(mod_name=Name, state=True, interface=ToolBoxInterfaces.api, api=True, test=False)
+def get_magick_link_email(app: App, username):
+    if app is None:
+        app = get_app(Name + '.get_magick_link_email')
+
+    if not db_helper_test_exist(app, username):
+        return Result.default_user_error(info=f"Username '{username}' not known", interface=ToolBoxInterfaces.remote)
+
+    user: User = get_user_by_name(app, username=username).get()
+
+    if user.challenge == '':
+        user = UserCreator(**asdict(user))
+
+    invitation = "01#" + Code.one_way_hash(user.user_pass_sync, "CM", "get_magick_link_email")
+    nl = len(user.name)
+    email_data_result = app.run_any(tbef.EMAIL_WAITING_LIST.CRATE_MAGICK_LICK_DEVICE_EMAIL,
+                                    user_email=user.email,
+                                    user_name=user.name,
+                                    link_id=invitation, nl=nl, get_results=True)
+
+    if email_data_result.is_error() and not email_data_result.is_data():
+        return email_data_result
+
+    email_data = email_data_result.get()
+
+    return app.run_any(tbef.EMAIL_WAITING_LIST.SEND_EMAIL, data=email_data, get_results=True)
+
+    # if not invitation.endswith(user.challenge[12:]):
+
+
+@export(mod_name=Name, state=True, interface=ToolBoxInterfaces.api, api=True, test=False)
+def add_user_device(app: App, data: AddUserDeviceObject = None, username: str = 'test-user',
+                    pub_key: str = '',
+                    invitation: str = '', web_data=False, as_base64=False) -> ApiResult:
+    username = data.name if data is not None else username
+    pub_key = data.pub_key if data is not None else pub_key
+    invitation = data.invitation if data is not None else invitation
+    web_data = data.web_data if data is not None else web_data
+    as_base64 = data.as_base64 if data is not None else as_base64
+
+    if app is None:
+        app = get_app(Name + '.add_user_device')
+
+    if not db_helper_test_exist(app, username):
+        return Result.default_user_error(info=f"Username '{username}' not known", interface=ToolBoxInterfaces.remote)
+
+    if not invitation.startswith("01#"):  # not db_valid_invitation(app, invitation):
+        return Result.default_user_error(info=f"Invalid invitation", interface=ToolBoxInterfaces.remote)
+    invitation = invitation.replace("01#", "")
+    test_bub_key = "Invalid"
 
     if pub_key:
         if as_base64:
             try:
                 pub_key = from_base64(pub_key)
                 pub_key = str(pub_key)
             except Exception as e:
                 return Result.default_internal_error(info=f"Invalid public key not a valid base64 string: {e}")
 
         test_bub_key = Code().encrypt_asymmetric(username, pub_key)
 
     if test_bub_key == "Invalid":
         return Result.default_user_error(info="Invalid public key parsed", interface=ToolBoxInterfaces.remote)
 
-    user = User(name=username, email=email, user_pass_pub_devices=[pub_key], pub_key=pub_key)
+    user: User = get_user_by_name(app, username=username).get()
+
+    if invitation != Code.one_way_hash(user.user_pass_sync, "CM", "get_magick_link_email"):
+        return Result.default_user_error(info=f"Invalid invitation", interface=ToolBoxInterfaces.remote)
+
+    user.user_pass_pub_devices.append(pub_key)
+    user.pub_key = pub_key
 
     db_delete_invitation(app, invitation)
 
     if web_data:
         return initialize_and_return(app, user)
 
     result_s = db_helper_save_user(app, asdict(user))
@@ -266,74 +379,105 @@
                      data=Code().encrypt_asymmetric(str(user.name), pub_key)
                      , interface=ToolBoxInterfaces.remote)
 
 
 class PersonalData(BaseModel):
     userId: str
     username: str
-    attestationObj: str  # arrayBufferToBase64
-    clientJSON: str  # arrayBufferToBase64
     pk: str  # arrayBufferToBase64
     pkAlgo: int
     authenticatorData: str  # arrayBufferToBase64
+    clientJson: str  # arrayBufferToBase64
     sing: str
     rawId: str  # arrayBufferToBase64
+    registration_credential: CustomRegistrationCredential
 
 
 @export(mod_name=Name, api=True, test=False)
 def register_user_personal_key(app: App, data: PersonalData) -> ApiResult:
     if not db_helper_test_exist(app, data.username):
         return Result.default_user_error(info=f"Username '{data.username}' not known")
 
     user_result = get_user_by_name(app, data.username, from_base64(data.userId).decode())
 
     if user_result.is_error() and not user_result.is_data():
         return Result.default_internal_error(info="No user found", data=user_result)
 
-    client_json = json.loads(from_base64(data.clientJSON))
+    client_json = json.loads(from_base64(data.clientJson))
     challenge = client_json.get("challenge")
     origin = client_json.get("origin")
-    crossOrigin = client_json.get("crossOrigin")
+    # crossOrigin = client_json.get("crossOrigin")
 
     if challenge is None:
         return Result.default_user_error(info="No challenge found in data invalid date parsed", data=user_result)
 
-    valid_origen = ["simpleCore.app", "http://localhost:5000"] + (["http://localhost:5000"] if app.debug else [])
+    valid_origen = ["https://simplecore.app", "http://localhost:5000"] + (
+        ["http://localhost:5000"] if app.debug else [])
 
     if origin not in valid_origen:
-        return Result.default_user_error(info=f'Invalid origen:{origin} not in {valid_origen}', data=user_result)
+        return Result.default_user_error(info=f'Invalid origen: {origin} not in {valid_origen}', data=user_result)
 
     user: User = user_result.get()
 
     if not challenge == to_base64(user.challenge).decode():
         return Result.default_user_error(info="Invalid challenge returned", data=user)
 
     if not Code.verify_signature(signature=from_base64(data.sing), message=user.challenge, public_key_str=user.pub_key,
                                  salt_length=32):
         return Result.default_user_error(info="Verification failed Invalid signature")
+    # c = {   "id": data.rawId,   "rawId": data.rawId,   "response": {       "attestationObject": data.attestationObj,
+    # "clientDataJSON": data.clientJSON,       "transports": ["usb", "nfc", "ble", "internal", "cable", "hybrid"],
+    # },   "type": "public-key",   "clientExtensionResults": {},   "authenticatorAttachment": "platform",}
+    try:
+        registration_verification = webauthn.verify_registration_response(
+            credential=data.registration_credential,
+            expected_challenge=user.challenge.encode(),
+            expected_origin=valid_origen,
+            expected_rp_id=os.environ.get('HOSTNAME', 'localhost'),  # simplecore.app
+            require_user_verification=True,
+        )
+    except InvalidRegistrationResponse as e:
+        return Result.default_user_error(info=f"Registration failure : {e}")
+
+    if not registration_verification.user_verified:
+        return Result.default_user_error(info="Invalid registration not user verified")
+
+    user_persona_pub_key = {
+        'public_key': registration_verification.credential_public_key,
+        'sign_count': registration_verification.sign_count,
+        'credential_id': registration_verification.credential_id,
+        'rawId': data.rawId,
+        'attestation_object': registration_verification.attestation_object,
+    }
 
     user.challenge = ""
-    user.user_pass_pub_persona = data.pk
-    user.user_pass_pub_persona_id = data.rawId
+    user.user_pass_pub_persona = user_persona_pub_key
+    user.is_persona = True
+
+    if user.level == 0:
+        user.level = 2
 
     # Speichern des neuen Benutzers in der Datenbank
     save_result = db_helper_save_user(app, asdict(user))
     if save_result.is_error():
         return save_result.to_api_result()
 
-    return Result.ok(info="User registered successfully")
+    key = "01#" + Code.one_way_hash(user.user_pass_sync, "CM", "get_magick_link_email")
+    url = f"/web/assets/m_log_in.html?key={quote(key)}&name={user.name}"
+
+    return Result.ok(info="User registered successfully", data=url)
 
 
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.cli, test=False)
 def crate_local_account(app: App, username: str, email: str = '', invitation: str = '', create=None) -> Result:
     if app is None:
         app = get_app(Name + '.crate_local_account')
     user_pri = app.config_fh.get_file_handler("Pk" + Code.one_way_hash(username, "dvp-k")[:8])
-    if user_pri is not None:
-        return Result.ok(info="User already registered on this device")
+    if user_pri is not None and db_helper_test_exist(app=app, username=username):
+        return Result.default_user_error(info="User already registered on this device")
     pub, pri = Code.generate_asymmetric_keys()
     app.config_fh.add_to_save_file_handler("Pk" + Code.one_way_hash(username, "dvp-k")[:8], pri)
     if ToolBox_over == 'root' and invitation == '':
         invitation = db_crate_invitation(app)
     if invitation == '':
         return Result.default_user_error(info="No Invitation key provided")
 
@@ -353,17 +497,18 @@
 def local_login(app: App, username: str) -> Result:
     if app is None:
         app = get_app(Name + '.crate_local_account')
     user_pri = app.config_fh.get_file_handler("Pk" + Code.one_way_hash(username, "dvp-k")[:8])
     if user_pri is None:
         return Result.ok(info="No User registered on this device")
 
-    signature = Code.create_signature(get_to_sing_data(app, username=username).as_result().get(), user_pri)
+    signature = Code.create_signature(get_to_sing_data(app, username=username).as_result().get('challenge'), user_pri
+                                      , row=True)
 
-    res = jwt_get_claim(app, username, signature).as_result()
+    res = jwt_get_claim(app, username, signature, web=False).as_result()
 
     if res.info.exec_code != 0:
         return Result.custom_error(data=res, info="user login failed!", exec_code=res.info.exec_code)
 
     return Result.ok(info="Success", data=res.get())
 
 
@@ -377,63 +522,86 @@
     if user_result.is_error() and not user_result.is_data():
         return Result.default_user_error(info=f"User {username} is not a valid user")
 
     user: User = user_result.get()
 
     if user.challenge == "":
         user.challenge = Code.encrypt_asymmetric(str(uuid.uuid4()), user.user_pass_pub)
+        db_helper_save_user(app, asdict(user))
 
     data = {'challenge': user.challenge}
 
     if personal_key:
-        data['rowId'] = user.user_pass_pub_persona_id
+        data['rowId'] = user.user_pass_pub_persona.get("rawId")
 
     return Result.ok(data=data)
 
 
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.native, api=False, level=999, test=False)
 def get_invitation(app: App) -> Result:
     if app is None:
         app = get_app(Name + '.test_invations')
-    print("Test invations api")
-    invitation = db_crate_invitation(app)
+
+    invitation = "00#" + str(Code.generate_seed())  # db_crate_invitation(app)
     return Result.ok(data=invitation)
 
 
 # a sync contention between server and user
 
 class VdUSER(BaseModel):
     username: str
     signature: str
 
 
 class VpUSER(VdUSER, BaseModel):
-    clientJSON: str
-    authenticatorData: str
+    authentication_credential: CustomAuthenticationCredential
 
 
 @export(mod_name=Name, api=True, test=False)
 def validate_persona(app: App, data: VpUSER) -> ApiResult:
     if app is None:
-        app = get_app(".validate_device")
+        app = get_app(".validate_persona")
 
     user_result = get_user_by_name(app, data.username)
 
     if user_result.is_error() or not user_result.is_data():
         return Result.default_user_error(info=f"Invalid username : {data.username}")
+    # from_base64(data.signature)
+    user: User = user_result.get()
 
-    jwt_claim = jwt_get_claim(app, data.username, from_base64(data.signature))
+    if user.is_persona == "":
+        return Result.default_user_error(info="No Persona key registered")
 
-    if isinstance(jwt_claim, ApiResult):
-        jwt_claim = jwt_claim.as_result()
+    valid_origen = ["https://simplecore.app", "http://localhost:5000"] + (
+        ["http://localhost:5000"] if app.debug else [])
 
-    if jwt_claim.is_error():
-        return jwt_claim.custom_error(data=jwt_claim, info="Error Processing user data")
+    try:
+        authentication_verification = webauthn.verify_authentication_response(
+            # Demonstrating the ability to handle a stringified JSON version of the WebAuthn response
+            credential=data.authentication_credential,
+            expected_challenge=user.challenge.encode(),
+            expected_rp_id=os.environ.get('HOSTNAME', 'localhost'),
+            expected_origin=valid_origen,
+            credential_public_key=user.user_pass_pub_persona.get("public_key"),
+            credential_current_sign_count=user.user_pass_pub_persona.get("sign_count"),
+            require_user_verification=True,
+        )
+        print(f"\n[Authentication Verification {user.name}]")
+        user.user_pass_pub_persona["sign_count"] = authentication_verification.new_sign_count
+    except InvalidAuthenticationResponse as e:
+        print(f"0Error authenticating user {data.username}, {e}")
+        return Result.default_user_error(info=f"Authentication failure : {e}")
 
-    return Result.ok(data=jwt_claim.get())
+    save_result = db_helper_save_user(app, asdict(user))
+    if save_result.is_error():
+        return save_result.to_api_result()
+
+    key = "01#" + Code.one_way_hash(user.user_pass_sync, "CM", "get_magick_link_email")
+    url = f"/web/assets/m_log_in.html?key={quote(key)}&name={user.name}"
+    return Result.ok(data=url, info="Auto redirect")
 
 
 @export(mod_name=Name, api=True, test=False)
 def validate_device(app: App, data: VdUSER) -> ApiResult:
     if app is None:
         app = get_app(".validate_device")
 
@@ -443,80 +611,92 @@
         return Result.default_user_error(info=f"Invalid username : {data.username}")
 
     user: User = user_result.get()
 
     valid = False
 
     for divce_keys in user.user_pass_pub_devices:
-
         valid = Code.verify_signature(signature=from_base64(data.signature),
                                       message=user.challenge,
                                       public_key_str=divce_keys,
                                       salt_length=32)
-
-        user.pub_key = divce_keys
-
         if valid:
+            user.pub_key = divce_keys
             break
 
     if not valid:
         return Result.default_user_error(info=f"Invalid signature : {data.username}")
 
     user.challenge = ""
     if user.user_pass_pri == "":
         user = UserCreator(**asdict(user))
     db_helper_save_user(app, asdict(user))
 
     claim = {
-        "pub": user.user_pass_pub,
         "u-key": user.uid,
     }
 
     row_jwt_claim = crate_jwt(claim, user.user_pass_pri)
 
-    return Result.ok(data=Code.encrypt_symmetric(row_jwt_claim, user.pub_key))
+    encrypt_jwt_claim = Code.encrypt_asymmetric(row_jwt_claim, user.pub_key)
+    print(encrypt_jwt_claim)
+    if encrypt_jwt_claim != "Invalid":
+        data = {'key': encrypt_jwt_claim, 'toPrivat': True}
+    else:
+        data = {'key': row_jwt_claim, 'toPrivat': False}
+
+    return Result.ok(data=data)
 
 
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.remote, api=True, test=False)
-def authenticate_user_get_sync_key(app: App, username: str, signature: str, get_user=False) -> ApiResult:
+def authenticate_user_get_sync_key(app: App, username: str, signature: str or bytes, get_user=False,
+                                   web=False) -> ApiResult:
     if app is None:
         app = get_app(Name + '.authenticate_user_get_sync_key')
 
     user: User = get_user_by_name(app, username).get()
 
     if user is None:
         return Result.default_internal_error(info="User not found", exec_code=404)
 
-    if not Code.verify_signature(signature=signature,
-                                 message=user.challenge if user.challenge else username + app.id + instance_bios,
-                                 public_key_str=user.user_pass_pub_persona):
-        return Result.default_user_error(info="Verification failed Invalid signature")
+    if web:
+        if not Code.verify_signature_web_algo(signature=signature,
+                                              message=to_base64(
+                                                  user.challenge),
+                                              public_key_str=user.pub_key):
+            return Result.default_user_error(info="Verification failed Invalid signature")
+    else:
+        if not Code.verify_signature(signature=signature,
+                                     message=user.challenge,
+                                     public_key_str=user.pub_key):
+            return Result.default_user_error(info="Verification failed Invalid signature")
 
     user = UserCreator(**asdict(user))
 
     db_helper_save_user(app, asdict(user))
 
     crypt_sync_key = Code.encrypt_asymmetric(user.user_pass_sync, user.pub_key)
 
     if get_user:
-        Result.ok(data_info="Returned Sync Key, read only for user", data=(crypt_sync_key, asdict(user)))
+        return Result.ok(data_info="Returned Sync Key, read only for user (withe user_data)",
+                         data=(crypt_sync_key, asdict(user)))
 
     return Result.ok(data_info="Returned Sync Key, read only for user", data=crypt_sync_key)
 
 
 # local user functions
 
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.native, test=False)
 def get_user_sync_key_local(app: App, username: str, ausk=None) -> Result:
     if app is None:
         app = get_app(Name + '.get_user_sync_key')
 
     user_pri = app.config_fh.get_file_handler("Pk" + Code.one_way_hash(username)[:8])
 
-    signature = Code.create_signature(username + app.id + instance_bios, user_pri)
+    signature = Code.create_signature(get_to_sing_data(app, username=username).get('challenge'), user_pri)
 
     authenticate_user_get_sync_key_ = lambda *args: authenticate_user_get_sync_key(*args)
     if ausk is not None:
         authenticate_user_get_sync_key_ = ausk
 
     res = authenticate_user_get_sync_key_(app, username, signature).as_result()
 
@@ -529,26 +709,25 @@
 
     return Result.ok(info="Success", data=Code.decrypt_asymmetric(sync_key, user_pri))
 
 
 # jwt claim
 
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.remote, api=True, test=False)
-def jwt_get_claim(app: App, username: str, signature: str or bytes) -> ApiResult:
+def jwt_get_claim(app: App, username: str, signature: str or bytes, web=False) -> ApiResult:
     if app is None:
         app = get_app(Name + '.jwt_claim_server_side_sync')
 
-    res = authenticate_user_get_sync_key(app, username, signature, get_user=True).as_result()
+    res = authenticate_user_get_sync_key(app, username, signature, get_user=True, web=web).as_result()
 
     if res.info.exec_code != 0:
         return res.custom_error(data=res)
 
     channel_key, userdata = res.get()
     claim = {
-        "pub": userdata.get("user_pass_pub"),
         "u-key": userdata.get("uid"),
     }
 
     row_jwt_claim = crate_jwt(claim, userdata.get("user_pass_pri"))
 
     return Result.ok(
         data={'claim': Code.encrypt_symmetric(row_jwt_claim, userdata.get("pub_key")), 'key': channel_key})
@@ -573,44 +752,108 @@
 @export(mod_name=Name, state=True, interface=ToolBoxInterfaces.remote, api=True, test=False)
 def jwt_check_claim_server_side(app: App, username: str, jwt_claim: str) -> ApiResult:
     res = get_user_by_name(app, username)
     if res.info.exec_code != 0:
         return Result.custom_error(data=res)
     user: User = res.get()
 
-    data = validate_jwt(jwt_claim, user.pub_key)
-
+    data = validate_jwt(jwt_claim, user.user_pass_pub)
+    # InvalidSignatureError
     if isinstance(data, str):
-        return Result.custom_error(info=data, data=False)
+        return Result.custom_error(info="Invalid", data=False)
 
     return Result.ok(data_info='Valid JWT', data=True)
 
 
 # ============================= Unit tests ===========================================
 
 # set up
 @export(mod_name=Name, test_only=True, initial=True, state=False)
 def prep_test():
     app = get_app(f"{Name}.prep_test")
     app.run_any(tbef.DB.EDIT_PROGRAMMABLE, mode=DatabaseModes.LC)
 
 
+def get_test_app_gen(app=None):
+    if app is None:
+        app = get_app('test-app', name='test-debug')
+    yield app
+    # Teardown-Logik hier, falls benötigt
+
+
+def helper_gen_test_app():
+    _ = get_test_app_gen(None)
+    TestAppGen.t = _, next(_)
+    prep_test()
+    return TestAppGen
+
+
+class TestAppGen:
+    t: tuple
+
+    @staticmethod
+    def get():
+        return TestAppGen.t
+
+
+@test_only
+def test_user():
+    app: App
+    test_app, app = helper_gen_test_app().get()
+    username = "testUser123"+uuid.uuid4().hex
+    email = "test_mainqmail.com"
+    db_helper_delete_user(app, username, "*", matching=True)
+    # Benutzer erstellen
+    r = crate_local_account(app, username, email, get_invitation(app).get())
+    assert not r.is_error(), r.print(show=False)
+    r = crate_local_account(app, username, email, get_invitation(app).get())
+    assert r.is_error(), r.print(show=False)
+    # Aufräumen
+    db_helper_delete_user(app, username, "*", matching=True)
+    app.config_fh.remove_key_file_handler("Pk" + Code.one_way_hash(username, "dvp-k")[:8])
+    return Result.ok()
+
+
+@test_only
+def test_create_user_and_login():
+    app: App
+    test_app, app = helper_gen_test_app().get()
+    username = "testUser123"+uuid.uuid4().hex
+    email = "test_mainqmail.com"
+    r = crate_local_account(app, username, email, get_invitation(app).get())
+    r2 = local_login(app, username)
+    assert not r.is_error(), r.print(show=False)
+    assert not r2.is_error(), r2.print(show=False)
+    app.config_fh.remove_key_file_handler("Pk" + Code.one_way_hash(username, "dvp-k")[:8])
+    db_helper_delete_user(app, username, "*", matching=True)
+    return Result.ok()
+
+
 @test_only
-def crate_user_test(app: App):
+def test_validate_device(app: App = None):
     if app is None:
-        app = get_app(f"{Name}.crate_user_test")
-    r = crate_local_account(app, "testUser123", "test_mainqmail.com", get_invitation(app).get())
-    r2 = local_login(app, "testUser123").lazy_return("crate_local_account + local_login failed")
-    res = [[r.is_error() is False, "r.is_error() "], [r2.is_error() is False, "r2.is_error()"],
-           [r.is_data() is True, "r.is_data() i"], [r2.is_data() is True, "r2.is_data() "],
-           [r.result.data_info == "Success", "r.result.data"], [r2.result.data_info == "Success", "r2.result.dat"]]
-    return res
+        app = get_app(f"{Name}.test_validate_device", name="test-debug")
 
+    # Schritt 1: Benutzer erstellen
+    username = "testUser"+uuid.uuid4().hex
+    email = "test@example.com"
+    pub_key, pri_key = Code.generate_asymmetric_keys()
+    user = UserCreator(name=username, email=email, user_pass_pub_devices=[pub_key], pub_key=pub_key)
+    db_helper_save_user(app, asdict(user))
 
+    # Schritt 2: Signatur generieren
+    signature = Code.create_signature(get_to_sing_data(app, username=username).as_result().get('challenge'),
+                                      pri_key, row=False, salt_length=32)
+
+    # Schritt 3: Testdaten vorbereiten
+    test_data = VdUSER(username=username, signature=signature)
+    # Schritt 4: validate_device Funktion testen
+    result = validate_device(app, test_data).as_result()
+    result.print()
+    # Schritt 5: Ergebnisse überprüfen
+    assert not result.is_error(), f"Test fehlgeschlagen: {result.print(show=False)}"
+    assert result.is_data(), "Kein Schlüssel im Ergebnis gefunden"
 
-if __name__ == '__main__':
-    singen = "HhSdUTQO0wKhKpBPg34422My3kciycjZPHnFRHboVFL5pDQikPTcLGhxjqP0xWUIVh+FbpOsIywCCPjRL7IlPBxmA3Zrb0YcWq3j4I11GORF6mCVoiJX3Qq2eDFBg27lR7bmP3QfFFjEDJrFXs2pNKSaCKfZrEH9tgnm7lq9tXnzOMoeHi+kO1StnWjO5qmlvodymeyAGMnBKpomgxP2we+cznlgb9Mk7GY9Mm0S4YFj2fNX6Fra7xCxtB+ErycTRCVPrTayQ2cwqBZ0LI5jNRaqJVOPXD5U8fiMnaNlOu1bMu9FtTVnqHfszK5qy9OVyKia0xyo2UdGOfymNJSFyJ+y3JJGnhdhuS0I2za25p/K7I5xwGEL5lIBpj+JaRV5pOwDcxGhn21Q/82VsmAseT7V4TbdrSSOo6bjycRiARiwl1LgzsUhQ8CPa86x3KxzYWddvNh3aRTqCoaPWfsnJHywZXi6gPZbsCVcytOnkxOZep6TfdULstyFNjvKO9X/UmLl9Qzc5rpmjGg8gYFju05lN+IWe5qCbbgNrydn615Y30Z15G88ZwWkzs/q/n2CkzUyBLK1nrt4hPt4SXzF02/3EYTl2JhUS1je0GDfgmcVSQ+Yhr/mfHhKfS0zQBtCFm0ua9AmcqrJu7B8+InONh16WBRdHmFUUundyifj3QcZBEJRvU4gF1xq+0cDNta0XnLgpl+FVJsliKycGYkAUuohMAysznLen1bG0TuorPNHAutWOu3JBdx/BHdc2001bUIuzJ5Gg8Mnx8PUy83g2JSE4CFtNFoutlhaY5XdD4ElzPdbFgMX6N+e9ZGYIYG/4H1QBzB3qkkWbpDLVOqtNKDnTma602pHQJOtns9qkIcmwlYmJK/4USZDjAj1zSX3n+u4RttBdsvmRiehMyJ4e1A5y5Rf7r2mLtzo3EaTYvu27evKrMmWfiR0/cgTdhxhlM9gXAi8Sq///HX+vL38lcibIypScBtGV09cHSCEl/Dmm4ZsFM2ppsbUqRkcWhcI"
-    msg = "0c538a042e321b968daab931ec9445dcafd7b12e1c30a338ae3a5fdd87a122188521d832fcc05741017921673f16a1491affc176f40feda81c9dc4621526748fb97af5a953df0b99be7fb0e4fa80679ebe3dbab973897d4a8baa0a209b6296757396297f0bb2cd0d3a97b892da12e1da108a7724126afcb1c3a70abb40ce3429b6333252999478731da82e0b2be355085cc5e80ecfd9fdf5d908e6fe66bf980bb9fcdf6d578dd83cf4d9f373a4bf65e9285d789e1a1b352dd12301b69f8a75ffce1679c1d767cc53bcee73da5e8cb6fb4f699dbbd429e3ffbf2e67ef57820706369e07d45f11198e528ba7ee83748ac3492060d2d611f61c4004cf8b522770d04091d277c884374970eda7c27b1bb3374f0d264f5b0e1384a83ebe29079bb274b41692f8fcec85147727c055ecfbdac51a136eb94de1f9b80f673463e6fb0aaa400db63f48a9c502cf551be39309b13fac027ccb8e69c384c0f127d56beb80d45fee60e93d69cae39dac74d2db6a0cb4a495d087ddbfb85ef3402ba19b82bc098287d9e53bf50402c7edf57e2c462c4db12ea94dff900a734e504c4c3ed90c80bc3cbc183a3e3510c86a8b123783c5b400a003fb1d8f299a897b209df8a18541550c82841867b642efd1e53435ea32bc105c7dc58d12c9d7b3eea41d63f6ab2a5e7424024fd87b35a91523d463f6016e40deccdea9ae559850b60a75e917120e6cbd209e1e00ff6f0e2ddd3c30c02a39af8ba9cf11ae9d7651afbfe9736df3d38a021297ccb11bdbe2b03a2ee603fdb5523f5f891ad482928eecba31f3e541793e87a0d8327ce7f1aa40c3f07015e712ea9af42ba51fddd42f5ce53c17ea01463f2b8722d94f928c285a35722e30694984fa79443d5ef91008205361b3936a50608436176fd23ffcece86339d79c510dcd73f7db5147d744625610ef2a776218d484c0e6173ffdaea28b6c131d62cef5d82f751c35fd7f70a02ae9c29197ac86a784b6957c2bf872aa408199b0e729e8712a30d73c745a061f914fcccd84ded5da9450ff47f8fd56ad8d803e4fbb1f0885801ed242fd30b9296a4d29dbd8556f', '"
-    key = "-----BEGIN PUBLIC KEY-----\nMIIDIjANBgkqhkiG9w0BAQEFAAOCAw8AMIIDCgKCAwEAjuWAq+adexJOA4SYLNjl\nSvY0QirC/kVAX2hWcC/93qer2WT1rd4CbK0h5zRhglgBpG5zYmwllqROfJdpfQSN\nHomq7zwz+IGqs7KKGvpXgIRyDdoFcvc5IfMjaVCu8tq7OEU7w1jjIRxcInlucgsk\nayJ9qeTtzbZo/4b1wiaPwIEhn1H//30IA0WOMNO0pffXRFFY7tnbuMBmSrPPkMTY\ngycTUKIOR+8bAyozLRMOwBZzT0f1EcJWL14QDIhb7FNAjjyw3a/QK62Laq2yEoUn\nTB90Ej/AuN133mhOQfqLKo4UR39mmVTP9PvqgCy/JlwMbiV8qHaX46WjmV4qB6Lt\nTQMQFBiulVHrKJJP99Nw7aEW0PLCaRPfJt/UN+YLgisUNSZIO/Cru7uF+kbsCoa0\nqGUldDmeqQaANLASR1SW2AHNl/m/L3yS/ZBSqw6p20RjlIwWh/2Pj5q81T/Z6hgG\nuib5BEU6U3D/MPWmdhxeaO9tVgF1gz0ENXlm7B9FZrZrpuIUMJh8tX+NAL9uLRGx\nnR28WQxGnnyh9vS6VBFq0Oo1xc8GaComL+UgiMi/L3mtzCUO3yyX3eoezJOZPNm+\nuCyz+I6RGXdxr5Vewksyqh80YyCjXj8NnP+k43nAM2GJf9toM8dP7RqOrQfpn3NB\njWaQLgAVkEZmat3blA/JSof/yb+fzmmAcsMhUYWGQttxW6KF8pKKzd6EPdeZu3Mu\nMzDfcwY6c3Pqmcn5cSF+S9dOLJBhehnILYatrlHdyohCdqiaxcBL5BM+N9AaEwHQ\nFPs26HgyjRgHuqSKRlF34n+KnLInSh4ReNXD05N9RSRNU4zRDW1WAB4jTl29z87C\ns7sGb1jhfu6jVCGnqelKhhoRcH2WX9+e49/mXYtNn/LSDXO3wEXvE4f3wVC5ck1l\n3cKCEDm9Fs6Ix1E90YUW17p+g7ZT+adJtChP8RYMv2n29FlautuFxjmIsncShAi7\nCXYfjyawdkDTGme78G2DvM09fw7u6LMbwzYn9rQMk6RtAgMBAAE=\n-----END PUBLIC KEY-----\n"
+    # Aufräumen: Benutzer aus der Datenbank entfernen
+    db_helper_delete_user(app, username, user.uid)
 
-    print(Code.verify_signature(singen, msg, key))
-    print(Code.verify_signature(singen, to_base64(msg).decode(), key))
+    return Result.ok()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/ModManager.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/ModManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,24 @@
 
     # Requirements installieren
     handle_requirements(data.get("requirements"), data.get("Name"), print_debug)
 
     print_debug("Installation abgeschlossen")
 
 
-def download_files(urls, directory, desc, print_func):
+def download_files(urls, directory, desc, print_func, filename=None):
     """ Hilfsfunktion zum Herunterladen von Dateien. """
     for url in tqdm(urls, desc=desc):
-        filename = os.path.basename(url)
+        if filename is None:
+            filename = os.path.basename(url)
         print_func(f"Download {filename}")
-        urllib.request.urlretrieve(url, f"{directory}/{filename}")
+        print_func(f"{url} -> {directory}\\{filename}")
+        os.makedirs(directory, exist_ok=True)
+        urllib.request.urlretrieve(url, f"{directory}\\{filename}")
+    return f"{directory}\\{filename}"
 
 
 def handle_additional_dirs(additional_dirs_url, print_func):
     """ Verarbeitet zusätzliche Verzeichnisse. """
     if additional_dirs_url:
         print_func(f"Download additional dirs {additional_dirs_url}")
         shutil.unpack_archive(additional_dirs_url, "/")
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/UserInstances.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/UserInstances.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from toolboxv2 import Style, get_app, tbef
+from toolboxv2 import Style, get_app
 from toolboxv2.utils import Singleton
 from toolboxv2.utils.cryp import Code
 from toolboxv2.utils.types import Result
 
 app = get_app("UserInstances")
 logger = app.logger
 Name = "CloudM.UserInstances"
@@ -16,54 +16,51 @@
 
 class UserInstances(metaclass=Singleton):
     live_user_instances = {}
     user_instances = {}
 
     @staticmethod
     @in_mem_chash_150
-    def get_si_id(uid: str):
+    def get_si_id(uid: str) -> Result or str:
         return Code.one_way_hash(uid, app.id, 'SiID')
 
     @staticmethod
     @in_mem_chash_150
-    def get_vt_id(uid: str):
+    def get_vt_id(uid: str) -> Result or str:
         return Code.one_way_hash(uid, app.id, 'VirtualInstanceID')
 
     @staticmethod
     @in_mem_chash_150
-    def get_web_socket_id(uid: str):
+    def get_web_socket_id(uid: str) -> Result or str:
         return Code.one_way_hash(uid, app.id, 'CloudM-Signed')
 
     # UserInstanceManager.py
 
 
 @e
 def close_user_instance(uid: str):
     if uid is None:
         return
-    if UserInstances.get_si_id(uid).get()not in UserInstances().live_user_instances.keys():
+    si_id = UserInstances.get_si_id(uid).get()
+    if si_id not in UserInstances().live_user_instances.keys():
         logger.warning("User instance not found")
         return "User instance not found"
-    instance = UserInstances().live_user_instances[UserInstances.get_si_id(uid).get()]
+    instance = UserInstances().live_user_instances[si_id]
     UserInstances().user_instances[instance['SiID']] = instance['webSocketID']
     app.run_any(
-        'db', 'set',
-        query=f"User::Instance::{uid}", data=
-        json.dumps({"saves": instance['save']}))
+        'DB', 'set',
+        query=f"User::Instance::{uid}",
+        data=json.dumps({"saves": instance['save']}))
     if not instance['live']:
         save_user_instances(instance)
         logger.info("No modules to close")
         return "No modules to close"
-    for key, val in instance['live'].items():
-        if key.startswith('v-'):
-            continue
-        try:
-            val._on_exit()
-        except Exception as e:
-            logger.error(f"Error closing {key}, {str(e)}")
+    for mode_name, spec in instance['live'].items():
+        logger.info(f"Closing {mode_name}")
+        app.remove_mod(mod_name=mode_name, spec=spec, delete=False)
     del instance['live']
     instance['live'] = {}
     logger.info("User instance live removed")
     save_user_instances(instance)
 
 
 @e
@@ -73,16 +70,16 @@
         data = app.run_any('DB', 'get',
                            query=f"user_instances::{app.id}")
         logger.info(f"validate_ws_id 2 {type(data)} {data}")
         if isinstance(data, str):
             try:
                 UserInstances().user_instances = json.loads(data)
                 logger.info(Style.GREEN("Valid instances"))
-            except Exception as e:
-                logger.info(Style.RED(f"Error : {str(e)}"))
+            except Exception as e_:
+                logger.info(Style.RED(f"Error : {str(e_)}"))
     logger.info(f"validate_ws_id ::{UserInstances().user_instances}::")
     for key in list(UserInstances().user_instances.keys()):
         value = UserInstances().user_instances[key]
         logger.info(f"validate_ws_id ::{value == ws_id}:: {key} {value}")
         if value == ws_id:
             return True, key
     return False, ""
@@ -95,64 +92,26 @@
     si_id = UserInstances.get_si_id(uid).get()
     if si_id not in UserInstances().user_instances.keys():
         return "User instance not found"
     if si_id in UserInstances().live_user_instances.keys():
         del UserInstances().live_user_instances[si_id]
 
     del UserInstances().user_instances[si_id]
-    app.run_any('db', 'del', query=f"User::Instance::{uid}")
+    app.run_any('DB', 'delete', query=f"User::Instance::{uid}")
     return "Instance deleted successfully"
 
 
-@export(mod_name=Name, state=False)
-def set_user_level():  # TODO Ad to user date default
-
-    if not UserInstances().live_user_instances.items():
-        app.print(f"User: No users registered")
-        return
-
-    users, keys = [(u['save'], _) for _, u in UserInstances().live_user_instances.items()]
-    users_names = [u['username'] for u in users]
-    for user in users:
-        app.print(f"User: {user['username']} level : {user['level']}")
-
-    rot_input = input("Username: ")
-    if not rot_input:
-        app.print(Style.YELLOW("Please enter a username"))
-        return "Please enter a username"
-    if rot_input not in users_names:
-        app.print(Style.YELLOW("Please enter a valid username"))
-        return "Please enter a valid username"
-
-    user = users[users_names.index(rot_input)]
-
-    app.print(Style.WHITE(f"Usr level : {user['level']}"))
-
-    level = input("set level :")
-    level = int(level)
-
-    instance = UserInstances().live_user_instances[keys[users_names.index(rot_input)]]
-
-    instance['save']['level'] = level
-
-    save_user_instances(instance)
-
-    app.print("done")
-
-    return True
-
-
 @e
 def save_user_instances(instance: dict):
     if instance is None:
         return
     logger.info("Saving instance")
     UserInstances().user_instances[instance['SiID']] = instance['webSocketID']
     UserInstances().live_user_instances[instance['SiID']] = instance
-    print(UserInstances().user_instances)
+    # print(UserInstances().user_instances)
     app.run_any(
         'DB', 'set',
         query=f"user_instances::{app.id}",
         data=json.dumps(UserInstances().user_instances))
 
 
 @e
@@ -160,59 +119,54 @@
     if si_id in UserInstances().live_user_instances:
         return UserInstances().live_user_instances[si_id]
     return False
 
 
 @e
 def get_user_instance(uid: str,
-                      username: str or None = None,
-                      token: str or None = None,
                       hydrate: bool = True):
     # Test if an instance exist locally -> instance = set of data a dict
     if uid is None:
         return
     instance = {
         'save': {
             'uid': uid,
-            'level': 0,
             'mods': [],
-            'username': username
         },
         'live': {},
         'webSocketID': UserInstances.get_web_socket_id(uid).get(),
         'SiID': UserInstances.get_si_id(uid).get(),
-        'token': token
+        'VtID': UserInstances.get_vt_id(uid).get()
     }
 
     if instance['SiID'] in UserInstances().live_user_instances.keys():
-        instance_live = UserInstances().live_user_instances.get([instance['SiID']], {})
+        instance_live = UserInstances().live_user_instances.get(instance['SiID'], {})
         if 'live' in instance_live.keys():
             if instance_live['live'] and instance_live['save']['mods']:
                 logger.info(Style.BLUEBG2("Instance returned from live"))
                 return instance_live
-            if instance_live['token']:
-                instance = instance_live
-                instance['live'] = {}
     chash = {}
     if instance['SiID'] in UserInstances().user_instances.keys(
     ):  # der nutzer ist der server instanz bekannt
         instance['webSocketID'] = UserInstances().user_instances[instance['SiID']]
     else:
         chash_data = app.run_any('DB', 'get', query=f"User::Instance::{uid}", get_results=True)
         if not chash_data.is_data():
             chash = {"saves": instance['save']}
         else:
             chash = chash_data.get()
     if chash != {}:
         app.print(chash)
-        try:
-            instance['save'] = json.loads(chash)["saves"]
-        except Exception as er:
+        if isinstance(chash, dict):
             instance['save'] = chash["saves"]
-            logger.error(Style.YELLOW(f"Error loading instance {er}"))
+        else:
+            try:
+                instance['save'] = json.loads(chash)["saves"]
+            except Exception as er:
+                logger.error(Style.YELLOW(f"Error loading instance {er}"))
 
     logger.info(Style.BLUEBG(f"Init mods : {instance['save']['mods']}"))
 
     app.print(Style.MAGENTA(f"instance : {instance}"))
 
     #   if no instance is local available look at the upper instance.
     #       if instance is available download and install the instance.
@@ -227,56 +181,41 @@
 
     return instance
 
 
 @e
 def hydrate_instance(instance: dict):
     # instance = {
-    # 'save': {'uid':'INVADE_USER','level': -1, 'mods': []},
+    # 'save': {'uid':'INVADE_USER', 'mods': []},
     # 'live': {},
     # 'webSocketID': 0000,
     # 'SiID': 0000,
     # }
 
     if instance is None:
         return
 
     chak = instance['live'].keys()
-    level = instance['save']['level']
-
-    # app . key generator
-    user_instance_name = UserInstances.get_vt_id(instance['save']['uid']).get()
 
     for mod_name in instance['save']['mods']:
 
         if mod_name in chak:
             continue
 
-        user_instance_name_mod = mod_name + '-' + user_instance_name
-
-        mod = app.get_mod(mod_name, user_instance_name)
+        mod = app.get_mod(mod_name, instance['VtID'])
         app.print(f"{mod_name}.instance_{mod.spec} online")
 
-        instance['live'][mod_name] = mod
-        instance['live']['v-' + mod_name] = user_instance_name_mod
+        instance['live'][mod_name] = mod.spec
 
     return instance
 
 
 @export(mod_name=Name, state=False)
 def save_close_user_instance(ws_id: str):
     valid, key = validate_ws_id(ws_id)
     if valid:
         user_instance = UserInstances().live_user_instances[key]
-        logger.info(f"Log out User : {user_instance['save']['username']}")
-        for key, mod in user_instance['live'].items():
-            logger.info(f"Closing {key}")
-            if isinstance(mod, str):
-                continue
-            try:
-                mod.on_exit()
-            except Exception as e:
-                logger.error(f"error closing mod instance {key}:{e}")
+        logger.info(f"Log out User : {ws_id}")
         close_user_instance(user_instance['save']['uid'])
 
         return Result.ok()
     return Result.default_user_error(info="invalid ws id")
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/extras.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/isaaclip2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,252 +1,213 @@
-import os
-import sys
-from pathlib import Path
-
-import requests
-from toolboxv2 import Style, Result
-from .AuthManager import get_invitation
-from toolboxv2 import get_app, Code
-
-Name = 'CloudM'
-version = "0.0.2"
-export = get_app(f"{Name}.EXPORT").tb
-no_test = export(mod_name=Name, test=False, version=version)
-to_api = export(mod_name=Name, api=True, version=version)
-
-
-@no_test
-def new_module(self, mod_name: str,
-               *options):  # updater wie AI Fuctonal and class based hybrie , file / folder |<futüre>| rust py
-    self.logger.info(f"Crazing new module : {mod_name}")
-    boilerplate = """import logging
-from toolboxv2 import MainTool, FileHandler, App, Style
-
-
-class Tools(MainTool, FileHandler):
-
-    def __init__(self, app=None):
-        self.version = "0.0.2"
-        self.name = "NAME"
-        self.logger: logging.Logger or None = app.logger if app else None
-        self.color = "WHITE"
-        # ~ self.keys = {}
-        self.tools = {
-            "all": [["Version", "Shows current Version"]],
-            "name": "NAME",
-            "Version": self.show_version, # TODO if functional replace line with [            "Version": show_version,]
-        }
-        # ~ FileHandler.__init__(self, "File name", app.id if app else __name__, keys=self.keys, defaults={})
-        MainTool.__init__(self, load=self.on_start, v=self.version, tool=self.tools,
-                        name=self.name, logs=self.logger, color=self.color, on_exit=self.on_exit)
-
-    def on_start(self):
-        self.logger.info(f"Starting NAME")
-        # ~ self.load_file_handler()
-
-    def on_exit(self):
-        self.logger.info(f"Closing NAME")
-        # ~ self.save_file_handler()
-
-"""
-    helper_functions_class = """
-    def show_version(self):
-        self.print("Version: ", self.version)
-        return self.version
-"""
-    helper_functions_func = """
-def get_tool(app: App):
-    return app.AC_MOD
-
-
-def show_version(_, app: App):
-    welcome_f: Tools = get_tool(app)
-    welcome_f.print(f"Version: {welcome_f.version}")
-    return welcome_f.version
-
-"""
-
-    self.logger.info(f"crating boilerplate")
-    if '-fh' in options:
-        boilerplate = boilerplate.replace('pass', '').replace('# ~ ', '')
-        self.logger.info(f"adding FileHandler")
-    if '-func' in options:
-        boilerplate += helper_functions_func
-        self.logger.info(f"adding functional based")
-    else:
-        boilerplate += helper_functions_class
-        self.logger.info(f"adding Class based")
-    self.print(f"Test existing {self.api_version=} ")
-
-    self.logger.info(f"Testing connection")
-
-    # self.get_version()
-
-    if self.api_version != '404':
-        if self.download(["", mod_name]):
-            self.print(
-                Style.Bold(Style.RED("MODULE exists-on-api pleas use a other name")))
-            return False
-
-    self.print("NEW MODULE: " + mod_name, end=" ")
-    if os.path.exists(f"mods/" + mod_name +
-                      ".py") or os.path.exists(f"mods_dev/" + mod_name +
-                                               ".py"):
-        self.print(Style.Bold(Style.RED("MODULE exists pleas use a other name")))
-        return False
-
-    fle = Path("mods_dev/" + mod_name + ".py")
-    fle.touch(exist_ok=True)
-    with open(f"mods_dev/" + mod_name + ".py", "wb") as mod_file:
-        mod_file.write(bytes(boilerplate.replace('NAME', mod_name),
-                             'ISO-8859-1'))
-
-    self.print("Successfully created new module")
-    return True
-
-
-@no_test
-def create_account(self):
-    version_command = self.app.config_fh.get_file_handler("provider::")
-    url = "https://simeplecore.app/app/signup"
-    if version_command is not None:
-        url = version_command + "/app/signup"
-    # os.system(f"start {url}")
-
-    try:
-        import webbrowser
-        webbrowser.open(url, new=0, autoraise=True)
-    except Exception as e:
-        self.logger.error(Style.YELLOW(str(e)))
-        self.print(Style.YELLOW(str(e)))
-        return False
-    return True
-
-
-@no_test
-def log_in(self, input_):
-    print(self, input_)
-    version_command = self.app.config_fh.get_file_handler("provider::")
-    url = "https://simeplecore.app/app/login"
-    if version_command is not None:
-        url = version_command + "/app/login"
-
-    if len(input_) == 3:
-        username = input_[1]
-        password = input_[2]
-
-        data = {"username": username, "password": password}
-
-        r = requests.post(url, json=data)
-        self.print(r.status_code)
-        self.print(str(r.content, 'utf-8'))
-        token = r.json()["token"]
-        error = r.json()["error"]
-
-        if not error:
-            claims = token.split(".")[1]
-            import base64
-            json_claims = base64.b64decode(claims + '==')
-            claims = eval(str(json_claims, 'utf-8'))
-            self.print(Style.GREEN(f"Welcome : {claims['username']}"))
-            self.print(Style.GREEN(f"Email : {claims['email']}"))
-            self.add_to_save_file_handler(self.keys["TOKEN"], token)
-            self.print("Saving token to file...")
-
-            self.on_exit()
-            self.load_open_file()
+import platform
+from urllib.parse import urlparse
 
-            self.print("Saved")
+import keyboard
 
-            return True
+# pyperclip.copy('The text to be copied to the clipboard.')
+# pyperclip.paste()
 
-        else:
-            self.print(Style.RED(f"ERROR: {error}"))
-    else:
-        self.print(
-            Style.RED(
-                f"ERROR: {input_} len {len(input_)} != 3 | login username password"))
-
-    return False
-
-
-@no_test
-def update_core(self, dackup=False, name=""):
-    self.print("Init Update..")
-    if dackup:
-        os.system("git fetch --all")
-        d = f"git branch backup-master-{self.app.id}-{self.version}-{name}"
-        os.system(d)
-        os.system("git reset --hard origin/master")
-    out = os.system("git pull")
-    self.app.remove_all_modules()
-    try:
-        com = " ".join(sys.orig_argv)
-    except AttributeError:
-        com = "python3 "
-        com += " ".join(sys.argv)
+import pyperclip
+from toolboxv2 import Style, tbef
+from dotenv import load_dotenv
+
+load_dotenv()
+NAME = "Iclip2"
+
+
+def get_speak_input():
+    pass
+
+
+def get_input(speek_mode=False, min_=30):
+    from toolboxv2.mods.isaa.isaa_modi import get_multiline_input
+    if speek_mode:
+        input("Start listig ->")
+        print("User (e) for exit:")
+        return get_multiline_input()
+    print("User (e) for exit:")
+    return get_multiline_input()
+
+
+def get_buffer(buffer):
+    if platform.system() != "Darwin":
+
+        event = keyboard.read_event()
 
-    if out == 0:
-        self.app.print_ok()
+        if event.event_type == keyboard.KEY_DOWN:
+            key_name = event.name
+
+            if key_name in ['backspace', 'enter', 'space']:
+                buffer = ' ' * 8
+            else:
+                buffer += str(key_name).lower()
+
+            print(buffer[len(buffer) - 8:], end='\r')
     else:
-        print("ther was an errer updateing...\n\n")
-        print(Style.RED(f"Error-code: os.system -> {out}"))
-        print(
-            "if you changet local files type $ cloudM #update-core save {name}")
-        print(
-            "your changes will be saved to a branch named : backup-master-{app.id}-{self.version}-{name}"
-        )
-        print(
-            "you can apply yur changes after the update with:\ngit stash\ngit stash pop"
-        )
-
-    if out == -1:
-        os.system("git fetch --all")
-        os.system("git reset --hard origin/master")
-
-    if "update" not in com:
-        print("Restarting...")
-        os.system(com)
-    exit(0)
-
-@no_test
-def register_initial_root_user(app, tbef=None):
-
-    root_key = app.config_fh.get_file_handler("Pk" + Code.one_way_hash("root", "dvp-k")[:8])
-
-    if root_key is not None:
-        return Result.default_user_error(info="root user already Registered")
-
-    email = input("enter ure Email:")
-    invitation = get_invitation().get()
-    app.run_any(tbef.AUTHMANAGER.CRATE_LOCAL_ACCOUNT, username="root", email=email,
-                     invitation=invitation)
-
-@no_test
-def clear_db(self, do_root=False):
-
-    db = self.app.get_mod('DB', spec=self.spec)
-
-    if db.data_base is None or not db:
-        self.print(
-            "No redis instance provided from db run DB first-redis-connection")
-        return "Pleas connect first to a redis instance"
-
-    if not do_root:
-        if 'y' not in input(
-            Style.RED("Ar u sure : the deb will be cleared type y :")):
-            return
-
-    db.delete('*', matching=True)
-    i = 0
-    for _ in db.get('all').get():
-        i += 1
-
-    if i != 0:
-        self.print("Pleas clean redis database first")
-        return "Data in database"
-    return True
-
-@to_api
-def show_version(self):
-    self.print(f"Version: {self.version} {self.api_version}")
-    return self.version
+        buffer = input(":")
+
+    return buffer
+
+
+def function_buffer_manager(buffer: str, functions: dict):
+    for name in functions.keys():
+        if name in buffer:
+            return functions[name]
+    return None
+
+
+def run(app, args):
+    from toolboxv2.mods.isaa import Tools as Isaa
+    from toolboxv2.mods.isaa.AgentFramwork import MarkdownRefactorMode
+    from toolboxv2.mods.isaa.subtools.file_loder import route_local_file_to_function
+    from toolboxv2.mods.isaa.subtools.web_loder import route_url_to_function
+    functions = {}
+    register = lambda n, f: functions.__setitem__(n, f)
+    speak_mode = [False, False]
+
+    # Trigger word to process the text
+    def toggle_helper(i):
+        def _(*_):
+            speak_mode[i] = not speak_mode[i]
+            print("set speak_mode: ", speak_mode)
+
+        return _
+
+    isaa: Isaa = app.get_mod("isaa")
+
+    isaa.summarization_mode = 1
+
+    isaa.register_agents_setter(lambda x: x
+                                .set_amd_model("ollama/llama2")
+                                .set_stream(True)
+                                .set_logging_callback(print_prompt)
+                                # .set_stream_function(stram_print)
+                                # .set_logging_callback(isaa.print)
+                                # .set_verbose(True)
+                                .set_max_tokens(1200)
+                                .set_amd_stop_sequence(['\n\n\n'])
+                                )
+
+    def mas_text_sum(text):
+        sum_text = isaa.mas_text_summaries(text)
+        return isaa.run_agent("think", sum_text, all_mem=True)
+
+    def questionl_helper(_):
+        text = get_input(speek_mode=speak_mode[0])
+        return isaa.run_agent("self", text, all_mem=False)
+
+    def question_helper(_):
+        text = get_input(speek_mode=speak_mode[0])
+        return isaa.run_agent("think", text, all_mem=True)
+
+    def exiquteion_once_helper(_):
+        text = get_input(speek_mode=speak_mode[0])
+        return isaa.run_agent("think", text, all_mem=True, running_mode='oncex')
+
+    def lineIs_helper(_):
+        text = get_input(speek_mode=speak_mode[0])
+        return isaa.run_agent("think", text, all_mem=True, running_mode='lineIs')
+
+    def url_getter(url):
+        print("Parsing", url)
+        parsed_url = urlparse(url)
+        dont_len = parsed_url.netloc.count('.')
+        domain = "www"
+        if dont_len == 1:
+            domain = parsed_url.netloc.split('.')[0]
+        if dont_len >= 2:
+            domain = parsed_url.netloc.split('.')[1]
+        if "wikipedia.org" in parsed_url.netloc:  # https://de.wikipedia.org/wiki/Erster_Weltkrieg##url
+            domain = "wikipedia"
+        loder, docs_loder = route_url_to_function(url)
+        docs = docs_loder
+        if not isinstance(docs_loder, list):
+            docs = docs_loder()
+        isaa.get_context_memory().add_data(domain, docs)
+        final_d = '\n\n'.join([doc.page_content for doc in docs])
+        return mas_text_sum(final_d)
+
+    def path_getter(path):
+        print("Parsing", path)
+        loder, docs_loder = route_local_file_to_function(path)
+        docs = docs_loder()
+        isaa.get_context_memory().add_data("localD", docs)
+        final_d = '\n\n'.join([doc.page_content for doc in docs])
+        return mas_text_sum(final_d)
+
+    def refactor_helper(text):
+        isaa.get_agent_class('self').mode = MarkdownRefactorMode
+        res = isaa.run_agent("self", text=text, all_mem=True)
+        isaa.get_agent_class('self').mode = None
+        return res
+
+    def exit_helper(*_):
+        app.alive = False
+
+    def save_mem_helper(*_):
+        isaa.save_to_mem()
+
+    register("##e", exit_helper)
+    register("##sm", save_mem_helper)
+    register("##si", toggle_helper(0))  # toggel speache input mode
+    register("##so", toggle_helper(1))  # toogel speache output mode
+    register("##sum", mas_text_sum)  # )Summaeryse( zummeryse clipborde & referra to known Nolage
+    register("##url", url_getter)  # )web( read curent url from clipord -> must contain an http(s) url and summs the content & ask a question to a wep page
+    register("##path", path_getter)  # -> path )folder / file( local data text pdf folders (image)
+    register("##rfc", refactor_helper)  # )refactor( refactor agiven txt form the cliport asking for parameters.
+    register("##q", question_helper)  # register("##cli",  # )refactor( refactor agiven txt form the cliport asking for parameters.
+    register("##x1", exiquteion_once_helper)
+    register("##x3", lineIs_helper)
+
+    # isaa.get_context_memory().load_all()
+
+    def print_prompt(msg_data):
+
+        messages = msg_data.get('messages', {})
+        print(Style.GREEN2("PROMPT START "))
+        for message in messages:
+            caller = Style.WHITE(message.get('role', 'NONE').upper()) if message.get('role',
+                                                                                     'NONE') == 'user' else 'NONE'
+            caller = Style.CYAN(message.get('role', 'NONE').upper()) if message.get('role',
+                                                                                    'NONE') == 'system' else caller
+            caller = Style.VIOLET2(message.get('role', 'NONE').upper()) if message.get('role',
+                                                                                       'NONE') == 'assistent' else caller
+            print(f"\n{caller}\n{Style.GREY(message.get('content', '--#--'))}\n")
+        print(Style.GREEN("PROMPT END -- "))
+
+    isaa.init_isaa(name='self', build=True)
+
+    print(f"Script running in the background")
+    f_names = list(functions.keys())
+    print(f"init completed waiting for trigger word: {f_names}")
+    buffer = ' ' * 8
+
+    while app.alive:
+
+        buffer = get_buffer(buffer)
+
+        function = function_buffer_manager(buffer, functions)
+
+        if function is None:
+            continue
+
+        context = pyperclip.paste()
+        res = function(context)
+
+        buffer = ' ' * 8
+
+        if res is None:
+            if speak_mode[1]:
+                print("No data to verbalise")
+            continue
+
+        if speak_mode[1]:
+            print("Start speaking")
+            app.run_any(tbef.AUDIO.SPEECH_STREAM, text=res, use_cache=True, provider="piper")
+
+        pyperclip.copy(res)
+
+        print(f"waiting for trigger word:: {f_names}")
+
+    app.exit()
+
+    print("\n Exiting...")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/module.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import binascii
 import hashlib
 import logging
 import math
+import os
 import time
 import json
-from toolboxv2 import MainTool, FileHandler
+
+import requests
+
+from toolboxv2 import MainTool, FileHandler, get_app, Style
 from .UserInstances import UserInstances
 from .ModManager import installer, delete_package
 from toolboxv2.utils.state_system import get_state_from_app, TbState
-from .extras import *
-
 Name = 'CloudM'
 version = "0.0.2"
 export = get_app(f"{Name}.EXPORT").tb
 no_test = export(mod_name=Name, test=False, version=version)
 to_api = export(mod_name=Name, api=True, version=version)
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/CloudM/settings_manager.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/CloudM/settings_manager.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/DB/local_instance.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/DB/local_instance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import os
 
-from toolboxv2 import Result, get_app
+from toolboxv2 import Result
 from .types import AuthenticationTypes
 from ...utils.cryp import Code
 
 
 class MiniDictDB:
     auth_type = AuthenticationTypes.location
 
     def __init__(self):
         self.data = {}
         self.key = ""
         self.location = ""
 
-    def scan_iter(self, serch=''):
-        # print(self.data)
+    def scan_iter(self, search=''):
+        print(self.data)
         if not self.data:
             return []
-        return [key for key in self.data.keys() if key.startswith(serch.replace('*', ''))]
+        search = search.replace('*', '')
+        return [key for key in self.data.keys() if key.startswith(search)]
 
     def initialize(self, location, key):
         if os.path.exists(location + 'MiniDictDB.json'):
             try:
                 self.data = eval(Code.decrypt_symmetric(load_from_json(location + 'MiniDictDB.json').get('data'), key))
             except Exception as er:
-                print(f"Data is currupted error : {er}")
+                print(f"Data is corrupted error : {er}")
                 self.data = {}
         else:
             print(f'Could not initialize MiniDictDB with data from MiniDictDB.json')
             self.data = {}
         self.key = key
         self.location = location + 'MiniDictDB.json'
-        return Result.ok()
+        return Result.ok().set_origin("Dict DB")
 
     def get(self, key: str) -> Result:
         data = []
-        data_info = ""
 
         if key == 'all':
             data_info = "Returning all data available "
             for key_ in self.data.items():
                 data.append(key_)
 
         elif key == "all-k":
@@ -49,62 +49,74 @@
         else:
             data_info = "Returning subset of keys "
             for key_ in self.scan_iter(key):
                 val = self.data.get(key_)
                 data.append(val)
 
         if not data:
-            return Result.default_internal_error(info=f"No data found for key {key}")
+            return Result.default_internal_error(info=f"No data found for key {key}").set_origin("Dict DB")
 
-        return Result.ok(data=data, data_info=data_info + key)
+        return Result.ok(data=data, data_info=data_info + key).set_origin("Dict DB")
 
     def set(self, key, value):
         if key and value:
             self.data[key] = value
-            return Result.ok()
-        return Result.default_user_error(info=f"key is {key}, type{type(key)}, value is {value}, type{type(value)}")
+            return Result.ok().set_origin("Dict DB")
+        return Result.default_user_error(info=f"key is {key}, type{type(key)}, value is {value}, type{type(value)}").set_origin("Dict DB")
 
-    def append_on_set(self, key, value):
+    def append_on_set(self, key: str, value: list):
         if key in self.data:
-            self.data[key].append(value)
-            return Result.ok()
-        return Result.default_user_error(info=f"key not found {key}")
+            for v in value:
+                if v in self.data[key]:
+                    return Result.default_user_error(info=f"key is {key}, {v} existing in set").set_origin("Dict DB")
+            self.data[key] += value
+            return Result.ok().set_origin("Dict DB")
+        self.data[key] = value
+        return Result.ok().set_origin("Dict DB")
+
+    def if_exist(self, key: str):
+        if key.endswith('*'):
+            return len(self.scan_iter(key))
+        return 1 if key in self.data else 0
 
     def delete(self, key, matching=False) -> Result:
 
         del_list = []
         n = 0
 
+        if not isinstance(key, str):
+            key = str(key, 'utf-8')
+
         if matching:
             for key_ in self.scan_iter():
                 # Check if the key contains the substring
-                if key_ in str(key, 'utf-8'):
+                if key_ in key:
                     n += 1
                     # Delete the key if it contains the substring
                     v = self.data.pop(key)
                     del_list.append((key_, v))
         else:
             v = self.data.pop(key)
             del_list.append((key, v))
             n += 1
 
-        return Result.ok(data=del_list, data_info=f"Data deleted successfully removed {n} items")
+        return Result.ok(data=del_list, data_info=f"Data deleted successfully removed {n} items").set_origin("Dict DB")
 
     def exit(self) -> Result:
         if self.key == "":
-            return Result.default_internal_error(info="No cryptographic key available")
+            return Result.default_internal_error(info="No cryptographic key available").set_origin("Dict DB")
         if self.location == "":
-            return Result.default_internal_error(info="No file location available")
+            return Result.default_internal_error(info="No file location available").set_origin("Dict DB")
         data = Code().encode_code(str(self.data), self.key)
         try:
             save_to_json({"data": data}, self.location)
         except PermissionError and FileNotFoundError as f:
-            return Result.custom_error(data=f, info=f"Error Exiting local DB instance {f}")
+            return Result.custom_error(data=f, info=f"Error Exiting local DB instance {f}").set_origin("Dict DB")
 
-        return Result.ok()
+        return Result.ok().set_origin("Dict DB")
 
 
 def save_to_json(data, filename):
     """
     Speichert die übergebenen Daten in einer JSON-Datei.
 
     :param data: Die zu speichernden Daten.
@@ -125,7 +137,8 @@
     :return: Die geladenen Daten.
     """
     if not os.path.exists(filename):
         return {'data': ''}
 
     with open(filename, 'r') as file:
         return json.load(file)
+
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/DB/tb_adapter.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/DB/tb_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 from abc import ABC
 from typing import Any
 
-from toolboxv2 import MainTool, FileHandler, Result, get_app, tbef
+from toolboxv2 import MainTool, FileHandler, Result, get_app
 from .reddis_instance import MiniRedis
 from .local_instance import MiniDictDB
 from .types import DatabaseModes, AuthenticationTypes
 from toolboxv2.utils.types import ToolBoxInterfaces
 from ...utils.cryp import Code
 
 Name = "DB"
-
-"""Alle Daten Banken sind mit dem selben device schlüssel verschlüsselt TODO ändern"""
+export = get_app(from_="DB.EXPORT").tb
 
 
 def pre_function(*args, **kwargs) -> (list, dict):
     # Verarbeitung der args mit der encode_code-Methode
     encoded_args = map(lambda x: str(x) if type(x).__name__ in ['str', 'int', 'dict', 'list', 'tupel'] else x, args)
 
     # Verarbeitung der kwargs mit der encode_code-Methode
@@ -41,16 +40,16 @@
 #     decoded_data = Code().decode_code(result.get())
 #
 # print("Decoded data", decoded_data)
 
 # if decoded_data == "Error decoding":
 #     return result.lazy_return('intern', result, info=f"post fuction decoding error")
 
-# return result.ok(data=decoded_data, data_info=result.result.data_info, info=result.info.help_text, interface=result.result.data_to)
-
+# return result.ok(data=decoded_data, data_info=result.result.data_info, info=result.info.help_text,
+# interface=result.result.data_to)
 
 class DB(ABC):
 
     def get(self, query: str) -> Result:
         """get data"""
 
     def set(self, query: str, value) -> Result:
@@ -58,44 +57,44 @@
 
     def append_on_set(self, query: str, value) -> Result:
         """append set data"""
 
     def delete(self, query: str, matching=False) -> Result:
         """delete data"""
 
+    def if_exist(self, query: str) -> bool:
+        """return True if query exists"""
+
     def exit(self) -> Result:
         """Close DB connection and optional save data"""
 
 
 class Tools(MainTool, FileHandler):
     version = "0.0.2"
 
-    export = get_app(from_="DB.EXPORT").tb
-
     def __init__(self, app=None):
         self.name = Name
-        self.logs = app.logger if app else None
         self.color = "YELLOWBG"
 
-        self.keys = {"url": "redis:url~"}
+        self.keys = {"mode": "db~mode~~:"}
         self.encoding = 'utf-8'
 
         self.data_base: MiniRedis or MiniDictDB or DB or None = None
-        self.mode = DatabaseModes.LC
+        self.mode = DatabaseModes.crate(os.getenv("DB_MODE_KEY", "LC") if 'test' not in get_app("DB_MODE_KEY").id else os.getenv("DB_MODE_KEY_TEST", "LC"))
         self.url = None
         self.passkey = None
         self.user_name = None
         self.password = None
 
         MainTool.__init__(self,
-                          load=self.initialized,
+                          load=self.initialize_database,
                           v=self.version,
                           name=self.name,
-                          logs=self.logs,
-                          color=self.color)
+                          color=self.color,
+                          on_exit=self.close_db)
 
     @export(
         mod_name=Name,
         name="Version",
         version=version,
     )
     def get_version(self):
@@ -119,14 +118,34 @@
         if self.mode.value == "REMOTE_DICT":
             return Result.custom_error(info="Not Implemented yet")  # TODO: add remote dict storage
 
         return Result.default_internal_error(info="Database is not configured")
 
     @export(
         mod_name=Name,
+        helper="Test if an key is in the Database instance",
+        version=version,
+        interface=ToolBoxInterfaces.internal,
+        post_compute=post_function,
+    )
+    def if_exist(self, query: str) -> Result:
+
+        if self.data_base is None:
+            return Result.default_internal_error(info="No database connection")
+
+        if self.mode.value == "LOCAL_DICT" or self.mode.value == "LOCAL_REDDIS" or self.mode.value == "REMOTE_REDDIS":
+            return Result.ok(data=self.data_base.if_exist(query)).set_origin(f"{self.mode.value}.DB.if_exist")
+
+        if self.mode.value == "REMOTE_DICT":
+            return Result.custom_error(info="Not Implemented yet")  # TODO: add remote dict storage
+
+        return Result.default_internal_error(info="Database is not configured")
+
+    @export(
+        mod_name=Name,
         helper="Set data to an Database instance",
         version=version,
         interface=ToolBoxInterfaces.internal,
         pre_compute=pre_function,
     )
     def set(self, query: str, data: Any) -> Result:
         if self.data_base is None:
@@ -175,16 +194,14 @@
         return Result.default_internal_error(info="Database is not configured")
 
     @export(
         mod_name=Name,
         helper="append data to an Database instance subset",
         version=version,
         interface=ToolBoxInterfaces.internal,
-        pre_compute=pre_function,
-        post_compute=post_function,
     )
     def append_on_set(self, query: str, data: Any) -> Result:
         if self.data_base is None:
             return Result.default_internal_error(info="No database connection")
 
         if data is None:
             return Result.default_user_error(info="None value is not valid value must have a to str & be serialise")
@@ -206,14 +223,15 @@
             self.data_base = MiniDictDB()
         elif self.mode.value == DatabaseModes.LR.value:
             self.data_base = MiniRedis()
         elif self.mode.value == DatabaseModes.RR.value:
             self.data_base = MiniRedis()
         else:
             return Result.default_internal_error(info="Not implemented")
+        print(f"Starting DB in {self.mode.value} mode")
         a = self._autoresize()
         if a.log(prifix="initialize_database: ").is_error():
             raise RuntimeError("DB Autoresize Error " + a.print(show=False))
 
         self.logger.info(f"Running DB in mode : {self.mode.value}")
 
     def _autoresize(self):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/DB/types.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/DB/types.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/WebSocketManager.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/WebSocketManager.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, app=None):
         self.version = "0.0.3"
         self.name = "WebSocketManager"
         self.logger: logging.Logger or None = app.logger if app else None
         if app is None:
             app = get_app()
 
-        self.app_ = app
+        self.app = app
         self.color = "BLUE"
         self.active_connections: dict = {}
         self.active_connections_client: dict = {}
         self.app_id = get_app().id
         self.keys = {
             "tools": "v-tools~~~"
         }
@@ -178,15 +178,15 @@
         def websocket_thread():
             asyncio.set_event_loop(loop)
             # websocket_handler()
             # loop.run_forever()
             # loop.run_in_executor(None, websocket_handler)
             loop.run_until_complete(websocket_handler())
 
-        ws_thread = threading.Thread(target=websocket_thread)
+        ws_thread = threading.Thread(target=websocket_thread, daemon=True)
         ws_thread.start()
 
         return send_queue, recv_queue
 
     def create_websocket(self, websocket_id: str, url: str = 'wss://0.0.0.0:5000/ws'):  # wss:
         if websocket_id is None:
             return
@@ -204,15 +204,15 @@
             self.print(f"websocket not found")
         self.active_connections_client[websocket_id].close()
         del self.active_connections_client[websocket_id]
 
     async def connect(self, websocket: WebSocket, websocket_id):
         websocket_id_sto = await valid_id(websocket_id, self.app_id, websocket)
 
-        data = self.app_.run_any("cloudM", "validate_ws_id", [websocket_id])
+        data = self.app.run_any("cloudM", "validate_ws_id", [websocket_id])
         valid, key = False, ''
         if isinstance(data, list) or isinstance(data, tuple):
             if len(data) == 2:
                 valid, key = data
             else:
                 self.logger.error(f"list error connect {data}")
                 return False
@@ -292,177 +292,129 @@
             return
 
         if data_type == "dict" and isinstance(data, dict):
             keys = list(data.keys())
             if "ServerAction" in keys:
                 action = data["ServerAction"]
 
-                if action == "getsMSG":
-                    # Sendeng system MSG message
-                    systemMSG_content = self.construct_render(content="./app/systemMSG/text.html",
-                                                              element_id="extra",
-                                                              externals=["/app/systemMSG/speech_balloon.js"],
-                                                              from_file=True)
-
-                    await websocket.send_text(systemMSG_content)
-                elif action == "getTextWidget":  # WigetNav
-                    # Sendeng system MSG message
-                    widgetText_content = self.construct_render(content="./app/1/textWidet/text.html",
-                                                               element_id="widgetText",
-                                                               externals=["/app/1/textWidet/testWiget.js"],
-                                                               from_file=True)
-
-                    await websocket.send_text(widgetText_content)
-                elif action == "getPathWidget":
-                    widgetPath_content = self.construct_render(content="./app/1/PathWidet/text.html",
-                                                               element_id="widgetPath",
-                                                               externals=["/app/1/PathWidet/pathWiget.js"],
-                                                               from_file=True)
-
-                    await websocket.send_text(widgetPath_content)
-                elif action == "getWidgetNave":
-                    # Sendeng system MSG message
-                    widgetText_content = self.construct_render(content="./app/1/WigetNav/navDrow.html",
-                                                               element_id="controls",
-                                                               externals=["/app/1/WigetNav/navDrow.js"],
-                                                               from_file=True)
-
-                    await websocket.send_text(widgetText_content)
-                elif action == "getDrag":
-                    drag_content = self.construct_render(content="./app/Drag/drag.html",
-                                                         element_id="DragControls",
-                                                         externals=["/app/Drag/drag.js"],
-                                                         from_file=True)
-                    await websocket.send_text(drag_content)
-                elif action == "getControls":
-                    controller_content = self.construct_render(content="",
-                                                               element_id="editorWidget",
-                                                               externals=["/app/1/Controler/controller.js"])
-
-                    await websocket.send_text(controller_content)
-                elif action == "serviceWorker":
-                    sw_content = self.construct_render(content="",
-                                                       element_id="control1",
-                                                       externals=["/app/index.js", "/app/sw.js"])
-                    await websocket.send_text(sw_content)
-                elif action == "logOut":
-                    user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                if action == "logOut":
+                    user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                     if user_instance is None or not user_instance:
                         return '{"res": "No User Instance Found"}'
 
                     if data['data']['token'] == "**SelfAuth**":
                         data['data']['token'] = user_instance['token']
 
                     api_data = ApiOb()
                     api_data.data = data['data']['data']
                     api_data.token = data['data']['token']
                     command = [api_data, data['command'].split('|')]
 
-                    self.app_.run_any("cloudM", "api_log_out_user", command)
+                    self.app.run_any("cloudM", "api_log_out_user", command)
                     websocket_id_sto = await valid_id(websocket_id, self.app_id)
                     for websocket_ in self.active_connections[websocket_id_sto]:
                         if websocket == websocket_:
                             continue
                         await self.disconnect(websocket_, websocket_id)
 
                     if len(self.active_connections[websocket_id_sto]) > 1:
                         await self.send_message(json.dumps({'exit': 'exit'}), websocket, websocket_id)
 
                     home_content = self.construct_render(content="",
                                                          element_id="main",
 
-                                                         externals=["/app/scripts/go_home.js"])
+                                                         externals=["/web/scripts/go_home.js"])
 
                     await websocket.send_text(home_content)
                 elif action == "getModListAll":
-                    return json.dumps({'modlistA': self.app_.get_all_mods()})
+                    return json.dumps({'modlistA': self.app.get_all_mods()})
                 elif action == "getModListInstalled":
-                    user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                    user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                     if user_instance is None or not user_instance:
                         self.logger.info("No valid user instance")
                         return '{"res": "No Mods Installed"}'
 
                     return json.dumps({'modlistI': user_instance['save']['mods']})
                 elif action == "getModData":
                     mod_name = data["mod-name"]
                     try:
-                        mod = self.app_.get_mod(mod_name)
+                        mod = self.app.get_mod(mod_name)
                         return {"settings": {'mod-description': mod.description}}
                     except ValueError:
                         content = self.construct_render(
                             content=f"""<p id="infoText" color: style="color:var(--error-color);">Mod {mod_name} not found
                         </p>
                         """, element_id="infoText")
                         return content
                 elif action == "installMod":
-                    user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                    user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                     if user_instance is None or not user_instance:
                         self.logger.info("No valid user instance")
                         return '{"res": "No User Instance Found Pleas Log in"}'
 
                     if data["name"] not in user_instance['save']['mods']:
                         self.logger.info(f"Appending mod {data['name']}")
                         user_instance['save']['mods'].append(data["name"])
 
-                    self.app_.new_ac_mod("cloudM")
-                    self.app_.AC_MOD.hydrate_instance(user_instance)
+                    self.app.new_ac_mod("cloudM")
+                    self.app.AC_MOD.hydrate_instance(user_instance)
                     self.print("Sending webInstaller")
                     installer_content = user_instance['live'][data["name"]].webInstall(user_instance,
                                                                                        self.construct_render)
-                    self.app_.new_ac_mod("cloudM")
-                    self.app_.AC_MOD.save_user_instances(user_instance)
+                    self.app.new_ac_mod("cloudM")
+                    self.app.AC_MOD.save_user_instances(user_instance)
                     await websocket.send_text(installer_content)
                 elif action == "addConfig":
-                    user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                    user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                     if data["name"] in user_instance['live'].keys():
                         user_instance['live'][data["name"]].add_str_to_config([data["key"], data["value"]])
                     else:
                         await websocket.send_text('{"res": "Mod nod installed or available"}')
                 elif action == "runMod":
-                    user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                    user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
 
                     self.print(f"{user_instance}, {data}")
                     if user_instance is None or not user_instance:
                         return '{"res": "No User Instance Found pleas log in"}'
 
                     if data['data']['token'] == "**SelfAuth**":
                         data['data']['token'] = user_instance['token']
 
                     api_data = ApiOb()
                     api_data.data = data['data']['data']
                     api_data.token = data['data']['token']
                     command = [api_data, data['command'].split('|')]
 
-                    token_data = self.app_.run_any('cloudM', "validate_jwt", command)
+                    token_data = self.app.run_any('cloudM', "validate_jwt", command)
 
                     if not isinstance(token_data, dict):
                         return json.dumps({'res': 'u ar using an invalid token pleas log in again'})
 
                     if token_data["uid"] != user_instance['save']['uid']:
                         self.logger.critical(
                             f"{Style.RED(f'''User {user_instance['save']['username']} {Style.CYAN('Accessed')} : {Style.Bold(token_data['username'])} token both log aut.''')}")
-                        self.app_.run_any('cloudM', "close_user_instance", token_data["uid"])
-                        self.app_.run_any('cloudM', "close_user_instance", user_instance['save']['uid'])
+                        self.app.run_any('cloudM', "close_user_instance", token_data["uid"])
+                        self.app.run_any('cloudM', "close_user_instance", user_instance['save']['uid'])
                         return json.dumps({'res': "The server registered: you are"
                                                   " trying to register with an not fitting token "})
 
                     if data['name'] not in user_instance['save']['mods']:
                         user_instance['save']['mods'].append(data['name'])
 
                     if data['name'] not in user_instance['live'].keys():
                         self.logger.info(f"'Crating live module:{data['name']}'")
-                        self.app_.new_ac_mod("cloudM")
-                        self.app_.AC_MOD.hydrate_instance(user_instance)
-                        self.app_.new_ac_mod("cloudM")
-                        self.app_.AC_MOD.save_user_instances(user_instance)
+                        self.app.new_ac_mod("cloudM")
+                        self.app.AC_MOD.hydrate_instance(user_instance)
+                        self.app.new_ac_mod("cloudM")
+                        self.app.AC_MOD.save_user_instances(user_instance)
 
                     try:
-                        self.app_.new_ac_mod("VirtualizationTool")
-                        if self.app_.run_function('set-ac', user_instance['live']['v-' + data['name']]):
-                            res = self.app_.run_function('api_' + data['function'], command)
+                        self.app.new_ac_mod("VirtualizationTool")
+                        if self.app.run_function('set-ac', user_instance['live']['v-' + data['name']]):
+                            res = self.app.run_function('api_' + data['function'], command)
                         else:
                             res = "Mod Not Found 404"
                     except Exception as e:
                         res = "Mod Error " + str(e)
 
                     if type(res) == str:
                         if (res.startswith('{') or res.startswith('[')) or res.startswith('"[') or res.startswith('"{') \
@@ -478,40 +430,42 @@
                     if function_action is None:
                         return json.dumps(Result.default_internal_error(f"ServerAction {action} is not available"))
 
                     res = function_action(data)
 
                     if not isinstance(res, str):
                         res = str(res)
-
+                    await websocket.send_text(res)
                     return res
             if "ValidateSelf" in keys:
-                user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                 if user_instance is None or not user_instance:
                     self.logger.info("No valid user instance")
                     return json.dumps({"res": "No User Instance Found Pleas Log in", "valid": False})
                 return json.dumps({"res": "User Instance is valid", "valid": True})
             if "ChairData" in keys:
-                user_instance = self.app_.run_any("cloudM", "wsGetI", [si_id])
+                user_instance = self.app.run_any("cloudM", "wsGetI", [si_id])
                 if user_instance is None or not user_instance:
                     self.logger.info("No valid user instance")
                     return json.dumps({"res": "No User Instance Found Pleas Log in", "valid": False})
                 if len(self.active_connections[websocket_id_sto]) < 1:
                     return json.dumps({"res": "No other connections found", "valid": True})
                 await self.send_message(json.dumps(data['data']), websocket, websocket_id)
                 return json.dumps({"res": "Data Send", "valid": True})
 
         if data_type == "str":
             await self.send_message(data, websocket, websocket_id)
 
     def construct_render(self, content: str, element_id: str, externals: List[str] or None = None,
-                         placeholder_content: str or None = None, from_file=False):
+                         placeholder_content: str or None = None, from_file=False, to_str=True):
 
         if externals is None:
             externals = []
+        if element_id is None:
+            element_id = ""
 
         if placeholder_content is None:
             placeholder_content = "<h1>Loading...</h1>"
 
         if from_file:
             if os.path.exists(content):
                 with open(content, 'r') as f:
@@ -528,8 +482,10 @@
                 "externals": externals,
                 "placeholderContent": placeholder_content
             }
         }
 
         self.logger.info(f"render content :  {render_data}")
 
-        return json.dumps(render_data)
+        if to_str:
+            return json.dumps(render_data)
+        return render_data
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/api_manager.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/api_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+import json
 import logging
 import os
 import threading
 import time
 from platform import system
 
 import requests
 
-from toolboxv2 import MainTool, FileHandler, App, get_app
-
+from toolboxv2 import MainTool, FileHandler, get_app
 
 export = get_app("api_manager.Export").tb
 Name = "api_manager"
 
 
 class Tools(MainTool, FileHandler):  # FileHandler
 
@@ -118,42 +118,46 @@
             return "api is already running"
 
         if live is True and reload is True:
             raise ValueError("Live and reload should not be used together")
 
         if api_name not in self.api_config.keys():
             host = "localhost"
-            if live:
-                host = "0.0.0.0"
 
             self.api_config[api_name] = {
                 "Name": api_name,
                 "version": self.version,
                 "port": 5000,
                 "host": host
             }
 
+            if live:
+                self.api_config[api_name]['host'] = "0.0.0.0"
+
             self.print(f"Auto addet {api_name} to config : {self.api_config[api_name]}")
 
+        if live:
+            self.api_config[api_name]['host'] = "0.0.0.0"
+
         api_data = self.api_config[api_name]
 
         self.print(api_data)
         g = f"uvicorn toolboxv2.api.fast_api_main:app --host {api_data['host']}" \
-            f" --port {api_data['port']} --header data:0:{api_name} {'--reload' if reload else ''}"
+            f" --port {api_data['port']} --header data:{self.app.debug}:{api_name} {'--reload' if reload else ''}"
 
         print("Running command : " + g)
 
         if api_thread is None:
-            self.running_apis[api_name] = threading.Thread(target=os.system, args=(g,))
+            self.running_apis[api_name] = threading.Thread(target=os.system, args=(g,), daemon=True)
             self.running_apis[api_name].start()
             return "starting api"
 
         self.print("API is already running")
 
-    def stop_api(self, api_name: str):
+    def stop_api(self, api_name: str, delete=True):
         if api_name not in list(self.api_config.keys()):
             return f"Api with the name {api_name} is not listed"
 
         api_thread = self.running_apis.get(api_name)
         api_data = self.api_config[api_name]
         host = api_data.get("host")
         port = api_data.get("port")
@@ -169,25 +173,31 @@
             if system() == "Windows":
                 os.system(f"taskkill /pid {api_pid} /F")
             else:
                 os.system(f"kill -9 {api_pid}")
         api_thread = self.running_apis.get(api_name)
         if api_thread:
             api_thread.join()
-        del self.running_apis[api_name]
+        if delete:
+            del self.running_apis[api_name]
         os.remove(f"./.data/api_pid_{api_name}")
 
     @export(mod_name="api_manager", test=False)
     def restart_api(self, api_name: str):
         self.stop_api(api_name)
         time.sleep(4)
         self.start_api(api_name)
 
     def on_start(self):
         self.load_file_handler()
-        self.api_config = self.get_file_handler(self.keys["Apis"])
+        data = self.get_file_handler(self.keys["Apis"])
+        if isinstance(data, str):
+            self.api_config = json.loads(data)
+        else:
+            self.api_config = data
 
     def on_exit(self):
-        self.add_to_save_file_handler(self.keys["Apis"], str(self.api_config))
+        self.add_to_save_file_handler(self.keys["Apis"], json.dumps(self.api_config))
         for key in self.running_apis:
-            self.stop_api(key)
+            self.stop_api(key, delete=False)
+        self.running_apis = {}
         self.save_file_handler()
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/cli_functions.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/cli_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from dataclasses import dataclass, field
 from threading import Thread
 
-from toolboxv2.utils.types import CallingObject
+from toolboxv2.utils.types import CallingObject, ApiResult
 
 try:
     from readchar import key as readchar_key
     from readchar import readkey
 
     READCHAR = True
     READCHAR_error = None
@@ -38,60 +38,67 @@
 
 
 @export(mod_name=Name, name='Version', version=version)
 def get_version():
     return version
 
 
+@dataclass
 class UserInputObject:
-    char: chr or str or None = None
-    word: str or None = None
-    offset_x: int or None = None
-    offset_y: int or None = None
+    char: chr or str or None = field(default=None)
+    word: str or None = field(default=None)
+    offset_x: int or None = field(default=None)
+    offset_y: int or None = field(default=None)
+
+    def is_last(self) -> bool:
+        return "LAST" == self.char
+
+    def is_v_error(self) -> bool:
+        return "ValueError" == self.char
 
     @classmethod
     def default(cls,
                 char: chr or str or None = None,
                 word: str or None = None,
                 offset_x: int or None = None,
                 offset_y: int or None = None):
-        cls.char = char
-        cls.word = word
-        cls.offset_x = offset_x
-        cls.offset_y = offset_y
-        return cls
+        return cls(
+            char=char,
+            word=word,
+            offset_x=offset_x,
+            offset_y=offset_y,
+        )
 
     @classmethod
     def final(cls):
-        cls.char = "LAST"
-        cls.word = "LAST"
-        cls.offset_x = 0
-        cls.offset_y = 0
-        return cls
+        return cls(char="LAST",
+                   word="LAST",
+                   offset_x=0,
+                   offset_y=0)
 
     @classmethod
     def ve(cls):
-        cls.char = "ValueError"
-        cls.word = "ValueError"
-        cls.offset_x = 0
-        cls.offset_y = 0
-        return cls
+        return cls(char="ValueError",
+                   word="ValueError",
+                   offset_x=0,
+                   offset_y=0, )
 
 
 @default_export
 def get_character():
     get_input = True
 
     offset_x = 0
     offset_y = 0
     word = ""
     char = ''
 
     # session_history += [c for c in app.command_history]
 
+    print("-->", end='\r')
     while get_input:
 
         key = readkey()
 
         if key == b'\x05' or key == '\x05':
             print('\033', end="")
             get_input = False
@@ -148,27 +155,26 @@
 @default_export
 def update_autocompletion_mods(app: App, autocompletion_dict=None):
     if app is None:
         app = get_app(from_="cliF.update_autocompletion_mods")
     if autocompletion_dict is None:
         autocompletion_dict = {}
 
-    for module_name, module in app.functions.items():
-        data = {}
-        for function_name, function_data in app.functions[module_name].items():
-            if not isinstance(function_data, dict):
-                continue
-            data[function_name] = {arg: None for arg in function_data.get("params", [])}  # TODO get default from sig
-        autocompletion_dict[module_name] = data
+    app.save_autocompletion_dict()
+    autocompletion_dict_ = app.get_autocompletion_dict()
+
+    if autocompletion_dict_ is not None:
+        autocompletion_dict = {**autocompletion_dict_, **autocompletion_dict}
 
     return autocompletion_dict
 
 
 @default_export
-def update_autocompletion_list_or_key(list_or_key: iter or None = None, autocompletion_dict=None, raise_e=True, do_lower=False):
+def update_autocompletion_list_or_key(list_or_key: iter or None = None, autocompletion_dict=None, raise_e=True,
+                                      do_lower=False):
     if list_or_key is None:
         list_or_key = []
     if autocompletion_dict is None:
         autocompletion_dict = {}
 
     for key in list_or_key:
         if raise_e and key in autocompletion_dict:
@@ -222,28 +228,57 @@
                 return
             fh.append_string(buff)
             os.system(buff)
 
         run_in_terminal(run_in_console)
         event.app.current_buffer.text = ""
 
+    @bindings.add('c-up')
+    def run_in_shell(event):
+        buff = event.app.current_buffer.text
+
+        def run_in_console():
+            if buff.startswith('cd'):
+                print("CD not available")
+                return
+            fh.append_string(buff)
+            if app.locals['user'].get('counts') is None:
+                app.locals['user']['counts'] = 0
+
+            try:
+                result = eval(buff, app.globals['root'], app.locals['user'])
+                if result is not None:
+                    print(f"#{app.locals['user']['counts']}>", result)
+                else:
+                    print(f"#{app.locals['user']['counts']}>")
+            except SyntaxError:
+                exec(buff, app.globals['root'], app.locals['user'])
+                print(f"#{app.locals['user']['counts']}> Statement executed")
+            except Exception as e:
+                print(f"Error: {e}")
+
+            app.locals['user']['counts'] += 1
+
+        run_in_terminal(run_in_console)
+        event.app.current_buffer.text = ""
+
     @bindings.add('s-left')
     def user_helper(event):
 
         buff = event.app.current_buffer.text.strip()
 
         def print_help():
             if buff == "":
                 print("All commands: ", completer_dict)
             user_input_buffer_info = buff.split(" ")
             if len(user_input_buffer_info) == 1:
                 if user_input_buffer_info[0] in completer_dict:
                     print("Avalabel functions:", completer_dict[user_input_buffer_info[0]])
                 else:
-                    print("Module is not available")
+                    os.system(f"{user_input_buffer_info[0]} --help")
             if len(user_input_buffer_info) > 1:
                 if user_input_buffer_info[0] in completer_dict:
                     if user_input_buffer_info[1] in completer_dict[user_input_buffer_info[0]]:
                         print("Avalabel args:", completer_dict[user_input_buffer_info[0]][user_input_buffer_info[1]])
                 else:
                     print("Module is not available")
 
@@ -286,54 +321,54 @@
 
         return user_input(app, completer_dict, get_rprompt, bottom_toolbar, active_modul)
     except EOFError:
 
         return user_input(app, completer_dict, get_rprompt, bottom_toolbar, active_modul)
     else:
         infos = text.split(" ")
-
         if len(infos) >= 1:
             call_obj.module_name = infos[0]
         if len(infos) >= 2:
             call_obj.function_name = infos[1]
         if len(infos) > 2:
             call_obj.kwargs = {}
             call_obj.args = infos[2:]
             if call_obj.module_name not in completer_dict:
                 return call_obj
-            if call_obj.function_name not in completer_dict[call_obj.module_name]:
+            if call_obj.function_name not in (
+            completer_dict[call_obj.module_name] if completer_dict[call_obj.module_name] is not None else {}):
                 return call_obj
             kwargs_name = completer_dict[call_obj.module_name][call_obj.function_name].get(
                 'params')  # TODO FIX parsm ist type list
             if kwargs_name is None:
                 return call_obj
             kwargs_name = kwargs_name.remove('app').remove('self')
             call_obj.kwargs = dict(zip(kwargs_name, infos[2:]))
         return call_obj
 
 
 @export(mod_name=Name, samples=[{
-                                 "obj": CallingObject(
-                                     module_name="welcome",
-                                     function_name="show_version",
-                                 ),
-                                 "build_in_commands": {},
-                                 }])
+    "obj": CallingObject(
+        module_name="welcome",
+    ),
+    "build_in_commands": {},
+}])
 def co_evaluate(app: App,
                 obj: CallingObject or None,
                 build_in_commands: dict,
                 threaded=False,
                 helper=None,
                 return_parm=False
                 ):
     if obj is None:
         return Result.default_user_error(info="No object specified")
 
     if app is None:
         app = get_app(from_="cliF.co_evaluate")
+
     command = obj.module_name
 
     if not command:
         return Result.default_user_error(info="No module Provided").set_origin("cli_functions.co_evaluate").print()
 
     if command in build_in_commands:
         return build_in_commands[command](obj).print()
@@ -342,23 +377,32 @@
 
     if not function_name:
         return Result.default_user_error(info="No function Provided").set_origin("cli_functions.co_evaluate").print()
 
     if obj.kwargs is None:
         obj.kwargs = {}
 
+    if app.locals['user'].get('res_id') is None:
+        app.locals['user']['res_id'] = 0
+
     if helper is None:
         def helper_function(obj_):
 
             # obj_.print()
             result = app.run_any((obj_.module_name, obj_.function_name), get_results=True,
                                  args_=obj_.args,
                                  kwargs_=obj_.kwargs)
 
-            result.print()
+            app.locals['user'][f"result{app.locals['user']['res_id']}"] = result
+            app.locals['user']['res_id'] += 1
+
+            if isinstance(result, Result) or isinstance(result, ApiResult):
+                result.print()
+            else:
+                print(result)
 
             if isinstance(return_parm, list):
                 return_parm[0] = result
             elif return_parm:
                 return return_parm
             else:
                 return None
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/dockerEnv.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/dockerEnv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import logging
 import os
 import tempfile
 import time
-from typing import Optional
 
 
 try:
     import docker
     from docker.models.containers import Container
     DOCKER = True
 except ModuleNotFoundError:
     DOCKER = False
 
-from toolboxv2 import MainTool, FileHandler, App, Style, Spinner
+from toolboxv2 import MainTool, FileHandler, App, Style, Spinner, get_app
 
 
 class Tools(MainTool, FileHandler):
 
     def __init__(self, app=None):
         self.version = "0.0.2"
         self.name = "dockerEnv"
@@ -214,7 +213,11 @@
             except Exception as e:
                 self.print(e)
                 running = False
 
             self.print(container.diff())
 
         self.stop_container(container_id)
+
+
+if __name__ == "__main__":
+    docker = get_app(from_="test_docker", name="debug").save_load("dockerEnv")
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/Interface.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/Interface.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/quickNote.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/quickNote.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,18 +180,18 @@
         tag_name: str = self.get_tag(tag_id).get().name
 
         del self.inbox["Tags"][tag_id]
 
         self.print(f"Adding tag... {tag_name}")
 
     def remove_note_by_name(self, note_name: str):
-        self.remove_note(self.get_by_id_ny_name(note_name))
+        self.remove_note(self.get_by_id_ny_name(note_name, t=":Note"))
 
     def remove_tag_by_name(self, tag_name: str):
-        self.remove_tag(self.get_by_id_ny_name(tag_name))
+        self.remove_tag(self.get_by_id_ny_name(tag_name, t=":Tag"))
 
     def view_note(self, show=False, data=False):
 
         notes = []
         for note in self.inbox["Notes"].values():
             res = note.print(show=show, debug=self.app.debug, data=data)
             notes.append(res)
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/quickNote/types.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/quickNote/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 class DataTypes(Enum):
     MD: str = "MarkDown"
     HTML: str = "HTML"
     TEXT: str = "TEXT"
     CUSTOM: str = "CUSTOM"
 
-
-class Tag(BaseModel):
+@dataclass
+class Tag:
     name: str
     id: str
     related: list[str]
 
     @classmethod
     def crate(cls, name: str, related=None):
         if related is None:
             related = []
-        return cls(name=name, id=get_id(name), related=related)
+        return cls(name=name, id=get_id(name+":Tag"), related=related)
 
     @classmethod
     def crate_root(cls):
-        return cls(name="root", id=get_id("root"), related=[])
+        return cls(name="root", id=get_id("root"+":Tag"), related=[])
 
     def add_related(self, other_tag):
         self.related.append(other_tag.id)
 
     def print(self, show=True, debug=False, data=False):
         string_data = f"= {self.name} ="
         if debug:
@@ -49,95 +49,95 @@
                 "related": self.related,
             }
         if show:
             print(string_data)
         else:
             return string_data
 
-
-class Note(BaseModel):
+@dataclass
+class Note:
     name: str
     id: str
     data: str
     data_type: DataTypes
     tags: list[Tag]
     links: list[str]
     parent: Tag
 
     @classmethod
     def crate_root(cls):
         root_tag = Tag.crate_root()
-        return cls(id=get_id("root"),
+        return cls(id=get_id("root"+":Note"),
                    name="root",
                    data="",
                    data_type=DataTypes.TEXT,
                    tags=[root_tag],
                    links=[],
                    parent=root_tag)
 
     @classmethod
     def crate_new_text(cls, name: str, data: str, tag: Tag, parent: Tag or None = None, links: list or None = None):
         if parent is None:
             parent = tag
         if links is None:
             links = []
-        return cls(id=get_id(name),
+        return cls(id=get_id(name+":Note"),
                    name=name,
                    data=data,
                    data_type=DataTypes.TEXT,
                    tags=[tag],
                    links=links,
                    parent=parent)
 
     @classmethod
     def crate_new_md(cls, name: str, data: str, tag: Tag, parent: Tag or None = None, links: list or None = None):
         if parent is None:
             parent = tag
         if links is None:
             links = []
-        return cls(id=get_id(name),
+        return cls(id=get_id(name+":Note"),
                    name=name,
                    data=data,
                    data_type=DataTypes.MD,
                    tags=[tag],
                    links=links,
                    parent=parent)
 
     @classmethod
     def crate_new_html(cls, name: str, data: str, tag: Tag, parent: Tag or None = None, links: list or None = None):
         if parent is None:
             parent = tag
         if links is None:
             links = []
-        return cls(id=get_id(name),
+        return cls(id=get_id(name+":Note"),
                    name=name,
                    data=data,
                    data_type=DataTypes.HTML,
                    tags=[tag],
                    links=links,
                    parent=parent)
 
     @classmethod
     def crate_new_custom(cls, name: str, data: str, tag: Tag, parent: Tag or None = None, links: list or None = None):
         if parent is None:
             parent = tag
         if links is None:
             links = []
-        return cls(id=get_id(name),
+        return cls(id=get_id(name+":Note"),
                    name=name,
                    data=data,
                    data_type=DataTypes.CUSTOM,
                    tags=[tag],
                    links=links,
                    parent=parent)
 
     def print(self, show=True, debug=False, data=False):
-        string_data = f"===========\n{self.data}===========\n --- Nama: {self.name} --- \n --- parent: {self.parent.name} --- "
+        string_data = f"_________ \n {self.data}\n _________ \n --- Nama: {self.name} --- \n --- parent: {self.parent.name} --- "
         if debug:
-            string_data += f"\n _________ debug Data _________\n{self.id}\n{self.data_type}\n --- \n"
+            string_data += f"\n =========== debug Data ===========\n{self.id}\n{self.data_type}\n --- \n"
         i = 0
         for tag in self.tags:
             string_data += f"Tag ({i}) {tag.name} \n"
             string_data += str(tag.related) + "\n" if len(tag.related) != 0 else ""
             string_data += tag.id if debug else ""
             i += 1
         if data:
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/mods/welcome.py` & `ToolBoxV2-0.1.8/toolboxv2/mods/welcome.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 export = get_app(from_="welcome.EXPORT").tb
 Name = 'welcome'
 version = '0.0.1'
 
 
 def webInstall(self, user_instance, construct_render) -> str:
     self.print("Installing Web")
-    return construct_render(content="./app/0/welcome/welcome.html",
+    return construct_render(content="./web/0/welcome/welcome.html",
                             element_id="main",
-                            externals=["/app/0/welcome/welcome.js"],
+                            externals=["/web/0/welcome/welcome.js"],
                             from_file=True)
 
 
 def webInstall_app_wrapper(self, command):
-    return command[1](content="./app/0/welcome/welcome.html",
+    return command[1](content="./web/0/welcome/welcome.html",
                       element_id="main",
-                      externals=["/app/0/welcome/welcome.js"],
+                      externals=["/web/0/welcome/welcome.js"],
                       from_file=True)
 
 
 @export(name="Version", mod_name=Name)
 def print_t():
     print(f"Version: {version} : {system()}")
     return version
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/__init__.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,21 +15,23 @@
     for file_name in os.listdir(dir_path):
         # Überprüfe, ob die Datei eine Python-Datei ist
         if file_name == "__init__.py":
             pass
         elif file_name.endswith('.py') and s in file_name:
             # Entferne die Erweiterung ".py" aus dem Dateinamen
             name = os.path.splitext(file_name)[0]
+            # print("Ent", name)
             # Lade das Modul
             spec = importlib.util.spec_from_file_location(name, os.path.join(dir_path, file_name))
             module = importlib.util.module_from_spec(spec)
             # try:
             spec.loader.exec_module(module)
             # except Exception as e:
             #    print("Error loading module ")
             #    print(e)
 
             # Füge das Modul der Dictionary hinzu
             if hasattr(module, 'run') and callable(module.run) and hasattr(module, 'NAME'):
+                # print("Collecing :", module.NAME)
                 runnable_dict_[module.NAME] = module.run
-    #  print(f"Getting all runnabels toock {time.perf_counter() -to:.2f} for {len(runnable_dict_.keys())} elements")
+    print(f"Getting all runnable took {time.perf_counter() -to:.2f} for {len(runnable_dict_.keys())} elements")
     return runnable_dict_
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/as_docker.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/as_docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-import io
-import os
 import sys
-import tempfile
 import uuid
 
-from toolboxv2 import App, AppArgs, Spinner
-#from toolboxv2.mods.dockerEnv import Tools
+from toolboxv2 import App, AppArgs
 
 NAME = 'docker'
 
 
 def get_multiline_input(x):
     print(x)
     print("exit with empty line")
@@ -89,15 +85,15 @@
 
     #WORKDIR /ToolBoxV2/
 
 
     # Install any needed packages specified in requirements.txt
     RUN pip install -e ./ToolBoxV2/
 
-    #RUN npm install ./ToolBoxV2/toolboxv2/app/node_modules/.package-lock.json
+    #RUN npm install ./ToolBoxV2/toolboxv2/web/node_modules/.package-lock.json
     # Make port 5000, 62435 available to the world outside this container
     EXPOSE 5000:5000
     EXPOSE 62435:62435
     """
 
     try:
         init_args = " ".join(sys.orig_argv)
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/demon.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/demon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 import time
 from threading import Thread
 
 from toolboxv2 import App, AppArgs, tbef
-from toolboxv2.mods.SocketManager import SocketType
 
 NAME = 'demon'
 
 
 def run(app: App, args: AppArgs, programmabel_interface=False, as_server=True):
     """
     The Demon runner is responsible for running a lightweight toolbox instance in the background
@@ -35,20 +34,23 @@
         remote
 
             $ ToolBoxV2 -m AnyMode[(default), cli, api] -n (full-name) --remote
                                                         optional --remote-direct-key [key] --host [host] --port [port]
 
     """
 
+    from toolboxv2.mods.SocketManager import SocketType
     # Start a New Demon
 
     status = 'unknown'
 
     client = app.run_any('SocketManager', 'create_socket',
-                         name="demon", host="localhost" if args.host == '0.0.0.0' else args.host, port=62436,
+                         name="demon",
+                         host="localhost" if args.host == '0.0.0.0' else args.host,
+                         port=62436 if args.port == 8000 else args.port,
                          type_id=SocketType.client,
                          max_connections=-1,
                          endpoint_port=None,
                          return_full_object=True)
     sender = None
     receiver_queue = None
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/minicli.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/minicli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import datetime
 import psutil
 
 from prompt_toolkit import HTML
 from prompt_toolkit.shortcuts import set_title, yes_no_dialog
 
-from toolboxv2.utils.Style import cls
 from toolboxv2 import App, Result, tbef
+from toolboxv2.utils import show_console
+from toolboxv2.utils.Style import cls
 from toolboxv2.utils.types import CallingObject
 
 NAME = 'minicli'
 
 
 def run(app: App, args):
-    set_title(f"ToolBox : {app.version}")
+    try:
+        set_title(f"ToolBox : {app.version}")
+    except:
+        pass
     threaded = False
 
     def bottom_toolbar():
         return HTML(f'Hotkeys shift:s control:c  <b><style bg="ansired">s+left</style></b> helper info '
                     f'<b><style bg="ansired">c+space</style></b> Autocompletion tips '
                     f'<b><style bg="ansired">s+up</style></b> run in shell')
 
     def exit_(_):
+        if app.debug:
+            app.hide_console()
         if 'main' in app.id:
             res = yes_no_dialog(
                 title='Exit ToolBox',
                 text='Do you want to Close the ToolBox?').run()
             app.alive = not res
         else:
             app.alive = False
@@ -120,62 +126,79 @@
         threaded = not threaded
         return Result.ok(info=f"in threaded mode {threaded}").set_origin("minicli::build-in").print()
 
     def infos(_):
         app.print_functions()
         return Result.ok(info=f"").set_origin("minicli::build-in")
 
+    def colose_console(_):
+        show_console(False)
+        return Result.ok(info=f"").set_origin("minicli::build-in")
+
+    def open_console(_):
+        app.show_console(True)
+        return Result.ok(info=f"").set_origin("minicli::build-in")
+
     bic = {
         "exit": exit_,
         "cls": cls_,
         "sdm:set_debug_mode": set_debug_mode,
         "open": open_,
         "close": close_,
         "run": run_,
         "infos": infos,
         "reload": hr,
         "remote": remote,
+        "hide_console": colose_console,
+        "show_console": open_console,
         "toggle_threaded": toggle_threaded,
         "..": lambda x: Result.ok(x),
     }
 
     all_modes = app.get_all_mods()
 
     # set up Autocompletion
+
     autocompletion_dict = {}
     autocompletion_dict = app.run_any(tbef.CLI_FUNCTIONS.UPDATE_AUTOCOMPLETION_LIST_OR_KEY, list_or_key=bic,
                                       autocompletion_dict=autocompletion_dict)
 
+    autocompletion_dict_ = app.get_autocompletion_dict()
+
+    if autocompletion_dict is None:
+        autocompletion_dict = {}
+
+    if autocompletion_dict_ is not None:
+        autocompletion_dict = {**autocompletion_dict, **autocompletion_dict_}
+
     autocompletion_dict["sdm:set_debug_mode"] = {arg: None for arg in ['on', 'off']}
     autocompletion_dict["open"] = autocompletion_dict["close"] = autocompletion_dict["reload"] = \
         {arg: None for arg in all_modes}
     autocompletion_dict["run"] = {arg: None for arg in list(app.runnable.keys())}
-    autocompletion_dict = app.run_any(tbef.CLI_FUNCTIONS.UPDATE_AUTOCOMPLETION_MODS,
-                                      autocompletion_dict=autocompletion_dict)
 
     active_modular = ""
 
     running_instance = None
     call = CallingObject.empty()
-
-    while app.alive:
+    running = True
+    while running:
         # Get CPU usage
         cpu_usage = psutil.cpu_percent(interval=1)
 
         # Get memory usage
         memory_usage = psutil.virtual_memory().percent
 
         # Get disk usage
         disk_usage = psutil.disk_usage('/').percent
 
         def get_rprompt():
-            current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-            # Get current time
+            current_time: str = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             return HTML(
-                f'''<b> App Infos: {app.id} \nCPU: {cpu_usage}% Memory: {memory_usage}% Disk :{disk_usage}%\nTime: {current_time}</b>''')
+                f'<b> App Infos: '
+                f'{app.id} \nCPU: {cpu_usage}% Memory: {memory_usage}% Disk :{disk_usage}%\nTime: {current_time}</b>')
 
         call = app.run_any(tbef.CLI_FUNCTIONS.USER_INPUT, completer_dict=autocompletion_dict,
                            get_rprompt=get_rprompt, bottom_toolbar=bottom_toolbar, active_modul=active_modular)
 
         print("", end="" + "start ->>\r")
 
         if call is None:
@@ -188,15 +211,22 @@
         running_instance = app.run_any(tbef.CLI_FUNCTIONS.CO_EVALUATE,
                                        obj=call,
                                        build_in_commands=bic,
                                        threaded=threaded,
                                        helper=helper_exequtor[0])
 
         print("", end="" + "done ->>\r")
+        running = app.alive
+
+    if hasattr(app, 'timeout'):
+        app.timeout = 2
 
     if running_instance is not None:
         print("Closing running instance")
         running_instance.join()
         print("Done")
 
-    set_title("")
+    try:
+        set_title("")
+    except:
+        pass
     app.exit()
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/qncli.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/qncli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import datetime
-import psutil
 
 from prompt_toolkit import HTML
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.shortcuts import set_title, yes_no_dialog
 
-from toolboxv2.mods.quickNote import Tools
-from toolboxv2.mods.quickNote.types import *
-from toolboxv2.utils.Style import cls
+
 from toolboxv2 import App, Result, tbef
+from toolboxv2.utils.Style import cls
 from toolboxv2.utils.types import CallingObject
 
 NAME = 'qncli'
 
 
-def run(app: App, args):
+def run(app: App, _):
+    from toolboxv2.mods.quickNote.quickNote import Tools
+    from toolboxv2.mods.quickNote.types import Tag, Note
+
     set_title(f"ToolBox : {app.version} quickNote")
     threaded = False
     qn_instance: Tools = app.get_mod('quickNote', 'app')
     if len(qn_instance.inbox.get("Notes", {}).keys()) == 0:
         qn_instance.add_note(qn_instance.note)
     if len(qn_instance.inbox.get("Tags", {}).keys()) == 0:
         qn_instance.add_tag(qn_instance.tag)
@@ -52,28 +53,27 @@
 
     def crate_note(call_: CallingObject):
         if not call_.function_name:
             return Result.default_user_error(info="add username").set_origin("quickNoteCli::build-in")
 
         name = call_.args[0]
         data = call_.args[1:]
-        call_.print()
-        print(f"Name={name}, {data}")
         if call_.function_name == "":
             return Result.default_user_error(info="No data provided")
-        elif call_.function_name.lower() in ["t", "text"]:
-            qn_instance.note = Note.crate_new_text(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
-        elif call_.function_name.lower() in ["m", "md"]:
-            qn_instance.note = Note.crate_new_md(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
-        elif call_.function_name.lower() in ["h", "html"]:
-            qn_instance.note = Note.crate_new_html(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
-        elif call_.function_name.lower() in ["c", "custom"]:
-            qn_instance.note = Note.crate_new_custom(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
-        else:
-            return Result.default_user_error(info=f"invalid Mode {call_.function_name} not t,m,h or c")
+        else: # call_.function_name.lower() in ["t", "text"]:
+            qn_instance.note = Note.crate_new_text(name=call_.function_name, data=' '.join(call_.args), tag=qn_instance.tag, parent=qn_instance.note)
+        # elif call_.function_name.lower() in ["m", "md"]:
+        #     qn_instance.note = Note.crate_new_md(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
+        # elif call_.function_name.lower() in ["h", "html"]:
+        #     qn_instance.note = Note.crate_new_html(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
+        # elif call_.function_name.lower() in ["c", "custom"]:
+        #     qn_instance.note = Note.crate_new_custom(name=name, data=data, tag=qn_instance.tag, parent=qn_instance.note)
+        # else:
+        #     return Result.default_user_error(info=f"invalid Mode {call_.function_name} not t,m,h or c")
+        qn_instance.note.print()
         return add_note(call_)
 
     def add_note(_):
         qn_instance.add_note(qn_instance.note)
         return Result.ok()
 
     def add_tag(_):
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/runabel/readchar_buldin_style_cli.py` & `ToolBoxV2-0.1.8/toolboxv2/runabel/readchar_buldin_style_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """Console script for toolboxv2. min dep readchar Style"""
-
 # Import default Pages
 import sys
 import os
 from platform import system, node
 
 import json
 from pygments import highlight
 from pygments.lexers import JsonLexer
 from pygments.formatters import TerminalFormatter
 
 # Import public Pages
 import readchar
+
 from toolboxv2 import App, Style
 from toolboxv2.utils import Singleton
 
 NAME = "cli"
 
 prefix = Style.CYAN(f"~{node()}@>")
 
 
 def user_input(app: App):
+
     get_input = True
     command = ""
     print_command = []
     helper = ""
     helper_index = 0
     options = []
     sh_index = 0
@@ -151,17 +152,16 @@
         print(f"{app.id = }\n\n"
               f"\n{app.debug = }")
         print(f"PREFIX={app.PREFIX}"
               f"\nMACRO={A().pretty_print(app.MACRO[:7])}"
               f"\nMODS={A().pretty_print(app.MACRO[7:])}"
               f"\nSUPER_SET={A().pretty_print(app.SUPER_SET)}")
 
-    elif command[0].lower() == "exit":  # builtin events(exit)
-        if input("Do you want to exit? (y/n): ") in ["y", "yes", "Y"]:
-            app.exit()
+    elif command[0].lower() == "exit" or command[0].lower() == 'e':  # builtin events(exit)
+        app.exit()
 
     elif command[0].lower() == "help":  # logs(event(helper))
         n = command[1] if len(command) > 2 else ''
         # app.help(n)
 
     elif command[0].lower() == 'load-mod':  # builtin events(event(cloudM(_)->event(Build)))
         if len(command) == 2:
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/Style.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/Style.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
         self.message = message
         self.running = False
         self.spinner_thread = None
 
     def __enter__(self) -> None:
         """Start the spinner"""
         self.running = True
-        self.spinner_thread = threading.Thread(target=self.spin)
+        self.spinner_thread = threading.Thread(target=self.spin, daemon=True)
         self.spinner_thread.start()
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
         """Stop the spinner"""
         self.running = False
         if self.spinner_thread is not None:
             self.spinner_thread.join()
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/TBConfig.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/TBConfig.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/cryp.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/cryp.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,21 +154,24 @@
     def encrypt_asymmetric(text: str, public_key_str: str) -> str:
         """
         Verschlüsselt einen Text mit einem gegebenen öffentlichen Schlüssel.
 
         Args:
             text (str): Der zu verschlüsselnde Text.
             public_key_str (str): Der öffentliche Schlüssel als String oder im pem format.
-            pem (bool): pem flag
 
         Returns:
             str: Der verschlüsselte Text.
         """
         try:
-            public_key = serialization.load_pem_public_key(public_key_str.encode())
+            public_key: RSAPublicKey = serialization.load_pem_public_key(public_key_str.encode())
+        except Exception as e:
+            get_logger().error(f"Error encrypt_asymmetric {e}")
+        try:
+            public_key: RSAPublicKey = serialization.load_pem_public_key(public_key_str.encode())
             encrypted = public_key.encrypt(
                 text.encode(),
                 padding.OAEP(
                     mgf=padding.MGF1(algorithm=hashes.SHA512()),
                     algorithm=hashes.SHA512(),
                     label=None
                 )
@@ -199,15 +202,15 @@
                     algorithm=hashes.SHA512(),
                     label=None
                 )
             )
             return decrypted.decode()
 
         except Exception as e:
-            get_logger().error(f"Error encrypt_asymmetric {e}")
+            get_logger().error(f"Error decrypt_asymmetric {e}")
         return "Invalid"
 
     @staticmethod
     def verify_signature(signature: str or bytes, message: str or bytes, public_key_str: str,
                          salt_length=padding.PSS.MAX_LENGTH) -> bool:
         if isinstance(signature, str):
             signature = signature.encode()
@@ -259,28 +262,32 @@
             pass
         except Exception as e:
             print(e)
             get_logger().error(f"Error validating signature: {e}")
         return False
 
     @staticmethod
-    def create_signature(message: str, private_key_str: str) -> str:
+    def create_signature(message: str, private_key_str: str, salt_length=padding.PSS.MAX_LENGTH,
+                         row=False) -> str or bytes:
         try:
             private_key = serialization.load_pem_private_key(private_key_str.encode(), password=None)
             signature = private_key.sign(
                 message.encode(),
                 padding.PSS(
-                    mgf=padding.MGF1(hashes.SHA256()),
-                    salt_length=padding.PSS.MAX_LENGTH
+                    mgf=padding.MGF1(hashes.SHA512()),
+                    salt_length=salt_length
                 ),
-                hashes.SHA256()
+                hashes.SHA512()
             )
-            return signature.decode()
+            if row:
+                return signature
+            return base64.b64encode(signature).decode()
         except Exception as e:
-            get_logger().error(f"Error encrypt_asymmetric {e}")
+            get_logger().error(f"Error create_signature {e}")
+            print(e)
         return "Invalid Key"
 
     @staticmethod
     def pem_to_public_key(pem_key: str):
         """
         Konvertiert einen PEM-kodierten öffentlichen Schlüssel in ein PublicKey-Objekt.
 
@@ -290,15 +297,15 @@
         Returns:
             PublicKey: Das PublicKey-Objekt.
         """
         public_key = serialization.load_pem_public_key(pem_key.encode())
         return public_key
 
     @staticmethod
-    def public_key_to_pem(public_key):
+    def public_key_to_pem(public_key: RSAPublicKey):
         """
         Konvertiert ein PublicKey-Objekt in einen PEM-kodierten String.
 
         Args:
             public_key (PublicKey): Das PublicKey-Objekt.
 
         Returns:
@@ -307,10 +314,12 @@
         pem = public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo
         )
         return pem.decode()
 
 
-DEVICE_KEY_PATH = "./divice.key"
-DEVICE_KEY = lambda: open(DEVICE_KEY_PATH, "r").read() if os.path.exists(DEVICE_KEY_PATH) else open(DEVICE_KEY_PATH,
-                                                                                                 "w").write(Fernet.generate_key().decode())
+DEVICE_KEY_PATH = ".info/device.key"
+DEVICE_KEY_ = lambda: open(DEVICE_KEY_PATH,
+                           "r").read(
+) if os.path.exists(DEVICE_KEY_PATH) else open(DEVICE_KEY_PATH, "wb").write(Fernet.generate_key())
+DEVICE_KEY = lambda: DEVICE_KEY_() if isinstance(DEVICE_KEY_(), str) else DEVICE_KEY_()
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/file_handler.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
             with open(self.file_handler_file_prefix + self.file_handler_filename, 'a'):
                 logger.info(Style.GREEN("File created successfully"))
                 self.file_handler_max_loaded_index_ = -1
             rdu()
         except OSError and PermissionError as e:
             raise e
+
     def open_s_file_handler(self):
         self._open_file_handler('w+', self.open_s_file_handler)
         return self
 
     def open_l_file_handler(self):
         self._open_file_handler('r+', self.open_l_file_handler)
         return self
@@ -108,14 +109,23 @@
             if key in self.file_handler_key_mapper:
                 key = self.file_handler_key_mapper[key]
 
         self.file_handler_load[key] = value
         self.file_handler_save[key] = self.encode_code(value)
         return True
 
+    def remove_key_file_handler(self, key: str):
+        if key == 'Pka7237327':
+            print("Cant remove Root Key")
+            return
+        if key in self.file_handler_load.keys():
+            del self.file_handler_load[key]
+        if key in self.file_handler_save.keys():
+            del self.file_handler_save[key]
+
     def load_file_handler(self):
         get_logger().info(
             Style.BLUE(
                 f"loading {self.file_handler_filename} "
             )
         )
         if self.file_handler_storage:
@@ -157,15 +167,15 @@
         self.file_handler_max_loaded_index_ = -1
         for objects in self.file_handler_load.items():
             self.file_handler_max_loaded_index_ += 1
             if obj == objects[0]:
 
                 try:
                     if len(objects[1]) > 0:
-                        return eval(objects[1])
+                        return eval(objects[1]) if isinstance(objects[1], str) else objects[1]
                     logger.warning(
                         Style.YELLOW(
                             f"No data  {obj}  ; {self.file_handler_filename}"
                         )
                     )
                 except ValueError:
                     logger.error(f"ValueError Loading {obj} ; {self.file_handler_filename}")
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/helper_functions.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/helper_functions.py`

 * *Files identical despite different names*

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/main_tool.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/main_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.todo = kwargs.get("load", lambda: None)
         self._on_exit = kwargs.get("on_exit", lambda: None)
         self.stuf = False
         if not hasattr(self, 'config'):
             self.config = {}
         if self.app is None:
             self.app = get_app()
-        self.ac_user_data_sto = {}
+        self.user = None
         self.description = "A toolbox mod" if kwargs.get("description") is None else kwargs.get("description")
         if MainTool.interface is None:
             MainTool.interface = self.app.interface_type
         # Result.default(self.app.interface)
         self.load()
 
     @staticmethod
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/state_system.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/state_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,10 +150,10 @@
 
 
 if __name__ == "__main__":
     # Provide the directory to search for Python files
     app = get_app()
     app.load_all_mods_in_file()
     state = get_state_from_app(app)
-    print(str(state))
+    print(state)
     # def get_state_from_app(app: App):
     #    """"""
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/tb_logger.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/tb_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,57 +38,58 @@
         raise ValueError(f"file_level must be one of {available_log_levels}, but logging level is {file_level}")
 
     log_date = datetime.datetime.today().strftime('%Y-%m-%d')
     log_levels = ["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET"]
     log_level_index = log_levels.index(logging.getLevelName(level))
 
     filename = f"Logs-{name}-{log_date}-{log_levels[log_level_index]}"
+    log_filename = f"{logs_directory}/{filename}.log"
 
     log_info_data = {
         filename: 0,
         "H": "localhost",
         "P": 62435
     }
 
     with open(f"{logs_directory}/Logs.info", "r") as li:
         log_info_data_str = li.read()
         try:
             log_info_data = eval(log_info_data_str)
         except SyntaxError:
             if log_info_data_str:
-                print(Style.RED(Style.Bold("Could not parse log")))
+                print(Style.RED(Style.Bold("Could not parse log info data")))
 
         if filename not in log_info_data:
             log_info_data[filename] = 0
 
-        if not os.path.exists(f"{logs_directory}/{filename}.log"):
+        if not os.path.exists(log_filename):
             log_info_data[filename] = 0
             print("new log file")
 
-        if os.path.exists(f"{logs_directory}/{filename}.log"):
+        if os.path.exists(log_filename):
             log_info_data[filename] += 1
 
             while os.path.exists(f"{logs_directory}/{filename}#{log_info_data[filename]}.log"):
                 log_info_data[filename] += 1
 
             try:
-                os.rename(f"{logs_directory}/{filename}.log",
+                os.rename(log_filename,
                           f"{logs_directory}/{filename}#{log_info_data[filename]}.log")
             except PermissionError:
                 print(Style.YELLOW(Style.Bold(f"Could not rename log file appending on {filename}")))
 
     with open(f"{logs_directory}/Logs.info", "w") as li:
         if len(log_info_data.keys()) >= 7:
             log_info_data = {
                 filename: log_info_data[filename],
                 "H": log_info_data["H"],
                 "P": log_info_data["P"]
             }
         li.write(str(log_info_data))
-    log_filename = f"{logs_directory}/{filename}.log"
+
     try:
         with open(log_filename, "a"):
             pass
     except OSError:
         log_filename = f"{logs_directory}/Logs-Test-{log_date}-{log_levels[log_level_index]}.log"
         with open(log_filename, "a"):
             pass
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/toolbox.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/toolbox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """Main module."""
 import concurrent.futures
+import json
 import os
+import queue
 import sys
+import threading
 import time
 import types
+from dataclasses import asdict
 from enum import Enum
 from platform import node, system
 from importlib import import_module
-from inspect import signature, getouterframes, currentframe
+from inspect import signature
+from random import uniform
 from types import ModuleType
 from functools import partial, wraps
 import requests
 import shelve
 from cachetools import TTLCache
 
 from toolboxv2.utils.file_handler import FileHandler
-from toolboxv2.utils import Singleton
+from toolboxv2.utils import Singleton, show_console
 from toolboxv2.utils.helper_functions import generate_test_cases
 from toolboxv2.utils.types import Result, AppArgs, ToolBoxInterfaces, ApiResult
 from toolboxv2.utils.tb_logger import setup_logging, get_logger
-from toolboxv2.utils.Style import Style
+from toolboxv2.utils.Style import Style, Spinner
 import toolboxv2
+from toolboxv2.utils.all_functions_enums import *
 
 import logging
 from dotenv import load_dotenv
 import dill
 
 load_dotenv()
 
@@ -65,14 +71,26 @@
 
 
 def save_module_dill(data_to_serialize, filename):
     with open(filename, 'wb') as file:
         dill.dump(data_to_serialize, file)
 
 
+def stram_print(text):
+    min_typing_speed, max_typing_speed = 0.0009, 0.0005
+    for i, word in enumerate(text):
+        if not word:
+            continue
+        print(word, end="", flush=True)
+        typing_speed = uniform(min_typing_speed, max_typing_speed)
+        time.sleep(typing_speed)
+        min_typing_speed = min_typing_speed * 0.04
+        max_typing_speed = max_typing_speed * 0.03
+
+
 class App(metaclass=Singleton):
 
     def __init__(self, prefix: str = "", args=AppArgs().default()):
 
         t0 = time.perf_counter()
         abspath = os.path.abspath(__file__)
         self.system_flag = system()  # Linux: Linux Mac: Darwin Windows: Windows
@@ -80,53 +98,58 @@
             dir_name = os.path.dirname(abspath).replace("/utils", "")
         else:
             dir_name = os.path.dirname(abspath).replace("\\utils", "")
         os.chdir(dir_name)
 
         self.start_dir = dir_name
 
+        lapp = dir_name + '\\.data\\'
+
+        if not prefix:
+            if not os.path.exists(f"{lapp}last-app-prefix.txt"):
+                os.makedirs(lapp, exist_ok=True)
+                open(f"{lapp}last-app-prefix.txt", "a").close()
+            with open(f"{lapp}last-app-prefix.txt", "r") as prefix_file:
+                cont = prefix_file.read()
+                if cont:
+                    prefix = cont
+        else:
+            if not os.path.exists(f"{lapp}last-app-prefix.txt"):
+                os.makedirs(lapp, exist_ok=True)
+                open(f"{lapp}last-app-prefix.txt", "a").close()
+            with open(f"{lapp}last-app-prefix.txt", "w") as prefix_file:
+                prefix_file.write(prefix)
+
         self.prefix = prefix
         self.id = prefix + '-' + node()
 
+        self.globals = {
+            "root": {},
+        }
+        self.locals = {
+            "user": {'app': self},
+        }
+
         identification = self.id
         if args.mm:
             identification = "MainNode"
 
         if "test" in prefix:
-            self.start_dir += '\\tests'
-            os.makedirs(self.start_dir, exist_ok=True)
             self.data_dir = self.start_dir + '\\.data\\' + "test"
             self.config_dir = self.start_dir + '\\.config\\' + "test"
         else:
             self.data_dir = self.start_dir + '\\.data\\' + identification
             self.config_dir = self.start_dir + '\\.config\\' + identification
 
         if not os.path.exists(self.data_dir):
             os.makedirs(self.data_dir, exist_ok=True)
         if not os.path.exists(self.config_dir):
             os.makedirs(self.config_dir, exist_ok=True)
 
-        lapp = dir_name + '\\.data\\'
-
-        if not prefix:
-            if not os.path.exists(f"{lapp}last-app-prefix.txt"):
-                os.makedirs(lapp, exist_ok=True)
-                open(f"{lapp}last-app-prefix.txt", "a").close()
-            with open(f"{lapp}last-app-prefix.txt", "r") as prefix_file:
-                cont = prefix_file.read()
-                if cont:
-                    prefix = cont
-        else:
-            if not os.path.exists(f"{lapp}last-app-prefix.txt"):
-                os.makedirs(lapp, exist_ok=True)
-                open(f"{lapp}last-app-prefix.txt", "a").close()
-            with open(f"{lapp}last-app-prefix.txt", "w") as prefix_file:
-                prefix_file.write(prefix)
-
-        print(f"Starting ToolBox as {prefix} from : ", Style.Bold(Style.CYAN(f"{os.getcwd()}")))
+        print(f"Starting ToolBox as {prefix} from :", Style.Bold(Style.CYAN(f"{os.getcwd()}")))
 
         logger_info_str, self.logger, self.logging_filename = self.set_logger(args.debug)
 
         print("Logger " + logger_info_str)
         print("================================")
         self.logger.info("Logger initialized")
         get_logger().info(Style.GREEN("Starting Application instance"))
@@ -143,14 +166,15 @@
             "HELPER": "helper~~~:",
             "debug": "debug~~~~:",
             "id": "name-spa~:",
             "st-load": "mute~load:",
             "comm-his": "comm-his~:",
             "develop-mode": "dev~mode~:",
             "all_main": "all~main~:",
+            "provider::": "provider::",
         }
 
         defaults = {
             "MACRO": ['Exit'],
             "MACRO_C": {},
             "HELPER": {},
             "debug": args.debug,
@@ -163,26 +187,28 @@
         FileHandler.all_main = args.mm
         self.config_fh = FileHandler(self.id + ".config", keys=self.keys, defaults=defaults)
         self.config_fh.load_file_handler()
         self._debug = args.debug
         self.runnable = {}
         self.dev_modi = self.config_fh.get_file_handler(self.keys["develop-mode"])
         if self.config_fh.get_file_handler("provider::") is None:
-            self.config_fh.add_to_save_file_handler("provider::", "https://simplecore.app")
+            self.config_fh.add_to_save_file_handler("provider::", os.environ.get("HOSTNAME", "https://simplecore.app"))
         self.functions = {}
 
         self.interface_type = ToolBoxInterfaces.native
         self.PREFIX = Style.CYAN(f"~{node()}@>")
         self.MOD_LIST = {}
         self.alive = True
         self.print(
             f"SYSTEM :: {node()}\nID -> {self.id},\nVersion -> {self.version},\n")
 
         if args.update:
-            self.run_any("cloudM", "#update-core")
+            os.system("git pull")
+            # self.save_load("CloudM")
+            # self.run_any("CloudM", "update_core")
 
         if args.get_version:
             v = self.version
             if args.mod_version_name != "mainTool":
                 v = self.run_any(args.mod_version_name, 'Version')
             self.print(f"Version {args.mod_version_name} : {v}")
 
@@ -190,14 +216,30 @@
             Style.GREEN(
                 f"Finish init up in t-{time.perf_counter() - t0}s"
             )
         )
 
         self.args_sto = args
 
+    @staticmethod
+    def exit_main(*args, **kwargs):
+        """proxi attr"""
+
+    @staticmethod
+    def hide_console(*args, **kwargs):
+        """proxi attr"""
+
+    @staticmethod
+    def show_console(*args, **kwargs):
+        """proxi attr"""
+
+    @staticmethod
+    def disconnect(*args, **kwargs):
+        """proxi attr"""
+
     def set_logger(self, debug=False):
         if "test" in self.prefix and not debug:
             logger, logging_filename = setup_logging(logging.NOTSET, name="toolbox-test", interminal=True,
                                                      file_level=logging.NOTSET)
             logger_info_str = "in Test Mode"
         elif "live" in self.prefix and not debug:
             logger, logging_filename = setup_logging(logging.DEBUG, name="toolbox-live", interminal=False,
@@ -212,14 +254,19 @@
             logger_info_str = "in debug Mode"
             self.debug = True
         elif debug:
             logger, logging_filename = setup_logging(logging.DEBUG, name=f"toolbox-{self.prefix}-debug",
                                                      interminal=True,
                                                      file_level=logging.DEBUG)
             logger_info_str = "in args debug Mode"
+        elif debug:
+            logger, logging_filename = setup_logging(logging.DEBUG, name=f"toolbox-{self.prefix}-debug",
+                                                     interminal=True,
+                                                     file_level=logging.DEBUG)
+            logger_info_str = "in args debug Mode"
         else:
             logger, logging_filename = setup_logging(logging.ERROR, name=f"toolbox-{self.prefix}")
             logger_info_str = "in Default"
 
         return logger_info_str, logger, logging_filename
 
     @property
@@ -231,15 +278,15 @@
             raise e
 
     def set_runnable(self, r):
         self.runnable = r
 
     def run_runnable(self, name, **kwargs):
         if name in self.runnable.keys():
-            return self.runnable[name](self, self.args_sto, **kwargs)
+            return self.runnable[name](get_app(from_="runner"), self.args_sto, **kwargs)
         self.print("Runnable Not Available")
 
     @debug.setter
     def debug(self, value):
         if not isinstance(value, bool):
             self.logger.debug(f"Value must be an boolean. is : {value} type of {type(value)}")
             raise ValueError("Value must be an boolean.")
@@ -294,16 +341,16 @@
         if self.mod_online(mod_name):
             self.logger.info(f"Reloading mod from : {loc + mod_name}")
             self.remove_mod(mod_name, spec=spec, delete=False)
 
         try:
             modular_file_object = import_module(loc + mod_name)
         except ModuleNotFoundError as e:
-            self.logger.error(Style.RED(f"module {loc +mod_name} not found is type sensitive {e}"))
-            self.print(Style.RED(f"module {loc +mod_name} not found is type sensitive {e}"))
+            self.logger.error(Style.RED(f"module {loc + mod_name} not found is type sensitive {e}"))
+            self.print(Style.RED(f"module {loc + mod_name} not found is type sensitive {e}"))
             return None
         try:
             tools_class = getattr(modular_file_object, "Tools")
         except AttributeError:
             tools_class = None
 
         modular_id = None
@@ -404,34 +451,38 @@
         return instance if tools_class is None else tools_class
 
     def save_initialized_module(self, tools_class, spec):
         tools_class.spec = spec
         live_tools_class = tools_class(app=self)
         return live_tools_class
 
-    def mod_online(self, mod_name):
+    def mod_online(self, mod_name, installed=False):
+        if installed and mod_name not in self.functions:
+            self.save_load(mod_name)
         return mod_name in self.functions
 
     def _get_function(self,
                       name: Enum or None,
                       state: bool = True,
                       specification: str = "app",
                       metadata=False, as_str: tuple or None = None, r=0):
 
-        if as_str is None:
+        if as_str is None and isinstance(name, Enum):
             modular_id = str(name.NAME.value)
             function_id = str(name.value)
+        elif as_str is None and isinstance(name, list):
+            modular_id, function_id = name[0], name[1]
         else:
             modular_id, function_id = as_str
 
         self.logger.info(f"getting function : {specification}.{modular_id}.{function_id}")
 
         if modular_id not in self.functions.keys():
             if r == 0:
-                self.save_load(modular_id)
+                self.save_load(modular_id, spec=specification)
                 return self.get_function(name=(modular_id, function_id),
                                          state=state,
                                          specification=specification,
                                          metadata=metadata,
                                          r=1)
             self.logger.warning(f"function modular not found {modular_id} 404")
             return "404", 100
@@ -465,15 +516,15 @@
             self.logger.info(f"returning stateless function")
             return function, 0
 
         instance = self.functions[modular_id].get(f"{specification}_instance")
         # instance_type = self.functions[modular_id].get(f"{specification}_instance_type", "functions/class")
 
         if params[0] == 'app':
-            instance = self
+            instance = get_app(from_=f"fuction {specification}.{modular_id}.{function_id}")
 
         if instance is None:
             self.logger.warning(f"No live Instance found")
             return "404", 400
 
         # if instance_type.endswith("/BC"):  # for backwards compatibility  functions/class/BC old modules
         #     # returning as stateless
@@ -497,15 +548,15 @@
         self.logger.info(f"returning stateful function")
         return higher_order_function, 0
 
     def save_exit(self):
         self.logger.info(f"save exiting saving data to {self.config_fh.file_handler_filename} states of {self.debug=}")
         self.config_fh.add_to_save_file_handler(self.keys["debug"], str(self.debug))
 
-    def load_mod(self, mod_name, mlm='I', **kwargs):
+    def load_mod(self, mod_name: str, mlm='I', **kwargs):
 
         self.logger.info(f"try opening module {mod_name}")
         action_list_helper = ['I (inplace load dill on error python)',
                               # 'C (coppy py file to runtime dir)',
                               # 'S (save py file to dill)',
                               # 'CS (coppy and save py file)',
                               # 'D (development mode, inplace load py file)'
@@ -544,15 +595,15 @@
 
         for om in open_modules:
             if om in module_list:
                 module_list.remove(om)
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             # Load modules in parallel using threads
-            futures = {executor.submit(self.load_mod, mod) for mod in module_list}
+            futures = {executor.submit(self.save_load, mod, 'app') for mod in module_list}
 
             for _ in concurrent.futures.as_completed(futures):
                 opened += 1
         self.logger.info(f"Opened {opened} modules in {time.perf_counter() - t0:.2f}s")
         return True
 
     def get_all_mods(self, working_dir="mods", path_to="./runtime"):
@@ -605,14 +656,19 @@
 
         def helper():
             if f"{spec}_instance" in self.functions[mod_name]:
                 del self.functions[mod_name][f"{spec}_instance"]
             if f"{spec}_instance_type" in self.functions[mod_name]:
                 del self.functions[mod_name][f"{spec}_instance_type"]
 
+        if on_exit is None and self.functions[mod_name].get(f"{spec}_instance_type", "").endswith("/BC"):
+            instanc = self.functions[mod_name].get(f"{spec}_instance", None)
+            if instanc is not None:
+                instanc._on_exit()
+
         if on_exit is None and delete:
             self.functions[mod_name] = {}
             del self.functions[mod_name]
             return
         if on_exit is None:
             helper()
             return
@@ -636,18 +692,20 @@
             helper()
 
             if delete:
                 self.functions[mod_name] = {}
                 del self.functions[mod_name]
 
     def exit(self):
+        if self.args_sto.debug:
+            self.hide_console()
+        self.disconnect()
         self.remove_all_modules()
-        self.logger.info("Exiting ToolBox")
-        self.print(Style.Bold(Style.CYAN("EXIT See U")))
-        self.print('\033', end="")
+        self.logger.info("Exiting ToolBox interface")
+        self.print(Style.Bold(Style.ITALIC("- ok -")))
         self.alive = False
         self.save_exit()
         self.config_fh.save_file_handler()
 
     def save_load(self, modname, spec='app'):
         self.logger.debug(f"Save load module {modname}")
         if not modname:
@@ -690,19 +748,22 @@
                      *args,
                      **kwargs) -> Result:
 
         if kwargs_ is not None and not kwargs:
             kwargs = kwargs_
         if args_ is not None and not args:
             args = args_
-
         if isinstance(mod_function_name, tuple):
             modular_name, function_name = mod_function_name
-        else:
+        elif isinstance(mod_function_name, list):
+            modular_name, function_name = mod_function_name[0], mod_function_name[1]
+        elif isinstance(mod_function_name, Enum):
             modular_name, function_name = mod_function_name.__class__.NAME.value, mod_function_name.value
+        else:
+            raise TypeError("Unknown function type")
 
         function_data, error_code = self.get_function(mod_function_name, state=tb_run_function_with_state,
                                                       metadata=True, specification=tb_run_with_specification)
         self.logger.info(f"Received fuction : {mod_function_name}, with execode: {error_code}")
         if error_code == 1 or error_code == 3 or error_code == 400:
             self.get_mod(modular_name)
             function_data, error_code = self.get_function(mod_function_name, state=tb_run_function_with_state,
@@ -736,15 +797,23 @@
         if not function:
             self.logger.warning(Style.RED(f"Function {function_name} not found"))
             return Result.default_internal_error(interface=self.interface_type,
                                                  exec_code=404,
                                                  info=f"function not found function").set_origin(mod_function_name)
 
         self.logger.info(f"Profiling function")
+        return self.fuction_runner(function, function_data, args, kwargs)
+
+    def fuction_runner(self, function, function_data: dict, args: list, kwargs: dict):
+
         parameters = function_data.get('params')
+        modular_name = function_data.get('module_name')
+        function_name = function_data.get('func_name')
+        mod_function_name = f"{modular_name}.{function_name}"
+
         if_self_state = 1 if 'self' in parameters else 0
 
         try:
             if len(parameters) == 0:
                 res = function()
             elif len(parameters) == len(args) + if_self_state:
                 res = function(*args)
@@ -753,14 +822,18 @@
             else:
                 res = function(*args, **kwargs)
             self.logger.info(f"Execution done")
             if isinstance(res, Result):
                 formatted_result = res
                 if formatted_result.origin is None:
                     formatted_result.set_origin(mod_function_name)
+            elif isinstance(res, ApiResult):
+                formatted_result = res
+                if formatted_result.origin is None:
+                    formatted_result.as_result().set_origin(mod_function_name).to_api_result()
             else:
                 # Wrap the result in a Result object
                 formatted_result = Result.ok(
                     interface=self.interface_type,
                     data_info="Auto generated result",
                     data=res,
                     info="Function executed successfully"
@@ -803,15 +876,15 @@
 
         if isinstance(mod_function_name, str) and isinstance(backwords_compability_variabel_string_holder, str):
             mod_function_name = (mod_function_name, backwords_compability_variabel_string_holder)
 
         res: Result = self.run_function(mod_function_name,
                                         tb_run_function_with_state=tb_run_function_with_state,
                                         tb_run_with_specification=tb_run_with_specification,
-                                        args_=args, kwargs_=kwargs)
+                                        args_=args, kwargs_=kwargs).as_result()
 
         if not get_results and isinstance(res, Result):
             return res.get()
 
         return res
 
     def get_mod(self, name, spec='app') -> ModuleType or toolboxv2.MainTool:
@@ -827,15 +900,31 @@
         if instance is None:
             return self.load_mod(name, spec=spec)
         return self.functions[name].get(f"{spec}_instance")
 
     @staticmethod
     def print(text, *args, **kwargs):
         # self.logger.info(f"Output : {text}")
-        print(text, *args, **kwargs)
+
+        # print(Style.CYAN("System:"), end=" ")
+        if isinstance(text, str) and kwargs == {} and text:
+            stram_print(text + ' '.join(args))
+        else:
+            print(text, *args, **kwargs)
+
+    @staticmethod
+    def sprint(text, *args, **kwargs):
+        # self.logger.info(f"Output : {text}")
+
+        print(Style.CYAN("System:"), end=" ")
+        if isinstance(text, str) and kwargs == {} and text:
+            stram_print(text + ' '.join(args))
+            print()
+        else:
+            print(text, *args, **kwargs)
 
     # ----------------------------------------------------------------
     # Decorators for the toolbox
 
     def _register_function(self, module_name, func_name, data):
         if module_name not in self.functions:
             self.functions[module_name] = {}
@@ -861,14 +950,15 @@
                           test=True,
                           samples=None,
                           state=None,
                           pre_compute=None,
                           post_compute=None,
                           memory_cache=False,
                           file_cache=False,
+                          request_as_kwarg=False,
                           memory_cache_max_size=100,
                           memory_cache_ttl=300):
 
         if isinstance(type_, Enum):
             type_ = type_.value
 
         if memory_cache and file_cache:
@@ -932,22 +1022,28 @@
             return wrapper
 
         def decorator(func):
             sig = signature(func)
             params = list(sig.parameters)
             module_name = mod_name if mod_name else func.__module__.split('.')[-1]
             func_name = name if name else func.__name__
+            if func_name == 'on_start':
+                func_name = 'on_startup'
+            if func_name == 'on_exit':
+                func_name = 'on_close'
             if api or pre_compute is not None or post_compute is not None or memory_cache or file_cache:
                 func = additional_process(func)
             if api and 'Result' == str(sig.return_annotation):
                 raise ValueError(f"Fuction {module_name}.{func_name} registered as "
                                  f"Api fuction but uses {str(sig.return_annotation)}\n"
                                  f"Please change the sig from ..)-> Result to ..)-> ApiResult")
             data = {
                 "type": type_,
+                "module_name": module_name,
+                "func_name": func_name,
                 "level": level,
                 "restrict_in_virtual_mode": restrict_in_virtual_mode,
                 "func": func,
                 "api": api,
                 "helper": helper,
                 "version": version,
                 "initial": initial,
@@ -955,14 +1051,15 @@
                 "__module__": func.__module__,
                 "signature": sig,
                 "params": params,
                 "state": (
                     False if len(params) == 0 else params[0] in ['self', 'state', 'app']) if state is None else state,
                 "do_test": test,
                 "samples": samples,
+                "request_as_kwarg": request_as_kwarg,
 
             }
             self._register_function(module_name, func_name, data)
             if exit_f:
                 if "on_exit" not in self.functions[module_name]:
                     self.functions[module_name]["on_exit"] = []
                 self.functions[module_name]["on_exit"].append(func_name)
@@ -985,14 +1082,15 @@
            restrict_in_virtual_mode: bool = False,
            api: bool = False,
            initial: bool = False,
            exit_f: bool = False,
            test_only: bool = False,
            memory_cache: bool = False,
            file_cache: bool = False,
+           request_as_kwarg: bool = False,
            state: bool or None = None,
            level: int = -1,
            memory_cache_max_size: int = 100,
            memory_cache_ttl: int = 300,
            samples: list or dict or None = None,
            interface: ToolBoxInterfaces or None or str = None,
            pre_compute=None,
@@ -1011,14 +1109,15 @@
         test (bool, optional): Flag to indicate if the function is for testing purposes.
         restrict_in_virtual_mode (bool, optional): Flag to restrict the function in virtual mode.
         api (bool, optional): Flag to indicate if the function is part of an API.
         initial (bool, optional): Flag to indicate if the function should be executed at initialization.
         exit_f (bool, optional): Flag to indicate if the function should be executed at exit.
         test_only (bool, optional): Flag to indicate if the function should only be used for testing.
         memory_cache (bool, optional): Flag to enable memory caching for the function.
+        request_as_kwarg (bool, optional): Flag to get request if the fuction is calld from api.
         file_cache (bool, optional): Flag to enable file caching for the function.
         state (bool or None, optional): Flag to indicate if the function maintains state.
         level (int, optional): The level of the function, used for prioritization or categorization.
         memory_cache_max_size (int, optional): Maximum size of the memory cache.
         memory_cache_ttl (int, optional): Time-to-live for the memory cache entries.
         samples (list or dict or None, optional): Samples or examples of function usage.
         interface (str, optional): The interface type for the function.
@@ -1027,15 +1126,15 @@
 
     Returns:
         function: The decorated function with additional processing and registration capabilities.
     """
         if interface is None:
             interface = "tb"
         if test_only and 'test' not in self.id:
-            return lambda x: x
+            return lambda *args, **kwargs: args
         return self._create_decorator(interface,
                                       name,
                                       mod_name,
                                       level=level,
                                       restrict_in_virtual_mode=restrict_in_virtual_mode,
                                       helper=helper,
                                       api=api,
@@ -1045,14 +1144,15 @@
                                       test=test,
                                       samples=samples,
                                       state=state,
                                       pre_compute=pre_compute,
                                       post_compute=post_compute,
                                       memory_cache=memory_cache,
                                       file_cache=file_cache,
+                                      request_as_kwarg=request_as_kwarg,
                                       memory_cache_max_size=memory_cache_max_size,
                                       memory_cache_ttl=memory_cache_ttl)
 
     def print_functions(self):
         if not self.functions:
             print("Nothing to see")
             return
@@ -1067,14 +1167,31 @@
                 func_type = data.get('type', 'Unknown')
                 func_level = 'r' if data['level'] == -1 else data['level']
                 api_status = 'Api' if data.get('api', False) else 'Non-Api'
 
                 print(f"  Function: {func_name}{data.get('signature', '()')}; "
                       f"Type: {func_type}, Level: {func_level}, {api_status}")
 
+    def save_autocompletion_dict(self):
+        autocompletion_dict = {}
+        for module_name, module in self.functions.items():
+            data = {}
+            for function_name, function_data in self.functions[module_name].items():
+                if not isinstance(function_data, dict):
+                    continue
+                data[function_name] = {arg: None for arg in
+                                       function_data.get("params", [])}  # TODO get default from sig
+                if len(data[function_name].keys()) == 0:
+                    data[function_name] = None
+            autocompletion_dict[module_name] = data if len(data.keys()) > 0 else None
+        self.config_fh.add_to_save_file_handler("auto~~~~~~", str(autocompletion_dict))
+
+    def get_autocompletion_dict(self):
+        return self.config_fh.get_file_handler("auto~~~~~~")
+
     def save_registry_as_enums(self, directory: str, filename: str):
         # Ordner erstellen, falls nicht vorhanden
         if not os.path.exists(directory):
             os.makedirs(directory)
 
         # Dateipfad vorbereiten
         filepath = os.path.join(directory, filename)
@@ -1084,15 +1201,20 @@
                         f'\nfrom enum import Enum\nfrom dataclasses import dataclass'
                         f'\n\n\n']
         for module, functions in self.functions.items():
             if module.startswith("APP_INSTANCE"):
                 continue
             class_name = module
             enum_members = "\n    ".join(
-                [f"{func_name.upper().replace('-', '')}: str = '{func_name}'" for func_name in functions])
+                [
+                    f"{func_name.upper().replace('-', '')}:"
+                    f" str = '{func_name}'  "
+                    f"# Input: ({fuction_data['params'] if isinstance(fuction_data, dict) else ''}),"
+                    f" Output: {fuction_data['signature'].return_annotation if isinstance(fuction_data, dict) else 'None'}"
+                    for func_name, fuction_data in functions.items()])
             enum_class = (f'@dataclass\nclass {class_name.upper().replace(".", "_").replace("-", "")}(Enum):'
                           f"\n    NAME = '{class_name}'\n    {enum_members}")
             enum_classes.append(enum_class)
 
         # Enums in die Datei schreiben
         with open(filepath, 'w') as file:
             file.write("\n\n\n".join(enum_classes))
@@ -1171,14 +1293,286 @@
                 all_data['errors'] += infos['error']
             all_data[module_name] = infos
         print(f"{all_data['modular_run']=}\n{all_data['modular_sug']=}\n{all_data['modular_fatal_error']=}")
 
         return Result.ok(data=all_data, data_info=analyze_data(all_data))
 
 
+class ProxyApp(metaclass=Singleton):
+    def __init__(self, app: App, host='0.0.0.0', port=6587, timeout=15):
+        self.app = app
+        self.client = None
+        self.port = port
+        self.host = host
+        self.timeout = timeout
+        self.remote_functions = ["run_any",
+                                 "remove_mod",
+                                 "save_load",
+                                 "exit_main",
+                                 "show_console",
+                                 "hide_console",
+                                 "rrun_runnable",
+                                 "get_autocompletion_dict",
+                                 "exit_main"]
+        self.connect()
+
+    def connect(self):
+        from toolboxv2.mods.SocketManager import SocketType
+        client_result = self.app.run_any(SOCKETMANAGER.CREATE_SOCKET,
+                                         get_results=True,
+                                         name='DemonApp-client',
+                                         host=self.host,
+                                         port=self.port,
+                                         type_id=SocketType.client,
+                                         max_connections=-1,
+                                         return_full_object=True)
+
+        if client_result.is_error():
+            raise Exception(f"Client error: {client_result.print(False)}")
+        if not client_result.is_data():
+            raise Exception(f"Client error: {client_result.print(False)}")
+        if client_result.get('connection_error') != 0:
+            raise Exception(f"Client error: {client_result.print(False)}")
+        # 'socket': socket,
+        # 'receiver_socket': r_socket,
+        # 'host': host,
+        # 'port': port,
+        # 'p2p-port': endpoint_port,
+        # 'sender': send,
+        # 'receiver_queue': receiver_queue,
+        # 'connection_error': connection_error,
+        # 'receiver_thread': s_thread,
+        # 'keepalive_thread': keep_alive_thread,
+        # 'running_dict': running_dict,
+        # 'client_to_receiver_thread': to_receive,
+        # 'client_receiver_threads': threeds,
+        self.client = client_result
+
+    def disconnect(self):
+        time.sleep(1)
+        running_dict = self.client.get("running_dict")
+        sender = self.client.get("sender")
+        running_dict["server_receiver"] = False
+        running_dict["receive"]['main'] = False
+        running_dict["keep_alive_var"] = False
+        sender({'exit': True})
+        self.client = None
+
+    def reconnect(self):
+        if self.client is not None:
+            self.disconnect()
+        self.connect()
+
+    def verify(self):
+        time.sleep(1)
+        self.client.get('sender')({'keepalive': 0})
+
+    def __getattr__(self, name):
+
+        if self.client is None:
+            self.reconnect()
+        # print(f"ProxyApp: {name}, {self.client is None}")
+        if name == "on_exit":
+            self.disconnect()
+        if name == "rc":
+            self.reconnect()
+            return
+        if name == "r":
+            try:
+                return self.client.get('receiver_queue').get(timeout=self.timeout)
+            except:
+                return "No data"
+
+        app_attr = getattr(self.app, name)
+
+        def method(*args, **kwargs):
+            # if name == 'run_any':
+            #     print("method", name, kwargs.get('get_results', False), args[0])
+            if kwargs.get('spec', '-') == 'app':
+                return app_attr(*args, **kwargs)
+            try:
+                if name in self.remote_functions:
+                    if name == 'run_any' and not kwargs.get('get_results', False):
+                        return app_attr(*args, **kwargs)
+                    if name == 'run_any' and kwargs.get('get_results', False):
+                        if isinstance(args[0], Enum):
+                            args = (args[0].__class__.NAME.value, args[0].value), args[1:]
+                    self.app.sprint(f"Calling method {name}")
+                    self.client.get('sender')({'name': name, 'args': args, 'kwargs': kwargs})
+                    while Spinner("Waiting for result"):
+                        try:
+                            data = self.client.get('receiver_queue').get(timeout=self.timeout)
+                            if isinstance(data, dict) and 'identifier' in data:
+                                del data["identifier"]
+                            if 'error' in data and 'origin' in data and 'result' in data and 'info' in data:
+                                data = ApiResult(**data).as_result()
+                            return data
+                        except:
+                            print("No data look later with app.r")
+                            return "No data look later"
+            except:
+                if self.client.get('socket') is None:
+                    self.client = None
+            return app_attr(*args, **kwargs)
+
+        if callable(app_attr) and name in self.remote_functions and self.client is not None:
+            return method
+        return app_attr
+
+
+class DemonApp(metaclass=Singleton):
+    def __init__(self, app: App, host='0.0.0.0', port=6587, t=False):
+        self.app: App = app
+        self.server = None
+        self.port = port
+        self.host = host
+        self.start_server()
+        if t:
+            threading.Thread(target=self.connect, daemon=True).start()
+
+    def start_server(self):
+        """Start the server using app and the socket manager"""
+
+        from toolboxv2.mods.SocketManager import SocketType
+        server_result = self.app.run_any(SOCKETMANAGER.CREATE_SOCKET,
+                                         get_results=True,
+                                         name='DemonApp-server',
+                                         host=self.host,
+                                         port=self.port,
+                                         type_id=SocketType.server,
+                                         max_connections=-1,
+                                         return_full_object=True)
+        if server_result.is_error():
+            raise Exception(f"Server error: {server_result.print(False)}")
+        if not server_result.is_data():
+            raise Exception(f"Server error: {server_result.print(False)}")
+        if server_result.get('connection_error') != 0:
+            raise Exception(f"Server error: {server_result.print(False)}")
+
+        self.server = server_result
+        # 'socket': socket,
+        # 'receiver_socket': r_socket,
+        # 'host': host,
+        # 'port': port,
+        # 'p2p-port': endpoint_port,
+        # 'sender': send,
+        # 'receiver_queue': receiver_queue,
+        # 'connection_error': connection_error,
+        # 'receiver_thread': s_thread,
+        # 'keepalive_thread': keep_alive_thread,
+        # 'running_dict': running_dict,
+        # 'client_to_receiver_thread': to_receive,
+        # 'client_receiver_threads': threeds,
+
+    def connect(self):
+        receiver_queue: queue.Queue = self.server.get('receiver_queue')
+        client_to_receiver_thread = self.server.get('client_to_receiver_thread')
+        running_dict = self.server.get('running_dict')
+        sender = self.server.get('sender')
+        known_clients = {}
+        valid_clients = {}
+        while self.app.alive:
+
+            if receiver_queue.not_empty:
+                data = receiver_queue.get()
+                if not data:
+                    continue
+                if 'identifier' not in data:
+                    continue
+
+                identifier = data.get('identifier', 'unknown')
+                try:
+
+                    if identifier == "new_con":
+                        client, address = data.get('data')
+                        print("New connection:", address)
+                        known_clients[str(address)] = client
+                        client_to_receiver_thread(client, str(address))
+
+                    # validation
+                    if identifier in known_clients:
+                        print(identifier)
+                        if identifier.startswith("('127.0.0.1'"):
+                            valid_clients[identifier] = known_clients[identifier]
+                        elif data.get("claim", False):
+                            do = self.app.run_any(("CloudM.UserInstances", "validate_ws_id"),
+                                             ws_id=data.get("claim"))[0]
+                            print(do)
+                            if do:
+                                valid_clients[identifier] = known_clients[identifier]
+                        else:
+                            print("Validating Failed: ", identifier)
+                            sender({'Validating Failed': -1}, eval(identifier))
+                        print("Validating New:", identifier)
+                        del known_clients[identifier]
+
+                    if identifier in valid_clients:
+                        print("New valid Request:", identifier)
+                        name = data.get('name')
+                        args = data.get('args')
+                        kwargs = data.get('kwargs')
+
+                        print("Request data:", name, args, kwargs)
+
+                        if name == 'exit_main':
+                            self.app.alive = False
+                            break
+
+                        if name == 'show_console':
+                            show_console(True)
+                            sender({'ok': 0}, eval(identifier))
+                            continue
+
+                        if name == 'hide_console':
+                            show_console(False)
+                            sender({'ok': 0}, eval(identifier))
+                            continue
+
+                        if name == 'rrun_runnable':
+                            show_console(True)
+                            runnner = getattr(self.app, "run_runnable")
+                            threading.Thread(target=runnner, args=args, kwargs=kwargs, daemon=True).start()
+                            sender({'ok': 0}, eval(identifier))
+                            show_console(False)
+                            continue
+
+                        def helper_runner():
+                            try:
+                                res = getattr(self.app, name)(*args, **kwargs)
+
+                                print("sending response0")
+                                if res is None:
+                                    res = {'data': res}
+                                elif isinstance(res, Result):
+                                    res = json.loads(res.to_api_result().json())
+                                elif isinstance(res, bytes):
+                                    pass
+                                elif isinstance(res, dict):
+                                    pass
+                                else:
+                                    res = {'data': 'unsupported type', 'type': str(type(res))}
+
+                                print("sending response", res, type(res))
+
+                                sender(res, eval(identifier))
+                            except Exception as e:
+                                sender({"data": str(e)}, eval(identifier))
+
+                        threading.Thread(target=helper_runner, daemon=True).start()
+
+                except Exception as e:
+                    print(Style.RED(f"An error occurred on {identifier} {str(e)}"))
+                    if identifier != "unknown":
+                        running_dict["receive"][str(identifier)] = False
+        running_dict["server_receiver"] = False
+        for x in running_dict["receive"].keys():
+            running_dict["receive"][x] = False
+        running_dict["keep_alive_var"] = False
+
+
 def analyze_data(data):
     report = []
 
     for mod_name, mod_info in data.items():
         if mod_name in ['modular_run', 'modular_fatal_error', 'modular_sug']:
             continue  # Überspringen der allgemeinen Statistiken
         if mod_name in ['errors']:
@@ -1220,16 +1614,34 @@
     fh.open_s_file_handler()
     fh.file_handler_storage.write(str(data))
     fh.file_handler_storage.close()
 
     logger.info("Done!")
 
 
-def get_app(from_=None, name=None, args=AppArgs().default()) -> App:
+registered_apps = [None]
+
+
+def override_main_app(app):
+    global registered_apps
+    registered_apps[0] = app
+    return app
+
+
+def get_app(from_=None, name=None, args=AppArgs().default(), app_con=None) -> App:
+    global registered_apps
+
+    # print(f"get app requested from: {from_}")
+    if registered_apps[0] is not None:
+        return registered_apps[0]
+
+    if app_con is None:
+        app_con = App
     logger = get_logger()
     logger.info(Style.GREYBG(f"get app requested from: {from_}"))
     if name:
-        app = App(name, args=args)
+        app = app_con(name, args=args)
     else:
-        app = App()
+        app = app_con()
     logger.info(Style.Bold(f"App instance, returned ID: {app.id}"))
+    registered_apps[0] = app
     return app
```

### Comparing `ToolBoxV2-0.1.6/toolboxv2/utils/types.py` & `ToolBoxV2-0.1.8/toolboxv2/utils/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     port = 8000
     host = '0.0.0.0'
     load_all_mod_in_files = False
     mods_folder = 'toolboxv2.mods.'
     debug = None
     test = None
     profiler = None
+    hot_reload = False
 
     def default(self):
         return self
 
 
 class ApiOb:
     token = ""
@@ -107,27 +108,39 @@
             info=ToolBoxInfo(
                 exec_code=self.info.exec_code,
                 help_text=self.info.help_text
             ) if self.info else None,
             origin=self.origin
         )
 
+    def to_api_result(self):
+        return self
+
+    def print(self, *args, **kwargs):
+        res = self.as_result().print(*args, **kwargs)
+        if not isinstance(res, str):
+            res = res.to_api_result()
+        return res
+
 
 class Result:
     def __init__(self,
                  error: ToolBoxError,
                  result: ToolBoxResult,
                  info: ToolBoxInfo,
                  origin: Optional[Any] = None,
                  ):
         self.error: ToolBoxError = error
         self.result: ToolBoxResult = result
         self.info: ToolBoxInfo = info
         self.origin = origin
 
+    def as_result(self):
+        return self
+
     def set_origin(self, origin):
         if self.origin is not None:
             raise ValueError("You cannot Change the origin of a Result!")
         self.origin = origin
         return self
 
     def is_error(self):
@@ -135,25 +148,25 @@
             return self.result.data.is_error()
         return self.info.exec_code != 0
 
     def is_data(self):
         return self.result.data is not None
 
     def to_api_result(self):
-        print(f" error={self.error}, result= {self.result}, info= {self.info}, origin= {self.origin}")
+        # print(f" error={self.error}, result= {self.result}, info= {self.info}, origin= {self.origin}")
         return ApiResult(
             error=self.error.value if isinstance(self.error, Enum) else self.error,
             result=ToolBoxResultBM(
                 data_to=self.result.data_to.value if isinstance(self.result.data_to, Enum) else self.result.data_to,
                 data_info=self.result.data_info,
                 data=self.result.data,
                 data_type=self.result.data_type
             ) if self.result else None,
             info=ToolBoxInfoBM(
-                exec_code=self.info.exec_code,
+                exec_code=self.info.exec_code,  # exec_code umwandel in http resposn codes
                 help_text=self.info.help_text
             ) if self.info else None,
             origin=self.origin
         )
 
     @classmethod
     def default(cls, interface=ToolBoxInterfaces.native):
@@ -187,38 +200,40 @@
     def default_internal_error(cls, info="", exec_code=-2, interface=ToolBoxInterfaces.native, data=None):
         error = ToolBoxError.internal_error
         info = ToolBoxInfo(exec_code, info)
         result = ToolBoxResult(data_to=interface, data=data, data_type=type(data).__name__)
         return cls(error=error, info=info, result=result)
 
     def print(self, show=True, show_data=True, prifix=""):
-        data = '\n' + f"{((prifix + 'Data: ' + str(self.result.data) if self.result.data is not None else 'NO Data') if not isinstance(self.result.data, Result) else self.print(show=False, show_data=show_data, prifix=prifix + '-')) if show_data else 'Data: private'}"
+        data = '\n' + f"{((prifix + 'Data: ' + str(self.result.data) if self.result.data is not None else 'NO Data') if not isinstance(self.result.data, Result) else self.result.data.print(show=False, show_data=show_data, prifix=prifix + '-')) if show_data else 'Data: private'}"
         origin = '\n' + f"{prifix + 'Origin: ' + str(self.origin) if self.origin is not None else 'NO Origin'}"
         text = (f"Function Exec coed: {self.info.exec_code}"
                 f"\n{prifix}Info's:"
-                f" {self.info.help_text} {'<|> '+str(self.result.data_info) if self.result.data_info is not None else ''}"
+                f" {self.info.help_text} {'<|> ' + str(self.result.data_info) if self.result.data_info is not None else ''}"
                 f"{origin}{data if not data.endswith('NO Data') else ''}")
         if not show:
             return text
-        print(text)
+        print("\n======== Result ========\n" + text + "\n------- EndOfD -------")
         return self
 
     def log(self, show_data=True, prifix=""):
         from toolboxv2 import get_logger
         get_logger().debug(self.print(show=False, show_data=show_data, prifix=prifix).replace("\n", " - "))
         return self
 
     def __str__(self):
         return self.print(show=False, show_data=True)
 
-    def get(self):
+    def get(self, key=None, default=None):
         data = self.result.data
         if isinstance(data, Result):
-            return data.get()
-        return data
+            return data.get(key=key, default=default)
+        if key is not None and isinstance(data, dict):
+            return data.get(key, default)
+        return data if data is not None else default
 
     def lazy_return(self, _=0, data=None, **kwargs):
         flags = ['raise', 'logg', 'user', 'intern']
         if isinstance(_, int):
             flag = flags[_]
         else:
             flag = _
@@ -227,17 +242,19 @@
         if flag == 'raise':
             raise ValueError(self.print(show=False))
         if flag == 'logg':
             from .. import get_logger
             get_logger().error(self.print(show=False))
 
         if flag == 'user':
-            return self if data is None else data if test_is_result(data) else self.default_user_error(data=data, **kwargs)
+            return self if data is None else data if test_is_result(data) else self.default_user_error(data=data,
+                                                                                                       **kwargs)
         if flag == 'intern':
-            return self if data is None else data if test_is_result(data) else self.default_internal_error(data=data, **kwargs)
+            return self if data is None else data if test_is_result(data) else self.default_internal_error(data=data,
+                                                                                                           **kwargs)
 
         return self if data is None else data if test_is_result(data) else self.custom_error(data=data, **kwargs)
 
 
 def test_is_result(data: Result):
     return isinstance(data, Result)
 
@@ -249,12 +266,20 @@
     args: list or None = field(default=None)
     kwargs: dict or None = field(default=None)
 
     @classmethod
     def empty(cls):
         return cls()
 
+    def __str__(self):
+        if self.args is not None and self.kwargs is not None:
+            return (f"{self.module_name} {self.function_name} " + ' '.join(self.args) +
+                    ' '.join([key + '-' + str(val) for key, val in self.kwargs.items()]))
+        if self.args is not None:
+            return f"{self.module_name} {self.function_name} " + ' '.join(self.args)
+        return f"{self.module_name} {self.function_name}"
+
     def print(self, show=True):
         s = f"{self.module_name=};{self.function_name=};{self.args=};{self.kwargs=}"
         if not show:
             return s
         print(s)
```

