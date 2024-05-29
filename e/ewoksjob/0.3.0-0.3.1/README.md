# Comparing `tmp/ewoksjob-0.3.0.tar.gz` & `tmp/ewoksjob-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksjob-0.3.0.tar", last modified: Tue Jan 30 13:22:19 2024, max compression
+gzip compressed data, was "ewoksjob-0.3.1.tar", last modified: Wed May 29 20:15:37 2024, max compression
```

## Comparing `ewoksjob-0.3.0.tar` & `ewoksjob-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2627 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1694 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/apps/
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1621 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/apps/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2795 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/apps/ewoks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/client/celery/
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/celery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/celery/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/client/celery/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/dummy_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/client/local/
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/local/pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/local/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/client/local/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5172 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-30 13:22:12.000000 ewoksjob-0.3.0/src/ewoksjob/events/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/events/handlers/
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1904 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/handlers/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/events/readers/
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5423 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/readers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/readers/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/events/readers/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-30 13:22:12.000000 ewoksjob-0.3.0/src/ewoksjob/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_cancel.py
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_convert.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_convert_and_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_events.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_execute_and_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     1800 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_feedback.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_future.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_futures.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/test_task_discovery.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob/worker/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/worker/executor.py
--rw-rw-rw-   0 root         (0) root         (0)     5824 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/worker/options.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/worker/process.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2024-01-30 09:46:09.000000 ewoksjob-0.3.0/src/ewoksjob/worker/process_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2734 2024-01-30 10:30:59.000000 ewoksjob-0.3.0/src/ewoksjob/worker/slurm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:22:19.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2627 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1710 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-30 13:22:18.000000 ewoksjob-0.3.0/src/ewoksjob.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.184004 ewoksjob-0.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-05-29 20:15:37.184004 ewoksjob-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2024-05-29 20:15:37.184004 ewoksjob-0.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.172004 ewoksjob-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.172004 ewoksjob-0.3.1/src/ewoksjob/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-29 20:10:32.000000 ewoksjob-0.3.1/src/ewoksjob/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/apps/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/apps/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2795 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/apps/ewoks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/client/celery/
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/celery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/celery/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/celery/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/dummy_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/client/local/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4410 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/local/pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/local/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/client/local/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/events/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:15:31.000000 ewoksjob-0.3.1/src/ewoksjob/events/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/events/handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/handlers/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/events/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/readers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/readers/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/events/readers/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 20:15:31.000000 ewoksjob-0.3.1/src/ewoksjob/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_cancel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_convert_and_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_events.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_execute_and_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_future.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_futures.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/test_task_discovery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob/worker/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/process_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2024-05-29 20:03:18.000000 ewoksjob-0.3.1/src/ewoksjob/worker/slurm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:15:37.176004 ewoksjob-0.3.1/src/ewoksjob.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-29 20:15:37.000000 ewoksjob-0.3.1/src/ewoksjob.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ewoksjob-0.3.0/LICENSE.md` & `ewoksjob-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/PKG-INFO` & `ewoksjob-0.3.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: ewoksjob
-Version: 0.3.0
-Summary: Asynchronous and distributed scheduling of Ewoks workflows from python
-Home-page: https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
-Author: ESRF
-Author-email: wout.de_nolf@esrf.fr
-License: MIT
-Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/
-Project-URL: Documentation, https://ewoksjob.readthedocs.io/
-Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoks/ewoksjob/issues/
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: worker
-Provides-Extra: redis
-Provides-Extra: sql
-Provides-Extra: monitor
-Provides-Extra: slurm
-Provides-Extra: beacon
-Provides-Extra: blissworker
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE.md
-
 # ewoksjob
 
 Utilities for job scheduling of [ewoks](https://ewoks.readthedocs.io/) workflows.
 
 Ewoksjob provides an ewoks interface for asynchronous and distributed scheduling of [ewoks](https://ewoks.readthedocs.io/) from python.
 
 Note that *ewoksjob* distributes the execution of workflows while [ewoksdask](https://ewoks.readthedocs.io/)
```

### Comparing `ewoksjob-0.3.0/setup.cfg` & `ewoksjob-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/__main__.py` & `ewoksjob-0.3.1/src/ewoksjob/__main__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/apps/errors.py` & `ewoksjob-0.3.1/src/ewoksjob/apps/errors.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/apps/ewoks.py` & `ewoksjob-0.3.1/src/ewoksjob/apps/ewoks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/celery/tasks.py` & `ewoksjob-0.3.1/src/ewoksjob/client/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/celery/utils.py` & `ewoksjob-0.3.1/src/ewoksjob/client/celery/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 def get_not_finished_futures() -> List[AsyncResult]:
     lst = [get_future(task_id) for task_id in get_not_finished_task_ids()]
     return [future for future in lst if future is not None]
 
 
 def get_workers() -> List[str]:
-    queues_dict: Optional[
-        Dict[str, List[dict]]
-    ] = current_app.control.inspect().active_queues()
+    queues_dict: Optional[Dict[str, List[dict]]] = (
+        current_app.control.inspect().active_queues()
+    )
     if queues_dict is None:
         return list()
 
     workers: Set[str] = set()
     for queue_infos in queues_dict.values():
         for queue_info in queue_infos:
             workers.add(queue_info["name"])
```

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/dummy_workflow.py` & `ewoksjob-0.3.1/src/ewoksjob/client/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/local/pool.py` & `ewoksjob-0.3.1/src/ewoksjob/client/local/pool.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/local/tasks.py` & `ewoksjob-0.3.1/src/ewoksjob/client/local/tasks.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/client/local/utils.py` & `ewoksjob-0.3.1/src/ewoksjob/client/local/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/config.py` & `ewoksjob-0.3.1/src/ewoksjob/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 def get_cfg_type(cfg_uri: str) -> str:
     presult = _parse_url(cfg_uri)
     if presult.scheme == "beacon":
         return "yaml"
     if presult.scheme in ("file", ""):
         cfg_uri = _url_to_filename(presult)
         ext = os.path.splitext(cfg_uri)[-1]
-        if ext in (".yaml", "yml"):
+        if ext in (".yaml", ".yml"):
             return "yaml"
         return "python"
     return ""
 
 
 def read_configuration(cfg_uri: str) -> dict:
     """Different types of URI's are supported:
```

### Comparing `ewoksjob-0.3.0/src/ewoksjob/events/handlers/redis.py` & `ewoksjob-0.3.1/src/ewoksjob/events/handlers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/events/readers/__init__.py` & `ewoksjob-0.3.1/src/ewoksjob/events/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/events/readers/base.py` & `ewoksjob-0.3.1/src/ewoksjob/events/readers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,17 @@
         if Variable is None:
             raise ImportError("requires 'ewoks'")
         input_uris = event.get("input_uris")
         if input_uris:
             if isinstance(input_uris, str):
                 input_uris = json.loads(input_uris)
             inputs = {
-                uri["name"]: Variable(data_uri=uri["value"])
-                if uri["value"]
-                else Variable()
+                uri["name"]: (
+                    Variable(data_uri=uri["value"]) if uri["value"] else Variable()
+                )
                 for uri in input_uris
             }
             event["inputs"] = VariableContainer(inputs)
         task_uri = event.get("task_uri")
         if task_uri:
             event["outputs"] = VariableContainer(data_uri=task_uri)
```

### Comparing `ewoksjob-0.3.0/src/ewoksjob/events/readers/redis.py` & `ewoksjob-0.3.1/src/ewoksjob/events/readers/redis.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/events/readers/sqlite3.py` & `ewoksjob-0.3.1/src/ewoksjob/events/readers/sqlite3.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/conftest.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_cancel.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_cancel.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_config.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_convert.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_convert_and_execute.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_convert_and_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_events.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_execute.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_execute_and_upload.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_execute_and_upload.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_feedback.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_future.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_futures.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/test_task_discovery.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/test_task_discovery.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/tests/utils.py` & `ewoksjob-0.3.1/src/ewoksjob/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/worker/options.py` & `ewoksjob-0.3.1/src/ewoksjob/worker/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 from .slurm import TaskPool as SlurmTaskPool
 from .process import TaskPool as ProcessTaskPool
 
 ALL_MP_CONTEXTS = list(get_all_start_methods())
 DEFAULT_MP_CONTEXT = get_context()._name
 
-concurrency.ALIASES[
-    "process"
-] = f"{ProcessTaskPool.__module__}:{ProcessTaskPool.__name__}"
+concurrency.ALIASES["process"] = (
+    f"{ProcessTaskPool.__module__}:{ProcessTaskPool.__name__}"
+)
 concurrency.ALIASES["slurm"] = f"{SlurmTaskPool.__module__}:{SlurmTaskPool.__name__}"
 worker.WORKERS_POOL.choices = list(worker.WORKERS_POOL.choices) + ["process", "slurm"]
 
 
 def add_options(app: Celery) -> None:
     _add_slurm_pool_options(app)
     _add_process_pool_options(app)
```

### Comparing `ewoksjob-0.3.0/src/ewoksjob/worker/process.py` & `ewoksjob-0.3.1/src/ewoksjob/worker/process.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob/worker/slurm.py` & `ewoksjob-0.3.1/src/ewoksjob/worker/slurm.py`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob.egg-info/SOURCES.txt` & `ewoksjob-0.3.1/src/ewoksjob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewoksjob-0.3.0/src/ewoksjob.egg-info/requires.txt` & `ewoksjob-0.3.1/src/ewoksjob.egg-info/requires.txt`

 * *Files identical despite different names*

