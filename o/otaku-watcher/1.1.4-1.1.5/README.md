# Comparing `tmp/otaku_watcher-1.1.4.tar.gz` & `tmp/otaku_watcher-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otaku_watcher-1.1.4.tar", last modified: Wed May  1 09:53:38 2024, max compression
+gzip compressed data, was "otaku_watcher-1.1.5.tar", last modified: Wed May 29 21:36:39 2024, max compression
```

## Comparing `otaku_watcher-1.1.4.tar` & `otaku_watcher-1.1.5.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:53:38.182571 otaku_watcher-1.1.4/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1063 2024-04-28 15:35:00.000000 otaku_watcher-1.1.4/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3083 2024-05-01 09:53:38.182571 otaku_watcher-1.1.4/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      850 2024-05-01 09:52:10.000000 otaku_watcher-1.1.4/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:53:38.179237 otaku_watcher-1.1.4/mov_cli_anime/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      117 2024-04-28 15:46:27.000000 otaku_watcher-1.1.4/mov_cli_anime/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:53:38.179237 otaku_watcher-1.1.4/otaku_watcher/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-05-01 09:53:30.000000 otaku_watcher-1.1.4/otaku_watcher/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:53:38.182571 otaku_watcher-1.1.4/otaku_watcher/anitaku/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 17:40:35.000000 otaku_watcher-1.1.4/otaku_watcher/anitaku/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5232 2024-04-09 23:43:21.000000 otaku_watcher-1.1.4/otaku_watcher/anitaku/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:53:38.182571 otaku_watcher-1.1.4/otaku_watcher.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3083 2024-05-01 09:53:38.000000 otaku_watcher-1.1.4/otaku_watcher.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      335 2024-05-01 09:53:38.000000 otaku_watcher-1.1.4/otaku_watcher.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-01 09:53:38.000000 otaku_watcher-1.1.4/otaku_watcher.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       86 2024-05-01 09:53:38.000000 otaku_watcher-1.1.4/otaku_watcher.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       28 2024-05-01 09:53:38.000000 otaku_watcher-1.1.4/otaku_watcher.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1226 2024-04-28 15:52:07.000000 otaku_watcher-1.1.4/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-01 09:53:38.182571 otaku_watcher-1.1.4/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1063 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3079 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      846 2024-05-28 21:10:14.000000 otaku_watcher-1.1.5/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      402 2024-05-29 21:36:30.000000 otaku_watcher-1.1.5/otaku_watcher/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher/anitaku/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/otaku_watcher/anitaku/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5233 2024-05-29 21:35:54.000000 otaku_watcher-1.1.5/otaku_watcher/anitaku/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:36:39.452244 otaku_watcher-1.1.5/otaku_watcher.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3079 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      309 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       86 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-05-29 21:36:39.000000 otaku_watcher-1.1.5/otaku_watcher.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1226 2024-05-01 10:29:15.000000 otaku_watcher-1.1.5/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-29 21:36:39.455577 otaku_watcher-1.1.5/setup.cfg
```

### Comparing `otaku_watcher-1.1.4/LICENSE` & `otaku_watcher-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `otaku_watcher-1.1.4/PKG-INFO` & `otaku_watcher-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otaku-watcher
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
         Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,15 +46,15 @@
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # otaku-watcher
   <sub>A mov-cli plugin for watching anime.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
+  <img src="https://github.com/JDALab/otaku-watcher/assets/123201787/2df8d707-b472-48b3-aaa1-f6d5154c686d">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
```

### Comparing `otaku_watcher-1.1.4/README.md` & `otaku_watcher-1.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
 
   # otaku-watcher
   <sub>A mov-cli plugin for watching anime.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
+  <img src="https://github.com/JDALab/otaku-watcher/assets/123201787/2df8d707-b472-48b3-aaa1-f6d5154c686d">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
```

### Comparing `otaku_watcher-1.1.4/otaku_watcher/anitaku/scraper.py` & `otaku_watcher-1.1.5/otaku_watcher/anitaku/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         dood = soup.find("li", {"class": "doodstream"})
 
         if streamwish:
             url = self.__streamwish(streamwish.find("a")["data-video"])
         elif dood:
             url = self.__dood(dood.find("a")["data-video"])
 
-        if metadata.type == MetadataType.MOVIE:
+        if metadata.type == MetadataType.SINGLE:
             return Single(
                 url,
                 title = metadata.title,
                 referrer = self.base_url,
                 year = metadata.year,
                 subtitles = None
             )
@@ -91,17 +91,17 @@
                 _soup = self.soup(page)
 
                 episode_page = _soup.find("ul", {"id": "episode_page"})
                 li = episode_page.findAll("li")
                 last = li[-1].find("a")["ep_end"]
 
                 if last == "1":
-                    type = MetadataType.MOVIE
+                    type = MetadataType.SINGLE
                 else:
-                    type = MetadataType.SERIES
+                    type = MetadataType.MULTI
 
                 info_body = _soup.find("div", {"class": "anime_info_body_bg"})
 
                 _p = info_body.findAll("p")
 
                 genres = _p[3].findAll("a")
```

### Comparing `otaku_watcher-1.1.4/otaku_watcher.egg-info/PKG-INFO` & `otaku_watcher-1.1.5/otaku_watcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otaku-watcher
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mov-cli plugin for watching anime.
 License: MIT License
         
         Copyright (c) 2024 JDALab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,15 +46,15 @@
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # otaku-watcher
   <sub>A mov-cli plugin for watching anime.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-gogotaku/assets/132799819/1436339c-f2c3-4c37-b9ae-0da6b83faf8d">
+  <img src="https://github.com/JDALab/otaku-watcher/assets/123201787/2df8d707-b472-48b3-aaa1-f6d5154c686d">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
```

### Comparing `otaku_watcher-1.1.4/pyproject.toml` & `otaku_watcher-1.1.5/pyproject.toml`

 * *Files identical despite different names*

