# Comparing `tmp/myfaasmctl-0.0.5.tar.gz` & `tmp/myfaasmctl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfaasmctl-0.0.5.tar", last modified: Sun May 26 12:15:33 2024, max compression
+gzip compressed data, was "myfaasmctl-0.0.6.tar", last modified: Wed May 29 01:38:13 2024, max compression
```

## Comparing `myfaasmctl-0.0.5.tar` & `myfaasmctl-0.0.6.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.401131 myfaasmctl-0.0.5/faasmctl/
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.401131 myfaasmctl-0.0.5/faasmctl/bin/
--rwxr-xr-x   0 root         (0) root         (0)     4533 2024-05-26 09:08:38.000000 myfaasmctl-0.0.5/faasmctl/bin/gen_proto_files.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.405130 myfaasmctl-0.0.5/faasmctl/tasks/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/cli.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/delete.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/deploy.py
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/flush.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/generate.py
--rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/invoke.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/logs.py
--rw-r--r--   0 root         (0) root         (0)    11843 2024-05-26 09:36:56.000000 myfaasmctl-0.0.5/faasmctl/tasks/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/restart.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/scale.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/status.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/faasmctl/util/
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/backend.py
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/batch.py
--rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/compose.py
--rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/config.py
--rw-r--r--   0 root         (0) root         (0)     5829 2024-05-21 14:28:54.000000 myfaasmctl-0.0.5/faasmctl/util/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/docker.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/env.py
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/faasm.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/flush.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/faasmctl/util/gen_proto/
--rw-r--r--   0 root         (0) root         (0)    12287 2024-05-26 09:01:33.000000 myfaasmctl-0.0.5/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5867 2024-05-26 09:01:33.000000 myfaasmctl-0.0.5/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.5/faasmctl/util/invoke.py
--rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/k8s.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/message.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/network.py
--rw-r--r--   0 root         (0) root         (0)     7290 2024-05-26 10:29:44.000000 myfaasmctl-0.0.5/faasmctl/util/planner.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/random.py
--rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/restart.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/results.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/time.py
--rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/upload.py
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-26 12:14:43.000000 myfaasmctl-0.0.5/faasmctl/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/myfaasmctl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      692 2024-05-26 12:14:33.000000 myfaasmctl-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.466716 myfaasmctl-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-29 01:38:13.466716 myfaasmctl-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.458716 myfaasmctl-0.0.6/faasmctl/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.458716 myfaasmctl-0.0.6/faasmctl/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     4533 2024-05-26 09:08:38.000000 myfaasmctl-0.0.6/faasmctl/bin/gen_proto_files.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.462716 myfaasmctl-0.0.6/faasmctl/tasks/
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-28 08:54:27.000000 myfaasmctl-0.0.6/faasmctl/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/cli.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/delete.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/flush.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/generate.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2024-05-28 00:37:57.000000 myfaasmctl-0.0.6/faasmctl/tasks/logs.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2024-05-26 09:36:56.000000 myfaasmctl-0.0.6/faasmctl/tasks/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/scale.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/status.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-29 01:04:52.000000 myfaasmctl-0.0.6/faasmctl/tasks/stream.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/tasks/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.462716 myfaasmctl-0.0.6/faasmctl/util/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/backend.py
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/batch.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/compose.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2024-05-21 14:28:54.000000 myfaasmctl-0.0.6/faasmctl/util/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/docker.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/env.py
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/faasm.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/flush.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.466716 myfaasmctl-0.0.6/faasmctl/util/gen_proto/
+-rw-r--r--   0 root         (0) root         (0)    12287 2024-05-28 09:31:55.000000 myfaasmctl-0.0.6/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2024-05-28 09:31:55.000000 myfaasmctl-0.0.6/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.6/faasmctl/util/invoke.py
+-rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/k8s.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/message.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/network.py
+-rw-r--r--   0 root         (0) root         (0)     9066 2024-05-29 01:05:40.000000 myfaasmctl-0.0.6/faasmctl/util/planner.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/random.py
+-rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/results.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/time.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.6/faasmctl/util/upload.py
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-29 01:34:34.000000 myfaasmctl-0.0.6/faasmctl/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 01:38:13.466716 myfaasmctl-0.0.6/myfaasmctl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-29 01:38:13.000000 myfaasmctl-0.0.6/myfaasmctl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      692 2024-05-29 01:34:28.000000 myfaasmctl-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-29 01:38:13.466716 myfaasmctl-0.0.6/setup.cfg
```

### Comparing `myfaasmctl-0.0.5/LICENSE.md` & `myfaasmctl-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/PKG-INFO` & `myfaasmctl-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.5/README.md` & `myfaasmctl-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/bin/gen_proto_files.py` & `myfaasmctl-0.0.6/faasmctl/bin/gen_proto_files.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/cli.py` & `myfaasmctl-0.0.6/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/delete.py` & `myfaasmctl-0.0.6/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/deploy.py` & `myfaasmctl-0.0.6/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/flush.py` & `myfaasmctl-0.0.6/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/invoke.py` & `myfaasmctl-0.0.6/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/logs.py` & `myfaasmctl-0.0.6/faasmctl/tasks/scale.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,47 @@
-from faasmctl.util.backend import COMPOSE_BACKEND, K8S_BACKEND
-from faasmctl.util.compose import run_compose_cmd
+from faasmctl.util.backend import COMPOSE_BACKEND
+from faasmctl.util.compose import (
+    get_container_ips_from_compose,
+    get_container_names_from_compose,
+    run_compose_cmd,
+)
 from faasmctl.util.config import (
     BACKEND_INI_STRING,
     get_faasm_ini_file,
     get_faasm_ini_value,
+    update_faasm_ini_value,
 )
