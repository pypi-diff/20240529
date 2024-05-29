# Comparing `tmp/dyatel-wrapper-2.2.1.tar.gz` & `tmp/dyatel_wrapper-2.2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyatel-wrapper-2.2.1.tar", last modified: Tue Apr 16 16:26:26 2024, max compression
+gzip compressed data, was "dyatel_wrapper-2.2.11.tar", last modified: Wed May 29 20:22:35 2024, max compression
```

## Comparing `dyatel-wrapper-2.2.1.tar` & `dyatel_wrapper-2.2.11.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.911593 dyatel-wrapper-2.2.1/
--rw-r--r--   0 pvladimir   (502) staff       (20)    11347 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.1/LICENSE
--rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-04-16 16:26:26.911398 dyatel-wrapper-2.2.1/PKG-INFO
--rw-r--r--   0 pvladimir   (502) staff       (20)      179 2023-01-16 08:38:34.000000 dyatel-wrapper-2.2.1/README.md
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.875964 dyatel-wrapper-2.2.1/dyatel/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.879585 dyatel-wrapper-2.2.1/dyatel/abstraction/
--rw-r--r--   0 pvladimir   (502) staff       (20)    12242 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/driver_wrapper_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    17159 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/element_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1427 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/mixin_abc.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2637 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/abstraction/page_abc.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.884708 dyatel-wrapper-2.2.1/dyatel/base/
--rw-r--r--   0 pvladimir   (502) staff       (20)     8635 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/base/driver_wrapper.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    20667 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/base/element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2304 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/base/group.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     7062 2023-11-25 17:52:02.000000 dyatel-wrapper-2.2.1/dyatel/base/page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.887090 dyatel-wrapper-2.2.1/dyatel/dyatel_play/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.888049 dyatel-wrapper-2.2.1/dyatel/dyatel_play/helpers/
--rw-r--r--   0 pvladimir   (502) staff       (20)      283 2024-03-01 20:10:58.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/helpers/Trace.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     8790 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    13858 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.889021 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.891926 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/
--rw-r--r--   0 pvladimir   (502) staff       (20)     7975 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    18716 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_page.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.893293 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/
--rw-r--r--   0 pvladimir   (502) staff       (20)     9868 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/mobile_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2300 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/web_driver.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.894643 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/
--rw-r--r--   0 pvladimir   (502) staff       (20)     5340 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/mobile_element.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2903 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/web_element.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.896536 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1361 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/mobile_page.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      116 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/web_page.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      497 2023-04-12 09:28:58.000000 dyatel-wrapper-2.2.1/dyatel/dyatel_sel/sel_utils.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1638 2023-10-17 08:41:12.000000 dyatel-wrapper-2.2.1/dyatel/exceptions.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     6007 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/js_scripts.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1963 2023-09-07 07:44:45.000000 dyatel-wrapper-2.2.1/dyatel/keyboard_keys.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.898892 dyatel-wrapper-2.2.1/dyatel/mixins/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1769 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.1/dyatel/mixins/driver_mixin.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2701 2023-11-25 17:03:56.000000 dyatel-wrapper-2.2.1/dyatel/mixins/internal_mixin.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.902731 dyatel-wrapper-2.2.1/dyatel/mixins/objects/
--rw-r--r--   0 pvladimir   (502) staff       (20)      261 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/box.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      167 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/location.py
--rw-r--r--   0 pvladimir   (502) staff       (20)      172 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/mixins/objects/size.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2999 2024-03-03 23:28:21.000000 dyatel-wrapper-2.2.1/dyatel/shared_utils.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.906805 dyatel-wrapper-2.2.1/dyatel/utils/
--rw-r--r--   0 pvladimir   (502) staff       (20)     8272 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/utils/internal_utils.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     2845 2023-11-25 17:03:52.000000 dyatel-wrapper-2.2.1/dyatel/utils/logs.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     1515 2023-11-26 12:42:22.000000 dyatel-wrapper-2.2.1/dyatel/utils/previous_object_driver.py
--rw-r--r--   0 pvladimir   (502) staff       (20)     4066 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/utils/selector_synchronizer.py
--rw-r--r--   0 pvladimir   (502) staff       (20)    17109 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/dyatel/visual_comparison.py
-drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-04-16 16:26:26.910687 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/
--rw-r--r--   0 pvladimir   (502) staff       (20)     1451 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 pvladimir   (502) staff       (20)     1382 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)        1 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)      136 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/requires.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)        7 2024-04-16 16:26:26.000000 dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/top_level.txt
--rw-r--r--   0 pvladimir   (502) staff       (20)       79 2024-04-16 16:26:26.912246 dyatel-wrapper-2.2.1/setup.cfg
--rw-r--r--   0 pvladimir   (502) staff       (20)     2334 2024-04-16 16:24:57.000000 dyatel-wrapper-2.2.1/setup.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.616078 dyatel_wrapper-2.2.11/
+-rw-r--r--   0 pvladimir   (502) staff       (20)    11347 2023-04-12 09:28:58.000000 dyatel_wrapper-2.2.11/LICENSE
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1452 2024-05-29 20:22:35.615857 dyatel_wrapper-2.2.11/PKG-INFO
+-rw-r--r--   0 pvladimir   (502) staff       (20)      179 2023-01-16 08:38:34.000000 dyatel_wrapper-2.2.11/README.md
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.576823 dyatel_wrapper-2.2.11/dyatel/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.582318 dyatel_wrapper-2.2.11/dyatel/abstraction/
+-rw-r--r--   0 pvladimir   (502) staff       (20)    12242 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/abstraction/driver_wrapper_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    17159 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/abstraction/element_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1427 2023-11-25 17:03:52.000000 dyatel_wrapper-2.2.11/dyatel/abstraction/mixin_abc.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2637 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/abstraction/page_abc.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.586658 dyatel_wrapper-2.2.11/dyatel/base/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8635 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/base/driver_wrapper.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    20667 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/base/element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2304 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/base/group.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     7062 2023-11-25 17:52:02.000000 dyatel_wrapper-2.2.11/dyatel/base/page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.589601 dyatel_wrapper-2.2.11/dyatel/dyatel_play/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.590499 dyatel_wrapper-2.2.11/dyatel/dyatel_play/helpers/
+-rw-r--r--   0 pvladimir   (502) staff       (20)      283 2024-03-01 20:10:58.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_play/helpers/Trace.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8790 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_play/play_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    13842 2024-05-29 20:22:16.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_play/play_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_play/play_page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.591833 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.596545 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     7975 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/core_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    18716 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/core_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)       52 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/core_page.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.598347 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/driver/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     9868 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/driver/mobile_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2300 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/driver/web_driver.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.600145 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/elements/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     5340 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/elements/mobile_element.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2903 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/elements/web_element.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.601890 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/pages/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1361 2023-11-25 17:03:52.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/pages/mobile_page.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      116 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/pages/web_page.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      497 2023-04-12 09:28:58.000000 dyatel_wrapper-2.2.11/dyatel/dyatel_sel/sel_utils.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1638 2023-10-17 08:41:12.000000 dyatel_wrapper-2.2.11/dyatel/exceptions.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     6007 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/js_scripts.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1963 2023-09-07 07:44:45.000000 dyatel_wrapper-2.2.11/dyatel/keyboard_keys.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.604125 dyatel_wrapper-2.2.11/dyatel/mixins/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1769 2023-11-25 17:03:56.000000 dyatel_wrapper-2.2.11/dyatel/mixins/driver_mixin.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2701 2023-11-25 17:03:56.000000 dyatel_wrapper-2.2.11/dyatel/mixins/internal_mixin.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.607946 dyatel_wrapper-2.2.11/dyatel/mixins/objects/
+-rw-r--r--   0 pvladimir   (502) staff       (20)      261 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/mixins/objects/box.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      167 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/mixins/objects/location.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)      172 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/mixins/objects/size.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2999 2024-03-03 23:28:21.000000 dyatel_wrapper-2.2.11/dyatel/shared_utils.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.611414 dyatel_wrapper-2.2.11/dyatel/utils/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     8272 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/utils/internal_utils.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2845 2023-11-25 17:03:52.000000 dyatel_wrapper-2.2.11/dyatel/utils/logs.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1515 2023-11-26 12:42:22.000000 dyatel_wrapper-2.2.11/dyatel/utils/previous_object_driver.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)     4066 2024-04-16 16:24:57.000000 dyatel_wrapper-2.2.11/dyatel/utils/selector_synchronizer.py
+-rw-r--r--   0 pvladimir   (502) staff       (20)    17109 2024-05-29 20:13:30.000000 dyatel_wrapper-2.2.11/dyatel/visual_comparison.py
+drwxr-xr-x   0 pvladimir   (502) staff       (20)        0 2024-05-29 20:22:35.614951 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1452 2024-05-29 20:22:35.000000 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 pvladimir   (502) staff       (20)     1382 2024-05-29 20:22:35.000000 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)        1 2024-05-29 20:22:35.000000 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)      136 2024-05-29 20:22:35.000000 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/requires.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)        7 2024-05-29 20:22:35.000000 dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 pvladimir   (502) staff       (20)       79 2024-05-29 20:22:35.616896 dyatel_wrapper-2.2.11/setup.cfg
+-rw-r--r--   0 pvladimir   (502) staff       (20)     2335 2024-05-29 20:22:16.000000 dyatel_wrapper-2.2.11/setup.py
```

### Comparing `dyatel-wrapper-2.2.1/LICENSE` & `dyatel_wrapper-2.2.11/LICENSE`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/PKG-INFO` & `dyatel_wrapper-2.2.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyatel-wrapper
-Version: 2.2.1
+Version: 2.2.11
 Summary: Wrapper of Selenium, Appium and Playwright with single API
 Home-page: https://github.com/EnvInc/dyatel
 Author: Podolian Vladimir
 Author-email: vladimir.podolyan64@gmail.com
 Project-URL: Source, https://github.com/EnvInc/dyatel
 Project-URL: Tracker, https://github.com/EnvInc/dyatel/issues
 Project-URL: Changelog, https://github.com/EnvInc/dyatel/blob/master/CHANGELOG.md
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Appium-Python-Client>=2.1.2
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: opencv-python==4.5.5.62
 Requires-Dist: Pillow>=6.2.2
-Requires-Dist: playwright>=1.30.0
+Requires-Dist: playwright>=1.41.0
 Requires-Dist: selenium>=4.1.0
 Requires-Dist: scikit-image>=0.17.1
 
 # Dyatel 
 
 Dyatel is a wrapper tool of Selenium/Appium/Playwright libraries to test 
 web applications in a single project with possibility to easy switching between these engines.
```

