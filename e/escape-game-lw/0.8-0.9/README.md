# Comparing `tmp/escape_game_lw-0.8.tar.gz` & `tmp/escape_game_lw-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "escape_game_lw-0.8.tar", last modified: Fri Dec  8 14:44:35 2023, max compression
+gzip compressed data, was "escape_game_lw-0.9.tar", last modified: Wed May 29 18:07:44 2024, max compression
```

## Comparing `escape_game_lw-0.8.tar` & `escape_game_lw-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2023-12-08 14:44:35.384539 escape_game_lw-0.8/
--rw-r--r--   0 l00758   (696090729) 1931062070     1060 2023-12-07 23:18:10.000000 escape_game_lw-0.8/LICENSE.txt
--rw-r--r--   0 l00758   (696090729) 1931062070      754 2023-12-08 14:44:35.384647 escape_game_lw-0.8/PKG-INFO
--rw-r--r--   0 l00758   (696090729) 1931062070       82 2023-12-07 23:17:31.000000 escape_game_lw-0.8/README.md
-drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2023-12-08 14:44:35.378688 escape_game_lw-0.8/escape_game_lw/
--rw-r--r--   0 l00758   (696090729) 1931062070       52 2023-12-08 09:36:24.000000 escape_game_lw-0.8/escape_game_lw/__init__.py
--rw-r--r--   0 l00758   (696090729) 1931062070    26357 2023-12-08 14:39:25.000000 escape_game_lw-0.8/escape_game_lw/main.py
-drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2023-12-08 14:44:35.384195 escape_game_lw-0.8/escape_game_lw.egg-info/
--rw-r--r--   0 l00758   (696090729) 1931062070      754 2023-12-08 14:44:35.000000 escape_game_lw-0.8/escape_game_lw.egg-info/PKG-INFO
--rw-r--r--   0 l00758   (696090729) 1931062070      279 2023-12-08 14:44:35.000000 escape_game_lw-0.8/escape_game_lw.egg-info/SOURCES.txt
--rw-r--r--   0 l00758   (696090729) 1931062070        1 2023-12-08 14:44:35.000000 escape_game_lw-0.8/escape_game_lw.egg-info/dependency_links.txt
--rw-r--r--   0 l00758   (696090729) 1931062070        6 2023-12-08 14:44:35.000000 escape_game_lw-0.8/escape_game_lw.egg-info/requires.txt
--rw-r--r--   0 l00758   (696090729) 1931062070       15 2023-12-08 14:44:35.000000 escape_game_lw-0.8/escape_game_lw.egg-info/top_level.txt
--rw-r--r--   0 l00758   (696090729) 1931062070       79 2023-12-08 14:44:35.385333 escape_game_lw-0.8/setup.cfg
--rw-r--r--   0 l00758   (696090729) 1931062070     1598 2023-12-08 14:44:30.000000 escape_game_lw-0.8/setup.py
+drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2024-05-29 18:07:44.727842 escape_game_lw-0.9/
+-rw-r--r--   0 l00758   (696090729) 1931062070     1060 2023-12-07 23:18:10.000000 escape_game_lw-0.9/LICENSE.txt
+-rw-r--r--   0 l00758   (696090729) 1931062070      754 2024-05-29 18:07:44.727943 escape_game_lw-0.9/PKG-INFO
+-rw-r--r--   0 l00758   (696090729) 1931062070       82 2023-12-07 23:17:31.000000 escape_game_lw-0.9/README.md
+drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2024-05-29 18:07:44.712703 escape_game_lw-0.9/escape_game_lw/
+-rw-r--r--   0 l00758   (696090729) 1931062070       52 2023-12-08 09:36:24.000000 escape_game_lw-0.9/escape_game_lw/__init__.py
+-rw-r--r--   0 l00758   (696090729) 1931062070    26474 2024-05-29 13:30:56.000000 escape_game_lw-0.9/escape_game_lw/main.py
+drwxr-xr-x   0 l00758   (696090729) 1931062070        0 2024-05-29 18:07:44.726694 escape_game_lw-0.9/escape_game_lw.egg-info/
+-rw-r--r--   0 l00758   (696090729) 1931062070      754 2024-05-29 18:07:44.000000 escape_game_lw-0.9/escape_game_lw.egg-info/PKG-INFO
+-rw-r--r--   0 l00758   (696090729) 1931062070      279 2024-05-29 18:07:44.000000 escape_game_lw-0.9/escape_game_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 l00758   (696090729) 1931062070        1 2024-05-29 18:07:44.000000 escape_game_lw-0.9/escape_game_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 l00758   (696090729) 1931062070        6 2024-05-29 18:07:44.000000 escape_game_lw-0.9/escape_game_lw.egg-info/requires.txt
+-rw-r--r--   0 l00758   (696090729) 1931062070       15 2024-05-29 18:07:44.000000 escape_game_lw-0.9/escape_game_lw.egg-info/top_level.txt
+-rw-r--r--   0 l00758   (696090729) 1931062070       79 2024-05-29 18:07:44.731536 escape_game_lw-0.9/setup.cfg
+-rw-r--r--   0 l00758   (696090729) 1931062070     1598 2024-05-29 18:06:51.000000 escape_game_lw-0.9/setup.py
```

### Comparing `escape_game_lw-0.8/LICENSE.txt` & `escape_game_lw-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `escape_game_lw-0.8/PKG-INFO` & `escape_game_lw-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: escape_game_lw
-Version: 0.8
+Version: 0.9
 Summary: Basic functions for escape game
 Home-page: https://github.com/Tchluwies/escape_game_lw
-Download-URL: https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.8.tar.gz
+Download-URL: https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.9.tar.gz
 Author: Luise Wiesalla
 Author-email: LuiseWiesalla@gmx.de
 License: MIT
 Keywords: Escape,Game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `escape_game_lw-0.8/escape_game_lw/main.py` & `escape_game_lw-0.9/escape_game_lw/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-
 from datetime import datetime, timedelta, date
 import numpy as np
 import random
 import string
 import time
 
 
 class EscapeGamePinaPython:
     # Chapter 0
     # ---------------
