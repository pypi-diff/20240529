# Comparing `tmp/wiederverwendbar-0.2.5.tar.gz` & `tmp/wiederverwendbar-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiederverwendbar-0.2.5.tar", last modified: Wed May 29 07:32:27 2024, max compression
+gzip compressed data, was "wiederverwendbar-0.2.6.tar", last modified: Wed May 29 08:20:08 2024, max compression
```

## Comparing `wiederverwendbar-0.2.5.tar` & `wiederverwendbar-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0       19 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/README.md
--rw-r--r--   0        0        0      682 2024-05-29 07:32:27.267164 wiederverwendbar-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      155 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/functions/__init__.py
--rw-r--r--   0        0        0      407 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/functions/find_class_method.py
--rw-r--r--   0        0        0      186 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/__init__.py
--rw-r--r--   0        0        0      600 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/rich_console_handler.py
--rw-r--r--   0        0        0      624 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/stream_console_handler.py
--rw-r--r--   0        0        0     2378 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
--rw-r--r--   0        0        0     3036 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger.py
--rw-r--r--   0        0        0     5665 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_settings.py
--rw-r--r--   0        0        0     2375 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_singleton.py
--rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/__init__.py
--rw-r--r--   0        0        0     2145 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/file_config.py
--rw-r--r--   0        0        0      762 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/indexable_model.py
--rw-r--r--   0        0        0     7477 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/src/wiederverwendbar/singleton.py
--rw-r--r--   0        0        0        0 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0      890 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/logger.py
--rw-r--r--   0        0        0      920 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/singletons.py
--rw-r--r--   0        0        0      466 2024-05-29 07:31:19.931136 wiederverwendbar-0.2.5/tests/test.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/README.md
+-rw-r--r--   0        0        0      718 2024-05-29 08:20:08.059440 wiederverwendbar-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/__init__.py
+-rw-r--r--   0        0        0     1113 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/admin.py
+-rw-r--r--   0        0        0     1734 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_file.py
+-rw-r--r--   0        0        0     3174 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/eval_value.py
+-rw-r--r--   0        0        0      407 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/find_class_method.py
+-rw-r--r--   0        0        0     1162 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/functions/wait_ping.py
+-rw-r--r--   0        0        0      186 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/rich_console_handler.py
+-rw-r--r--   0        0        0      624 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/stream_console_handler.py
+-rw-r--r--   0        0        0     2378 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py
+-rw-r--r--   0        0        0     3036 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger.py
+-rw-r--r--   0        0        0     5665 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_settings.py
+-rw-r--r--   0        0        0     2375 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/__init__.py
+-rw-r--r--   0        0        0     2145 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/file_config.py
+-rw-r--r--   0        0        0      762 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/indexable_model.py
+-rw-r--r--   0        0        0     7477 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/src/wiederverwendbar/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/logger.py
+-rw-r--r--   0        0        0      920 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/singletons.py
+-rw-r--r--   0        0        0      466 2024-05-29 08:19:29.363451 wiederverwendbar-0.2.6/tests/test.py
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 wiederverwendbar-0.2.6/PKG-INFO
```

### Comparing `wiederverwendbar-0.2.5/pyproject.toml` & `wiederverwendbar-0.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 ]
 dependencies = [
     "pydantic>=2.7.1",
     "pydantic-settings>=2.2.1",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.optional-dependencies]
 rich = [
     "rich>=13.7.1",
 ]
 typer = [
     "typer>=0.12.3",
 ]
+ping = [
+    "pythonping>=1.1.4",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/rich_console_handler.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/rich_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/stream_console_handler.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/stream_console_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/handlers/tar_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_settings.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_settings.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/logger/logger_singleton.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/logger/logger_singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/file_config.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/file_config.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/pydantic/indexable_model.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/pydantic/indexable_model.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/src/wiederverwendbar/singleton.py` & `wiederverwendbar-0.2.6/src/wiederverwendbar/singleton.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/tests/logger.py` & `wiederverwendbar-0.2.6/tests/logger.py`

 * *Files identical despite different names*

### Comparing `wiederverwendbar-0.2.5/tests/singletons.py` & `wiederverwendbar-0.2.6/tests/singletons.py`

 * *Files identical despite different names*