### Comparing `dyatel-wrapper-2.2.1/dyatel/abstraction/driver_wrapper_abc.py` & `dyatel_wrapper-2.2.11/dyatel/abstraction/driver_wrapper_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/abstraction/element_abc.py` & `dyatel_wrapper-2.2.11/dyatel/abstraction/element_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/abstraction/mixin_abc.py` & `dyatel_wrapper-2.2.11/dyatel/abstraction/mixin_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/abstraction/page_abc.py` & `dyatel_wrapper-2.2.11/dyatel/abstraction/page_abc.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/base/driver_wrapper.py` & `dyatel_wrapper-2.2.11/dyatel/base/driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/base/element.py` & `dyatel_wrapper-2.2.11/dyatel/base/element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/base/group.py` & `dyatel_wrapper-2.2.11/dyatel/base/group.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/base/page.py` & `dyatel_wrapper-2.2.11/dyatel/base/page.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_driver.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_play/play_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_play/play_element.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_play/play_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import time
 from abc import ABC
 from typing import Union, List, Any
 
 from PIL.Image import Image
-from playwright._impl._api_types import TimeoutError as PlayTimeoutError  # noqa
+from playwright.sync_api import TimeoutError as PlayTimeoutError
 from playwright.sync_api import Page as PlaywrightPage
 from playwright.sync_api import Locator, Page, Browser, BrowserContext
 
 from dyatel.mixins.objects.size import Size
 from dyatel.mixins.objects.location import Location
 from dyatel.utils.selector_synchronizer import get_platform_locator, get_playwright_locator
 from dyatel.abstraction.element_abc import ElementABC
