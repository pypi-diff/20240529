# Comparing `tmp/t_bug_catcher-0.5.0.tar.gz` & `tmp/t_bug_catcher-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-9z9fd929/t_bug_catcher-0.5.0.tar", last modified: Thu May 16 08:16:28 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-ng8slq_7/t_bug_catcher-0.5.1.tar", last modified: Wed May 29 10:33:50 2024, max compression
```

## Comparing `t_bug_catcher-0.5.0.tar` & `t_bug_catcher-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    54360 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5219 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     4524 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/validation.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-16 08:16:28.000000 t_bug_catcher-0.5.0/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 08:16:28.991963 t_bug_catcher-0.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-05-16 08:16:01.000000 t_bug_catcher-0.5.0/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.790150 t_bug_catcher-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 10:33:50.790150 t_bug_catcher-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-29 10:33:50.790150 t_bug_catcher-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.786150 t_bug_catcher-0.5.1/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    54360 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.786150 t_bug_catcher-0.5.1/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.786150 t_bug_catcher-0.5.1/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.790150 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-05-29 10:33:50.000000 t_bug_catcher-0.5.1/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:33:50.790150 t_bug_catcher-0.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-05-29 10:33:23.000000 t_bug_catcher-0.5.1/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.5.0/PKG-INFO` & `t_bug_catcher-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.5.0/README.rst` & `t_bug_catcher-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/setup.py` & `t_bug_catcher-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.5.0",
+    version="0.5.1",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.5.1/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.5.1/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/config.py` & `t_bug_catcher-0.5.1/t_bug_catcher/config.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/jira.py` & `t_bug_catcher-0.5.1/t_bug_catcher/jira.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.5.1/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.5.1/t_bug_catcher/stack_saver.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/utils/common.py` & `t_bug_catcher-0.5.1/t_bug_catcher/utils/common.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.5.1/t_bug_catcher/utils/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Logger."""
+import logging
+
 try:
     from libraries import logger
-except ImportError:
-    import logging
 
+    if not isinstance(logger, logging.Logger):
+        raise TypeError("Logger is not an instance of logging.Logger.")
+except (ImportError, TypeError):
     log_format = logging.Formatter(
         r"%(asctime)s - %(levelname)-7s %(threadName)-12s [%(filename)s:%(lineno)s - %(funcName)s()] - %(message)s"
     )
     log_level = logging.DEBUG
 
     logger = logging.getLogger("t_bug_catcher")
     if logger.hasHandlers():
```

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher/validation.py` & `t_bug_catcher-0.5.1/t_bug_catcher/validation.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.5.1/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.5.0
+Version: 0.5.1
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.5.0/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.5.1/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.5.0/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.5.1/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

