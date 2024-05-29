# Comparing `tmp/film_central-1.3.14.tar.gz` & `tmp/film_central-1.3.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "film_central-1.3.14.tar", last modified: Wed May  1 09:32:25 2024, max compression
+gzip compressed data, was "film_central-1.3.16.tar", last modified: Wed May 29 21:50:11 2024, max compression
```

## Comparing `film_central-1.3.14.tar` & `film_central-1.3.16.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.182373 film_central-1.3.14/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 film_central-1.3.14/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3147 2024-05-01 09:32:25.182373 film_central-1.3.14/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      851 2024-05-01 07:25:53.000000 film_central-1.3.14/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.179040 film_central-1.3.14/film_central/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      580 2024-05-01 07:27:34.000000 film_central-1.3.14/film_central/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.179040 film_central-1.3.14/film_central/vadapav/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vadapav/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7071 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vadapav/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.179040 film_central-1.3.14/film_central/vidsrcme/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcme/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4309 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcme/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.182373 film_central-1.3.14/film_central/vidsrcto/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcto/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.182373 film_central-1.3.14/film_central/vidsrcto/ext/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcto/ext/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcto/ext/vidplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4508 2024-05-01 07:13:14.000000 film_central-1.3.14/film_central/vidsrcto/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.182373 film_central-1.3.14/film_central.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3147 2024-05-01 09:32:25.000000 film_central-1.3.14/film_central.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      536 2024-05-01 09:32:25.000000 film_central-1.3.14/film_central.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-01 09:32:25.000000 film_central-1.3.14/film_central.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-05-01 09:32:25.000000 film_central-1.3.14/film_central.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       27 2024-05-01 09:32:25.000000 film_central-1.3.14/film_central.egg-info/top_level.txt
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-01 09:32:25.182373 film_central-1.3.14/mov_cli_films/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      115 2024-05-01 08:48:28.000000 film_central-1.3.14/mov_cli_films/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1279 2024-05-01 07:27:31.000000 film_central-1.3.14/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-01 09:32:25.182373 film_central-1.3.14/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 film_central-1.3.16/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3143 2024-05-29 21:50:11.921027 film_central-1.3.16/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      848 2024-05-29 21:46:07.000000 film_central-1.3.16/README.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.917693 film_central-1.3.16/film_central/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      580 2024-05-29 21:50:05.000000 film_central-1.3.16/film_central/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/film_central/vadapav/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.16/film_central/vadapav/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7072 2024-05-29 21:46:07.000000 film_central-1.3.16/film_central/vadapav/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/film_central/vidsrcme/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.16/film_central/vidsrcme/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4308 2024-05-29 21:46:07.000000 film_central-1.3.16/film_central/vidsrcme/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/film_central/vidsrcto/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.16/film_central/vidsrcto/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/film_central/vidsrcto/ext/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-05-01 07:13:14.000000 film_central-1.3.16/film_central/vidsrcto/ext/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-05-01 07:13:14.000000 film_central-1.3.16/film_central/vidsrcto/ext/vidplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4481 2024-05-29 21:46:07.000000 film_central-1.3.16/film_central/vidsrcto/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-29 21:50:11.921027 film_central-1.3.16/film_central.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3143 2024-05-29 21:50:11.000000 film_central-1.3.16/film_central.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      510 2024-05-29 21:50:11.000000 film_central-1.3.16/film_central.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-29 21:50:11.000000 film_central-1.3.16/film_central.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-05-29 21:50:11.000000 film_central-1.3.16/film_central.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-05-29 21:50:11.000000 film_central-1.3.16/film_central.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1261 2024-05-29 21:50:00.000000 film_central-1.3.16/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-29 21:50:11.921027 film_central-1.3.16/setup.cfg
```

### Comparing `film_central-1.3.14/LICENSE` & `film_central-1.3.16/LICENSE`

 * *Files identical despite different names*

### Comparing `film_central-1.3.14/PKG-INFO` & `film_central-1.3.16/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: film-central
-Version: 1.3.14
+Version: 1.3.16
 Summary: A mov-cli plugin for watching Films and Shows.
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -47,15 +47,15 @@
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # film-central
   <sub>A mov-cli plugin for watching Films and Shows.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+  <img src="https://github.com/JDALab/film-central/assets/123201787/e8150d96-64bf-437b-a768-4fdd6a45a2a0">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
```

### Comparing `film_central-1.3.14/README.md` & `film_central-1.3.16/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
 
   # film-central
   <sub>A mov-cli plugin for watching Films and Shows.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+  <img src="https://github.com/JDALab/film-central/assets/123201787/e8150d96-64bf-437b-a768-4fdd6a45a2a0">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
@@ -29,8 +29,8 @@
 [mov-cli.plugins]
 films = "film-central"
 ```
 
 ## Usage
 ```sh
 mov-cli -s films the rookie
-```
+```
```

### Comparing `film_central-1.3.14/film_central/__init__.py` & `film_central-1.3.16/film_central/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
         "DEFAULT": VidSrcToScraper,
         "vidsrcme": VidSrcMeScraper,
         "vadapav": VadapavScraper,
         "vidsrcto": VidSrcToScraper
     } # NOTE: WE ARE IN NEED OF GOOD AND STABLE PROVIDERS 😭
 }
 
-__version__ = "1.3.14"
+__version__ = "1.3.16"
```

### Comparing `film_central-1.3.14/film_central/vadapav/scraper.py` & `film_central-1.3.16/film_central/vadapav/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             else:  # If "4K" is found
                 return 2160  # Assumed resolution for 4K
         else:
             return 0  # Default to 0 if resolution is not found
 
     def scrape(self, metadata: Metadata, episode: utils.EpisodeSelector) -> Multi | Single:
 
