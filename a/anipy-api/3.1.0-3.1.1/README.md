# Comparing `tmp/anipy_api-3.1.0.tar.gz` & `tmp/anipy_api-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.1.0.tar", max compression
+gzip compressed data, was "anipy_api-3.1.1.tar", max compression
```

## Comparing `anipy_api-3.1.0.tar` & `anipy_api-3.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      227 2024-05-25 15:13:05.716186 anipy_api-3.1.0/README.md
--rw-r--r--   0        0        0      847 2024-05-25 15:13:05.716186 anipy_api-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5493 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11550 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/error.py
--rw-r--r--   0        0        0     7953 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2651 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0      183 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12240 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     8521 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/yugen_provider.py
--rw-r--r--   0        0        0     1482 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-29 11:08:11.630784 anipy_api-3.1.1/README.md
+-rw-r--r--   0        0        0      825 2024-05-29 11:08:11.630784 anipy_api-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-29 11:08:11.630784 anipy_api-3.1.1/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5493 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/error.py
+-rw-r--r--   0        0        0     8130 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2651 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0      183 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12198 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     8588 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/providers/yugen_provider.py
+-rw-r--r--   0        0        0      896 2024-05-29 11:08:11.634784 anipy_api-3.1.1/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 anipy_api-3.1.1/PKG-INFO
```

### Comparing `anipy_api-3.1.0/pyproject.toml` & `anipy_api-3.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.1.0"
+version = "3.1.1"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
@@ -14,15 +14,14 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-ffmpeg = "^2.0.11"
 pycryptodomex = "^3.20.0"
 requests = "^2.32.0"
-pypresence = "^4.3.0"
 m3u8 = "^4.1.0"
 beautifulsoup4 = "^4.12.3"
 python-mpv = "^1.0.6"
 dataclasses-json = "^0.6.4"
 levenshtein = "^0.25.1"
 
 [tool.poetry.urls]
```

### Comparing `anipy_api-3.1.0/src/anipy_api/anime.py` & `anipy_api-3.1.1/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/download.py` & `anipy_api-3.1.1/src/anipy_api/download.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/error.py` & `anipy_api-3.1.1/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/locallist.py` & `anipy_api-3.1.1/src/anipy_api/locallist.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,17 @@
             try:
                 self.data = LocalListData.from_json(self.file.read_text())
             except KeyError:
                 if migrate_cb is None:
                     raise
                 self.data = migrate_cb(self.file)
 
+    def _read(self):
+        self.data = LocalListData.from_json(self.file.read_text())
+
     def update(
         self, anime: Union[Anime, LocalListEntry], **update_fields
     ) -> LocalListEntry:
         """Update (or add) an anime in the local list.
 
         Example:
             ```python
@@ -132,14 +135,16 @@
         Returns:
             The updated entry
 
         Raises:
             ArgumentError: Raised if updating a anime that does not exist (adding) and not providing at
                 least the `episode` and `language` to the update_fields.
         """
