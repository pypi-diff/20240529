# Comparing `tmp/twiner-0.3.0.tar.gz` & `tmp/twiner-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twiner-0.3.0.tar", max compression
+gzip compressed data, was "twiner-0.4.0.tar", max compression
```

## Comparing `twiner-0.3.0.tar` & `twiner-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-01-31 20:23:18.857000 twiner-0.3.0/LICENSE
--rw-r--r--   0        0        0     5752 2024-02-22 19:32:17.391760 twiner-0.3.0/README.md
--rw-r--r--   0        0        0     1013 2024-05-12 23:34:57.344763 twiner-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       45 2024-02-22 20:08:23.511838 twiner-0.3.0/twiner/__init__.py
--rw-r--r--   0        0        0    11273 2024-05-12 18:16:12.352203 twiner-0.3.0/twiner/cli.py
--rw-r--r--   0        0        0     1422 2024-02-08 00:09:53.321000 twiner-0.3.0/twiner/config.py
--rw-r--r--   0        0        0      456 2024-02-10 16:00:12.105000 twiner-0.3.0/twiner/notify.py
--rw-r--r--   0        0        0     3301 2024-02-10 13:15:05.951000 twiner-0.3.0/twiner/twitch.py
--rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 twiner-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-31 20:23:18.857000 twiner-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5752 2024-02-22 19:32:17.391760 twiner-0.4.0/README.md
+-rw-r--r--   0        0        0     1013 2024-05-29 03:00:14.299737 twiner-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-02-22 20:08:23.511838 twiner-0.4.0/twiner/__init__.py
+-rw-r--r--   0        0        0     9521 2024-05-29 02:54:14.645165 twiner-0.4.0/twiner/cli.py
+-rw-r--r--   0        0        0     1563 2024-05-29 01:56:02.340583 twiner-0.4.0/twiner/config.py
+-rw-r--r--   0        0        0      506 2024-05-28 22:48:07.269984 twiner-0.4.0/twiner/notify.py
+-rw-r--r--   0        0        0     6592 2024-05-29 01:55:48.447366 twiner-0.4.0/twiner/twitch.py
+-rw-r--r--   0        0        0     6781 1970-01-01 00:00:00.000000 twiner-0.4.0/PKG-INFO
```

### Comparing `twiner-0.3.0/LICENSE` & `twiner-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twiner-0.3.0/README.md` & `twiner-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `twiner-0.3.0/pyproject.toml` & `twiner-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twiner"
-version = "0.3.0"
+version = "0.4.0"
 description = "CLI that helps you with notifications for your favorite streamers on Twitch.tv."
 authors = ["febits <febits@proton.me>"]
 readme = "README.md"
 classifiers = [
   "Environment :: Console",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `twiner-0.3.0/twiner/cli.py` & `twiner-0.4.0/twiner/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import time
-from datetime import datetime, timedelta
+from datetime import timedelta
 from typing import Optional
 
 import typer
 from rich.console import Console
 from rich.panel import Panel
 from typing_extensions import Annotated
 
@@ -12,16 +11,17 @@
 from twiner.notify import send_notify
 from twiner.twitch import Twitch
 
 app = typer.Typer(help="🎮 Twiner CLI (Twitch Notifier)")
 console = Console()
 
 
-def version(value: bool):
+def version_cb(value: bool):
     """Callback that shows the current version."""
+
     if value:
         console.print(__appname__, __version__)
         raise typer.Exit(0)
 
 
 @app.callback()
 def main(
@@ -29,29 +29,31 @@
         Optional[bool],
         typer.Option(
             "--version",
             "-v",
             "-V",
             help="Show the current version.",
             is_flag=True,
-            callback=version,
+            callback=version_cb,
         ),
     ] = False
-): ...
+):
+    """Configure a callback to print version number."""
 
 
 @app.command()
 def add(
     user: Annotated[str, typer.Argument(..., help="Username from Twitch.")],
     configfile: Annotated[
         Optional[str],
         typer.Option("--config", "-c", help="Specify a custom config path."),
     ] = TwinerConfig.DEFAULT_CONFIG_PATH,
 ):
     """Add a user to the notification pool."""
+
     try:
         config = TwinerConfig(configfile)
         config.read_from_config()
 
         twitch = Twitch(config)
 
         if twitch.is_api_working():
@@ -79,14 +81,15 @@
     user: Annotated[str, typer.Argument(..., help="Username from Twitch.")],
     configfile: Annotated[
         Optional[str],
         typer.Option("--config", "-c", help="Specify a custom config path."),
     ] = TwinerConfig.DEFAULT_CONFIG_PATH,
 ):
     """Remove a user from the notification pool."""
+
     try:
         config = TwinerConfig(configfile)
         config.read_from_config()
 
         try:
             del config.yaml["tonotify"][user]
             usericon = config.datadir / f"{user}.png"
@@ -117,14 +120,15 @@
     ],
     configfile: Annotated[
         Optional[str],
         typer.Option("--config", "-c", help="Specify a custom config path."),
     ] = TwinerConfig.DEFAULT_CONFIG_PATH,
 ):
     """Configure the Twitch Credentials."""