-        if metadata.type == MetadataType.MOVIE:
+        if metadata.type == MetadataType.SINGLE:
             mov_dir_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
             movie_soup = self.soup(mov_dir_html)
             mov_files = [
                 x
                 for x in movie_soup.find_all("a", {"class": "file-entry"})
                 if x.string[-4:] not in [".srt", ".txt"]
             ]
```

### Comparing `film_central-1.3.14/film_central/vidsrcme/scraper.py` & `film_central-1.3.16/film_central/vidsrcme/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,19 @@
             if hls_url is not None:
                 url = hls_url
                 break
 
         return url
 
     def __get_embed(self, metadata: Metadata, episode: EpisodeSelector) -> Response:
-        media_type = "tv" if metadata.type == MetadataType.SERIES else "movie"
+        media_type = "tv" if metadata.type == MetadataType.MULTI else "movie"
 
         url = f"{self.base_url}/embed/{media_type}/{metadata.id}"
 
-        if metadata.type == MetadataType.SERIES:
+        if metadata.type == MetadataType.MULTI:
             url += f"/{episode.season}/{episode.episode}"
 
         return self.http_client.get(url)
 
     def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:        
         for _ in range(self.MAX_TRIES):
             vidsrc = self.__get_embed(metadata, episode)
@@ -111,15 +111,15 @@
             prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers.get("Location", None)
 
             if prourl is not None:
                 break
 
         url = self.__get_url(prourl)
 
-        if metadata.type == MetadataType.MOVIE:
+        if metadata.type == MetadataType.SINGLE:
             return Single(
                 url = url,
                 title = metadata.title,
                 referrer = "https://vidsrc.stream/",
                 year = metadata.year
             )
```

### Comparing `film_central-1.3.14/film_central/vidsrcto/ext/vidplay.py` & `film_central-1.3.16/film_central/vidsrcto/ext/vidplay.py`

 * *Files identical despite different names*

### Comparing `film_central-1.3.14/film_central/vidsrcto/scraper.py` & `film_central-1.3.16/film_central/vidsrcto/scraper.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
     from httpx import Response
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
+from mov_cli.scraper import Scraper
 from mov_cli.utils import EpisodeSelector
-from mov_cli.scraper import Scraper, MediaNotFound
 from mov_cli import Multi, Single, Metadata, MetadataType
 
 import base64
 from urllib.parse import unquote
 from .ext import VidPlay
 from mov_cli.utils.scraper import TheMovieDB
 
@@ -41,46 +41,49 @@
                 continue
 
             yield search_result
 
     def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
         return self.tmdb.scrape_episodes(metadata)
 
-    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:
+    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Optional[Multi | Single]:
         embed_response = self.__get_embed(metadata, episode)
 
         soup = self.soup(embed_response)
 
         id = soup.find('a', {'data-id': True})
 
         if not id:
-            raise MediaNotFound(metadata.title, self)
+            return None
 
         id = id.get("data-id", None)
 
         sources = self.http_client.get(self.sources.format(id)).json()
 
         vidplay_id = None
 
         for source in sources["result"]:
             if source["title"] == "Vidplay":
                 vidplay_id = source["id"]
 
         if not vidplay_id:
-            raise MediaNotFound(metadata.title, self)
+            return None
 
         get_source = self.http_client.get(self.source.format(vidplay_id)).json()["result"]["url"]
 
         vidplay_url = self.__deobf(get_source)
 
         vidplay = VidPlay(self.http_client)
 
         url = vidplay.resolve_source(vidplay_url)[0]
-        
-        if metadata.type == MetadataType.SERIES:
+
+        if url is None:
+            return None
+
+        if metadata.type == MetadataType.MULTI:
             return Multi(
                 url = url,
                 title = metadata.title,
                 episode = episode,
                 referrer = self.referrer
             )
 
@@ -88,19 +91,19 @@
             url = url,
             title = metadata.title,
             year = metadata.year,
             referrer = self.referrer
         )
 
     def __get_embed(self, metadata: Metadata, episode: EpisodeSelector) -> Response:
-        media_type = "tv" if metadata.type == MetadataType.SERIES else "movie"
+        media_type = "tv" if metadata.type == MetadataType.MULTI else "movie"
 
         url = f"{self.base_url}/embed/{media_type}/{metadata.id}"
 
-        if metadata.type == MetadataType.SERIES:
+        if metadata.type == MetadataType.MULTI:
             url += f"/{episode.season}/{episode.episode}"
 
         return self.http_client.get(url)
 
     def __deobf(self, encoded_url: str) -> str | bool:
         # This is based on https://github.com/Ciarands/vidsrc-to-resolver/blob/dffa45e726a4b944cb9af0c9e7630476c93c0213/vidsrc.py#L16
         # Thanks to @Ciarands!
```

### Comparing `film_central-1.3.14/film_central.egg-info/PKG-INFO` & `film_central-1.3.16/film_central.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: film-central
-Version: 1.3.14
+Version: 1.3.16
 Summary: A mov-cli plugin for watching Films and Shows.
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -47,15 +47,15 @@
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # film-central
   <sub>A mov-cli plugin for watching Films and Shows.</sub>
 
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+  <img src="https://github.com/JDALab/film-central/assets/123201787/e8150d96-64bf-437b-a768-4fdd6a45a2a0">
 
 </div>
 
 > [!CAUTION]
 > We are on the lookout for maintainers and if we don't find any soon this project may become unmaintained! Please consider or nominate a friend. Thank you.
 
 ## Installation
```

### Comparing `film_central-1.3.14/pyproject.toml` & `film_central-1.3.16/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 version = { attr = "film_central.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["mov_cli_films*", "film_central*"]
+include = ["film_central*"]
```

