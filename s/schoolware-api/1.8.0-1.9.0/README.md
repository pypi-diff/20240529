# Comparing `tmp/schoolware_api-1.8.0.tar.gz` & `tmp/schoolware_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.8.0.tar", last modified: Fri Nov  3 13:55:57 2023, max compression
+gzip compressed data, was "schoolware_api-1.9.0.tar", last modified: Fri Dec  1 17:14:38 2023, max compression
```

## Comparing `schoolware_api-1.8.0.tar` & `schoolware_api-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:55:57.523993 schoolware_api-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-11-03 13:55:57.523993 schoolware_api-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2023-11-03 13:55:45.000000 schoolware_api-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-11-03 13:55:45.000000 schoolware_api-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:55:57.523993 schoolware_api-1.8.0/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-03 13:55:45.000000 schoolware_api-1.8.0/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2023-11-03 13:55:45.000000 schoolware_api-1.8.0/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:55:57.523993 schoolware_api-1.8.0/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-11-03 13:55:57.000000 schoolware_api-1.8.0/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-03 13:55:57.000000 schoolware_api-1.8.0/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 13:55:57.000000 schoolware_api-1.8.0/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-03 13:55:57.000000 schoolware_api-1.8.0/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-03 13:55:57.000000 schoolware_api-1.8.0/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 13:55:57.523993 schoolware_api-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-11-03 13:55:45.000000 schoolware_api-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 17:14:38.222791 schoolware_api-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-12-01 17:14:38.222791 schoolware_api-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-12-01 17:14:28.000000 schoolware_api-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-01 17:14:28.000000 schoolware_api-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 17:14:38.218791 schoolware_api-1.9.0/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-01 17:14:28.000000 schoolware_api-1.9.0/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2023-12-01 17:14:28.000000 schoolware_api-1.9.0/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 17:14:38.222791 schoolware_api-1.9.0/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-12-01 17:14:38.000000 schoolware_api-1.9.0/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-12-01 17:14:38.000000 schoolware_api-1.9.0/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 17:14:38.000000 schoolware_api-1.9.0/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-01 17:14:38.000000 schoolware_api-1.9.0/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-01 17:14:38.000000 schoolware_api-1.9.0/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 17:14:38.222791 schoolware_api-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-01 17:14:28.000000 schoolware_api-1.9.0/setup.py
```

### Comparing `schoolware_api-1.8.0/PKG-INFO` & `schoolware_api-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.8.0
+Version: 1.9.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
-License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -31,20 +30,20 @@
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | schoolware_login | set true if using schoolware login
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a some more info
-| debug | show a some more info
+| verbose | show some more info
+| debug | show even more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
-* `playwright install &&  playwright install-deps`
+* `playwright install &&  playwright install-deps` only for microsoft login 
 
 ## optional
 * `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
```

### Comparing `schoolware_api-1.8.0/README.md` & `schoolware_api-1.9.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | schoolware_login | set true if using schoolware login
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a some more info
-| debug | show a some more info
+| verbose | show some more info
+| debug | show even more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
-* `playwright install &&  playwright install-deps`
+* `playwright install &&  playwright install-deps` only for microsoft login 
 
 ## optional
 * `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
```

### Comparing `schoolware_api-1.8.0/pyproject.toml` & `schoolware_api-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.8.0"
+version = "1.9.0"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.8.0/schoolware_api/schoolware_api.py` & `schoolware_api-1.9.0/schoolware_api/schoolware_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,29 +42,33 @@
             logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.WARNING)
 
         if("schoolware_login" in config):
             self.schoolware_login = config["schoolware_login"]
         else:
             self.schoolware_login = False
 
+        if("telegram_msg" in config):
+            self.telegram_msg = config["telegram_msg"]
+        else:
+            self.telegram_msg = ""
         self.domain = self.config["domain"]
         self.user = self.config["user"]
         self.password = self.config["password"]
         
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
         self.verbose_print(message="starting schoolware_api",level=1)        
 
         if("bot_token" in config):
             self.num_points = len(self.punten())
             self.scores_prev = self.scores
-            self.telegram_bg = threading.Thread(target=self.telegram_def, args=(0,))
+            self.telegram_bg = threading.Thread(target=self.telegram_setup, args=(0,))
             self.telegram_bg.start()
         
 #Token&cookie stuff
     def get_new_token(self):
         ##########VERBOSE##########
         self.verbose_print("get_token")
         ##########VERBOSE##########
@@ -334,62 +338,54 @@
                     today_filterd.append(agenda)
         ##########VERBOSE##########
         self.verbose_end("filter-agenda")
         ##########VERBOSE##########
 
         return today_filterd
     
-    def telegram_manual_send(self, msg):
-        """Manualy send a telegram message
-
-        Args:
-            msg (String): Message to send
-        """
-        import asyncio
-        asyncio.run(self.telegram_send_msg(msg))
-
     ##########OTHER##########
 
     #telegram bot
-    def telegram_def(self, none):
+    def telegram_setup(self, none):
         """The setup function for Telegram
         """
-        
+        import telegram
         from time import sleep
-        self.num_prev = len(self.punten())
-        self.scores_prev = self.scores
+        self.bot = telegram.Bot(self.config["bot_token"])
+        self.prev_scores = self.scores
         while True:
             sleep(5*60)
             try:
                 if(self.verbose):
                     self.verbose_print(message=f"telegram checking")
+                
                 self.telegram_point_diff()
             except:
                 logging.warning(f"error in telegram loop")
 
+    def telegram_point_diff(self):
+            import asyncio
 
+            new_scores = self.punten()
 
-    def telegram_point_diff(self):
 
-            import asyncio
-            import telegram
-            scores_now = self.punten()
-            num_now = len(scores_now)
-            if(self.num_prev < num_now):
+            if(len(self.prev_scores) < len(new_scores)):
                 
-                    diff_list = [i for i in scores_now if i not in self.scores_prev]
+                    diff_list = [i for i in new_scores if i not in self.prev_scores]
                     diff = len(diff_list)
-                    self.num_prev = num_now
-                    self.scores_prev = scores_now
+                    self.prev_scores = new_scores
                     
-                    msg = f"{diff} New points for:\n"
-                    for item in diff_list:
-                        msg = msg + f"{item['vak']}\n"
+                    if(self.telegram_msg == ""):
+                        msg = f"{diff} New points:\n"
+                        for item in diff_list:
+                            msg = msg + f"{item['vak']} {item['titel']}: {float(item['score']) * float(item['tot_sc']) if item['score'] != 'n/a' else 'n/a'}/{item['tot_sc']}\n"
+                    else:
+                        eval(self.telegram_msg)
+
                     self.verbose_print(message=f"telegram send msg msg={msg}", level=1)
-                    self.bot = telegram.Bot(self.config["bot_token"])
                     asyncio.run(self.telegram_send_msg(msg))
 
 
     async def telegram_send_msg(self, msg):
         """Function to send a telegram message to a set message-id
 
         Args:
```

### Comparing `schoolware_api-1.8.0/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.9.0/schoolware_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.8.0
+Version: 1.9.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
-License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -31,20 +30,20 @@
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
 | schoolware_login | set true if using schoolware login
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a some more info
-| debug | show a some more info
+| verbose | show some more info
+| debug | show even more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
-* `playwright install &&  playwright install-deps`
+* `playwright install &&  playwright install-deps` only for microsoft login 
 
 ## optional
 * `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
```

