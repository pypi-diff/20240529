# Comparing `tmp/ambientctl-0.1.2.tar.gz` & `tmp/ambientctl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambientctl-0.1.2.tar", last modified: Mon May 27 20:00:33 2024, max compression
+gzip compressed data, was "ambientctl-0.2.0.tar", last modified: Wed May 29 06:25:04 2024, max compression
```

## Comparing `ambientctl-0.1.2.tar` & `ambientctl-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:33.786172 ambientctl-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 20:00:33.786172 ambientctl-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:33.782172 ambientctl-0.1.2/ambientctl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:33.786172 ambientctl-0.1.2/ambientctl/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/parsers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/parsers/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-27 20:00:26.000000 ambientctl-0.1.2/ambientctl/parsers/ports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:00:33.786172 ambientctl-0.1.2/ambientctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 20:00:33.000000 ambientctl-0.1.2/ambientctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:00:33.786172 ambientctl-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-27 20:00:26.000000 ambientctl-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:04.440198 ambientctl-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 06:25:04.440198 ambientctl-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:04.440198 ambientctl-0.2.0/ambientctl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:04.440198 ambientctl-0.2.0/ambientctl/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/parsers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/parsers/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/parsers/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-29 06:24:55.000000 ambientctl-0.2.0/ambientctl/parsers/ports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:25:04.440198 ambientctl-0.2.0/ambientctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 06:25:04.000000 ambientctl-0.2.0/ambientctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:25:04.440198 ambientctl-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-29 06:24:55.000000 ambientctl-0.2.0/setup.py
```

### Comparing `ambientctl-0.1.2/ambientctl/main.py` & `ambientctl-0.2.0/ambientctl/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 
-from ambientctl.parsers import auth, ping, ports
+from ambientctl.parsers import auth, daemon, ping, ports
 
 
 def main():
     parser = argparse.ArgumentParser(prog="ambientctl")
     subparsers = parser.add_subparsers(dest="command")
 
     # add parsers to the list below
-    parsers = [ping, ports, auth]
+    parsers = [ping, ports, auth, daemon]
 
     # this loops through the parsers and adds them to the subparsers
     for _parser in parsers:
         parser_ = _parser.get_parser()
         parser_name = _parser.__name__.split(".")[-1]
         subparser = subparsers.add_parser(parser_name, parents=[parser_], add_help=True)
         subparser.set_defaults(func=_parser.run)
```

### Comparing `ambientctl-0.1.2/ambientctl/parsers/auth.py` & `ambientctl-0.2.0/ambientctl/parsers/auth.py`

 * *Files identical despite different names*

### Comparing `ambientctl-0.1.2/ambientctl/parsers/ping.py` & `ambientctl-0.2.0/ambientctl/parsers/ping.py`

 * *Files identical despite different names*

### Comparing `ambientctl-0.1.2/ambientctl/parsers/ports.py` & `ambientctl-0.2.0/ambientctl/parsers/ports.py`

 * *Files identical despite different names*