-from faasmctl.util.k8s import run_k8s_cmd
 from invoke import task
 
 
-def get_compose_logs(s, follow, ini_file, last_restart):
-    compose_cmd = [
-        "logs",
-        "--since {}".format(last_restart),
-        "-f" if follow else "",
-        "{}".format(" ".join(s)),
-    ]
-    compose_cmd = " ".join(compose_cmd)
-    run_compose_cmd(ini_file, compose_cmd)
-
-
-def get_k8s_logs(s, follow, ini_file, last_restart):
-    if len(s) > 1:
-        raise RuntimeError(
-            "Getting the logs for a K8s service only works with one service at a time!"
-        )
-
-    service_to_k8s_str = {
-        "planner": "pod/planner",
-        "worker": "-l run=faasm-worker",
-        "upload": "pod/upload",
-    }
-
-    service = s[0]
-    if service not in service_to_k8s_str:
-        raise RuntimeError(
-            "Unrecognised service name: {} (must be one in: {})".format(
-                service, service_to_k8s_str.keys()
-            )
-        )
-
-    k8s_cmd = [
-        "logs",
-        "-f" if follow else "",
-        service_to_k8s_str[service],
-        "--tail=-1",
-    ]
-    k8s_cmd = " ".join(k8s_cmd)
-    k8s_config = get_faasm_ini_value(ini_file, "Faasm", "k8s_config")
-    run_k8s_cmd(k8s_config, "faasm", k8s_cmd)
-
-
-@task(default=True, iterable=["s"])
-def logs(ctx, s, follow=False, ini_file=None):
+@task(default=True)
+def scale(ctx, service, replicas, ini_file=None):
     """
-    Get the logs of a running service in the cluster
+    Scale a service to a number of replicas
 
     Parameters:
-    - s (str, repeateble): service to get the logs from
-    - ini_file (str): path to the cluster's INI file
+    - service (str): service to scale
+    - replicas (int): number of replicas to scale to
     """
     if not ini_file:
         ini_file = get_faasm_ini_file()
 
     backend = get_faasm_ini_value(ini_file, "Faasm", BACKEND_INI_STRING)