+
     try:
         config = TwinerConfig(configfile)
         config.read_from_config()
 
         twitch = Twitch(config)
         response = twitch.get_access_token(client_id, client_secret)
 
@@ -154,14 +158,15 @@
 def start(
     configfile: Annotated[
         Optional[str],
         typer.Option("--config", "-c", help="Specify a custom config path."),
     ] = TwinerConfig.DEFAULT_CONFIG_PATH
 ):
     """Start the notification loop."""
+
     try:
         config = TwinerConfig(configfile)
         config.read_from_config()
 
         twitch = Twitch(config)
 
         if twitch.is_api_working():
@@ -171,56 +176,16 @@
                     title="Users to Notify",
                     highlight=True,
                     border_style="grey42",
                     expand=False,
                 )
             )
 
-            counter = 1
-            while True:
-                console.print(
-                    f"< Loop {counter} : {datetime.now().strftime('%H:%M:%S')} >"
-                )
-                for user in twitch.users:
-                    if twitch.is_user_streaming(user.username):
-                        if user.previously_shown:
-                            continue
-                        else:
-                            user.is_streaming = True
-                            user.previously_shown = True
-
-                            stream_title = twitch.get_streams_info(
-                                user.username
-                            )["title"]
-                            user.stream_title = (
-                                stream_title
-                                if len(stream_title) < 50
-                                else stream_title[:50] + "..."
-                            )
-                            user.viewer_count = twitch.get_streams_info(
-                                user.username
-                            )["viewer_count"]
-
-                            console.print(
-                                f'\t[b]{user.username}[/]: "{user.stream_title}" - {user.viewer_count} viewers'
-                            )
-                            console.print(
-                                f"\t(ready to notify: [b][i]{user.username}[/])\n"
-                            )
-
-                            send_notify(user, config)
-                    else:
-                        if user.is_streaming:
-                            user.is_streaming = False
-                            user.previously_shown = False
-                            user.stream_title = ""
-                            user.viewer_count = 0
+            twitch.notification_loop(config, send_notify)
 
-                time.sleep(config.yaml["geral"]["loop_period"])
-                counter += 1
         else:
             console.print("❌ Invalid credentials")
             raise typer.Exit(1)
 
     except FileNotFoundError as exc:
         raise FileNotFoundError("Run 'twiner init' first.") from exc
 
@@ -330,14 +295,15 @@
     configfile: Annotated[
         Optional[str],
         typer.Option("--config", "-c", help="Specify a custom config path."),
     ] = TwinerConfig.DEFAULT_CONFIG_PATH
 ):
     """Init the config file (it will perform a redefining action through
     the config file, using it exclusively for the initial setup)."""
+
     config = TwinerConfig(configfile)
 
     if not config.path.exists():
         console.print(
             f"[b]✅ Config file was successfully created at {config.path}[/]"
         )
     else:
```

### Comparing `twiner-0.3.0/twiner/config.py` & `twiner-0.4.0/twiner/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from os import getenv
 from pathlib import Path
+from typing import Dict
 
 import yaml
 
 
 class TwinerConfig:
     """Define a way/wrapper for the application to manipulate the config
     aspects."""
 
     DEFAULT_CONFIG_PATH = f"{getenv('HOME')}/.config/twiner/twiner.yaml"
     DEFAULT_DATA_DIR = f"{getenv('HOME')}/.local/share/twiner"
 
-    def __init__(self, path):
+    def __init__(self, path: str | None):
         self.template = {
             "geral": {
                 "loop_period": 300,
                 "notification_timeout": 5,
                 "show_user_picture": True,
             },
             "creds": {
@@ -26,23 +27,27 @@
             },
             "tonotify": {},
         }
         self.yaml = {}
         self.path = Path(path)
         self.datadir = Path(self.DEFAULT_DATA_DIR)
 
-    def write_to_config(self, data):
+    def write_to_config(self, data: Dict[str, Dict]):
         """Write the given data to the config file."""
+
         if not self.path.exists():
             self.path.parent.mkdir(mode=0o744, exist_ok=True)
             self.path.touch(mode=0o644)
 
-        yaml.dump(data, self.path.open(mode="w"))
+        with self.path.open(mode="w", encoding="utf-8") as f:
+            yaml.dump(data, f)
 
     def read_from_config(self):
         """Read the config file."""
 
-        self.yaml = yaml.safe_load(self.path.open(mode="r"))
+        with self.path.open(mode="r", encoding="utf-8") as f:
+            self.yaml = yaml.safe_load(f)
 
     def create_datadir(self):
         """Create data dir where will be stored the usericons."""
+
         self.datadir.mkdir(mode=0o755, parents=True, exist_ok=True)
```

### Comparing `twiner-0.3.0/PKG-INFO` & `twiner-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twiner
-Version: 0.3.0
+Version: 0.4.0
 Summary: CLI that helps you with notifications for your favorite streamers on Twitch.tv.
 Author: febits
 Author-email: febits@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