-    def __init__(self):
+    def __init__(self, strict_mode=False):
         """ Init game with current time"""
-        self.completed = [0]
+        
+        if strict_mode:
+            self.completed = [0]
+        else:
+            self.completed = list(range(10))
         self.start_time = datetime.now()
         
         # chapter 8
         self.map = []
         self.level = 1
         # chapter 9
         self.__command_device = []
@@ -100,15 +103,15 @@
             pin_elevator (str): pin for elevator; info in pin_codes
             pin_3rd_floor_right (str): pin for right corridor on 3rd floor
             pin_office (str): pin for office room 3.09
         
         """
         
         if 1 not in self.completed:
-            print("Did you gather the information frist?")
+            print("Did you gather the information frist? (chapter 1) ")
             return False
         
         if pin_elevator == "003301":
 
             if pin_3rd_floor_right == "430091368":
 
                 if pin_office == "4300366359":
@@ -156,15 +159,15 @@
         if 3 not in self.completed:
             print("You need to be logged in first (chaper 3).")
             return False
 
         random.seed(42)
 
         today = date.today()
-        day =  today - timedelta(days=today.weekday() + 1) - timedelta(weeks=1)
+        day =  today - timedelta(days=(today.weekday() - 1 + 7) % 7)
 
         # day sollte ein datetime-Objekt sein, das den Tag repräsentiert, für den die Zeiten generiert werden sollen
         login_times = []
         logout_times = []
 
         online_code = {
             8 : [1,0,1,0,1,0], # each row is an hour, one element in list is 10min
@@ -607,7 +610,8 @@
             Thank you very much for your important part in the investigation!
 
             ...
 
             You solved the case. Congratulation! You finished in {duration_min} min.""")
         else:
             print("Try to solve the problems first")
+
```

### Comparing `escape_game_lw-0.8/escape_game_lw.egg-info/PKG-INFO` & `escape_game_lw-0.9/escape_game_lw.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: escape-game-lw
-Version: 0.8
+Version: 0.9
 Summary: Basic functions for escape game
 Home-page: https://github.com/Tchluwies/escape_game_lw
-Download-URL: https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.8.tar.gz
+Download-URL: https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.9.tar.gz
 Author: Luise Wiesalla
 Author-email: LuiseWiesalla@gmx.de
 License: MIT
 Keywords: Escape,Game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `escape_game_lw-0.8/setup.py` & `escape_game_lw-0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'escape_game_lw',         # How you named your package folder (MyLib)
   packages = ['escape_game_lw'],   # Chose the same as "name"
-  version = '0.8',      # Start with a small number and increase it with every change you make
+  version = '0.9',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Basic functions for escape game',   # Give a short description about your library
   author = 'Luise Wiesalla',                   # Type in your name
   author_email = 'LuiseWiesalla@gmx.de',      # Type in your E-Mail
   url = 'https://github.com/Tchluwies/escape_game_lw',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.8.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/Tchluwies/escape_game_lw/archive/refs/tags/0.9.tar.gz',    # I explain this later on
   keywords = ['Escape','Game'],   # Keywords that define your package best
   install_requires=[
       'numpy'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

