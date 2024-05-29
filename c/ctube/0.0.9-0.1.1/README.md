# Comparing `tmp/ctube-0.0.9.tar.gz` & `tmp/ctube-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.9.tar", max compression
+gzip compressed data, was "ctube-0.1.1.tar", max compression
```

## Comparing `ctube-0.0.9.tar` & `ctube-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.9/LICENSE
--rw-r--r--   0        0        0     1030 2024-05-27 16:09:35.545847 ctube-0.0.9/README.md
--rw-r--r--   0        0        0       22 2024-05-27 16:09:35.545847 ctube-0.0.9/ctube/__init__.py
--rw-r--r--   0        0        0     5015 2024-05-27 16:09:35.549180 ctube-0.0.9/ctube/app.py
--rw-r--r--   0        0        0     1990 2024-05-27 16:09:35.549180 ctube-0.0.9/ctube/callbacks.py
--rw-r--r--   0        0        0      552 2024-05-25 21:58:58.300542 ctube-0.0.9/ctube/cli.py
--rw-r--r--   0        0        0     2223 2024-05-26 06:41:38.369693 ctube-0.0.9/ctube/cmds.py
--rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.9/ctube/colors.py
--rw-r--r--   0        0        0      293 2024-05-27 16:09:35.549180 ctube-0.0.9/ctube/containers.py
--rw-r--r--   0        0        0     4065 2024-05-27 16:09:35.549180 ctube-0.0.9/ctube/download.py
--rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.9/ctube/errors.py
--rw-r--r--   0        0        0     2085 2024-05-27 16:09:35.549180 ctube-0.0.9/ctube/extractors.py
--rw-r--r--   0        0        0     2264 2024-05-27 16:09:35.559181 ctube-0.0.9/ctube/helpers.py
--rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.9/ctube/parser.py
--rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.9/ctube/paths.py
--rw-r--r--   0        0        0     1634 2024-05-27 16:09:35.562515 ctube-0.0.9/ctube/printers.py
--rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.9/ctube/terminal.py
--rw-r--r--   0        0        0      641 2024-05-27 16:09:35.562515 ctube-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 ctube-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-28 13:50:44.292748 ctube-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1030 2024-05-29 08:14:11.031332 ctube-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 08:14:17.121290 ctube-0.1.1/ctube/__init__.py
+-rw-r--r--   0        0        0     5694 2024-05-29 08:05:47.505350 ctube-0.1.1/ctube/app.py
+-rw-r--r--   0        0        0     1978 2024-05-28 13:50:44.469417 ctube-0.1.1/ctube/callbacks.py
+-rw-r--r--   0        0        0      638 2024-05-28 13:50:44.486084 ctube-0.1.1/ctube/cli.py
+-rw-r--r--   0        0        0     2223 2024-05-28 13:50:44.446083 ctube-0.1.1/ctube/cmds.py
+-rw-r--r--   0        0        0      664 2024-05-28 13:50:44.419417 ctube-0.1.1/ctube/colors.py
+-rw-r--r--   0        0        0      293 2024-05-28 13:50:44.446083 ctube-0.1.1/ctube/containers.py
+-rw-r--r--   0        0        0     4349 2024-05-29 07:50:49.396834 ctube-0.1.1/ctube/download.py
+-rw-r--r--   0        0        0      486 2024-05-29 07:50:10.927208 ctube-0.1.1/ctube/errors.py
+-rw-r--r--   0        0        0     2085 2024-05-28 13:50:44.456084 ctube-0.1.1/ctube/extractors.py
+-rw-r--r--   0        0        0     2271 2024-05-29 08:02:17.744257 ctube-0.1.1/ctube/helpers.py
+-rw-r--r--   0        0        0     1892 2024-05-28 13:50:44.419417 ctube-0.1.1/ctube/parser.py
+-rw-r--r--   0        0        0       79 2024-05-28 13:50:44.419417 ctube-0.1.1/ctube/paths.py
+-rw-r--r--   0        0        0     1634 2024-05-28 13:50:44.469417 ctube-0.1.1/ctube/printers.py
+-rw-r--r--   0        0        0     2072 2024-05-28 13:50:44.432750 ctube-0.1.1/ctube/terminal.py
+-rw-r--r--   0        0        0      641 2024-05-29 08:14:34.107842 ctube-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 ctube-0.1.1/PKG-INFO
```

### Comparing `ctube-0.0.9/LICENSE` & `ctube-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/README.md` & `ctube-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.9-blue)
+![Version](https://img.shields.io/badge/version-0.1.1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
```

### Comparing `ctube-0.0.9/ctube/app.py` & `ctube-0.1.1/ctube/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 from typing import List, Optional, Tuple
+from urllib import request
 from urllib.error import URLError
 from innertube.clients import InnerTube
 from ctube.download import Downloader
 from ctube.errors import InvalidIndexSyntax
 from ctube.terminal import Prompt
 from ctube.containers import Album
 from ctube.colors import Color
@@ -32,22 +33,26 @@
 
 
 class App:
     def __init__(
             self, 
             output_path: str,
             skip_existing: bool = True,
+            timeout: int = 5,
+            max_retries: int = 3
     ):
         self.client = InnerTube("WEB_REMIX")
         self.prompt = Prompt()
         self.downloader = Downloader(
             output_path=output_path, 
             skip_existing=skip_existing,
             on_complete_callback=on_complete_callback,
-            on_progress_callback=on_progress_callback
+            on_progress_callback=on_progress_callback,
+            timeout=timeout,
+            max_retries=max_retries
         )
 
         # last search
         self._albums: Optional[List[Album]] = None
         self._artist_name: Optional[str] = None
 
     def main_loop(self) -> None:
@@ -130,19 +135,30 @@
                     write(f"Selected items:", Color.BLUE)
 
                 for album in albums:
                     write(f"\u2022 {album.title}", Color.BOLD)
 
                 for album in albums:
                     write(f":: Downloading: {album.title}", Color.GREEN)
+
                     try:
-                        self.downloader.download(album=album, artist=self._artist_name)
-                    except (URLError, TimeoutError) as error:
-                        write(f"A connection error occurred while downloading: {album.title}", Color.RED)
-                        write(f"Reason: {str(error)}", Color.RED)
-                        break
+                        response = request.urlopen(album.thumbnail_url)
+                        image_data = response.read()
+                    except URLError:
+                        write(f"An error occurred while downloading {album.title} cover art", Color.RED)
+                        write(f"Skipping {album.title}", Color.YELLOW)
+                    else:
+                        for song, error in self.downloader.download_album(
+                                album=album, 
+                                artist=self._artist_name,
+                                image_data=image_data
+                        ):
+                            print()
+                            if error:
+                                write(f"An error occurred while downloading {song.title}", Color.RED)
+                                write(f"Reason: {str(error)}", Color.RED)
                 print('\033[?25h', end="")
 
     @staticmethod
     def _exit():
         sys.stdout.write('\033[?25h')
         sys.exit(0)
```

### Comparing `ctube-0.0.9/ctube/callbacks.py` & `ctube-0.1.1/ctube/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 def on_complete_callback(song: Song) -> None:
     output = f"{os.path.splitext(song.filepath)[0]}.mp3"
     mp4 = AudioSegment.from_file(song.filepath, "mp4")
     mp4.export(output, format="mp3")
     set_metadata(filepath=output, song=song)
     os.remove(song.filepath)
-    print()
 
 
 def set_metadata(filepath: str, song: Song) -> None:
     audio = eyed3.load(filepath)
     album = song.album
     if audio and audio.tag:
         tag = audio.tag
```

### Comparing `ctube-0.0.9/ctube/cli.py` & `ctube-0.1.1/ctube/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 
 socket.setdefaulttimeout(3)
 signal(SIGINT, lambda signum, _: signal_handler(signum))
 request.default_range_size = request.default_range_size // 15
 
 
 def main() -> None:
-    app = App(output_path=MUSIC)
+    app = App(
+        output_path=MUSIC, 
+        skip_existing=False,
+        timeout=5,
+        max_retries=3
+    )
     app.main_loop()
     signal_handler()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ctube-0.0.9/ctube/cmds.py` & `ctube-0.1.1/ctube/cmds.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/ctube/colors.py` & `ctube-0.1.1/ctube/colors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/ctube/download.py` & `ctube-0.1.1/ctube/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
+from urllib.error import HTTPError
 from pathvalidate import sanitize_filename
+from http.client import IncompleteRead
 from enum import Enum
-from urllib import request
-from urllib.error import HTTPError
-from typing import Callable, List
+from typing import Callable, Generator
 from ctube.containers import Album, Song
 from pytubefix import Playlist, Stream, YouTube
-from pytubefix.exceptions import (
-        MembersOnly, 
-        RecordingUnavailable, 
-        VideoPrivate, 
-        VideoUnavailable
-)
+from pytubefix.exceptions import VideoUnavailable
+from ctube.errors import NoMP4StreamAvailable, EmptyStreamQuery
 
 
 class BaseURL(str, Enum):
     PLAYLIST = "https://music.youtube.com/playlist?list="
 
 
 class Downloader:
     def __init__(
             self,
             output_path: str,
             on_complete_callback: Callable[[Song], None],
             on_progress_callback: Callable[[Song, int, int], None],
-            skip_existing: bool = False
+            skip_existing: bool = False,
+            timeout: int = 5,
+            max_retries: int = 2
     ):
         self.output_path = output_path
         self.on_complete_callback = on_complete_callback 
         self.on_progress_callback = on_progress_callback
         self.skip_existing = skip_existing
+        self.timeout = timeout
+        self.max_retries = max_retries
 
     @property
     def output_path(self) -> str:
         return self._output_path
 
     @output_path.setter
     def output_path(self, output_path: str) -> None:
@@ -50,51 +50,32 @@
         self.on_complete_callback(data)
 
     def _on_progress_callback(self, data: Song, bytes_remaining: int, stream: Stream) -> None:
         filesize = stream.filesize
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
-    def download(self, album: Album, artist: str) -> List[YouTube]:
-        playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{album.playlist_id}")
-        failed_downloads: List[YouTube] = []
-
-        response = request.urlopen(album.thumbnail_url)
-        image_data = response.read()
-
-        final_destination = os.path.join(
+    def download_album(
+            self, 
+            album: Album, 
+            artist: str, 
+            image_data: bytes, 
+    ) -> Generator:
+        output_path = os.path.join(
             os.path.join(
                 self.output_path, sanitize_filename(artist)
             ), 
             sanitize_filename(album.title)
         )
+        os.makedirs(output_path, exist_ok=True)
 
-        os.makedirs(final_destination, exist_ok=True)
-
+        playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{album.playlist_id}")
         for i, url in enumerate(playlist):
             youtube = YouTube(url=url)
 
-            try:
-                stream = youtube.streams
-            except (
-                    MembersOnly, 
-                    RecordingUnavailable, 
-                    VideoPrivate, 
-                    VideoUnavailable,
-                    KeyError  # This is a bug in pytubefix I think.
-            ):
-                failed_downloads.append(youtube)
-                continue
-
-            audio_stream = stream.get_audio_only(subtype="mp4")
-
-            if not audio_stream:
-                failed_downloads.append(youtube)
-                continue
-
             song = Song(
                 title=youtube.title,
                 artist=artist,
                 track_num=i + 1,
                 image_data=image_data,
                 filepath="",
                 album=album
@@ -104,22 +85,43 @@
                 lambda stream, _, bytes_remaining: self._on_progress_callback(
                     song, bytes_remaining, stream
                 )
             )
             youtube.register_on_complete_callback(
                 lambda _, filepath: self._on_complete_callback(
                     song, 
-                    filepath  # type: ignore
-                    # pytubefix says that 'filepath' can be None, 
-                    # but this is not possible.
+                    filepath  # type: ignore | another problem with pytubefix ?
                 )
             )
 
             try:
-                audio_stream.download(
-                    output_path=final_destination,
-                    skip_existing=self.skip_existing
-                )
-            except HTTPError:
-                failed_downloads.append(youtube)
-
-        return failed_downloads
+                self._download_song(youtube, output_path=output_path)
+            except (
+                    VideoUnavailable,
+                    IncompleteRead, 
+                    TimeoutError,
+                    EmptyStreamQuery,
+                    NoMP4StreamAvailable,
+                    HTTPError,
+                    KeyError # https://github.com/JuanBindez/pytubefix/issues/88
+            ) as err:
+                error = err
+            else:
+                error = None
+
+            yield song, error
+
+    def _download_song(self, youtube: YouTube, output_path: str) -> None:
+        streams = youtube.streams
+        if not len(streams):
+            raise EmptyStreamQuery(f"The song '{youtube.title}' did not provide any data streams")
+        else:
+            stream = streams.get_audio_only(subtype="mp4")
+            if stream is None:
+                raise NoMP4StreamAvailable("Unexpected status: MP4 stream unavailable")
+
+        stream.download(
+            output_path=output_path,
+            skip_existing=self.skip_existing,
+            timeout=self.timeout,
+            max_retries=self.max_retries
+        )
```

### Comparing `ctube-0.0.9/ctube/extractors.py` & `ctube-0.1.1/ctube/extractors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/ctube/helpers.py` & `ctube-0.1.1/ctube/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 def handle_connection_errors(func: Callable) -> Callable:
     def inner(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except RequestError:
             write("Invalid request", Color.RED)
         except (ConnectTimeout, ReadTimeout):
-            write("An error occurred. try again.", Color.RED)
+            write("A timeout error occurred. Try again.", Color.RED)
         except (ConnectError, URLError):
             write("No internet connection", Color.RED)
     return inner
 
 
 def connected_to_internet(url: str = 'http://www.google.com/', timeout: int = 5) -> bool:
     try:
```

### Comparing `ctube-0.0.9/ctube/parser.py` & `ctube-0.1.1/ctube/parser.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/ctube/printers.py` & `ctube-0.1.1/ctube/printers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/ctube/terminal.py` & `ctube-0.1.1/ctube/terminal.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.9/pyproject.toml` & `ctube-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.9"
+version = "0.1.1"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
```

### Comparing `ctube-0.0.9/PKG-INFO` & `ctube-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.9
+Version: 0.1.1
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,15 +21,15 @@
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
 Requires-Dist: requests (>=2.32.2,<3.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
-![Version](https://img.shields.io/badge/version-0.0.9-blue)
+![Version](https://img.shields.io/badge/version-0.1.1-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ---
 ctube is a simple program for downloading music. Written in Python, ctube has a command line interface.\
 Download in mp3 at the highest quality available. Metadata is automatically embedded in files (including cover art).\
 Type help for more information about the available commands and how they work.
```

