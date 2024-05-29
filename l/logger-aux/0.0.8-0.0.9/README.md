# Comparing `tmp/logger_aux-0.0.8.tar.gz` & `tmp/logger_aux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_aux-0.0.8.tar", last modified: Mon May 20 11:41:42 2024, max compression
+gzip compressed data, was "logger_aux-0.0.9.tar", last modified: Mon May 20 14:41:40 2024, max compression
```

## Comparing `logger_aux-0.0.8.tar` & `logger_aux-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.853786 logger_aux-0.0.8/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    25194 2024-05-20 11:41:42.853105 logger_aux-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    24394 2024-05-20 11:40:57.000000 logger_aux-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.843429 logger_aux-0.0.8/logger_aux/
--rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.8/logger_aux/__init__.py
--rw-rw-rw-   0        0        0     6675 2024-05-20 11:40:57.000000 logger_aux-0.0.8/logger_aux/main.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:41:42.850626 logger_aux-0.0.8/logger_aux.egg-info/
--rw-rw-rw-   0        0        0    25194 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 11:41:42.000000 logger_aux-0.0.8/logger_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 11:41:42.855341 logger_aux-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:41:40.573696 logger_aux-0.0.9/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 logger_aux-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    25194 2024-05-20 14:41:40.573696 logger_aux-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    24394 2024-05-20 14:40:56.000000 logger_aux-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 14:41:40.564308 logger_aux-0.0.9/logger_aux/
+-rw-rw-rw-   0        0        0       21 2024-01-15 06:52:12.000000 logger_aux-0.0.9/logger_aux/__init__.py
+-rw-rw-rw-   0        0        0     6895 2024-05-20 14:40:53.000000 logger_aux-0.0.9/logger_aux/main.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:41:40.572696 logger_aux-0.0.9/logger_aux.egg-info/
+-rw-rw-rw-   0        0        0    25194 2024-05-20 14:41:40.000000 logger_aux-0.0.9/logger_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-20 14:41:40.000000 logger_aux-0.0.9/logger_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:41:40.000000 logger_aux-0.0.9/logger_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-20 14:41:40.000000 logger_aux-0.0.9/logger_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:41:40.575696 logger_aux-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-04-26 07:47:41.000000 logger_aux-0.0.9/setup.py
```

### Comparing `logger_aux-0.0.8/LICENSE` & `logger_aux-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_aux-0.0.8/PKG-INFO` & `logger_aux-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_aux
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple logging
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/logger_aux
 Keywords: logger
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# logger_aux (v0.0.8)
+# logger_aux (v0.0.9)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.8/README.md` & `logger_aux-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# logger_aux (v0.0.8)
+# logger_aux (v0.0.9)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.8/logger_aux/main.py` & `logger_aux-0.0.9/logger_aux/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 class Logger:
     """
     NOTES:
         DONT use directly root as secondary logger - use it only as first or it would be applyed automatically!
     """
 
     # SETTINGS ---------------------------------------
-    LOG_NAME: None | str = None     # None=self "root"="root", if not StrNone=get ClassName!
+    LOG_NAME: None | str = None  # None=self "root"="root", if not StrNone=get ClassName!
 
     LOG_LEVEL: int = logging.DEBUG
     LOG_PATTERN: str = '%(asctime)s[%(levelname)s]%(name)s(%(filename)s).%(funcName)s(line%(lineno)d)/thread%(thread)s::%(msg)s'
 
     LOG_DIRPATH: None | pathlib.Path = None
 
     LOG_FILE_STARTWITH: None | str = None
@@ -52,14 +52,17 @@
     LOG_USE_STREAM: bool = True
     LOG_USE_FILE: bool = False
 
     # AUX ---------------------------------------
     _formatter: logging.Formatter
     LOGGER: Self = None
 
+    _handler_stream: logging.StreamHandler | None = None
+    _handler_file: logging.FileHandler | None = None
+
     @property
     def LOG_FILENAME(self) -> str:
         return f"{self.LOG_FILE_STARTWITH or 'logger'}__{self.LOG_NAME or 'root'}.{self.LOG_FILE_EXTENTION or 'log'}"
 
     @property
     def LOG_FILEPATH(self) -> pathlib.Path:
         if self.LOG_DIRPATH is None:
@@ -105,14 +108,15 @@
         if self.LOG_NAME is None:
             class_name = self.__class__.__name__
             if class_name == "Logger":
                 self.LOG_NAME = "root"
             else:
                 self.LOG_NAME = class_name
         elif not isinstance(self.LOG_NAME, str):
+            # if set name by passing object
             self.LOG_NAME = self.LOG_NAME.__class__.__name__
 
         # if not self.__class__.LOGGER:
         #     # place here MRO name??? for classmethods???
         #     # useful for methods starts after inited first instance
         #     self.__class__.LOGGER = logging.getLogger(self.LOG_NAME)
 
@@ -121,31 +125,31 @@
         # DISABLE ------------------------------------------
         if self.LOG_NAME == "root" and log_enable:
             pass
 
         elif not self.LOG_ENABLE:
             return
 
+        if self.LOGGER.handlers:  # already created logger from previous inition
+            return
+
         # --------------------------------------------------
         # TODO: create not exists LOG_DIRPATH
 
         # INIT ---------------------------------------------
         self.LOGGER.setLevel(self.LOG_LEVEL)
 
         self._formatter = logging.Formatter(self.LOG_PATTERN)
 
-        self._handler_stream = None
-        self._handler_file = None
-
         # CONNECT -------------------------------------------
         if self.LOG_USE_STREAM:
-            self._handler_stream = logging.StreamHandler()
-            # self._handler_stream.setLevel(self.LOG_LEVEL)
-            self._handler_stream.setFormatter(self._formatter)
-            self.LOGGER.addHandler(self._handler_stream)
+            self.__class__._handler_stream = logging.StreamHandler()
+            # self.__class__._handler_stream.setLevel(self.LOG_LEVEL)
+            self.__class__._handler_stream.setFormatter(self._formatter)
+            self.LOGGER.addHandler(self.__class__._handler_stream)
 
         if self.LOG_USE_FILE:
             self._handler_file = RotatingFileHandler(self.LOG_FILEPATH, maxBytes=self.LOG_FILE_MAXBYTES, backupCount=self.LOG_FILE_BACKUPCOUNT)
             # self._handler_file.setLevel(self.LOG_LEVEL)
             self._handler_file.setFormatter(self._formatter)
             self.LOGGER.addHandler(self._handler_file)
 
@@ -168,15 +172,15 @@
         DONT USE IT DIRECTLY!!!
         it would used always automated!!!
         """
         if not log_enable:
             return
         logger_root = logging.getLogger()
         if not logger_root.hasHandlers():
-            Logger(log_enable=log_enable)        # DONT USE cls()!!!
+            Logger(log_enable=log_enable)  # DONT USE cls()!!!
 
 
 # =====================================================================================================================
 if __name__ == "__main__":
     pass
```

### Comparing `logger_aux-0.0.8/logger_aux.egg-info/PKG-INFO` & `logger_aux-0.0.9/logger_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_aux
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple logging
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/logger_aux
 Keywords: logger
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# logger_aux (v0.0.8)
+# logger_aux (v0.0.9)
 
 ## DESCRIPTION_SHORT
 simple logging
 
 ## DESCRIPTION_LONG
 designed for DRY simple/easy usage logging
```

### Comparing `logger_aux-0.0.8/setup.py` & `logger_aux-0.0.9/setup.py`

 * *Files identical despite different names*

