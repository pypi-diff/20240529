# Comparing `tmp/dp-launching-app-0.0.7.tar.gz` & `tmp/dp-launching-app-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-launching-app-0.0.7.tar", last modified: Thu May 23 08:05:00 2024, max compression
+gzip compressed data, was "dp-launching-app-0.0.8.tar", last modified: Wed May 29 08:19:19 2024, max compression
```

## Comparing `dp-launching-app-0.0.7.tar` & `dp-launching-app-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.521910 dp-launching-app-0.0.7/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/MANIFEST.in
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-23 08:05:00.521730 dp-launching-app-0.0.7/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/README.md
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.512064 dp-launching-app-0.0.7/dp/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.512652 dp-launching-app-0.0.7/dp/launching/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.513067 dp-launching-app-0.0.7/dp/launching/cli/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    12658 2024-05-23 08:02:43.000000 dp-launching-app-0.0.7/dp/launching/cli/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.513976 dp-launching-app-0.0.7/dp/launching/cli/api/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/model.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/persistent_service.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514431 dp-launching-app-0.0.7/dp/launching/cli/commands/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/launching.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.509291 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514700 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/basic.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514964 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.515350 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/dflow.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.515803 dp-launching-app-0.0.7/dp/launching/cli/utils/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/utils/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/utils/random.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.516048 dp-launching-app-0.0.7/dp/launching/report/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/report/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.519213 dp-launching-app-0.0.7/dp/launching/typing/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.520120 dp-launching-app-0.0.7/dp/launching/typing/addon/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/sysmbol.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/ui.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.7/dp/launching/typing/basic.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/benchmark.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/bio.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    10526 2024-05-20 09:36:59.000000 dp-launching-app-0.0.7/dp/launching/typing/bohrium.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      944 2024-05-20 10:13:32.000000 dp-launching-app-0.0.7/dp/launching/typing/dataset.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/dflow.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/io.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.521475 dp-launching-app-0.0.7/dp_launching_app.egg-info/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1123 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/SOURCES.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/dependency_links.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/entry_points.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/requires.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/top_level.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-23 08:05:00.521952 dp-launching-app-0.0.7/setup.cfg
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-23 08:04:09.000000 dp-launching-app-0.0.7/setup.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.857271 dp-launching-app-0.0.8/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/MANIFEST.in
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-29 08:19:19.857111 dp-launching-app-0.0.8/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/README.md
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.848115 dp-launching-app-0.0.8/dp/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.848580 dp-launching-app-0.0.8/dp/launching/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.848904 dp-launching-app-0.0.8/dp/launching/cli/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    12658 2024-05-23 08:02:43.000000 dp-launching-app-0.0.8/dp/launching/cli/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.850060 dp-launching-app-0.0.8/dp/launching/cli/api/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/api/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/api/model.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/api/persistent_service.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.850534 dp-launching-app-0.0.8/dp/launching/cli/commands/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/commands/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/commands/launching.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.846393 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.850764 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/basic/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/basic/basic.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.850987 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/bohrium/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.851224 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/dflow/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/dflow/dflow.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.851757 dp-launching-app-0.0.8/dp/launching/cli/utils/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/utils/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/cli/utils/random.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.852074 dp-launching-app-0.0.8/dp/launching/report/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/report/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.854599 dp-launching-app-0.0.8/dp/launching/typing/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.855486 dp-launching-app-0.0.8/dp/launching/typing/addon/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/addon/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/addon/sysmbol.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/addon/ui.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.8/dp/launching/typing/basic.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1431 2024-05-29 07:48:26.000000 dp-launching-app-0.0.8/dp/launching/typing/benchmark.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/bio.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    10526 2024-05-20 09:36:59.000000 dp-launching-app-0.0.8/dp/launching/typing/bohrium.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      944 2024-05-20 10:13:32.000000 dp-launching-app-0.0.8/dp/launching/typing/dataset.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/dflow.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.8/dp/launching/typing/io.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-29 08:19:19.856901 dp-launching-app-0.0.8/dp_launching_app.egg-info/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1123 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/SOURCES.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/dependency_links.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/entry_points.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/requires.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-29 08:19:19.000000 dp-launching-app-0.0.8/dp_launching_app.egg-info/top_level.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-29 08:19:19.857308 dp-launching-app-0.0.8/setup.cfg
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-29 08:19:08.000000 dp-launching-app-0.0.8/setup.py
```

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/__init__.py` & `dp-launching-app-0.0.8/dp/launching/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/api/model.py` & `dp-launching-app-0.0.8/dp/launching/cli/api/model.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/api/persistent_service.py` & `dp-launching-app-0.0.8/dp/launching/cli/api/persistent_service.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/commands/launching.py` & `dp-launching-app-0.0.8/dp/launching/cli/commands/launching.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/basic.py` & `dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/basic/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/bohrium.py` & `dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/bohrium/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/dflow.py` & `dp-launching-app-0.0.8/dp/launching/cli/commands/scaffold/dflow/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/report/__init__.py` & `dp-launching-app-0.0.8/dp/launching/report/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/addon/sysmbol.py` & `dp-launching-app-0.0.8/dp/launching/typing/addon/sysmbol.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/addon/ui.py` & `dp-launching-app-0.0.8/dp/launching/typing/addon/ui.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/basic.py` & `dp-launching-app-0.0.8/dp/launching/typing/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/bio.py` & `dp-launching-app-0.0.8/dp/launching/typing/bio.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/bohrium.py` & `dp-launching-app-0.0.8/dp/launching/typing/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/dataset.py` & `dp-launching-app-0.0.8/dp/launching/typing/dataset.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/dflow.py` & `dp-launching-app-0.0.8/dp/launching/typing/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp/launching/typing/io.py` & `dp-launching-app-0.0.8/dp/launching/typing/io.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/dp_launching_app.egg-info/SOURCES.txt` & `dp-launching-app-0.0.8/dp_launching_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.7/setup.py` & `dp-launching-app-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dp-launching-app",
-    version="0.0.7",
+    version="0.0.8",
     author="",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     entry_points={
```

