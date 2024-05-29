# Comparing `tmp/wiederverwendbar-0.2.3.tar.gz` & `tmp/wiederverwendbar-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.3.tar", last modified: Thu May 23 16:13:49 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.4.tar", last modified: Tue May 28 08:35:28 2024, max compression
```

## Comparing `wiederverwendbar-0.2.3.tar` & `wiederverwendbar-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       19 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/README.md
--rw-r--r--   0        0        0      682 2024-05-23 16:13:49.928846 wiederverwendbar-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0      407 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0      186 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0     2169 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0        0 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/models/__init__.py
--rw-r--r--   0        0        0     2145 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/models/file_config.py
--rw-r--r--   0        0        0      762 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/models/indexable_model.py
--rw-r--r--   0        0        0     6632 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      890 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/tests/logger.py
--rw-r--r--   0        0        0      734 2024-05-23 16:13:04.552276 wiederverwendbar-0.2.3/tests/singletons.py
--rw-r--r--   0        0        0      462 2024-05-23 16:13:04.556276 wiederverwendbar-0.2.3/tests/test.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-28 08:33:57.242628 wiederverwendbar-0.2.4/README.md
+-rw-r--r--   0        0        0      682 2024-05-28 08:35:28.439628 wiederverwendbar-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-28 08:33:57.242628 wiederverwendbar-0.2.4/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0      186 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0     2169 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/indexable_model.py
+-rw-r--r--   0        0        0     6632 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/logger.py
+-rw-r--r--   0        0        0      734 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/singletons.py
+-rw-r--r--   0        0        0      466 2024-05-28 08:33:57.246628 wiederverwendbar-0.2.4/tests/test.py
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.4/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.3/pyproject.toml` & `wiederverwendbar-0.2.4/pyproject.toml`

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
-version = "0.2.3"
+version = "0.2.4"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
```

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/logger/logger_singleton.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/logger/logger_singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/models/file_config.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/file_config.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/models/indexable_model.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/pydantic/indexable_model.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.4/src/wiederverwendbar/singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/tests/logger.py` & `wiederverwendbar-0.2.4/tests/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.3/tests/singletons.py` & `wiederverwendbar-0.2.4/tests/singletons.py`

 * *Files identical despite different names*

