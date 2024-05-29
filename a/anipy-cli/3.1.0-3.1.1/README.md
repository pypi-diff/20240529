# Comparing `tmp/anipy_cli-3.1.0.tar.gz` & `tmp/anipy_cli-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.1.0.tar", max compression
+gzip compressed data, was "anipy_cli-3.1.1.tar", max compression
```

## Comparing `anipy_cli-3.1.0.tar` & `anipy_cli-3.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2308 2024-05-25 15:11:01.412294 anipy_cli-3.1.0/README.md
--rw-r--r--   0        0        0      855 2024-05-25 15:11:59.031561 anipy_cli-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-25 15:11:59.038561 anipy_cli-3.1.0/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      609 2024-05-16 13:57:50.981018 anipy_cli-3.1.0/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2815 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3197 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2675 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2258 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15422 2024-05-25 14:53:26.203390 anipy_cli-3.1.0/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-16 13:57:50.982018 anipy_cli-3.1.0/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24077 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     6179 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-16 13:57:50.983018 anipy_cli-3.1.0/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     7229 2024-05-25 14:53:26.203390 anipy_cli-3.1.0/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-25 14:04:15.858789 anipy_cli-3.1.0/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2308 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/README.md
+-rw-r--r--   0        0        0      855 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      817 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2806 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3187 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2666 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-29 11:13:09.800448 anipy_cli-3.1.1/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15422 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24105 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     6772 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7229 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-05-29 11:13:09.804448 anipy_cli-3.1.1/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 anipy_cli-3.1.1/PKG-INFO
```

### Comparing `anipy_cli-3.1.0/README.md` & `anipy_cli-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/pyproject.toml` & `anipy_cli-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.1.0"
+version = "3.1.1"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 yaspin = "^3.0.2"
 inquirerpy = "^0.3.4"
 appdirs = "^1.4.4"
 pypresence = "^4.3.0"
-anipy-api = "^3.1.0"
+anipy-api = "^3.1.1"
 
 [tool.poetry.scripts]
 anipy-cli = "anipy_cli.cli:run_cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sdaqo/anipy-cli/issues"
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/arg_parser.py` & `anipy_cli-3.1.1/src/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/cli.py` & `anipy_cli-3.1.1/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/default_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from typing import TYPE_CHECKING, Optional
 
 from anipy_api.locallist import LocalList
 
 from anipy_cli.clis.base_cli import CliBase
 from anipy_cli.colors import colors
 from anipy_cli.config import Config
@@ -50,22 +49,22 @@
             )
             self.epsiode = episodes[0]
             return
 
         anime = search_show_prompt("default")
 
         if anime is None:
-            sys.exit(0)
+            return False
 
         self.lang = lang_prompt(anime)
 
         episode = pick_episode_prompt(anime, self.lang)
 
         if episode is None:
-            sys.exit(0)
+            return False
 
         self.anime = anime
         self.epsiode = episode
 
     def process(self):
         assert self.anime is not None
         assert self.epsiode is not None
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/download_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from typing import TYPE_CHECKING, Optional, List
 
 from anipy_api.download import Downloader
 
 from anipy_cli.clis.base_cli import CliBase
 from anipy_cli.colors import colors, cprint
 from anipy_cli.config import Config
@@ -46,15 +45,15 @@
                 "download", self.options.search
             )
             return
 
         anime = search_show_prompt("download")
 
         if anime is None:
-            sys.exit(0)
+            return False
 
         self.lang = lang_prompt(anime)
 
         episodes = pick_episode_range_prompt(anime, self.lang)
 
         self.anime = anime
         self.episodes = episodes
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/history_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 from typing import TYPE_CHECKING, Optional
 
 from anipy_api.anime import Anime
 from anipy_api.locallist import LocalList, LocalListEntry
 from InquirerPy import inquirer
 
 from anipy_cli.clis.base_cli import CliBase
@@ -35,25 +34,25 @@
 
     def take_input(self):
         history = self.history_list.get_all()
         history.sort(key=lambda h: h.timestamp, reverse=True)
 
         if not history:
             print("You have no History, exiting")
-            sys.exit(0)
+            return False
 
         entry = inquirer.fuzzy(  # type: ignore
             message="Select History Entry:",
             choices=history,
             long_instruction="To cancel this prompt press ctrl+z",
             mandatory=False,
         ).execute()
 
         if entry is None:
-            sys.exit(0)
+            return False
 
         self.history_entry = entry
         self.anime = Anime.from_local_list_entry(entry)
 
     def process(self):
         assert self.anime is not None
         assert self.history_entry is not None
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.1.1/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/colors.py` & `anipy_cli-3.1.1/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/config.py` & `anipy_cli-3.1.1/src/anipy_cli/config.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/discord.py` & `anipy_cli-3.1.1/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.1.1/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.1.1/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.1.1/src/anipy_cli/menus/mal_menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,15 @@
                         mappings.update({anime: result})
                         s.write(
                             f"> Successfully mapped {anime.id} to {result.identifier}"
                         )
 
                     counter += 1
                     s.set_text(f"Progress: {counter / to_map_length * 100:.1f}%")