```

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_driver.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/core_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/core/core_element.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/core/core_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/mobile_driver.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/driver/mobile_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/driver/web_driver.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/driver/web_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/mobile_element.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/elements/mobile_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/elements/web_element.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/elements/web_element.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/dyatel_sel/pages/mobile_page.py` & `dyatel_wrapper-2.2.11/dyatel/dyatel_sel/pages/mobile_page.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/exceptions.py` & `dyatel_wrapper-2.2.11/dyatel/exceptions.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/js_scripts.py` & `dyatel_wrapper-2.2.11/dyatel/js_scripts.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/keyboard_keys.py` & `dyatel_wrapper-2.2.11/dyatel/keyboard_keys.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/mixins/driver_mixin.py` & `dyatel_wrapper-2.2.11/dyatel/mixins/driver_mixin.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/mixins/internal_mixin.py` & `dyatel_wrapper-2.2.11/dyatel/mixins/internal_mixin.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/shared_utils.py` & `dyatel_wrapper-2.2.11/dyatel/shared_utils.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/utils/internal_utils.py` & `dyatel_wrapper-2.2.11/dyatel/utils/internal_utils.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/utils/logs.py` & `dyatel_wrapper-2.2.11/dyatel/utils/logs.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/utils/previous_object_driver.py` & `dyatel_wrapper-2.2.11/dyatel/utils/previous_object_driver.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/utils/selector_synchronizer.py` & `dyatel_wrapper-2.2.11/dyatel/utils/selector_synchronizer.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel/visual_comparison.py` & `dyatel_wrapper-2.2.11/dyatel/visual_comparison.py`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/PKG-INFO` & `dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyatel-wrapper
-Version: 2.2.1
+Version: 2.2.11
 Summary: Wrapper of Selenium, Appium and Playwright with single API
 Home-page: https://github.com/EnvInc/dyatel
 Author: Podolian Vladimir
 Author-email: vladimir.podolyan64@gmail.com
 Project-URL: Source, https://github.com/EnvInc/dyatel
 Project-URL: Tracker, https://github.com/EnvInc/dyatel/issues
 Project-URL: Changelog, https://github.com/EnvInc/dyatel/blob/master/CHANGELOG.md