+        self._read()
+
         uid = self._get_uid(anime)
         entry = self.data.data.get(uid, None)
 
         if entry is None:
             if not ("episode" in update_fields and "language" in update_fields):
                 raise ArgumentError(
                     "The anime you are trying to update is not added to the list and you are not"
@@ -177,14 +182,16 @@
 
         Args:
             anime: The anime to delete this can be a [Anime][anipy_api.anime.Anime] or [LocalListEntry][anipy_api.locallist.LocalListEntry] object
 
         Returns:
             The deleted object or None if the anime to delete was not found in the local list
         """
+        self._read()
+
         entry = self.data.data.pop(self._get_uid(anime), None)
         self.data.write(self.file)
 
         return entry
 
     def get(self, anime: Anime) -> Optional[LocalListEntry]:
         """Get a specific local list entry.
@@ -192,22 +199,26 @@
         Args:
             anime: The anime to get the local list entry from
 
         Returns:
             A local list entry if it exists for the provided anime
 
         """
+        self._read()
+
         return self.data.data.get(self._get_uid(anime), None)
 
     def get_all(self) -> List[LocalListEntry]:
         """Get all of the local list entries.
 
         Returns:
             A list of all local list entries
         """
+        self._read()
+
         return list(self.data.data.values())
 
     @staticmethod
     def _get_uid(anime: Union[Anime, LocalListEntry]) -> str:
         if isinstance(anime, Anime):
             provider = anime.provider.NAME
             identifier = anime.identifier
```

### Comparing `anipy_api-3.1.0/src/anipy_api/mal.py` & `anipy_api-3.1.1/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/base.py` & `anipy_api-3.1.1/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/player.py` & `anipy_api-3.1.1/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/players/mpv.py` & `anipy_api-3.1.1/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.1.1/src/anipy_api/player/players/mpv_control.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.1.1/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/player/players/vlc.py` & `anipy_api-3.1.1/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/__init__.py` & `anipy_api-3.1.1/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/base.py` & `anipy_api-3.1.1/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/filter.py` & `anipy_api-3.1.1/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/provider.py` & `anipy_api-3.1.1/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.1.1/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     BaseFilter,
     FilterCapabilities,
     Filters,
     MediaType,
     Season,
     Status,
 )
-from anipy_api.provider.utils import weak_lru, parsenum, request_page
+from anipy_api.provider.utils import parsenum, request_page
 
 if TYPE_CHECKING:
     from anipy_api.provider import Episode
 
 
 @functools.lru_cache()
 def _get_enc_keys(session: Session, embed_url: str):
@@ -172,15 +172,14 @@
                             identifier, name, languages={LanguageTypeEnum.SUB}
                         )
                     else:
                         results[identifier].languages.add(LanguageTypeEnum.SUB)
 
         return list(results.values())
 
-    @weak_lru()
     def get_episodes(self, identifier: str, lang: LanguageTypeEnum) -> List["Episode"]:
         if lang == LanguageTypeEnum.DUB:
             urls = [
                 f"{self.BASE_URL}/category/{identifier}-dub",
                 f"{self.BASE_URL}/category/{identifier}-japanese-dub",
             ]
         else:
@@ -217,15 +216,14 @@
             )
             for x in BeautifulSoup(res.text, "html.parser").find_all("li")
         ]
         ep_list.reverse()
 
         return ep_list
 
-    @weak_lru()
     def get_info(self, identifier: str) -> "ProviderInfoResult":
         req = Request("GET", f"{self.BASE_URL}/category/{identifier}")
         res = request_page(self.session, req)
 
         soup = BeautifulSoup(res.text, "html.parser")
         info_body = soup.find("div", {"class": "anime_info_body_bg"})
```

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/providers/yugen_provider.py` & `anipy_api-3.1.1/src/anipy_api/provider/providers/yugen_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     BaseFilter,
     FilterCapabilities,
     Filters,
     MediaType,
     Season,
     Status,
 )
-from anipy_api.provider.utils import weak_lru, request_page
+from anipy_api.provider.utils import request_page
 
 if TYPE_CHECKING:
     from anipy_api.provider import Episode
 
 
 class YugenFilter(BaseFilter):
     def _apply_query(self, query: str):
@@ -123,15 +123,14 @@
                         identifier=identifier, name=name, languages=languages
                     )
                 )
 
             page += 1
         return results
 
-    @weak_lru()
     def get_episodes(self, identifier: str, lang: LanguageTypeEnum) -> List["Episode"]:
         identifier = base64.b64decode(identifier).decode()
         req = Request("GET", f"{self.BASE_URL}/anime/{identifier}")
         result = request_page(self.session, req)
 
         if lang == LanguageTypeEnum.SUB:
             match = re.search(
@@ -146,15 +145,14 @@
 
         if match is None:
             raise LangTypeNotAvailableError(identifier, self.NAME, lang)
 
         eps = int(match.group(1))
         return list(range(1, eps + 1))
 
-    @weak_lru()
     def get_info(self, identifier: str) -> "ProviderInfoResult":
         identifier = base64.b64decode(identifier).decode()
         req = Request("GET", f"{self.BASE_URL}/anime/{identifier}")
         result = request_page(self.session, req)
         data_map = {
             "name": None,
             "image": None,
@@ -162,14 +160,19 @@
             "synopsis": None,
             "release_year": None,
             "status": None,
             "alternative_names": [],
         }
 
         soup = BeautifulSoup(result.text, "html.parser")
+
+        name = soup.find("h1")
+        if name is not None:
+            data_map["name"] = name.get_text()
+
         synopsis = soup.find("p", attrs={"class": "description"})
         if synopsis is not None:
             data_map["synopsis"] = synopsis.get_text("\n")
 
         image = soup.find("img", attrs={"class": "cover"})
         if image is not None:
             data_map["image"] = image.get("src")  # type: ignore
```

### Comparing `anipy_api-3.1.0/src/anipy_api/provider/utils.py` & `anipy_api-3.1.1/src/anipy_api/provider/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """These are only internal utils, which are not made to be used outside"""
 
-import functools
-import weakref
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from requests import Request, Session, Response
 
 
 def request_page(session: "Session", req: "Request") -> "Response":
@@ -36,29 +34,7 @@
     Returns:
 
     """
     try:
         return int(n)
     except ValueError:
         return float(n)
-
-
-def weak_lru(maxsize: int = 128):
-    """Decorator to memoize a class method
-    (see: [https://stackoverflow.com/a/68052994](https://stackoverflow.com/a/68052994))
-
-    Args:
-        maxsize: Maximum cache size
-    """
-
-    def wrapper(func):
-        @functools.lru_cache(maxsize)
-        def _func(_self, *args, **kwargs):
-            return func(_self(), *args, **kwargs)
-
-        @functools.wraps(func)
-        def inner(self, *args, **kwargs):
-            return _func(weakref.ref(self), *args, **kwargs)
-
-        return inner
-
-    return wrapper
```

### Comparing `anipy_api-3.1.0/PKG-INFO` & `anipy_api-3.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.1.0
+Version: 3.1.1
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: levenshtein (>=0.25.1,<0.26.0)
 Requires-Dist: m3u8 (>=4.1.0,<5.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
-Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: python-ffmpeg (>=2.0.11,<3.0.0)
 Requires-Dist: python-mpv (>=1.0.6,<2.0.0)
 Requires-Dist: requests (>=2.32.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-api
 Project-URL: Repository, https://github.com/sdaqo/anipy-cli
 Description-Content-Type: text/markdown
```

