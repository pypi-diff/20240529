# Comparing `tmp/linuxfabrik-lib-2023051201.post1.tar.gz` & `tmp/linuxfabrik_lib-2024052901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxfabrik-lib-2023051201.post1.tar", last modified: Thu Aug 24 06:26:53 2023, max compression
+gzip compressed data, was "linuxfabrik_lib-2024052901.tar", last modified: Wed May 29 15:52:14 2024, max compression
```

## Comparing `linuxfabrik-lib-2023051201.post1.tar` & `linuxfabrik_lib-2024052901.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 markus.frei  (1000) markus.frei  (1000)        0 2023-08-24 06:26:53.562661 linuxfabrik-lib-2023051201.post1/
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1210 2022-03-01 16:20:39.000000 linuxfabrik-lib-2023051201.post1/LICENSE
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     6550 2023-08-24 06:26:53.561661 linuxfabrik-lib-2023051201.post1/PKG-INFO
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     3402 2023-08-23 11:33:35.000000 linuxfabrik-lib-2023051201.post1/README.md
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)       59 2022-03-01 16:20:39.000000 linuxfabrik-lib-2023051201.post1/__init__.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     2581 2023-05-12 11:59:31.000000 linuxfabrik-lib-2023051201.post1/args.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)    19446 2023-07-12 19:27:52.000000 linuxfabrik-lib-2023051201.post1/base.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     3972 2023-07-07 14:33:19.000000 linuxfabrik-lib-2023051201.post1/cache.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     4385 2023-05-12 11:59:29.000000 linuxfabrik-lib-2023051201.post1/db_mysql.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)    15884 2023-08-23 11:29:48.000000 linuxfabrik-lib-2023051201.post1/db_sqlite.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     7628 2023-05-12 11:59:29.000000 linuxfabrik-lib-2023051201.post1/disk.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)    10909 2023-05-12 11:59:30.000000 linuxfabrik-lib-2023051201.post1/distro.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     7519 2023-05-12 11:59:26.000000 linuxfabrik-lib-2023051201.post1/dmidecode.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)    44867 2023-08-17 12:21:13.000000 linuxfabrik-lib-2023051201.post1/endoflifedate.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     3260 2023-05-12 11:59:27.000000 linuxfabrik-lib-2023051201.post1/feedparser.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1489 2023-05-12 11:59:27.000000 linuxfabrik-lib-2023051201.post1/globals.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     4843 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/grassfish.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)    16328 2023-07-11 07:26:50.000000 linuxfabrik-lib-2023051201.post1/huawei.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     7404 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/human.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     6689 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/icinga.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     2892 2023-07-14 07:36:20.000000 linuxfabrik-lib-2023051201.post1/infomaniak.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1447 2023-05-12 11:59:29.000000 linuxfabrik-lib-2023051201.post1/jitsi.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1803 2023-05-12 11:59:30.000000 linuxfabrik-lib-2023051201.post1/librenms.py
-drwxr-xr-x   0 markus.frei  (1000) markus.frei  (1000)        0 2023-08-24 06:26:53.561661 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     6550 2023-08-24 06:26:53.000000 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/PKG-INFO
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)      656 2023-08-24 06:26:53.000000 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/SOURCES.txt
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)        1 2023-08-24 06:26:53.000000 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/dependency_links.txt
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)      160 2023-08-24 06:26:53.000000 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/requires.txt
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)        4 2023-08-24 06:26:53.000000 linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/top_level.txt
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     7746 2023-05-12 11:59:27.000000 linuxfabrik-lib-2023051201.post1/net.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)      967 2023-05-12 11:59:27.000000 linuxfabrik-lib-2023051201.post1/nodebb.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1211 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/powershell.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1170 2023-05-12 11:59:26.000000 linuxfabrik-lib-2023051201.post1/psutil.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     2420 2023-08-23 10:00:31.000000 linuxfabrik-lib-2023051201.post1/pyproject.toml
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)    15397 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/redfish.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     2143 2023-05-12 11:59:27.000000 linuxfabrik-lib-2023051201.post1/rocket.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)       38 2023-08-24 06:26:53.562661 linuxfabrik-lib-2023051201.post1/setup.cfg
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     6171 2023-05-12 11:59:26.000000 linuxfabrik-lib-2023051201.post1/shell.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     3322 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/smb.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     1127 2023-05-12 11:59:29.000000 linuxfabrik-lib-2023051201.post1/test.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     2386 2023-05-12 11:59:30.000000 linuxfabrik-lib-2023051201.post1/time.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)    15484 2023-05-12 11:59:29.000000 linuxfabrik-lib-2023051201.post1/txt.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     7331 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/url.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     2116 2023-05-12 11:59:26.000000 linuxfabrik-lib-2023051201.post1/veeam.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     4716 2023-07-10 06:13:13.000000 linuxfabrik-lib-2023051201.post1/version.py
--rw-r--r--   0 markus.frei  (1000) markus.frei  (1000)     1225 2023-05-12 11:59:26.000000 linuxfabrik-lib-2023051201.post1/wildfly.py
--rw-rw-r--   0 markus.frei  (1000) markus.frei  (1000)     2508 2023-05-12 11:59:28.000000 linuxfabrik-lib-2023051201.post1/winrm.py
+drwxr-xr-x   0 markusfrei  (1000) markusfrei  (1000)        0 2024-05-29 15:52:14.383489 linuxfabrik_lib-2024052901/
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1210 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/LICENSE
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     7167 2024-05-29 15:52:14.383489 linuxfabrik_lib-2024052901/PKG-INFO
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     3655 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/README.md
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)       59 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/__init__.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     3340 2024-03-31 16:42:07.000000 linuxfabrik_lib-2024052901/args.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)    20829 2024-04-12 11:18:33.000000 linuxfabrik_lib-2024052901/base.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     3972 2024-03-26 16:14:56.000000 linuxfabrik_lib-2024052901/cache.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     4715 2024-03-28 15:26:15.000000 linuxfabrik_lib-2024052901/db_mysql.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)    15954 2024-03-27 19:12:37.000000 linuxfabrik_lib-2024052901/db_sqlite.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)    10177 2024-04-01 12:48:45.000000 linuxfabrik_lib-2024052901/disk.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)    10909 2024-04-17 09:15:45.000000 linuxfabrik_lib-2024052901/distro.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     7519 2023-11-29 13:44:06.000000 linuxfabrik_lib-2024052901/dmidecode.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)    53573 2024-05-28 08:47:06.000000 linuxfabrik_lib-2024052901/endoflifedate.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     3600 2024-04-10 06:12:59.000000 linuxfabrik_lib-2024052901/feedparser.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1489 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/globals.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     4965 2024-03-14 14:18:55.000000 linuxfabrik_lib-2024052901/grassfish.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)    16346 2024-03-14 14:40:59.000000 linuxfabrik_lib-2024052901/huawei.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)    11596 2024-03-30 16:39:27.000000 linuxfabrik_lib-2024052901/human.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     7236 2024-03-14 15:11:45.000000 linuxfabrik_lib-2024052901/icinga.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     3270 2024-03-14 15:33:16.000000 linuxfabrik_lib-2024052901/infomaniak.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1537 2024-03-14 18:44:48.000000 linuxfabrik_lib-2024052901/jitsi.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     2088 2024-03-29 10:00:54.000000 linuxfabrik_lib-2024052901/librenms.py
+drwxr-xr-x   0 markusfrei  (1000) markusfrei  (1000)        0 2024-05-29 15:52:14.383489 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     7167 2024-05-29 15:52:14.000000 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/PKG-INFO
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)      665 2024-05-29 15:52:14.000000 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)        1 2024-05-29 15:52:14.000000 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)      160 2024-05-29 15:52:14.000000 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/requires.txt
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)        4 2024-05-29 15:52:14.000000 linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/top_level.txt
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     8208 2024-04-10 09:47:59.000000 linuxfabrik_lib-2024052901/net.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)      999 2024-03-14 19:11:48.000000 linuxfabrik_lib-2024052901/nodebb.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1211 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/powershell.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1170 2023-11-29 13:44:06.000000 linuxfabrik_lib-2024052901/psutil.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     2418 2024-05-29 15:51:57.000000 linuxfabrik_lib-2024052901/pyproject.toml
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     2156 2024-03-15 09:26:35.000000 linuxfabrik_lib-2024052901/qts.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)    15397 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/redfish.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     2425 2024-03-15 09:43:18.000000 linuxfabrik_lib-2024052901/rocket.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)       38 2024-05-29 15:52:14.383489 linuxfabrik_lib-2024052901/setup.cfg
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     6334 2023-11-29 13:44:06.000000 linuxfabrik_lib-2024052901/shell.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     3322 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/smb.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     1127 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/test.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     2386 2024-03-21 07:06:42.000000 linuxfabrik_lib-2024052901/time.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)    16595 2024-03-31 16:44:57.000000 linuxfabrik_lib-2024052901/txt.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     7331 2024-03-29 09:51:36.000000 linuxfabrik_lib-2024052901/url.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     2157 2024-03-15 10:08:18.000000 linuxfabrik_lib-2024052901/veeam.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     7749 2024-03-15 14:40:53.000000 linuxfabrik_lib-2024052901/version.py
+-rw-r--r--   0 markusfrei  (1000) markusfrei  (1000)     1361 2024-03-15 10:22:41.000000 linuxfabrik_lib-2024052901/wildfly.py
+-rw-rw-r--   0 markusfrei  (1000) markusfrei  (1000)     2508 2023-11-29 13:44:05.000000 linuxfabrik_lib-2024052901/winrm.py
```

### Comparing `linuxfabrik-lib-2023051201.post1/LICENSE` & `linuxfabrik_lib-2024052901/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxfabrik-lib-2023051201.post1/PKG-INFO` & `linuxfabrik_lib-2024052901/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxfabrik-lib
-Version: 2023051201.post1
+Version: 2024052901
 Summary: Python libraries used in various Linuxfabrik projects, including the 'Linuxfabrik Monitoring Plugins' project.
 Author-email: "Linuxfabrik GmbH, Zurich, Switzerland" <info@linuxfabrik.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -52,48 +52,141 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: netifaces