-                except:
+                except:  # noqa: E722
                     failed.append(anime)
 
             with ThreadPoolExecutor(max_workers=5) as pool:
                 futures = [pool.submit(do_map, a, len(to_map)) for a in to_map]
                 try:
                     for future in as_completed(futures):
                         future.result()
@@ -578,15 +578,15 @@
                         mappings.update({entry: result})
                         s.write(
                             f"> Successfully mapped {anime.identifier} to {result.id}"
                         )
 
                     counter += 1
                     s.set_text(f"Progress: {counter / to_map_length * 100}%")
-                except:
+                except:  # noqa: E722
                     failed.append(entry)
 
             with ThreadPoolExecutor(max_workers=5) as pool:
                 futures = [pool.submit(do_map, a, len(to_map)) for a in to_map]
                 try:
                     for future in as_completed(futures):
                         future.result()
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/menus/menu.py` & `anipy_cli-3.1.1/src/anipy_cli/menus/menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,28 +32,31 @@
         self.anime = anime
         self.stream = stream
         self.player = player
         self.lang = stream.language
         self.history_list = LocalList(
             Config()._history_file_path, migrate_cb=migrate_locallist
         )
+        self.seasonal_list = LocalList(Config()._seasonal_file_path, migrate_locallist)
 
     @property
     def menu_options(self) -> List["MenuOption"]:
         return [
             MenuOption("Next Episode", self.next_ep, "n"),
             MenuOption("Previous Episode", self.prev_ep, "p"),
             MenuOption("Replay Episode", self.repl_ep, "r"),
             MenuOption(
                 f"Change to {'sub' if self.lang == LanguageTypeEnum.DUB else 'dub'}",
                 self.change_type,
                 "c",
             ),
             MenuOption("Select episode", self.selec_ep, "s"),
+            MenuOption("Select from history", self.selec_hist, "h"),
             MenuOption("Search for Anime", self.search, "a"),
+            MenuOption("Add to seasonals", self.add_seasonal, "t"),
             MenuOption("Print Video Info", self.video_info, "i"),
             MenuOption("Download Episode", self.download_video, "d"),
             MenuOption("Quit", self.quit, "q"),
         ]
 
     def print_header(self):
         cprint(
@@ -132,14 +135,20 @@
     def selec_ep(self):
         episode = pick_episode_prompt(self.anime, self.lang)
         if episode is None:
             return
         self._start_episode(episode)
         self.print_options()
 
+    def selec_hist(self):
+        from anipy_cli.clis.history_cli import HistoryCli
+
+        hist_cli = HistoryCli(self.options)
+        hist_cli.run()
+
     def search(self):
         search_result = search_show_prompt("default")
         if search_result is None:
             return
         self.anime = search_result
         episode = pick_episode_prompt(self.anime, self.lang)
         if episode is None:
@@ -149,14 +158,20 @@
 
     def video_info(self):
         print(f"Show Name: {self.anime.name}")
         print(f"Provider: {self.anime.provider.NAME}")
         print(f"Stream Url: {self.stream.url}")
         print(f"Quality: {self.stream.resolution}p")
 
+    def add_seasonal(self):
+        self.seasonal_list.update(
+            self.anime, episode=self.stream.episode, language=self.stream.language
+        )
+        cprint(colors.GREEN, "Anime added to seasonals!")
+
     def download_video(self):
         config = Config()
         with DotSpinner("Starting Download...") as s:
 
             def progress_indicator(percentage: float):
                 s.set_text(f"Downloading ({percentage:.1f}%)")
```

### Comparing `anipy_cli-3.1.0/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.1.1/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/prompts.py` & `anipy_cli-3.1.1/src/anipy_cli/prompts.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/src/anipy_cli/util.py` & `anipy_cli-3.1.1/src/anipy_cli/util.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.1.0/PKG-INFO` & `anipy_cli-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.1.0
+Version: 3.1.1
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anipy-api (>=3.1.0,<4.0.0)
+Requires-Dist: anipy-api (>=3.1.1,<4.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-cli
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.0 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.1.1 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Requires-Dist: anipy-api (>=3.1.0,<4.0.0) Requires-Dist: appdirs
+Python :: 3.12 Requires-Dist: anipy-api (>=3.1.1,<4.0.0) Requires-Dist: appdirs
 (>=1.4.4,<2.0.0) Requires-Dist: inquirerpy (>=0.3.4,<0.4.0) Requires-Dist:
 pypresence (>=4.3.0,<5.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
 Dist: yaspin (>=3.0.2,<4.0.0) Project-URL: Bug Tracker, https://github.com/
 sdaqo/anipy-cli/issues Project-URL: Documentation, https://sdaqo.github.io/
 anipy-cli/getting-started-cli Project-URL: Repository, https://github.com/
 sdaqo/anipy-cli Description-Content-Type: text/markdown # ANIPY-CLI **Anime
 from the comfort of your Terminal**
```