-    last_restart = get_faasm_ini_value(ini_file, "Faasm", "last_restart")
-    if backend == COMPOSE_BACKEND:
-        get_compose_logs(s, follow, ini_file, last_restart)
-    elif backend == K8S_BACKEND:
-        get_k8s_logs(s, follow, ini_file, last_restart)
-    else:
-        raise RuntimeError("Unrecognised backend: {}".format(backend))
+    if backend != COMPOSE_BACKEND:
+        raise RuntimeError(
+            "Can only get a CLI shell for a cluster that is "
+            "running on a '{}' backend".format(COMPOSE_BACKEND)
+        )
+
+    run_compose_cmd(ini_file, "scale {}={}".format(service, replicas))
+
+    # Update the worker names and ips in the INI file
+    faasm_checkout = get_faasm_ini_value(ini_file, "Faasm", "working_dir")
+    cluster_name = get_faasm_ini_value(ini_file, "Faasm", "cluster_name")
+    worker_names = "{}".format(
+        ",".join(get_container_names_from_compose(faasm_checkout, cluster_name))
+    )
+    worker_ips = "{}".format(
+        ",".join(get_container_ips_from_compose(faasm_checkout, cluster_name))
+    )
+    update_faasm_ini_value(ini_file, "Faasm", "worker_names", worker_names)
+    update_faasm_ini_value(ini_file, "Faasm", "worker_ips", worker_ips)
```

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/monitor.py` & `myfaasmctl-0.0.6/faasmctl/tasks/monitor.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/restart.py` & `myfaasmctl-0.0.6/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/status.py` & `myfaasmctl-0.0.6/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/tasks/upload.py` & `myfaasmctl-0.0.6/faasmctl/tasks/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/compose.py` & `myfaasmctl-0.0.6/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/config.py` & `myfaasmctl-0.0.6/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/deploy.py` & `myfaasmctl-0.0.6/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/docker.py` & `myfaasmctl-0.0.6/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/faasm.py` & `myfaasmctl-0.0.6/faasmctl/util/faasm.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/flush.py` & `myfaasmctl-0.0.6/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/gen_proto/faabric_pb2.py` & `myfaasmctl-0.0.6/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/gen_proto/planner_pb2.py` & `myfaasmctl-0.0.6/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\x91\x03\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\xa7\x02\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x19\n\x15\x46LUSH_AVAILABLE_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x1a\n\x16\x46LUSH_SCHEDULING_STATE\x10\x04\x12\x17\n\x13GET_AVAILABLE_HOSTS\x10\x05\x12\x0e\n\nGET_CONFIG\x10\x06\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x07\x12\x16\n\x12GET_IN_FLIGHT_APPS\x10\x08\x12\x11\n\rEXECUTE_BATCH\x10\n\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x0b\x12\x1f\n\x1bPRELOAD_SCHEDULING_DECISION\x10\x0c\x12\x18\n\x14GET_FUNCTION_METRICS\x10\r\"\xa3\x01\n\x17GetInFlightAppsResponse\x12\x42\n\x04\x61pps\x18\x01 \x03(\x0b\x32\x34.faabric.planner.GetInFlightAppsResponse.InFlightApp\x12\x15\n\rnumMigrations\x18\x02 \x01(\x05\x1a-\n\x0bInFlightApp\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07hostIps\x18\x02 \x03(\t\".\n\x15NumMigrationsResponse\x12\x15\n\rnumMigrations\x18\x01 \x01(\x05\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"d\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Host\"V\n\x1a\x43hainedFunctionsMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\"\xac\x01\n\x12\x46unctionMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\x12\x1a\n\x12\x61verageWaitingTime\x18\x04 \x01(\x05\x12\x0e\n\x06hostIp\x18\x05 \x01(\t\x12\x1a\n\x12lockCongestionTime\x18\x06 \x01(\x05\x12\x14\n\x0clockHoldTime\x18\x07 \x01(\x05\"\x9b\x01\n\x16\x46unctionMetricResponse\x12\x43\n\x0e\x63hainedMetrics\x18\x01 \x03(\x0b\x32+.faabric.planner.ChainedFunctionsMetricsRes\x12<\n\x0f\x66unctionMetrics\x18\x02 \x03(\x0b\x32#.faabric.planner.FunctionMetricsResb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\xc7\x03\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\xdd\x02\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x19\n\x15\x46LUSH_AVAILABLE_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x1a\n\x16\x46LUSH_SCHEDULING_STATE\x10\x04\x12\x17\n\x13GET_AVAILABLE_HOSTS\x10\x05\x12\x0e\n\nGET_CONFIG\x10\x06\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x07\x12\x16\n\x12GET_IN_FLIGHT_APPS\x10\x08\x12\x11\n\rEXECUTE_BATCH\x10\n\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x0b\x12\x1f\n\x1bPRELOAD_SCHEDULING_DECISION\x10\x0c\x12\x18\n\x14GET_FUNCTION_METRICS\x10\r\x12\x1e\n\x1aSCALE_FUNCTION_PARALLELISM\x10\x0e\x12\x14\n\x10RESET_BATCH_SIZE\x10\x0f\"\xa3\x01\n\x17GetInFlightAppsResponse\x12\x42\n\x04\x61pps\x18\x01 \x03(\x0b\x32\x34.faabric.planner.GetInFlightAppsResponse.InFlightApp\x12\x15\n\rnumMigrations\x18\x02 \x01(\x05\x1a-\n\x0bInFlightApp\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07hostIps\x18\x02 \x03(\t\".\n\x15NumMigrationsResponse\x12\x15\n\rnumMigrations\x18\x01 \x01(\x05\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"d\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Host\"V\n\x1a\x43hainedFunctionsMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\"\xac\x01\n\x12\x46unctionMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\x12\x1a\n\x12\x61verageWaitingTime\x18\x04 \x01(\x05\x12\x0e\n\x06hostIp\x18\x05 \x01(\t\x12\x1a\n\x12lockCongestionTime\x18\x06 \x01(\x05\x12\x14\n\x0clockHoldTime\x18\x07 \x01(\x05\"\x9b\x01\n\x16\x46unctionMetricResponse\x12\x43\n\x0e\x63hainedMetrics\x18\x01 \x03(\x0b\x32+.faabric.planner.ChainedFunctionsMetricsRes\x12<\n\x0f\x66unctionMetrics\x18\x02 \x03(\x0b\x32#.faabric.planner.FunctionMetricsRes\"K\n\x14\x46unctionScaleRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08\x66unction\x18\x02 \x01(\t\x12\x13\n\x0bparallelism\x18\x03 \x01(\x05\"&\n\x11\x42\x61tchResetRequest\x12\x11\n\tbatchsize\x18\x01 \x01(\x05\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.planner.planner_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EMPTYRESPONSE._serialized_start=46
@@ -27,39 +27,43 @@
   _RESPONSESTATUS._serialized_start=109
   _RESPONSESTATUS._serialized_end=210
   _RESPONSESTATUS_STATUS._serialized_start=183
   _RESPONSESTATUS_STATUS._serialized_end=210
   _TIMESTAMP._serialized_start=212
   _TIMESTAMP._serialized_end=240
   _HTTPMESSAGE._serialized_start=243
-  _HTTPMESSAGE._serialized_end=644
+  _HTTPMESSAGE._serialized_end=698
   _HTTPMESSAGE_TYPE._serialized_start=349
-  _HTTPMESSAGE_TYPE._serialized_end=644
-  _GETINFLIGHTAPPSRESPONSE._serialized_start=647
-  _GETINFLIGHTAPPSRESPONSE._serialized_end=810
-  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_start=765
-  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_end=810
-  _NUMMIGRATIONSRESPONSE._serialized_start=812
-  _NUMMIGRATIONSRESPONSE._serialized_end=858
-  _PLANNERCONFIG._serialized_start=860
-  _PLANNERCONFIG._serialized_end=938
-  _HOST._serialized_start=940
-  _HOST._serialized_end=1040
-  _PINGRESPONSE._serialized_start=1042
-  _PINGRESPONSE._serialized_end=1104
-  _REGISTERHOSTREQUEST._serialized_start=1106
-  _REGISTERHOSTREQUEST._serialized_end=1183
-  _REGISTERHOSTRESPONSE._serialized_start=1186
-  _REGISTERHOSTRESPONSE._serialized_end=1321
-  _REMOVEHOSTREQUEST._serialized_start=1323
-  _REMOVEHOSTREQUEST._serialized_end=1379
-  _REMOVEHOSTRESPONSE._serialized_start=1381
-  _REMOVEHOSTRESPONSE._serialized_end=1450
-  _AVAILABLEHOSTSRESPONSE._serialized_start=1452
-  _AVAILABLEHOSTSRESPONSE._serialized_end=1514
-  _CHAINEDFUNCTIONSMETRICSRES._serialized_start=1516
-  _CHAINEDFUNCTIONSMETRICSRES._serialized_end=1602
-  _FUNCTIONMETRICSRES._serialized_start=1605
-  _FUNCTIONMETRICSRES._serialized_end=1777
-  _FUNCTIONMETRICRESPONSE._serialized_start=1780
-  _FUNCTIONMETRICRESPONSE._serialized_end=1935
+  _HTTPMESSAGE_TYPE._serialized_end=698
+  _GETINFLIGHTAPPSRESPONSE._serialized_start=701
+  _GETINFLIGHTAPPSRESPONSE._serialized_end=864
+  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_start=819
+  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_end=864
+  _NUMMIGRATIONSRESPONSE._serialized_start=866
+  _NUMMIGRATIONSRESPONSE._serialized_end=912
+  _PLANNERCONFIG._serialized_start=914
+  _PLANNERCONFIG._serialized_end=992
+  _HOST._serialized_start=994
+  _HOST._serialized_end=1094
+  _PINGRESPONSE._serialized_start=1096
+  _PINGRESPONSE._serialized_end=1158
+  _REGISTERHOSTREQUEST._serialized_start=1160
+  _REGISTERHOSTREQUEST._serialized_end=1237
+  _REGISTERHOSTRESPONSE._serialized_start=1240
+  _REGISTERHOSTRESPONSE._serialized_end=1375
+  _REMOVEHOSTREQUEST._serialized_start=1377
+  _REMOVEHOSTREQUEST._serialized_end=1433
+  _REMOVEHOSTRESPONSE._serialized_start=1435
+  _REMOVEHOSTRESPONSE._serialized_end=1504
+  _AVAILABLEHOSTSRESPONSE._serialized_start=1506
+  _AVAILABLEHOSTSRESPONSE._serialized_end=1568
+  _CHAINEDFUNCTIONSMETRICSRES._serialized_start=1570
+  _CHAINEDFUNCTIONSMETRICSRES._serialized_end=1656
+  _FUNCTIONMETRICSRES._serialized_start=1659
+  _FUNCTIONMETRICSRES._serialized_end=1831
+  _FUNCTIONMETRICRESPONSE._serialized_start=1834
+  _FUNCTIONMETRICRESPONSE._serialized_end=1989
+  _FUNCTIONSCALEREQUEST._serialized_start=1991
+  _FUNCTIONSCALEREQUEST._serialized_end=2066
+  _BATCHRESETREQUEST._serialized_start=2068
+  _BATCHRESETREQUEST._serialized_end=2106
 # @@protoc_insertion_point(module_scope)
```

