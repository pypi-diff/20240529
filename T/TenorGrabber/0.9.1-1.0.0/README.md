# Comparing `tmp/tenorgrabber-0.9.1.tar.gz` & `tmp/tenorgrabber-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenorgrabber-0.9.1.tar", last modified: Wed May 29 08:03:11 2024, max compression
+gzip compressed data, was "tenorgrabber-1.0.0.tar", last modified: Wed May 29 08:06:15 2024, max compression
```

## Comparing `tenorgrabber-0.9.1.tar` & `tenorgrabber-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:11.338462 tenorgrabber-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-29 08:03:11.338462 tenorgrabber-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:11.334462 tenorgrabber-0.9.1/TenorGrabber/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/TenorGrabber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/TenorGrabber/tenorgrabber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:11.338462 tenorgrabber-0.9.1/TenorGrabber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-29 08:03:11.000000 tenorgrabber-0.9.1/TenorGrabber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-29 08:03:11.000000 tenorgrabber-0.9.1/TenorGrabber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:03:11.000000 tenorgrabber-0.9.1/TenorGrabber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 08:03:11.000000 tenorgrabber-0.9.1/TenorGrabber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:03:11.338462 tenorgrabber-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:11.338462 tenorgrabber-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 08:03:07.000000 tenorgrabber-0.9.1/tests/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/TenorGrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/TenorGrabber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/TenorGrabber/tenorgrabber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/TenorGrabber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-29 08:06:15.000000 tenorgrabber-1.0.0/TenorGrabber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-29 08:06:15.000000 tenorgrabber-1.0.0/TenorGrabber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:06:15.000000 tenorgrabber-1.0.0/TenorGrabber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 08:06:15.000000 tenorgrabber-1.0.0/TenorGrabber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:15.385105 tenorgrabber-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-29 08:06:11.000000 tenorgrabber-1.0.0/tests/tenorgrabber.py
```

### Comparing `tenorgrabber-0.9.1/LICENSE` & `tenorgrabber-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenorgrabber-0.9.1/PKG-INFO` & `tenorgrabber-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 0.9.1
+Version: 1.0.0
 Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Useful for discord/guilded bots to grab a tenor gif link and embed it
+<br>
 Usage:
 ```
 from TenorGrabber import tenorgrabber
 tenorgrabber.getgiflink("https://tenor.com/view/GIF")
 ```
 Example:
 ```
```

### Comparing `tenorgrabber-0.9.1/TenorGrabber.egg-info/PKG-INFO` & `tenorgrabber-1.0.0/TenorGrabber.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: TenorGrabber
-Version: 0.9.1
+Version: 1.0.0
 Summary: Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Author: user0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TenorGrabber
 Tired of /view links on tenor? This python library allows you to get the direct link of the GIF!
 Useful for discord/guilded bots to grab a tenor gif link and embed it
+<br>
 Usage:
 ```
 from TenorGrabber import tenorgrabber
 tenorgrabber.getgiflink("https://tenor.com/view/GIF")
 ```
 Example:
 ```
```

