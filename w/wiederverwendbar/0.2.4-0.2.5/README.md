# Comparing `tmp/wiederverwendbar-0.2.4.tar.gz` & `tmp/wiederverwendbar-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.4.tar", last modified: Tue May 28 08:35:28 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.5.tar", last modified: Wed May 29 07:32:27 2024, max compression
```

## Comparing `wiederverwendbar-0.2.4.tar` & `wiederverwendbar-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       19 2024-05-28 08:33:57.242628 wiederverwendbar-0.2.4/README.md
--rw-r--r--   0        0        0      682 2024-05-28 08:35:28.439628 wiederverwendbar-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-28 08:33:57.242628 wiederverwendbar-0.2.4/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0      407 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0      186 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0     2169 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/__init__.py
--rw-r--r--   0        0        0     2145 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/file_config.py
--rw-r--r--   0        0        0      762 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/indexable_model.py
--rw-r--r--   0        0        0     6632 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      890 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/logger.py
--rw-r--r--   0        0        0      734 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/singletons.py
--rw-r--r--   0        0        0      466 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/test.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/README.md
+-rw-r--r--   0        0        0      682 2024-05-29 07:32:27.267164 wiederverwendbar-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0      186 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0     2375 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/indexable_model.py
+-rw-r--r--   0        0        0     7477 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/logger.py
+-rw-r--r--   0        0        0      920 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/singletons.py
+-rw-r--r--   0        0        0      466 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/test.py
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.5/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.4/pyproject.toml` & `wiederverwendbar-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 dependencies = [
     "pydantic>=2.7.1",
     "pydantic-settings>=2.2.1",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
-version = "0.2.4"
+version = "0.2.5"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
```

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_singleton.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_singleton.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,36 +16,40 @@
         if ignored_loggers_equal is None:
             ignored_loggers_equal = []
         if ignored_loggers_like is None:
             ignored_loggers_like = []
 
         super().__init__(name, settings)
 
+        self.ignored_loggers_equal = ignored_loggers_equal
+        self.ignored_loggers_like = ignored_loggers_like
+
         if use_sub_logger:
             logging.setLoggerClass(SubLogger)
 
-        self.ignored_loggers_equal = ignored_loggers_equal
-        self.ignored_loggers_like = ignored_loggers_like
+            for logger in logging.Logger.manager.loggerDict.values():
+                if not isinstance(logger, logging.Logger):
+                    continue
+                _configure_logger(logger)
+
+
+def _configure_logger(cls: logging.Logger):
+    logger_singleton = LoggerSingleton()
+    if cls.name in logger_singleton.ignored_loggers_equal or any([ignored in cls.name for ignored in logger_singleton.ignored_loggers_like]):
+        return
+    cls.setLevel(logger_singleton.level)
+    cls.parent = logger_singleton
 
 
 class SubLogger(logging.Logger):
     def __init__(self, name: str, level=logging.NOTSET):
         self.init = False
-        logger_singleton = LoggerSingleton()
-
-        if name in logger_singleton.ignored_loggers_equal:
-            super().__init__(name, level)
-        elif any([ignored in name for ignored in logger_singleton.ignored_loggers_like]):
-            super().__init__(name, level)
-        else:
-            super().__init__(name, level)
-
-            self.parent = logger_singleton
-
-            self.init = True
+        super().__init__(name, level)
+        _configure_logger(self)
+        self.init = True
 
     def __setattr__(self, key, value):
         if key == "init":
             return super().__setattr__(key, value)
         if not self.init:
             return super().__setattr__(key, value)
```

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/file_config.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/file_config.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/indexable_model.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/indexable_model.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.4/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.5/src/wiederverwendbar/singleton.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import atexit
+import logging
 from abc import ABCMeta
 from typing import Any
 
 from pydantic import BaseModel
 from pydantic._internal._model_construction import ModelMetaclass
 
 from wiederverwendbar.functions.find_class_method import find_class_method
 
+logger = logging.getLogger(__name__)
+
 
 class Singleton(ModelMetaclass):
     """
     Singleton metaclass
     """
 
     singleton_map: dict[str, Any] = {}
     singleton_order: dict[str, int] = {}
+    delete_all_on_exit = True
+    delete_ordered_on_exit = True
 
     def __new__(cls, name, bases, attrs, order: int | None = None):
         # get __init__ method
         __init__ = attrs.pop("__init__", None)
         if __init__ is None:
             __init__ = find_class_method(bases, "__init__")
 
@@ -28,14 +34,15 @@
                 _order = Singleton.get_next_order()
             self_name = self.__class__.__name__
             if _order in Singleton.singleton_order.values():
                 raise RuntimeError(f"Singleton order {_order} already initialized. Use {self_name}() to get the instance.")
             if self_name not in Singleton.singleton_map:
                 Singleton.singleton_map[self_name] = self
                 Singleton.singleton_order[self_name] = _order
+                logger.debug(f"Singleton '{self_name}' with order {_order} initialized.")
                 if __init__ is not None:
                     __init__(self, *args, **kwargs)
             else:
                 raise RuntimeError(f"Singleton {self_name} already initialized. Use {self_name}() to get the instance.")
 
         attrs["__singleton__"] = True
 
@@ -84,17 +91,19 @@
         Return all singletons in map
 
         :param ordered: Return ordered map
         :return: Singleton map
         """
 
         if ordered:
-            return {k: v for k, v in sorted(cls.singleton_map.items(), key=lambda item: cls.singleton_order[item[0]])}
+            singleton_map = {k: v for k, v in sorted(cls.singleton_map.items(), key=lambda item: cls.singleton_order[item[0]])}
+        else:
+            singleton_map = cls.singleton_map
 
-        return cls.singleton_map
+        return singleton_map
 
     @classmethod
     def get_by_name(cls, name: str) -> Any:
         """
         Get singleton by name
 
         :param name: Name of singleton
@@ -157,19 +166,25 @@
 
         if len(cls.singleton_order) == 0:
             return 1
         else:
             return max(cls.singleton_order.values()) + 1
 
     @classmethod
-    def delete_all(cls, ordered: bool = True):
+    def delete_all(cls, ordered: bool | None = None):
         """
         Delete all singletons in map
         """
 
+        # if ordered is None, delete by class attribute
+        if ordered is None:
+            ordered = cls.delete_ordered_on_exit
+
+        print(ordered)
+
         singleton_names = list(cls.get_all(ordered=ordered).keys())
         singleton_names.reverse()
         for name in singleton_names:
             cls.delete_by_name(name)
 
     @classmethod
     def delete_by_name(cls, name: str):
@@ -178,34 +193,51 @@
 
         :param name: Name of singleton
         """
 
         current = cls.get_all().get(name, None)
         if current is None:
             raise RuntimeError(f"Singleton {name} not found.")
+        logger.debug(f"Singleton '{name}' deleted.")
         del cls.singleton_map[name]
 
     @classmethod
     def delete_by_type(cls, t: type | str):
         """
         Delete singleton by type
 
         :param t: Type of singleton
         """
 
         current = cls.get_by_type(t)
         if current is None:
             raise RuntimeError(f"Singleton {t} not found.")
+        logger.debug(f"Singleton '{current.__class__.__name__}' deleted.")
         del cls.singleton_map[current.__class__.__name__]
 
     @classmethod
     def delete_by_order(cls, order: int):
         """
         Delete singleton by order
 
         :param order: Order of singleton
         """
 
         current = cls.get_by_order(order)
         if current is None:
             raise RuntimeError(f"Singleton order {order} not found.")
+        logger.debug(f"Singleton '{current.__class__.__name__}' deleted.")
         del cls.singleton_map[current.__class__.__name__]
+
+
+def _on_exit():
+    """
+    On exit hook
+    """
+
+    logger.debug("Running on exit hook.")
+
+    if Singleton.delete_all_on_exit:
+        Singleton.delete_all()
+
+
+atexit.register(_on_exit)
```

### Comparing `wiederverwendbar-0.2.4/tests/logger.py` & `wiederverwendbar-0.2.5/tests/logger.py`

 * *Files identical despite different names*