@@ -19,15 +19,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Appium-Python-Client>=2.1.2
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: opencv-python==4.5.5.62
 Requires-Dist: Pillow>=6.2.2
-Requires-Dist: playwright>=1.30.0
+Requires-Dist: playwright>=1.41.0
 Requires-Dist: selenium>=4.1.0
 Requires-Dist: scikit-image>=0.17.1
 
 # Dyatel 
 
 Dyatel is a wrapper tool of Selenium/Appium/Playwright libraries to test 
 web applications in a single project with possibility to easy switching between these engines.
```

### Comparing `dyatel-wrapper-2.2.1/dyatel_wrapper.egg-info/SOURCES.txt` & `dyatel_wrapper-2.2.11/dyatel_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyatel-wrapper-2.2.1/setup.py` & `dyatel_wrapper-2.2.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 
 
 cleanup()
 
 
 setup(
     name=pypi_name,
-    version='2.2.1',
+    version='2.2.11',
     url=f'https://github.com/EnvInc/{project_name}',
     packages=get_packages(project_name),
     install_requires=[
         'Appium-Python-Client>=2.1.2',
         'numpy>=1.18.1',
         'opencv-python==4.5.5.62',
         'Pillow>=6.2.2',
-        'playwright>=1.30.0',
+        'playwright>=1.41.0',
         'selenium>=4.1.0',
         'scikit-image>=0.17.1',
     ],
     keywords='selenium appium playwright web_automation mobile_automation',
     description='Wrapper of Selenium, Appium and Playwright with single API',
     long_description=description,
     long_description_content_type='text/markdown',
```

