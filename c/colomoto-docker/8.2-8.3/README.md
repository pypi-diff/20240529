# Comparing `tmp/colomoto-docker-8.2.tar.gz` & `tmp/colomoto_docker-8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colomoto-docker-8.2.tar", last modified: Wed Oct  4 20:56:25 2023, max compression
+gzip compressed data, was "colomoto_docker-8.3.tar", last modified: Wed May 29 06:38:44 2024, max compression
```

## Comparing `colomoto-docker-8.2.tar` & `colomoto_docker-8.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2023-10-04 20:56:25.207298 colomoto-docker-8.2/
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)      245 2023-10-04 20:56:25.207298 colomoto-docker-8.2/PKG-INFO
-drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2023-10-04 20:56:25.207298 colomoto-docker-8.2/colomoto_docker.egg-info/
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)       27 2023-10-04 20:56:25.000000 colomoto-docker-8.2/colomoto_docker.egg-info/SOURCES.txt
--rwxr-xr-x   0 pauleve   (1000) pauleve   (1000)    11202 2023-10-04 20:55:48.000000 colomoto-docker-8.2/colomoto_docker.py
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)       38 2023-10-04 20:56:25.207298 colomoto-docker-8.2/setup.cfg
--rw-r--r--   0 pauleve   (1000) pauleve   (1000)      645 2023-10-04 20:42:18.000000 colomoto-docker-8.2/setup.py
+drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 06:38:44.913926 colomoto_docker-8.3/
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)      245 2024-05-29 06:38:44.913926 colomoto_docker-8.3/PKG-INFO
+drwxr-xr-x   0 pauleve   (1000) pauleve   (1000)        0 2024-05-29 06:38:44.912926 colomoto_docker-8.3/colomoto_docker.egg-info/
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)       27 2024-05-29 06:38:44.000000 colomoto_docker-8.3/colomoto_docker.egg-info/SOURCES.txt
+-rwxr-xr-x   0 pauleve   (1000) pauleve   (1000)    11376 2024-05-29 06:37:35.000000 colomoto_docker-8.3/colomoto_docker.py
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)       38 2024-05-29 06:38:44.913926 colomoto_docker-8.3/setup.cfg
+-rw-r--r--   0 pauleve   (1000) pauleve   (1000)      645 2023-10-19 22:28:21.000000 colomoto_docker-8.3/setup.py
```

### Comparing `colomoto-docker-8.2/colomoto_docker.py` & `colomoto_docker-8.3/colomoto_docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import random
 import re
 import socket
 import subprocess
 import sys
 import webbrowser
 
-__version__ = "8.2"
+__version__ = "8.3"
 
 on_linux = platform.system() == "Linux"
 
 pat_tag = re.compile(r"\d{4}-\d{2}-\d{2}")
 
 persistent_volume = "colomoto-{}".format(getuser())
 persistent_dir = "persistent"
@@ -107,15 +107,19 @@
 
     group = parser.add_argument_group("docker run options")
     group.add_argument("-e", "--env", action="append",
         help="Set environment variables")
     group.add_argument("--name", help="Name of the container")
     group.add_argument("-v", "--volume", action="append",
         help="Bind mount a volume")
-    docker_run_opts = ["env", "volume"]
+    group.add_argument("--network", type=str,
+        help="Network access")
+    group.add_argument("--ulimit", type=str,
+        help="Resource limit")
+    docker_run_opts = ["env", "volume", "network", "ulimit"]
 
     parser.add_argument("command", nargs=REMAINDER, help="Command to run instead of colomoto-nb")
     args = parser.parse_args()
 
     info(f"colomoto-docker {__version__}")
 
     image_tag = args.version
```

### Comparing `colomoto-docker-8.2/setup.py` & `colomoto_docker-8.3/setup.py`

 * *Files identical despite different names*