### Comparing `myfaasmctl-0.0.5/faasmctl/util/invoke.py` & `myfaasmctl-0.0.6/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/k8s.py` & `myfaasmctl-0.0.6/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/network.py` & `myfaasmctl-0.0.6/faasmctl/util/network.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/planner.py` & `myfaasmctl-0.0.6/faasmctl/util/planner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from faasmctl.util.config import get_faasm_ini_file, get_faasm_planner_host_port
 from faasmctl.util.gen_proto.planner_pb2 import (
     AvailableHostsResponse,
     GetInFlightAppsResponse,
     HttpMessage,
     #SetEvictedVmIpsRequest,
     FunctionMetricResponse,
+    FunctionScaleRequest,
+    BatchResetRequest,
 )
-from google.protobuf.json_format import MessageToJson, Parse
+from google.protobuf.json_format import MessageToJson, Parse, ParseDict
 from requests import post
 from time import sleep
 
 PLANNER_JSON_MESSAGE_FAILED = {"dead": "beef"}
 
 # ----------
 # Util
@@ -43,14 +45,18 @@
         http_message.type = HttpMessage.Type.PRELOAD_SCHEDULING_DECISION
     elif msg_type == "SET_NEXT_EVICTED_VM":
         http_message.type = HttpMessage.Type.SET_NEXT_EVICTED_VM
     elif msg_type == "SET_POLICY":
         http_message.type = HttpMessage.Type.SET_POLICY
     elif msg_type == "GET_FUNCTION_METRICS":
         http_message.type = HttpMessage.Type.GET_FUNCTION_METRICS