+Requires-Dist: psutil
+Requires-Dist: pymysql
+Requires-Dist: pysmbclient
+Requires-Dist: python-keystoneclient
+Requires-Dist: python-novaclient
+Requires-Dist: python-swiftclient
+Requires-Dist: pywinrm
+Requires-Dist: requests
+Requires-Dist: smbprotocol
+Requires-Dist: vici
+Requires-Dist: xmltodict
 
 # Linuxfabrik's Python Libraries
 
 These Python libraries are used in various projects of Linuxfabrik, including the [Linuxfabrik Monitoring Plugins project](https://github.com/Linuxfabrik/monitoring-plugins).
 
-List of libraries:
 
-* args.py: Extends argparse by new input argument data types on demand.
-* base.py: Provides very common every-day functions.
-* cache.py: Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
-* db_mysql.py: Library for accessing MySQL/MariaDB servers.
-* db_sqlite.py: Library for accessing SQLite databases.
-* disk.py: Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
-* distro.py: Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
-* dmidecode.py: Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
-* endoflifedate.py: This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
-* feedparser.py: Parse Atom and RSS feeds in Python.
-* globals.py: This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
-* grassfish.py: Provides functions using the Grassfish REST-API.
-* huawei.py: This library collects some Huawei related functions that are needed by Huawei check plugins.
-* human.py: Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
-* icinga.py: This module tries to make accessing the Icinga2 API easier.
-* infomaniak.py: Provides functions using the Infomanik REST-API.
-* jitsi.py: This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
-* librenms.py: This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
-* net.py: Provides network related functions and variables.
-* nodebb.py: This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
-* powershell.py: This library collects some Microsoft PowerShell related functions.
-* psutil.py: Wrapper library for functions from psutil.
-* redfish.py: This library parses data returned from the Redfish API.
-* rocket.py: This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
-* shell.py: Communicates with the Shell.
-* smb.py: Provides functions to establish native SMB connections.
-* test.py: Provides test functions for unit tests.
-* time.py: Provides datetime functions.
-* txt.py: A collection of text functions.
-* url.py: Get for example HTML or JSON from an URL.
-* veeam.py: This library interacts with the Veeam Enterprise Manager API.
-* version.py: Provides functions for handling software versions.
-* wildfly.py: This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
-* winrm.py: This library collects some Microsoft WinRM related functions.
+## Installation
+
+`pip install linuxfabrik-lib`
+
+
+## Documentation
+
+For example by browsing http://localhost:8080/ after starting `pydoc -p 8080`.
+
+
+## List of libraries
+
+
+* args.py:  
+Extends argparse by new input argument data types on demand.
+
+* base.py:  
+Provides very common every-day functions.
+
+* cache.py:  
+Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
+
+* db_mysql.py:  
+Library for accessing MySQL/MariaDB servers.
+
+* db_sqlite.py:  
+Library for accessing SQLite databases.
+
+* disk.py:  
+Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
+
+* distro.py:  
+Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
+
+* dmidecode.py:  
+Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
+
+* endoflifedate.py:  
+This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
+
+* feedparser.py:  
+Parse Atom and RSS feeds in Python.
+
+* globals.py:  
+This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
+
+* grassfish.py:  
+Provides functions using the Grassfish REST-API.
+
+* huawei.py:  
+This library collects some Huawei related functions that are needed by Huawei check plugins.
+
+* human.py:  
+Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
+
+* icinga.py:  
+This module tries to make accessing the Icinga2 API easier.
+
+* infomaniak.py:  
+Provides functions using the Infomanik REST-API.
+
+* jitsi.py:  
+This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
+
+* librenms.py:  
+This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
+
+* net.py:  
+Provides network related functions and variables.
+
+* nodebb.py:  
+This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
+
+* powershell.py:  
+This library collects some Microsoft PowerShell related functions.
+
+* psutil.py:  
+Wrapper library for functions from psutil.
+
+* redfish.py:  
+This library parses data returned from the Redfish API.
+
+* rocket.py:  
+This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
+
+* shell.py:  
+Communicates with the Shell.
+
+* smb.py:  
+Provides functions to establish native SMB connections.
+
+* test.py:  
+Provides test functions for unit tests.
+
+* time.py:  
+Provides datetime functions.
+
+* txt.py:  
+A collection of text functions.
+
+* url.py:  
+Get for example HTML or JSON from an URL.
+
+* veeam.py:  
+This library interacts with the Veeam Enterprise Manager API.
+
+* version.py:  
+Provides functions for handling software versions.
+
+* wildfly.py:  
+This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
+
+* winrm.py:  
+This library collects some Microsoft WinRM related functions.
```

### Comparing `linuxfabrik-lib-2023051201.post1/README.md` & `linuxfabrik_lib-2024052901/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,119 @@
 # Linuxfabrik's Python Libraries
 
 These Python libraries are used in various projects of Linuxfabrik, including the [Linuxfabrik Monitoring Plugins project](https://github.com/Linuxfabrik/monitoring-plugins).
 
-List of libraries:
 
-* args.py: Extends argparse by new input argument data types on demand.
-* base.py: Provides very common every-day functions.
-* cache.py: Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
-* db_mysql.py: Library for accessing MySQL/MariaDB servers.
-* db_sqlite.py: Library for accessing SQLite databases.
-* disk.py: Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
-* distro.py: Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
-* dmidecode.py: Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
-* endoflifedate.py: This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
-* feedparser.py: Parse Atom and RSS feeds in Python.
-* globals.py: This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
-* grassfish.py: Provides functions using the Grassfish REST-API.
-* huawei.py: This library collects some Huawei related functions that are needed by Huawei check plugins.
-* human.py: Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
-* icinga.py: This module tries to make accessing the Icinga2 API easier.
-* infomaniak.py: Provides functions using the Infomanik REST-API.
-* jitsi.py: This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
-* librenms.py: This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
-* net.py: Provides network related functions and variables.
-* nodebb.py: This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
-* powershell.py: This library collects some Microsoft PowerShell related functions.
-* psutil.py: Wrapper library for functions from psutil.
-* redfish.py: This library parses data returned from the Redfish API.
-* rocket.py: This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
-* shell.py: Communicates with the Shell.
-* smb.py: Provides functions to establish native SMB connections.
-* test.py: Provides test functions for unit tests.
-* time.py: Provides datetime functions.
-* txt.py: A collection of text functions.
-* url.py: Get for example HTML or JSON from an URL.
-* veeam.py: This library interacts with the Veeam Enterprise Manager API.
-* version.py: Provides functions for handling software versions.
-* wildfly.py: This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
-* winrm.py: This library collects some Microsoft WinRM related functions.
+## Installation
+
+`pip install linuxfabrik-lib`
+
+
+## Documentation
+
+For example by browsing http://localhost:8080/ after starting `pydoc -p 8080`.
+
+
+## List of libraries
+
+
+* args.py:  
+Extends argparse by new input argument data types on demand.
+
+* base.py:  
+Provides very common every-day functions.
+
+* cache.py:  
+Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
+
+* db_mysql.py:  
+Library for accessing MySQL/MariaDB servers.
+
+* db_sqlite.py:  
+Library for accessing SQLite databases.
+
+* disk.py:  
+Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
+
+* distro.py:  
+Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
+
+* dmidecode.py:  
+Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
+
+* endoflifedate.py:  
+This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
+
+* feedparser.py:  
+Parse Atom and RSS feeds in Python.
+
+* globals.py:  
+This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
+
+* grassfish.py:  
+Provides functions using the Grassfish REST-API.
+
+* huawei.py:  
+This library collects some Huawei related functions that are needed by Huawei check plugins.
+
+* human.py:  
+Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
+
+* icinga.py:  
+This module tries to make accessing the Icinga2 API easier.
+
+* infomaniak.py:  
+Provides functions using the Infomanik REST-API.
+
+* jitsi.py:  
+This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
+
+* librenms.py:  
+This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
+
+* net.py:  
+Provides network related functions and variables.
+
+* nodebb.py:  
+This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
+
+* powershell.py:  
+This library collects some Microsoft PowerShell related functions.
+
+* psutil.py:  
+Wrapper library for functions from psutil.
+
+* redfish.py:  
+This library parses data returned from the Redfish API.
+
+* rocket.py:  
+This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
+
+* shell.py:  
+Communicates with the Shell.
+
+* smb.py:  
+Provides functions to establish native SMB connections.
+
+* test.py:  
+Provides test functions for unit tests.
+
+* time.py:  
+Provides datetime functions.
+
+* txt.py:  
+A collection of text functions.
+
+* url.py:  
+Get for example HTML or JSON from an URL.
+
+* veeam.py:  
+This library interacts with the Veeam Enterprise Manager API.
+
+* version.py:  
+Provides functions for handling software versions.
+
+* wildfly.py:  
+This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
+
+* winrm.py:  
+This library collects some Microsoft WinRM related functions.
```

### Comparing `linuxfabrik-lib-2023051201.post1/args.py` & `linuxfabrik_lib-2024052901/args.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """Extends argparse by new input argument data types on demand.
 """
 
 import re  # pylint: disable=C0413
 
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024033101'
 
 
 def csv(arg):
     """Returns a list from a `csv` input argument.
     """
     return [x.strip() for x in arg.split(',')]
 
@@ -28,14 +28,34 @@
     """Returns None or float from a `float_or_none` input argument.
     """
     if arg is None or str(arg).lower() == 'none':
         return None
     return float(arg)
 
 
+def help(param):
+    """Return global valid help text for a parameter.
+    """
+    h = {
+        '--match':
+            'Uses Python regular expressions without any external flags like `re.IGNORECASE`. '
+            'The regular expression is applied to each line of the output. '
+            'Examples: '
+            '`(?i)example` to match the word "example" in a case-insensitive manner. '
+            '`^(?!.*example).*$` to match any string except "example" (negative lookahead). '
+            '`(?: ... )*` is a non-capturing group that matches any sequence of characters  '
+            'that satisfy the condition inside it, zero or more times. ',
+        }
+    return h[param]
+    try:
+        return h[param]
+    except KeyError:
+        return ''
+
+
 def int_or_none(arg):
     """Returns None or int from a `int_or_none` input argument.
     """
     if arg is None or str(arg).lower() == 'none':
         return None
     return int(arg)
```

### Comparing `linuxfabrik-lib-2023051201.post1/base.py` & `linuxfabrik_lib-2024052901/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Provides very common every-day functions.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023071202'
+__version__ = '2024041201'
 
 import collections
 import numbers
 import operator
 import os
 import sys
 
@@ -138,15 +138,15 @@
     _operator : string
         `eq` = equal to
         `ge` = greater or equal
         `gt` = greater than
         `le` = less or equal
         `lt` = less than
         `ne` = not equal to
-        `range` = match range
+        `range` = match Nagios range definition
 
     Returns
     -------
     int
         `STATE_OK`, `STATE_WARN` or `STATE_CRIT`
     """
     # make sure to use float comparison
@@ -256,15 +256,15 @@
     for idx, row in enumerate(data):
         for col in cols:
             try:
                 if strip:
                     data[idx][col] = str(row[col]).strip()
                 else:
                     data[idx][col] = str(row[col])
-            except:
+            except KeyError as e:
                 return 'Unknown column "{}"'.format(col)
             # get the maximum length
             try:
                 column_widths[col] = max(column_widths[col], len(data[idx][col]))
             except:
                 column_widths[col] = len(data[idx][col])
 
@@ -373,34 +373,42 @@
     True
     >>> is_numeric('53.4')
     False
     """
     return isinstance(value, numbers.Number)
 
 
-def lookup_lod(dicts, key, needle, default=None):
-    """Search in a list of dictionaries ("lod)" for a value in a given dict key.
-    Return a default if not found.
+def lookup_lod(haystack, key, needle):
+    """Search in a list of dictionaries ("lod)" for the key containing a specific value
+    and return the first dictionary item found.
+    Returns (index, item) if needle was found, (-1, None) in every other case.
 
-    >>> dicts = [
+    >>> haystack = [
     ...     { "name": "Tom", "age": 10 },
     ...     { "name": "Mark", "age": 5 },
     ...     { "name": "Pam", "age": 7 },
     ...     { "name": "Dick", "age": 12 }
     ... ]
-    >>> lookup_lod(dicts, 'name', 'Pam')
-    {'name': 'Pam', 'age': 7}
-    >>> lookup_lod(dicts, 'name', 'Pamela')
+    >>> lookup_lod(haystack, 'name', 'Pam')
+    (2, {'name': 'Pam', 'age': 7})
+    >>> lookup_lod(haystack, 'name', 'Pamela')
+    (-1, None)
     >>>
     """
-    return next((item for item in dicts if item[key] == needle), None)
+    try:
+        for index, item in enumerate(haystack):
+            if item[key] == needle:
+                return index, item
+    except:
+        return -1, None
+    return -1, None
 
 
 def match_range(value, spec):
-    """Decides if `value` is inside/outside the threshold spec.
+    """Decides if `value` is inside/outside the Nagios threshold spec.
 
     Parameters
     ----------
     spec : str
         Nagios range specification
     value : int or float
         Numeric value
@@ -408,14 +416,33 @@
     Returns
     -------
     bool
         `True` if `value` is inside the bounds for a non-inverted
         `spec`, or outside the bounds for an inverted `spec`. Otherwise `False`.
 
     Inspired by https://github.com/mpounsett/nagiosplugin/blob/master/nagiosplugin/range.py
+
+    >>> match_range(15, '10')
+    0 10 False
+    >>> match_range(15, '-10')
+    (False, 'Start 0 must not be greater than end -10')
+    >>> match_range(15, '10:')
+    10 inf False
+    >>> match_range(15, ':')
+    0 inf False
+    >>> match_range(15, '~:10')
+    -inf 10 False
+    >>> match_range(15, '10:20')
+    10 20 False
+    >>> match_range(15, '@10')
+    0 10 True
+    >>> match_range(15, '@~:20')
+    -inf 20 True
+    >>> match_range(15, '@')
+    0 inf True
     """
     def parse_range(spec):
         """
         Inspired by https://github.com/mpounsett/nagiosplugin/blob/master/nagiosplugin/range.py
 
         +--------+-------------------+-------------------+--------------------------------+
         | -w, -c | OK if result is   | WARN/CRIT if      | lib.base.parse_range() returns |
@@ -488,18 +515,24 @@
 def oao(msg, state=STATE_OK, perfdata='', always_ok=False):
     """Over and Out (OaO)
 
     Print the stripped plugin message. If perfdata is given, attach it
     by `|` and print it stripped. Exit with `state`, or with STATE_OK (0) if
     `always_ok` is set to `True`.
     """
+    msg = msg.strip()
+    # The `|` character is a reserved one to seperate plugin output from performance data.
+    # There is actually no way to escape it, so replace it.
+    msg = msg.replace('|', '!')
+    if always_ok:
+        msg += ' (always ok)'
     if perfdata:
-        print(msg.strip() + '|' + perfdata.strip())
+        print(msg + '|' + perfdata.strip())
     else:
-        print(msg.strip())
+        print(msg)
     if always_ok:
         sys.exit(STATE_OK)
     sys.exit(state)
 
 
 def smartcast(value):
     """Returns the value converted to float if possible, else string, else the
@@ -549,14 +582,38 @@
     if state == STATE_CRIT:
         return '{}[CRITICAL]{}'.format(prefix, suffix)
     if state == STATE_UNKNOWN:
         return '{}[UNKNOWN]{}'.format(prefix, suffix)
     return state
 
 
+def str2bool(s):
+    """Return True or False depending on the given string.
+
+    >>> str2bool("")
+    False
+    >>> str2bool("false")
+    False
+    >>> str2bool("FalSE")
+    False
+    >>> str2bool("true")
+    True
+    >>> str2bool("Linuxfabrik")
+    True
+    >>> str2bool("0")
+    True
+    """
+    if not s:
+        return False
+    elif s.lower() == 'false':
+        return False
+    else:
+        return True
+
+
 def str2state(string, ignore_error=True):
     """Return the numeric state based on a (case-insensitive) string.
     Matches up to the first four characters.
 
     >>> str2state('ok')
     0
     >>> str2state('okidoki')
```

### Comparing `linuxfabrik-lib-2023051201.post1/cache.py` & `linuxfabrik_lib-2024052901/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 u'123abc'
 >>> time.sleep(6)
 >>> cache.get('session-key')
 False
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023070701'
+__version__ = '2023112901'
 
 from . import time
 from . import db_sqlite
 
 
 def get(key, as_dict=False, path='', filename='linuxfabrik-monitoring-plugins-cache.db'):
     """Get the value of key. If the key does not exist, `False` is returned.
```

### Comparing `linuxfabrik-lib-2023051201.post1/db_mysql.py` & `linuxfabrik_lib-2024052901/db_mysql.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """Library for accessing MySQL/MariaDB servers.
 """
 
 import warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='pymysql')
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024032801'
 
 import sys
 
 from .globals import STATE_UNKNOWN
 try:
     import pymysql.cursors
 except ImportError as e:
@@ -121,24 +121,34 @@
             myvar[row['Variable_name']] = row['Value']
         except:
             for key, value in row.items():
                 myvar[key] = value
     return myvar
 
 
-def select(conn, sql, data={}, fetchone=False):
+def select(conn, sql, data=[], fetchone=False):
     """The SELECT statement is used to query the database. The result of a
     SELECT is zero or more rows of data where each row has a fixed number
     of columns. A SELECT statement does not make any changes to the
     database.
+
+    >>> data = ['val1%']
+    >>> sql = 'select * from t where c like %s'
+    >>> db_mysql.select(conn, sql, data)
+
+    >>> data = ['val1', 'val2']
+    >>> sql = 'select * from t where c in ({})'.format(
+    ...    ', '.join('%s' for d in data),  # print "%s" for each argument
+    ... )
+    >>> db_mysql.select(conn, sql, data)
     """
     with conn.cursor() as cursor:
         try:
             if data:
-                cursor.execute(sql, (data,))
+                cursor.execute(sql, (*data,))
             else:
                 cursor.execute(sql)
             if fetchone:
                 return (True, cursor.fetchone())
             return (True, cursor.fetchall())
         except Exception as e:
             return (False, 'Query failed: {}, Error: {}, Data: {}'.format(sql, e, data))
```

### Comparing `linuxfabrik-lib-2023051201.post1/db_sqlite.py` & `linuxfabrik_lib-2024052901/db_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         'SELECT * FROM perfdata WHERE name = :name ORDER BY timestamp DESC LIMIT 2',
         {'name': disk}
 
 >>> lib.db_sqlite.close(conn)
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023082301'
+__version__ = '2024032701'
 
 import csv
 import hashlib
 import os
 import re
 import sqlite3
 
@@ -64,15 +64,15 @@
     """This closes the database connection. Note that this does not
     automatically call commit(). If you just close your database connection
     without calling commit() first, your changes will be lost.
     """
     try:
         conn.close()
     except:
-        pass
+        return False
     return True
 
 
 def commit(conn):
     """Save (commit) any changes.
     """
     try:
@@ -108,15 +108,16 @@
             path = disk.get_tmpdir()
         if not filename:
             filename = 'linuxfabrik-monitoring-plugins-sqlite.db'
         return os.path.join(path, filename)
 
     db = get_filename(path, filename)
     try:
-        conn = sqlite3.connect(db, timeout=1)
+        # https://docs.python.org/3/library/sqlite3.html#sqlite3.connect
+        conn = sqlite3.connect(db)
         # https://stackoverflow.com/questions/3300464/how-can-i-get-dict-from-sqlite-query
         conn.row_factory = sqlite3.Row
         # https://stackoverflow.com/questions/3425320/sqlite3-programmingerror-you-must-not-use-8-bit-bytestrings-unless-you-use-a-te
         conn.text_factory = str
         conn.create_function("REGEXP", 2, regexp)
     except Exception as e:
         return(False, 'Connecting to DB {} failed, Error: {}'.format(db, e))
```

### Comparing `linuxfabrik-lib-2023051201.post1/disk.py` & `linuxfabrik_lib-2024052901/url.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,231 +4,184 @@
 # Author:  Linuxfabrik GmbH, Zurich, Switzerland
 # Contact: info (at) linuxfabrik (dot) ch
 #          https://www.linuxfabrik.ch/
 # License: The Unlicense, see LICENSE file.
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
-"""Offers file and disk related functions, like getting a list of
-partitions, grepping a file, etc.
+"""Get for example HTML or JSON from an URL.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
-import csv
-import os
+import json
 import re
-import tempfile
-
-
-def file_exists(path, allow_empty=False):
-    # not finding the file, exit early
-    if not os.path.exists(path):
-        return False
-
-    # if just the path needs to exists (ie, it can be empty) we are done
-    if allow_empty:
-        return True
-
-    # file exists but is empty and we dont allow_empty
-    if os.path.getsize(path) == 0:
-        return False
-
-    # file exists with some content
-    return True
-
-
-def get_cwd():
-    """Gets the current working directory.
-    """
-    return os.getcwd()
-
-
-def get_tmpdir():
-    """ Return the name of the directory used for temporary files, always
-    without trailing '/'.
-
-    Searches a standard list of directories to find one which the calling user
-    can create files in. The list is:
-
-    * The directory named by the TMPDIR environment variable.
-    * The directory named by the TEMP environment variable.
-    * The directory named by the TMP environment variable.
-    * A platform-specific location:
-      - On Windows, the directories C:\\TEMP, C:\\TMP, \\TEMP, and \\TMP,
-        in that order.
-      - On all other platforms, the directories /tmp, /var/tmp, and /usr/tmp,
-        in that order.
-    * As a last resort, the current working directory.
-    """
-    try:
-        return tempfile.gettempdir()
-    except:
-        return '/tmp'
-
-
-def grep_file(filename, pattern):
-    """Like `grep` searches for `pattern` in `filename`. Returns the
-    match, otherwise `False`.
-
-    >>> success, nc_version=lib.disk.grep_file('version.php', r'\\$OC_version=array\\((.*)\\)')
-
-    Parameters
-    ----------
-    filename : str
-        The file.
-    pattern : str
-        A Python regular expression.
-
-    Returns
-    -------
-    tuple
-        tuple[0]: bool: if successful (no I/O or file handling errors) or not
-        tuple[1]: str: the string matched by `pattern` (if any)
-    """
-    try:
-        with open(filename, 'r') as file:
-            data = file.read()
-    except IOError as e:
-        return (False, 'I/O error "{}" while opening or reading {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error opening or reading {}'.format(filename))
+import ssl
+import urllib
+import urllib.parse
+import urllib.request
+
+from . import txt
+
+def fetch(url, insecure=False, no_proxy=False, timeout=8,
+          header={}, data={}, encoding='urlencode',
+          digest_auth_user=None, digest_auth_password=None,
+          extended=False, to_text=True):
+    """Fetch any URL.
+
+    If using `extended=True`, the result is returned as a dict, also including the response header
+    and the HTTP status code.
+
+    Basic authentication:
+    >>> auth = '{}:{}'.format(args.USERNAME, args.PASSWORD)
+    >>> encoded_auth = lib.txt.to_text(base64.b64encode(lib.txt.to_bytes(auth)))
+    >>> result = lib.base.coe(lib.url.fetch(url, timeout=args.TIMEOUT,
+            header={'Authorization': 'Basic {}'.format(encoded_auth)}))
+
+    POST: the HTTP request will be a POST instead of a GET when the data parameter is provided
+    >>> result = fetch(URL, header=header, data={...})
+
+    Cookies: To fetch Cookies, parse the response header. To get the response header, use extended=True
+    >>> result = fetch(URL, header=header, data={...}, extended=True)
+    >>> result['response_header'].getheader('Set-Cookie')
+
+    Setting `to_text=False` disables the automatic converison to a text string. Use this when downloading binary files.
+    """
+    try:
+        if digest_auth_user is not None and digest_auth_password is not None:
+            # HTTP Digest Authentication
+            passmgr = urllib.request.HTTPPasswordMgrWithDefaultRealm()
+            passmgr.add_password(None, url, digest_auth_user, digest_auth_password)
+            auth_handler = urllib.request.HTTPDigestAuthHandler(passmgr)
+            opener = urllib.request.build_opener(auth_handler)
+            urllib.request.install_opener(opener)
+        if data:
+            # serializing dictionary
+            if encoding == 'urlencode':
+                data = urllib.parse.urlencode(data)
+            if encoding == 'serialized-json':
+                data = json.dumps(data)
+            data = txt.to_bytes(data)
+            # the HTTP request will be a POST instead of a GET when the data parameter is provided
+            request = urllib.request.Request(url, data=data)
+        else:
+            # the HTTP request will be a POST instead of a GET when the data parameter is provided
+            request = urllib.request.Request(url)
+
+        for key, value in header.items():
+            request.add_header(key, value)
+        # close http connections by myself
+        request.add_header('Connection', 'close')
+        # identify as Linuxfabrik Monitoring-Plugin
+        request.add_header('User-Agent', 'Linuxfabrik Monitoring Plugins')
+
+        # SSL/TLS certificate validation
+        # see: https://stackoverflow.com/questions/19268548/python-ignore-certificate-validation-urllib2
+        ctx = ssl.create_default_context()
+        if insecure:
+            ctx.check_hostname = False
+            ctx.verify_mode = ssl.CERT_NONE
+
+        # Proxy handler
+        if no_proxy:
+            proxy_handler = urllib.request.ProxyHandler({})
+            ctx_handler = urllib.request.HTTPSHandler(context=ctx)
+            opener = urllib.request.build_opener(proxy_handler, ctx_handler)
+            response = opener.open(request)
+        elif digest_auth_user is not None:
+            response = urllib.request.urlopen(request, timeout=timeout)
+        else:
+            response = urllib.request.urlopen(request, context=ctx, timeout=timeout)
+    except urllib.request.HTTPError as e:
+        # hide passwords
+        url = re.sub(r'(token|password)=([^&]+)', r'\1********', url)
+        return (False, 'HTTP error "{} {}" while fetching {}'.format(e.code, e.reason, url))
+    except urllib.request.URLError as e:
+        # hide passwords
+        url = re.sub(r'(token|password)=([^&]+)', r'\1********', url)
+        return (False, 'URL error "{}" for {}'.format(e.reason, url))
+    except TypeError as e:
+        return (False, 'Type error "{}", data="{}"'.format(e, data))
+    except:
+        # hide passwords
+        url = re.sub(r'(token|password)=([^&]+)', r'\1********', url)
+        return (False, 'Unknown error while fetching {}, maybe timeout or '
+                       'error on webserver'.format(url))
     else:
-        match = re.search(pattern, data).group(1)
-        return (True, match)
-
-
-def read_csv(filename, delimiter=',', quotechar='"', newline='', as_dict=False, skip_empty_rows=False):
-    """Reads a CSV file, and returns a list or a dict.
-    """
-    try:
-        with open(filename, newline=newline) as csvfile:
-            if not as_dict:
-                reader = csv.reader(csvfile, delimiter=delimiter, quotechar=quotechar)
+        try:
+            charset = response.headers.get_content_charset()
+            if charset is None:
+                # if the server doesn't send charset info
+                charset = 'UTF-8'
+            if not extended:
+                if to_text:
+                    result = txt.to_text(response.read(), encoding=charset)
+                else:
+                    result = response.read()
             else:
-                reader = csv.DictReader(csvfile, delimiter=delimiter, quotechar=quotechar)
-            data = []
-            for row in reader:
-                # check if the list contains empty strings only
-                if skip_empty_rows and all(s == '' or s.isspace() for s in row):
-                    continue
-                data.append(row)
-    except csv.Error as e:
-        return (False, 'CSV error in file {}, line {}: {}'.format(filename, reader.line_num, e))
-    except IOError as e:
-        return (False, 'I/O error "{}" while opening or reading {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error opening or reading {}'.format(filename))
-    return (True, data)
-
-
-def read_env(filename, delimiter='='):
-    """Reads an shell script for setting environment variables,
-    and returns a dict with all of them.
+                result = {}
+                if to_text:
+                    result['response'] = txt.to_text(response.read(), encoding=charset)
+                else:
+                    result['response'] = response.read()
+                result['status_code'] = response.getcode()
+                result['response_header'] = response.info()
+        except:
+            return (False, 'Unknown error while fetching {}, maybe timeout or '
+                       'error on webserver'.format(url))
+        return (True, result)
+
+
+def fetch_json(url, insecure=False, no_proxy=False, timeout=8,
+               header={}, data={}, encoding='urlencode',
+               digest_auth_user=None, digest_auth_password=None,
+               extended=False):
+    """Fetch JSON from an URL.
+
+    >>> fetch_json('https://1.2.3.4/api/v2/?resource=cpu')
+    """
+    success, jsonst = fetch(
+        url,
+        data=data,
+        digest_auth_password=digest_auth_password,
+        digest_auth_user=digest_auth_user,
+        encoding=encoding,
+        extended=extended,
+        header=header,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
+    )
+    if not success:
+        return (False, jsonst)
+    try:
+        if not extended:
+            result = json.loads(jsonst)
+        else:
+            result = jsonst
+            result['response_json'] = json.loads(jsonst['response'])
+    except:
+        return (False, 'ValueError: No JSON object could be decoded')
+    return (True, result)
+
+
+def get_latest_version_from_github(user, repo, key='tag_name'):
+    """Get the newest release tag from a GitHub repo.
+
+    >>> get_latest_version_from_github('matomo-org', 'matomo')
+    """
+    github_url = 'https://api.github.com/repos/{}/{}/releases/latest'.format(user, repo)
+    success, result = fetch_json(github_url)
+    if not success:
+        return (success, result)
+    if not result:
+        return (True, False)
 
-    Example shell script:
+    # on GitHub, here is the version (format of the version string depends on the maintainer)
+    return (True, result[key])
 
-        export OS_AUTH_URL="https://api/v3"
-        export OS_PROJECT_NAME=myproject
-        # comment
-        OS_PASSWORD='linuxfabrik'
-        [ -z "$OS_PASSWORD" ] && read -e -p "Pass: " OS_PASSWORD
-        export OS_PASSWORD
 
-    >>> read_env(filename)
-    {'OS_AUTH_URL': 'https://api/v3', 'OS_PROJECT_NAME': 'myproject', 'OS_PASSWORD': 'linuxfabrik'}
+def strip_tags(html):
+    """Tries to return a string with all HTML tags stripped from a given string.
     """
-    try:
-        with open(filename) as envfile:
-            data = {}
-            for line in envfile.readlines():
-                line = line.strip().split(delimiter)
-                try:
-                    if not line[0].startswith('#'):
-                        data[line[0].replace('export ', '')] = line[1].replace("'", '').replace('"', '')
-                except:
-                    continue
-    except IOError as e:
-        return (False, 'I/O error "{}" while opening or reading {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error opening or reading {}'.format(filename))
-    return (True, data)
-
-
-def read_file(filename):
-    """Reads a file.
-    """
-    try:
-        with open(filename, 'r') as f:
-            data = f.read()
-    except IOError as e:
-        return (False, 'I/O error "{}" while opening or reading {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error opening or reading {}'.format(filename))
-    return (True, data)
-
-
-def rm_file(filename):
-    """Deletes/Removes a file.
-
-    >>> rm_file('test.txt')
-    (True, None)
-    """
-    try:
-        os.remove(filename)
-    except OSError as e:
-        return (False, 'OS error "{}" while deleting {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error deleting {}'.format(filename))
-    return (True, None)
-
-
-def walk_directory(path, exclude_pattern=r'', include_pattern=r'', relative=True):
-    """Walks recursively through a directory and creates a list of files.
-    If an exclude_pattern (regex) is specified, files matching this pattern
-    are ignored. If an include_pattern (regex) is specified, only files matching
-    this pattern are put on the list (in this particular order).
-
-    >>> walk_directory('/tmp')
-    ['cpu-usage.db', 'segv_output.MCiVt9']
-    >>> walk_directory('/tmp', exclude_pattern='.*Temp-.*', relative=False)
-    ['/tmp/cpu-usage.db', '/tmp/segv_output.MCiVt9']
-    """
-    if exclude_pattern:
-        exclude_pattern = re.compile(exclude_pattern, re.IGNORECASE)
-    if include_pattern:
-        include_pattern = re.compile(include_pattern, re.IGNORECASE)
-    if not path.endswith('/'):
-        path += '/'
-
-    result = []
-    for current, dirs, files in os.walk(path):
-        for file in files:
-            file = os.path.join(current, file)
-            if exclude_pattern and exclude_pattern.match(file) is not None:
-                continue
-            if include_pattern and include_pattern.match(file) is None:
-                continue
-            if relative:
-                result.append(file.replace(path, ''))
-            else:
-                result.append(file)
-
-    return result
-
-
-def write_file(filename, content, append=False):
-    """Writes a string to a file.
-
-    >>> write_file('test.txt', 'First line\nSecond line')
-    (True, None)
-    """
-    try:
-        with open(filename, 'w' if not append else 'a') as f:
-            f.write(content)
-        f.close()
-    except IOError as e:
-        return (False, 'I/O error "{}" while writing {}'.format(e.strerror, filename))
-    except:
-        return (False, 'Unknown error writing {}, or content is not a string'.format(filename))
-    return (True, None)
+    return re.sub(r'<[^<]+?>', '', html)
```

### Comparing `linuxfabrik-lib-2023051201.post1/distro.py` & `linuxfabrik_lib-2024052901/distro.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 Source Code is taken, shortened and modified from
 * lib/ansible/module_utils/distro/_distro.py
 * lib/ansible/module_utils/common/sys_info.py
 * lib/ansible/module_utils/facts/system/distribution.py
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 
 import platform
 
 from . import disk # pylint: disable=C0413
```

### Comparing `linuxfabrik-lib-2023051201.post1/dmidecode.py` & `linuxfabrik_lib-2024052901/dmidecode.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 """Library for parsing information from dmidecode. Have a look at `man dmidecode` for details
 about dmidecode.
 Copied and refactored from py-dmidecode (https://github.com/zaibon/py-dmidecode).
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 import re
 import subprocess
 
 from . import shell
```

### Comparing `linuxfabrik-lib-2023051201.post1/feedparser.py` & `linuxfabrik_lib-2024052901/feedparser.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 """Parse Atom and RSS feeds in Python.
 
 Time zone handling is not implemented.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024041001'
 
 import sys
 
 from .globals import STATE_UNKNOWN
 try:
     from bs4 import BeautifulSoup
 except ImportError as e:
@@ -30,24 +30,30 @@
 
 
 def parse_atom(soup):
     result = {}
     result['title'] = soup.title.string
     result['updated'] = soup.updated.string
     # cut the timezone part
-    result['updated_parsed'] = time.timestr2datetime(result['updated'][0:19], pattern='%Y-%m-%dT%H:%M:%S')
+    result['updated_parsed'] = time.timestr2datetime(
+        result['updated'][0:19],
+        pattern='%Y-%m-%dT%H:%M:%S',
+    )
 
     result['entries'] = []
     for entry in soup.find_all('entry'):
         tmp = {}
         tmp['title'] = entry.title.string
         tmp['id'] = entry.id.string
         tmp['updated'] = entry.updated.string
         # cut the timezone part
-        tmp['updated_parsed'] = time.timestr2datetime(tmp['updated'][0:19], pattern='%Y-%m-%dT%H:%M:%S')
+        tmp['updated_parsed'] = time.timestr2datetime(
+            tmp['updated'][0:19],
+            pattern='%Y-%m-%dT%H:%M:%S',
+        )
         try:
             soup = BeautifulSoup(entry.summary.string, 'lxml')
             tmp['summary'] = soup.get_text()
         except:
             try:
                 soup = BeautifulSoup(entry.content.string, 'lxml')
                 tmp['summary'] = soup.get_text()
@@ -56,41 +62,58 @@
         result['entries'].append(tmp)
     return result
 
 
 def parse_rss(soup):
     result = {}
     result['title'] = soup.rss.channel.title.string
-    result['updated'] = soup.rss.channel.pubDate.string
-    # cut the timezone part
-    result['updated_parsed'] = time.timestr2datetime(result['updated'][0:25], pattern='%a, %d %b %Y %H:%M:%S')
+    try:
+        result['updated'] = soup.rss.channel.pubDate.string
+    except:
+        try:
+            result['updated'] = soup.rss.channel.lastBuildDate.string
+        except:
+            return result
+    # cut the timezone part from "Wed, 10 Apr 2024 06:12:00 Z"
+    result['updated_parsed'] = time.timestr2datetime(
+        result['updated'][0:25],
+        pattern='%a, %d %b %Y %H:%M:%S',
+    )
 
     result['entries'] = []
     for entry in soup.find_all('item'):
         tmp = {}
         tmp['title'] = entry.title.string
         tmp['id'] = entry.guid.string
         tmp['updated'] = entry.pubDate.string
         # cut the timezone part
-        tmp['updated_parsed'] = time.timestr2datetime(tmp['updated'][0:25], pattern='%a, %d %b %Y %H:%M:%S')
+        tmp['updated_parsed'] = time.timestr2datetime(
+            tmp['updated'][0:25],
+            pattern='%a, %d %b %Y %H:%M:%S',
+        )
         try:
             soup = BeautifulSoup(entry.description.string, 'lxml')
             tmp['summary'] = soup.get_text()
         except:
             pass
         result['entries'].append(tmp)
     return result
 
 
 def parse(feed_url, insecure=False, no_proxy=False, timeout=5, encoding='urlencode'):
     """Parse a feed from a URL, file, stream, or string.
     """
 
-    success, xml = url.fetch(feed_url, insecure=insecure, no_proxy=no_proxy, timeout=timeout,
-        encoding=encoding)
+    success, xml = url.fetch(
+        feed_url,
+        encoding=encoding,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
+    )
     if not success:
         return (False, xml)
 
     try:
         soup = BeautifulSoup(xml, 'xml')
     except Exception as e:
         return (False, e)
```

### Comparing `linuxfabrik-lib-2023051201.post1/globals.py` & `linuxfabrik_lib-2024052901/globals.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 fork, or open a tcp socket) that prevent it from performing the
 specified operation. Higher-level errors (such as name resolution
 errors, socket timeouts, etc) are outside of the control of plugins and
 should generally NOT be reported as UNKNOWN states.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 
 STATE_OK = 0
 STATE_WARN = 1
 STATE_CRIT = 2
 STATE_UNKNOWN = 3
 #STATE_DEPENDENT = 4
```

### Comparing `linuxfabrik-lib-2023051201.post1/grassfish.py` & `linuxfabrik_lib-2024052901/grassfish.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Provides functions using the Grassfish REST-API.
 https://ds.example.com/gv2/webservices/API/swagger/ui/index
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031401'
 
 from . import url
 
 
-def fetch_json(token, host, port, uri, version, func):
+def fetch_json(token, host, port, uri, version, func, insecure=False, no_proxy=False, timeout=8):
     """curl --request GET --header 'Accept: application/json' --header 'X-ApiKey: token' 'https://$host:$port/$uri'
     """
     uri = 'https://{}:{}{}/v{}/{}'.format(host, port, uri, version, func)
     success, result = url.fetch_json(
         uri,
         header={'X-ApiKey': token},
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
     if not success:
         return (success, result)
     if not result:
         return (False, 'There was no result from {}.'.format(uri))
 
     return (True, result)
```

### Comparing `linuxfabrik-lib-2023051201.post1/huawei.py` & `linuxfabrik_lib-2024052901/huawei.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some Huawei related functions that are
 needed by Huawei check plugins.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023071001'
+__version__ = '2024031401'
 
 import time as _time
 
 from . import base
 from . import cache
 from . import time
 from . import url
@@ -42,15 +42,15 @@
     }
     result = base.coe(url.fetch_json(
         uri,
         data=data,
         encoding='serialized-json',
         extended=True,
         header=header,
-        insecure=True,
+        insecure=args.INSECURE,
         no_proxy=args.NO_PROXY,
         timeout=args.TIMEOUT,
     ))
     ibasetoken = result.get('response_json').get('data').get('iBaseToken')
     # In Python 3, getheader() should be get()
     cookie = result.get('response_header').get('Set-Cookie')
     expire = time.now() + args.CACHE_EXPIRE*60
@@ -81,15 +81,15 @@
     # info multiple times, but limit the queries to a certain amount.
     counter = 0
     while True:
         counter += 1
         result = base.coe(url.fetch_json(
             uri,
             header=header,
-            insecure=True,
+            insecure=args.INSECURE,
             no_proxy=args.NO_PROXY,
             timeout=args.TIMEOUT,
         ))
         if result.get('error').get('code') == 0:
             break
         if counter == 9:
             break
```

### Comparing `linuxfabrik-lib-2023051201.post1/icinga.py` & `linuxfabrik_lib-2024052901/icinga.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This module tries to make accessing the Icinga2 API easier.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031401'
 
 import base64
 import time
 
 from . import txt
 from . import url
 
 # Take care of Icinga and throttle the amount of requests, don't overload it
 # with too fast subsequent api-calls.
 DEFAULT_SLEEP = 1.0
 
 
 def api_post(uri, username, password, data={}, method_override='',
-             insecure=True, no_proxy=False, timeout=3):
+             insecure=False, no_proxy=False, timeout=3):
     """POST a low level (handmade) request to the Icinga API.
 
     Example:
     >>> uri = 'https://icinga-server:5665/v1/objects/services'
     >>> data = {
     >>>    'filter': 'match("special-service", service.name)',
     >>>    'attrs': [ 'name', 'state', 'acknowledgement' ],
@@ -57,15 +57,16 @@
         no_proxy=no_proxy,
         timeout=timeout,
     )
     time.sleep(DEFAULT_SLEEP)
     return result
 
 
-def get_service(uri, username, password, servicename, attrs='state'):
+def get_service(uri, username, password, servicename, attrs='state',
+                insecure=False, no_proxy=False, timeout=3):
     """POST a high level request to the Icinga `objects/service` API
     (with less possibilities). The service name should be unique and has
     to be taken from the `__name` attribute.
 
     Example: Does a check show a warning and/or was acknowledged?
 
     >>> uri = 'https://icinga-server:5665'
@@ -87,20 +88,22 @@
     }
     return api_post(
         uri=uri,
         username=username,
         password=password,
         data=data,
         method_override='GET',
-        insecure=True,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
 
 
-def set_ack(uri, username, password, objectname, _type='service',
-            author='Linuxfabrik lib.icinga'):
+def set_ack(uri, username, password, objectname, _type='service', author='Linuxfabrik lib.icinga',
+            insecure=False, no_proxy=False, timeout=3):
     """Allows you to acknowledge the current problem for hosts or
     services. By acknowledging the current problem, future notifications
     (for the same state if sticky is set to false) are disabled.  The
     host or service name should be unique and has to be taken from the
     `__name` attribute.
 
     Acknowledging an already acknowledged problem is ok until 2.11, while
@@ -117,22 +120,24 @@
         'notify': False,
     }
     return api_post(
         uri=uri,
         username=username,
         password=password,
         data=data,
-        insecure=True,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
 
 
 def set_downtime(uri, username, password, objectname, _type='service',
-                 starttime=int(time.time()),
-                 endtime=int(time.time())+60*60,
-                 author='Linuxfabrik lib.icinga'):
+                 starttime=int(time.time()), endtime=int(time.time())+60*60,
+                 author='Linuxfabrik lib.icinga',
+                 insecure=False, no_proxy=False, timeout=3):
     """POST a high level request to the Icinga `actions/schedule-downtime
     API (with less possibilities). The host or service name should be
     unique and has to be taken from the `__name` attribute.
 
     You will get a downtime name, which you have to use if you want to
     use `remove_ack()` later on.
 
@@ -157,22 +162,25 @@
         'end_time': endtime,
     }
     success, result = api_post(
         uri=uri,
         username=username,
         password=password,
         data=data,
-        insecure=True,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
     if success and result['results'][0]['code'] == 200:
         return (True, result['results'][0]['name'])
     return (False, result)
 
 
-def remove_ack(uri, username, password, objectname, _type='service'):
+def remove_ack(uri, username, password, objectname, _type='service',
+               insecure=False, no_proxy=False, timeout=3):
     """Removes the acknowledgements for services or hosts. Once the
     acknowledgement has been removed the next notification will be sent
     again. Always returns ok.
 
     >>> uri = 'https://icinga-server:5665'
     >>> icinga.remove_ack(
     >>>     uri,
@@ -187,26 +195,31 @@
         'type': _type.capitalize(),
         'filter': 'match("{}", {}.__name)'.format(objectname, _type.lower()),
     }
     return api_post(uri=uri,
         username=username,
         password=password,
         data=data,
-        insecure=True,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
 
 
-def remove_downtime(uri, username, password, downtime):
+def remove_downtime(uri, username, password, downtime,
+                    insecure=False, no_proxy=False, timeout=3):
     """Remove the downtime using its name you got from `set_downtime()`.
     Always returns ok.
     """
 
     uri = uri + '/v1/actions/remove-downtime'
     data = {
         'downtime': downtime,
     }
     return api_post(uri=uri,
         username=username,
         password=password,
         data=data,
-        insecure=True,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
     )
```

### Comparing `linuxfabrik-lib-2023051201.post1/jitsi.py` & `linuxfabrik_lib-2024052901/jitsi.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some Jitsi related functions that are
 needed by more than one Jitsi plugin."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031401'
 
 import base64 # pylint: disable=C0413
 
 from . import url
 
 
 def get_data(args, _type='json'):
@@ -29,22 +29,24 @@
             base64.b64encode(args.USERNAME + ':' + args.PASSWORD)
         )
     if _type == 'json':
         success, result = url.fetch_json(
             args.URL,
             extended=True,
             header=header,
-            insecure=True,
+            insecure=args.INSECURE,
+            no_proxy=args.NO_PROXY,
             timeout=args.TIMEOUT,
         )
     else:
         success, result = url.fetch(
             args.URL,
             extended=True,
             header=header,
-            insecure=True,
+            insecure=args.INSECURE,
+            no_proxy=args.NO_PROXY,
             timeout=args.TIMEOUT,
         )
 
     if not success:
         return (success, result, False)
     return (True, result)
```

### Comparing `linuxfabrik-lib-2023051201.post1/librenms.py` & `linuxfabrik_lib-2024052901/librenms.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some LibreNMS related functions that are
 needed by LibreNMS check plugins."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024032902'
 
 from .globals import STATE_CRIT, STATE_OK, STATE_UNKNOWN, STATE_WARN
 
 from . import base # pylint: disable=C0413
 from . import txt # pylint: disable=C0413
 from . import url # pylint: disable=C0413
 
 
 def get_data(args, uri=''):
+    if args.URL.endswith('/'):
+        args.URL = args.URL[:-1]
+    if not uri.startswith('/'):
+        uri = '/' + uri
     uri = '{}{}'.format(args.URL, uri)
     header = {'X-Auth-Token': args.TOKEN}
     result = base.coe(url.fetch_json(
         uri,
         header=header,
         insecure=args.INSECURE,
         no_proxy=args.NO_PROXY,
@@ -49,15 +53,20 @@
         return ''
     if prop in obj:
         if obj[prop] is not None:
             return obj[prop]
     return None
 
 
-def get_state(librestate):
-    if librestate == 'ok':
+def get_state(librestate, severity='crit'):
+    """Translate LibreNMS' state to the Nagios world.
+    0 = ok, 1 = alert, 2 = ack
+    """
+    if not librestate: # including NULL
         return STATE_OK
-    if librestate == 'warning':
+    if librestate == 1:
+        if severity == 'crit':
+            return STATE_CRIT
         return STATE_WARN
-    if librestate == 'critical':
-        return STATE_CRIT
+    if librestate == 2:
+        return STATE_OK
     return STATE_UNKNOWN
```

### Comparing `linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/PKG-INFO` & `linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxfabrik-lib
-Version: 2023051201.post1
+Version: 2024052901
 Summary: Python libraries used in various Linuxfabrik projects, including the 'Linuxfabrik Monitoring Plugins' project.
 Author-email: "Linuxfabrik GmbH, Zurich, Switzerland" <info@linuxfabrik.ch>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -52,48 +52,141 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
+Requires-Dist: netifaces
+Requires-Dist: psutil
+Requires-Dist: pymysql
+Requires-Dist: pysmbclient
+Requires-Dist: python-keystoneclient
+Requires-Dist: python-novaclient
+Requires-Dist: python-swiftclient
+Requires-Dist: pywinrm
+Requires-Dist: requests
+Requires-Dist: smbprotocol
+Requires-Dist: vici
+Requires-Dist: xmltodict
 
 # Linuxfabrik's Python Libraries
 
 These Python libraries are used in various projects of Linuxfabrik, including the [Linuxfabrik Monitoring Plugins project](https://github.com/Linuxfabrik/monitoring-plugins).
 
-List of libraries:
 
-* args.py: Extends argparse by new input argument data types on demand.
-* base.py: Provides very common every-day functions.
-* cache.py: Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
-* db_mysql.py: Library for accessing MySQL/MariaDB servers.
-* db_sqlite.py: Library for accessing SQLite databases.
-* disk.py: Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
-* distro.py: Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
-* dmidecode.py: Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
-* endoflifedate.py: This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
-* feedparser.py: Parse Atom and RSS feeds in Python.
-* globals.py: This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
-* grassfish.py: Provides functions using the Grassfish REST-API.
-* huawei.py: This library collects some Huawei related functions that are needed by Huawei check plugins.
-* human.py: Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
-* icinga.py: This module tries to make accessing the Icinga2 API easier.
-* infomaniak.py: Provides functions using the Infomanik REST-API.
-* jitsi.py: This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
-* librenms.py: This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
-* net.py: Provides network related functions and variables.
-* nodebb.py: This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
-* powershell.py: This library collects some Microsoft PowerShell related functions.
-* psutil.py: Wrapper library for functions from psutil.
-* redfish.py: This library parses data returned from the Redfish API.
-* rocket.py: This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
-* shell.py: Communicates with the Shell.
-* smb.py: Provides functions to establish native SMB connections.
-* test.py: Provides test functions for unit tests.
-* time.py: Provides datetime functions.
-* txt.py: A collection of text functions.
-* url.py: Get for example HTML or JSON from an URL.
-* veeam.py: This library interacts with the Veeam Enterprise Manager API.
-* version.py: Provides functions for handling software versions.
-* wildfly.py: This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
-* winrm.py: This library collects some Microsoft WinRM related functions.
+## Installation
+
+`pip install linuxfabrik-lib`
+
+
+## Documentation
+
+For example by browsing http://localhost:8080/ after starting `pydoc -p 8080`.
+
+
+## List of libraries
+
+
+* args.py:  
+Extends argparse by new input argument data types on demand.
+
+* base.py:  
+Provides very common every-day functions.
+
+* cache.py:  
+Simple Cache in the form of a Key-Value Store (KVS) like Redis, based on SQLite, optionally supporting expiration of keys. No detailed error handling here. If the cache does not work, we (currently) don't report the reason and simply return `False`.
+
+* db_mysql.py:  
+Library for accessing MySQL/MariaDB servers.
+
+* db_sqlite.py:  
+Library for accessing SQLite databases.
+
+* disk.py:  
+Offers file and disk related functions, like getting a list of partitions, grepping a file, etc.
+
+* distro.py:  
+Provides information about the Linux distribution it runs on, such as a reliable machine-readable distro ID and "os_family" (known from Ansible).
+
+* dmidecode.py:  
+Library for parsing information from dmidecode. Have a look at `man dmidecode` for details about dmidecode.
+
+* endoflifedate.py:  
+This library stores information from https://endoflife.date/api/ for offline usage and therefore needs to be updated periodically when version checks don't have access to the Internet.
+
+* feedparser.py:  
+Parse Atom and RSS feeds in Python.
+
+* globals.py:  
+This library defines the global plugin states, based on the POSIX spec of returning a positive value and just like in `monitoring-plugins/plugins-scripts/utils.sh.in`, except that we do not make use of `STATE_DEPENDENT`.
+
+* grassfish.py:  
+Provides functions using the Grassfish REST-API.
+
+* huawei.py:  
+This library collects some Huawei related functions that are needed by Huawei check plugins.
+
+* human.py:  
+Functions to convert raw numbers, times etc. to a human readable representation (and sometimes back).
+
+* icinga.py:  
+This module tries to make accessing the Icinga2 API easier.
+
+* infomaniak.py:  
+Provides functions using the Infomanik REST-API.
+
+* jitsi.py:  
+This library collects some Jitsi related functions that are needed by more than one Jitsi plugin.
+
+* librenms.py:  
+This library collects some LibreNMS related functions that are needed by LibreNMS check plugins.
+
+* net.py:  
+Provides network related functions and variables.
+
+* nodebb.py:  
+This library collects some NodeBB related functions that are needed by more than one NodeBB plugin.
+
+* powershell.py:  
+This library collects some Microsoft PowerShell related functions.
+
+* psutil.py:  
+Wrapper library for functions from psutil.
+
+* redfish.py:  
+This library parses data returned from the Redfish API.
+
+* rocket.py:  
+This library collects some Rocket.Chat related functions that are needed by more than one Rocket.Chat plugin.
+
+* shell.py:  
+Communicates with the Shell.
+
+* smb.py:  
+Provides functions to establish native SMB connections.
+
+* test.py:  
+Provides test functions for unit tests.
+
+* time.py:  
+Provides datetime functions.
+
+* txt.py:  
+A collection of text functions.
+
+* url.py:  
+Get for example HTML or JSON from an URL.
+
+* veeam.py:  
+This library interacts with the Veeam Enterprise Manager API.
+
+* version.py:  
+Provides functions for handling software versions.
+
+* wildfly.py:  
+This library collects some WildFly/JBoss related functions that are needed by more than one WildFly/JBoss plugin.
+
+* winrm.py:  
+This library collects some Microsoft WinRM related functions.
```

### Comparing `linuxfabrik-lib-2023051201.post1/linuxfabrik_lib.egg-info/SOURCES.txt` & `linuxfabrik_lib-2024052901/linuxfabrik_lib.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ./infomaniak.py
 ./jitsi.py
 ./librenms.py
 ./net.py
 ./nodebb.py
 ./powershell.py
 ./psutil.py
+./qts.py
 ./redfish.py
 ./rocket.py
 ./shell.py
 ./smb.py
 ./test.py
 ./time.py
 ./txt.py
```

### Comparing `linuxfabrik-lib-2023051201.post1/net.py` & `linuxfabrik_lib-2024052901/net.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 
 """Provides network related functions and variables.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024041001'
 
 import random
 import re
 import socket
 try:
     import netifaces
     HAVE_NETIFACES = True
@@ -193,15 +193,15 @@
         try:
             stats['public_address'] = get_ip_public()
         except:
             return []
         return stats
 
 
-def get_public_ip(services):
+def get_public_ip(services, insecure=False, no_proxy=False, timeout=2):
     """Retrieve the public IP address from a list of online services.
     The list of "what is my ip" services is shuffled before being used. The first service
     returning an IP "wins".
 
     >>> get_public_ip('https://ipv4.icanhazip.com,https://ipecho.net/plain,https://ipinfo.io/ip')
     1.2.3.4
     """
@@ -209,24 +209,40 @@
         return (False, None)
 
     services = services.split(',')
     random.shuffle(services)
 
     ip = None
     for uri in services:
-        success, ip = url.fetch(uri.strip(), timeout=2)
+        success, ip = url.fetch(
+            uri.strip(),
+            insecure=insecure,
+            no_proxy=no_proxy,
+            timeout=timeout,
+        )
         if success and ip:
             ip = ip.strip()
             try:
                 return (True, txt.to_text(ip))
             except:
                 return (True, ip)
     return (False, ip)
 
 
+def ip_to_cidr(ip):
+    """Convert IP address to CIDR.
+    Example: '255.255.255.0' will return 24
+    """
+    # Thanks to @Atticfire
+    # See https://github.com/nicolargo/glances/issues/1417#issuecomment-469894399
+    if ip is None:
+        return 0
+    return sum(bin(int(x)).count('1') for x in ip.split('.'))
+
+
 def is_valid_hostname(hostname):
     """True for a validated fully-qualified domain name (FQDN), in full
     compliance with RFC 1035, and the "preferred form" specified in RFC
     3686 s. 2, whether relative or absolute.
 
     If and only if the FQDN ends with a dot (in place of the RFC1035
     trailing null byte), it may have a total length of 254 bytes, still it
```

### Comparing `linuxfabrik-lib-2023051201.post1/nodebb.py` & `linuxfabrik_lib-2024052901/nodebb.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some NodeBB related functions that are
 needed by more than one NodeBB plugin."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031401'
 
 from . import base
 from . import url
 
 
 def get_data(args, uri=''):
     """Fetch json from the NodeBB API using an user token. For details have a look at
     https://docs.nodebb.org/api/
     """
     return base.coe(url.fetch_json(
         args.URL + uri,
-        insecure=args.INSECURE,
-        timeout=args.TIMEOUT,
         header={
             'Accept': 'application/json',
             'Authorization': 'Bearer {}'.format(args.TOKEN),
         },
+        insecure=args.INSECURE,
+        no_proxy=args.NO_PROXY,
+        timeout=args.TIMEOUT,
     ))
```

### Comparing `linuxfabrik-lib-2023051201.post1/powershell.py` & `linuxfabrik_lib-2024052901/powershell.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some Microsoft PowerShell related functions.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 import subprocess
 
 from . import txt
 
 
 def run_ps(cmd):
```

### Comparing `linuxfabrik-lib-2023051201.post1/psutil.py` & `linuxfabrik_lib-2024052901/psutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Wrapper library for functions from psutil.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 import sys
 
 from .globals import STATE_UNKNOWN
 try:
     import psutil
 except ImportError as e:
```

### Comparing `linuxfabrik-lib-2023051201.post1/pyproject.toml` & `linuxfabrik_lib-2024052901/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # In setuptools before version 61.0.0 there is no support for writing the
 # project's packaging metadata in pyproject.toml
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linuxfabrik-lib"
-version = "2023051201-1"
+version = "2024052901"
 description = "Python libraries used in various Linuxfabrik projects, including the 'Linuxfabrik Monitoring Plugins' project."
 readme = "README.md"
 authors = [
     { name = "Linuxfabrik GmbH, Zurich, Switzerland", email = "info@linuxfabrik.ch" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `linuxfabrik-lib-2023051201.post1/redfish.py` & `linuxfabrik_lib-2024052901/redfish.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library parses data returned from the Redfish API.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 from . import base
 from . import human
 from .globals import STATE_OK, STATE_WARN, STATE_CRIT
 
 
 # The "Status" property is common to many Redfish schema, and contains:
```

### Comparing `linuxfabrik-lib-2023051201.post1/rocket.py` & `linuxfabrik_lib-2024052901/rocket.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,63 +8,75 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some Rocket.Chat related functions that are
 needed by more than one Rocket.Chat plugin."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031501'
 
 from . import url
 
 
-def get_token(rc_url, user, password):
+def get_token(rc_url, user, password, insecure=False, no_proxy=False, timeout=3):
     """Gets an API token from Rocket.Chat, using your credentials.
     Equivalent to:
 
     $ curl -X "POST" \\
     $      -d "user=admin&password=mypassword" \\
     $      http://localhost:3000/api/v1/login
     """
 
     if not rc_url.endswith('/login'):
         rc_url += '/login'
     data = {
         'user': user,
         'password': password,
-        }
+    }
 
-    success, result = url.fetch_json(rc_url, data=data)
+    success, result = url.fetch_json(
+        rc_url,
+        data=data,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
+    )
     if not success:
         return (success, result)
     if not result:
         return (False, 'There was no result from {}.'.format(rc_url))
 
     if not 'authToken' in result['data']:
         return (False, 'Something went wrong, maybe user is unauthorized.')
     return (True, result['data']['authToken'] + ':' + result['data']['userId'])
 
 
-def get_stats(rc_url, auth_token, user_id):
+def get_stats(rc_url, auth_token, user_id, insecure=False, no_proxy=False, timeout=3):
     """Calls api/v1/statistics. You need to get a token using
     `get_token()` first. Equivalent to:
 
     $ https://rocket.chat/docs/developer-guides/rest-api/miscellaneous/statistics/
     $ curl -H "X-Auth-Token: 8h2mKAwxB3AQrFSjLVKMooJyjdCFaA7W45sWlHP8IzO" \\
     $      -H "X-User-Id: ew28DpvKw3R" \\
     $      http://localhost:3000/api/v1/statistics
     """
 
     if not rc_url.endswith('/statistics'):
         rc_url += '/statistics'
     header = {
         'X-Auth-Token': auth_token,
         'X-User-Id': user_id,
-        }
+    }
 
-    success, result = url.fetch_json(rc_url, header=header)
+    success, result = url.fetch_json(
+        rc_url,
+        header=header,
+        insecure=insecure,
+        no_proxy=no_proxy,
+        timeout=timeout,
+    )
     if not success:
         return (success, result)
     if not result:
         return (False, 'There was no result from {}.'.format(rc_url))
 
     return (True, result)
```

### Comparing `linuxfabrik-lib-2023051201.post1/shell.py` & `linuxfabrik_lib-2024052901/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Communicates with the Shell.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 
 import os
 import re
 import shlex
 import subprocess
 
@@ -99,14 +99,17 @@
             True:  result[1] contains the result of the called `cmd`
                    as a tuple (stdout, stderr, retc)
 
     https://docs.python.org/2/library/subprocess.html
     """
     if not env:
         env = os.environ.copy()
+    else:
+        # merge the OS environment variables with the ones set by the env parameter
+        env = {**os.environ.copy(), **env}
     # set cmd output to English, no matter what the user has choosen
     env['LC_ALL'] = 'C'
 
     # subprocess.PIPE: Special value that can be used as the stdin,
     # stdout or stderr argument to Popen and indicates that a pipe to
     # the standard stream should be opened.
     if shell or stdin:
@@ -116,15 +119,15 @@
         try:
             p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
                                   stderr=subprocess.PIPE, env=env, shell=True, cwd=cwd)
         except OSError as e:
             return (False, 'OS Error "{} {}" calling command "{}"'.format(e.errno, e.strerror, cmd))
         except ValueError as e:
             return (False, 'Value Error "{}" calling command "{}"'.format(e, cmd))
-        except e:
+        except Exception as e:
             return (False, 'Unknown error "{}" while calling command "{}"'.format(e, cmd))
 
         if stdin:
             # provide stdin as input for the cmd
             stdout, stderr = p.communicate(input=txt.to_bytes(stdin))
         else:
             stdout, stderr = p.communicate()
@@ -145,15 +148,15 @@
             stdin = p.stdout if p else subprocess.PIPE
             p = subprocess.Popen(args, stdin=stdin, stdout=subprocess.PIPE,
                                   stderr=subprocess.PIPE, env=env, shell=False, cwd=cwd)
         except OSError as e:
             return (False, 'OS Error "{} {}" calling command "{}"'.format(e.errno, e.strerror, cmd))
         except ValueError as e:
             return (False, 'Value Error "{}" calling command "{}"'.format(e, cmd))
-        except e:
+        except Exception as e:
             return (False, 'Unknown error "{}" while calling command "{}"'.format(e, cmd))
 
     try:
         stdout, stderr = p.communicate(timeout=timeout)
     except subprocess.TimeoutExpired:
         p.kill()
         outs, errs = p.communicate()
```

### Comparing `linuxfabrik-lib-2023051201.post1/smb.py` & `linuxfabrik_lib-2024052901/smb.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Provides functions to establish native SMB connections.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 import sys
 
 from .globals import STATE_UNKNOWN
 import smbclient
 import smbprotocol.exceptions
```

### Comparing `linuxfabrik-lib-2023051201.post1/test.py` & `linuxfabrik_lib-2024052901/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import os
 
 from . import disk
 
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 
 def test(args):
     """Returns the content of two files as well as the provided return code. The first file stands
     for STDOUT, the second for STDERR. The function can be used to enable unit tests.
 
     >>> test('path/to/stdout.txt', 'path/to/stderr.txt', 128)
```

### Comparing `linuxfabrik-lib-2023051201.post1/time.py` & `linuxfabrik_lib-2024052901/time.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """Provides datetime functions.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024032101'
 
 import datetime
 import time
 
 
 def epoch2iso(timestamp):
     """Returns the ISO representaton of a UNIX timestamp (epoch).
@@ -28,27 +28,27 @@
     return time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(timestamp))
 
 
 def now(as_type=''):
     """Returns the current date and time as UNIX time in seconds (default), or
     as a datetime object.
 
-    lib.base.now()
+    lib.time.now()
     >>> 1586422786
 
-    lib.base.now(as_type='float')
+    lib.time.now(as_type='float')
     >>> 1586422786.1521912
 
-    lib.base.now(as_type='epoch')
+    lib.time.now(as_type='epoch')
     >>> 1586422786
 
-    lib.base.now(as_type='datetime')
+    lib.time.now(as_type='datetime')
     >>> datetime.datetime(2020, 4, 9, 11, 1, 41, 228752)
 
-    lib.base.now(as_type='iso')
+    lib.time.now(as_type='iso')
     >>> '2020-04-09 11:31:24'
     """
     if as_type == 'datetime':
         return datetime.datetime.now()
     if as_type == 'iso':
         return time.strftime("%Y-%m-%d %H:%M:%S")
     if as_type == 'float':
```

### Comparing `linuxfabrik-lib-2023051201.post1/txt.py` & `linuxfabrik_lib-2024052901/txt.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 """A collection of text functions.
 
 The functions "to_text()" and "to_bytes()" are copied from
 /usr/lib/python3.10/site-packages/ansible/module_utils/_text.py (BSD license).
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024033101'
 
 import codecs
+import re
 try:
     codecs.lookup_error('surrogateescape')
     HAS_SURROGATEESCAPE = True
 except LookupError:
     HAS_SURROGATEESCAPE = False
 import operator
 
@@ -32,14 +33,37 @@
 binary_type = bytes
 
 _COMPOSED_ERROR_HANDLERS = frozenset((None, 'surrogate_or_replace',
                                       'surrogate_or_strict',
                                       'surrogate_then_replace'))
 
 
+def compile_regex(regex, key=''):
+    """Return a compiled regex from a string or list.
+    Optionally, add a key qualifier/string to help identify the regex in case of an error.
+    """
+
+    def cr(regex, key=''):
+        """Return a compiled regex from a string.
+        """
+        try:
+            return (True, re.compile(regex))
+        except re.error as e:
+            return (False, '`{}`{} contains one or more errors: {}'.format(
+                regex,
+                ' ({})'.format(key) if key else '',
+                e,
+            ))
+
+    if isinstance(regex, str):
+        return cr(regex, key=key)
+    else:
+        return [cr(item, key=key) for item in regex]
+
+
 def extract_str(s, from_txt, to_txt, include_fromto=False, be_tolerant=True):
     """Extracts text between `from_txt` to `to_txt`.
     If `include_fromto` is set to False (default), text is returned without both search terms,
     otherwise `from_txt` and `to_txt` are included.
     If `from_txt` is not found, always an empty string is returned.
     If `to_txt` is not found and `be_tolerant` is set to True (default), text is returned from
     `from_txt` til the end of input text. Otherwise an empty text is returned.
@@ -106,14 +130,28 @@
     filtered_input = ''
     for line in _input.splitlines():
         if not any(i_line in line for i_line in ignore):
             filtered_input += line + '\n'
     return filtered_input
 
 
+def match_regex(regex, string, key=''):
+    """Match a regex on a string.
+    Optionally, add a key qualifier/string to help identify the regex in case of an error.
+    """
+    try:
+        return (True, re.match(regex, string))
+    except re.error as e:
+        return (False, '`{}` contains one or more errors: {}'.format(
+            regex,
+            ' ({})'.format(key) if key else '',
+            e,
+        ))
+
+
 def mltext2array(_input, skip_header=False, sort_key=-1):
     """
     >>> s = '1662130953 timedatex\n1662130757 python3-pip-wheel\n1662130975 python3-dateutil\n'
     >>> mltext2array(s, skip_header=False, sort_key=0)
     [['1662130757', 'python3-pip-wheel'], ['1662130953', 'timedatex'], ['1662130975', 'python3-dateutil']]
     >>> mltext2array(s, skip_header=False, sort_key=1)
     [['1662130975', 'python3-dateutil'], ['1662130757', 'python3-pip-wheel'], ['1662130953', 'timedatex']]
```

### Comparing `linuxfabrik-lib-2023051201.post1/veeam.py` & `linuxfabrik_lib-2024052901/veeam.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library interacts with the Veeam Enterprise Manager API.
 Credits go to https://github.com/surfer190/veeam/blob/master/veeam/client.py."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031501'
 
 import base64
 
 from . import txt
 from . import url
 
 
@@ -40,17 +40,18 @@
     header['Content-Length'] = 0
     # make this a POST request by filling data with anything
     data = {'make-this': 'a-post-request'}
     success, result = url.fetch_json(
         uri,
         header=header,
         data=data,
-        timeout=args.TIMEOUT,
-        insecure=True,
         extended=True,
+        insecure=args.INSECURE,
+        no_proxy=args.NO_PROXY,
+        timeout=args.TIMEOUT,
     )
     if not success:
         return (success, result)
     if not result:
         return (False, 'There was no result from {}.'.format(uri))
     # In Python 3, getheader() should be get()
     result['X-RestSvcSessionId'] = result.get('response_header').get('X-RestSvcSessionId')
```

### Comparing `linuxfabrik-lib-2023051201.post1/wildfly.py` & `linuxfabrik_lib-2024052901/wildfly.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,37 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some WildFly/JBoss related functions that are
 needed by more than one WildFly/JBoss plugin."""
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2024031501'
 
 from . import base
 from . import url
 from .globals import STATE_UNKNOWN
 
 
 def get_data(args, data, uri=''):
     uri = args.URL + '/management' + uri
     if args.MODE == 'domain':
         uri = '{}/host/{}/server/{}'.format(uri, args.NODE, args.INSTANCE)
     header = {'Content-Type': 'application/json'}
     result = base.coe(url.fetch_json(
-        uri, timeout=args.TIMEOUT,
-        header=header, data=data,
-        digest_auth_user=args.USERNAME, digest_auth_password=args.PASSWORD,
-        encoding='serialized-json'
+        uri,
+        data=data,
+        digest_auth_password=args.PASSWORD,
+        digest_auth_user=args.USERNAME,
+        encoding='serialized-json',
+        header=header,
+        insecure=args.INSECURE,
+        no_proxy=args.NO_PROXY,
+        timeout=args.TIMEOUT,
     ))
     if result['outcome'] != 'success':
-        base.oao('Error fetching data: "{}"'.format(result), STATE_UNKNOWN, always_ok=args.ALWAYS_OK)
+        base.oao(
+            'Error fetching data: "{}"'.format(result),
+            STATE_UNKNOWN,
+            always_ok=args.ALWAYS_OK,
+        )
     return result['result']
```

### Comparing `linuxfabrik-lib-2023051201.post1/winrm.py` & `linuxfabrik_lib-2024052901/winrm.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # https://github.com/Linuxfabrik/monitoring-plugins/blob/main/CONTRIBUTING.rst
 
 """This library collects some Microsoft WinRM related functions.
 """
 
 __author__ = 'Linuxfabrik GmbH, Zurich/Switzerland'
-__version__ = '2023051201'
+__version__ = '2023112901'
 
 try:
     import winrm
     HAVE_WINRM = True
 except ImportError:
     HAVE_WINRM = False
```