+    elif msg_type == "SCALE_FUNCTION_PARALLELISM":
+        http_message.type = HttpMessage.Type.SCALE_FUNCTION_PARALLELISM
+    elif msg_type == "RESET_BATCH_SIZE":
+        http_message.type = HttpMessage.Type.RESET_BATCH_SIZE
     else:
         raise RuntimeError("Unrecognised HTTP msg type: {}".format(msg_type))
 
     if msg_body:
         http_message.payloadJson = msg_body
 
     return MessageToJson(http_message, indent=None)
@@ -216,8 +222,47 @@
                 response.status_code, response.text
             )
         )
         raise RuntimeError("Error getting metrics")
 
     metrics = Parse(response.text, FunctionMetricResponse())
 
-    return metrics 
+    return metrics 
+
+def scale_function_parallelism(user, function, parallelism):
+    host, port = get_faasm_planner_host_port(get_faasm_ini_file())
+    url = "http://{}:{}".format(host, port)
+    req_dict = {"user": user, "function": function, "parallelism": parallelism}
+    req = ParseDict(req_dict, FunctionScaleRequest())
+
+    planner_msg = prepare_planner_msg("SCALE_FUNCTION_PARALLELISM", MessageToJson(req, indent=None))
+    response = post(url, data=planner_msg, timeout=None)
+
+    if response.status_code != 200:
+        print(
+            "Error setting parallelism (code: {}): {}".format(
+                response.status_code, response.text
+            )
+        )
+        raise RuntimeError("Error setting parallelism")
+    
+    print("Function {}-{} parallelism set to {}".format(user,function, parallelism))
+
+
+def reset_batch_size(batchsize):
+    host, port = get_faasm_planner_host_port(get_faasm_ini_file())
+    url = "http://{}:{}".format(host, port)
+    req_dict = {"batchsize": batchsize}
+    req = ParseDict(req_dict, BatchResetRequest())
+
+    planner_msg = prepare_planner_msg("RESET_BATCH_SIZE", MessageToJson(req, indent=None))
+    response = post(url, data=planner_msg, timeout=None)
+
+    if response.status_code != 200:
+        print(
+            "Error setting batchsize (code: {}): {}".format(
+                response.status_code, response.text
+            )
+        )
+        raise RuntimeError("Error setting batchsize")
+    
+    print("Batch size set to {}".format(batchsize))
```

### Comparing `myfaasmctl-0.0.5/faasmctl/util/restart.py` & `myfaasmctl-0.0.6/faasmctl/util/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/results.py` & `myfaasmctl-0.0.6/faasmctl/util/results.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/faasmctl/util/upload.py` & `myfaasmctl-0.0.6/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.5/myfaasmctl.egg-info/PKG-INFO` & `myfaasmctl-0.0.6/myfaasmctl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.5/myfaasmctl.egg-info/SOURCES.txt` & `myfaasmctl-0.0.6/myfaasmctl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 faasmctl/tasks/generate.py
 faasmctl/tasks/invoke.py
 faasmctl/tasks/logs.py
 faasmctl/tasks/monitor.py
 faasmctl/tasks/restart.py
 faasmctl/tasks/scale.py
 faasmctl/tasks/status.py
+faasmctl/tasks/stream.py
 faasmctl/tasks/upload.py
 faasmctl/util/backend.py
 faasmctl/util/batch.py
 faasmctl/util/compose.py
 faasmctl/util/config.py
 faasmctl/util/deploy.py
 faasmctl/util/docker.py
```

### Comparing `myfaasmctl-0.0.5/pyproject.toml` & `myfaasmctl-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myfaasmctl"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

