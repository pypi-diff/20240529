# Comparing `tmp/3way-1.2.1.tar.gz` & `tmp/3way-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3way-1.2.1.tar", last modified: Mon May 27 12:05:37 2024, max compression
+gzip compressed data, was "3way-1.2.2.tar", last modified: Wed May 29 14:39:30 2024, max compression
```

## Comparing `3way-1.2.1.tar` & `3way-1.2.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.737558 3way-1.2.1/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.581558 3way-1.2.1/.github/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.637558 3way-1.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 kali      (1000) kali      (1000)      368 2024-05-27 00:00:00.000000 3way-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 kali      (1000) kali      (1000)      324 2024-05-27 00:00:00.000000 3way-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.653558 3way-1.2.1/3way.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     7618 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      836 2024-05-27 12:05:37.000000 3way-1.2.1/3way.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-27 12:05:34.000000 3way-1.2.1/3way.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    21165 2024-05-27 10:57:51.000000 3way-1.2.1/Freeway
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.693558 3way-1.2.1/FreewayTools/
--rw-r--r--   0 kali      (1000) kali      (1000)      570 2024-05-27 10:34:51.000000 3way-1.2.1/FreewayTools/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)    20007 2024-05-27 11:00:13.000000 3way-1.2.1/FreewayTools/audit.py
--rw-r--r--   0 kali      (1000) kali      (1000)    13348 2024-05-27 10:59:24.000000 3way-1.2.1/FreewayTools/beacon_spam.py
--rw-r--r--   0 kali      (1000) kali      (1000)      739 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/checkmac.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1634 2024-05-24 20:28:12.000000 3way-1.2.1/FreewayTools/colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19102 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/deauth.py
--rw-r--r--   0 kali      (1000) kali      (1000)    20583 2024-05-27 11:12:12.000000 3way-1.2.1/FreewayTools/evil_twin.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11726 2024-05-20 16:16:19.000000 3way-1.2.1/FreewayTools/fuzzer.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2056 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/hopper.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.697558 3way-1.2.1/FreewayTools/lists/
--rw-r--r--   0 kali      (1000) kali      (1000)    10865 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/lists/ssid_list.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    27655 2024-05-20 13:21:18.000000 3way-1.2.1/FreewayTools/monitor.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1384 2024-05-27 12:04:49.000000 3way-1.2.1/FreewayTools/updater.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1063 2024-05-27 11:22:15.000000 3way-1.2.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     7618 2024-05-27 12:05:37.737558 3way-1.2.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     7392 2024-05-27 12:02:23.000000 3way-1.2.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-05-20 13:21:18.000000 3way-1.2.1/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-27 12:05:37.737558 3way-1.2.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1779 2024-05-27 12:04:41.000000 3way-1.2.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.613558 3way-1.2.1/templates/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.705558 3way-1.2.1/templates/Valentines/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 21:25:53.000000 3way-1.2.1/templates/Valentines/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3585 2024-05-24 21:26:16.000000 3way-1.2.1/templates/Valentines/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.713558 3way-1.2.1/templates/google/
--rw-r--r--   0 kali      (1000) kali      (1000)       68 2024-05-23 21:57:13.000000 3way-1.2.1/templates/google/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)    13219 2024-05-25 14:16:01.000000 3way-1.2.1/templates/google/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.717558 3way-1.2.1/templates/mcd/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 16:00:34.000000 3way-1.2.1/templates/mcd/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     3813 2024-05-25 14:16:01.000000 3way-1.2.1/templates/mcd/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.725558 3way-1.2.1/templates/mrhacker/
--rw-r--r--   0 kali      (1000) kali      (1000)      224 2024-05-24 20:43:05.000000 3way-1.2.1/templates/mrhacker/action.html
--rw-r--r--   0 kali      (1000) kali      (1000)     6536 2024-05-25 14:16:01.000000 3way-1.2.1/templates/mrhacker/index.html
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-27 12:05:37.729558 3way-1.2.1/templates/mrhacker/static/
--rw-r--r--   0 kali      (1000) kali      (1000)    31471 2024-05-24 21:06:33.000000 3way-1.2.1/templates/mrhacker/static/mrhacker.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.565661 3way-1.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.413661 3way-1.2.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.457661 3way-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-27 12:11:30.000000 3way-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-27 12:11:30.000000 3way-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.473661 3way-1.2.2/3way.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7904 2024-05-29 14:39:29.000000 3way-1.2.2/3way.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-29 14:39:30.000000 3way-1.2.2/3way.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:39:29.000000 3way-1.2.2/3way.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-29 14:39:29.000000 3way-1.2.2/3way.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-29 14:39:29.000000 3way-1.2.2/3way.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    21165 2024-05-27 12:11:30.000000 3way-1.2.2/Freeway
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.521661 3way-1.2.2/FreewayTools/
+-rw-r--r--   0 root         (0) root         (0)      570 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20007 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/audit.py
+-rw-r--r--   0 root         (0) root         (0)    13348 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/beacon_spam.py
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/checkmac.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    19102 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/deauth.py
+-rw-r--r--   0 root         (0) root         (0)    20583 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/evil_twin.py
+-rw-r--r--   0 root         (0) root         (0)    11726 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/fuzzer.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/hopper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.525661 3way-1.2.2/FreewayTools/lists/
+-rw-r--r--   0 root         (0) root         (0)    10865 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/lists/ssid_list.txt
+-rw-r--r--   0 root         (0) root         (0)    27655 2024-05-27 12:11:30.000000 3way-1.2.2/FreewayTools/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2024-05-29 14:31:46.000000 3way-1.2.2/FreewayTools/updater.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-27 12:11:30.000000 3way-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-29 14:28:35.000000 3way-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7904 2024-05-29 14:39:30.565661 3way-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7678 2024-05-29 12:25:30.000000 3way-1.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 12:11:30.000000 3way-1.2.2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 14:39:30.565661 3way-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-05-29 14:31:42.000000 3way-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.429661 3way-1.2.2/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.533661 3way-1.2.2/templates/Valentines/
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-27 12:11:30.000000 3way-1.2.2/templates/Valentines/action.html
+-rw-r--r--   0 root         (0) root         (0)     3585 2024-05-27 12:11:30.000000 3way-1.2.2/templates/Valentines/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.541661 3way-1.2.2/templates/google/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-27 12:11:30.000000 3way-1.2.2/templates/google/action.html
+-rw-r--r--   0 root         (0) root         (0)    13219 2024-05-27 12:11:30.000000 3way-1.2.2/templates/google/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.549661 3way-1.2.2/templates/mcd/
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-27 12:11:30.000000 3way-1.2.2/templates/mcd/action.html
+-rw-r--r--   0 root         (0) root         (0)     3813 2024-05-27 12:11:30.000000 3way-1.2.2/templates/mcd/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.557660 3way-1.2.2/templates/mrhacker/
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-27 12:11:30.000000 3way-1.2.2/templates/mrhacker/action.html
+-rw-r--r--   0 root         (0) root         (0)     6536 2024-05-27 12:11:30.000000 3way-1.2.2/templates/mrhacker/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:30.557660 3way-1.2.2/templates/mrhacker/static/
+-rw-r--r--   0 root         (0) root         (0)    31471 2024-05-27 12:11:30.000000 3way-1.2.2/templates/mrhacker/static/mrhacker.png
```

### Comparing `3way-1.2.1/3way.egg-info/PKG-INFO` & `3way-1.2.2/3way.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3way
-Version: 1.2.1
+Version: 1.2.2
 Summary: Freeway for network pentesting
 Home-page: https://github.com/FLOCK4H/Freeway
 Author: FLOCK4H
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -172,17 +172,26 @@
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
 
+> 27.05
+> 1. Added `updater.py`
+> 2. Added `evil_twin.py`
+> 3. Added `/templates` folder
+> 4. Added Evil Twin to actions list
+> 5. Updated README.md
+> 6. PyPi Release 
+
 <h2>Known Issues</h2>
 
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on Android 11+, versions below Android 11  and above Android 5 were not tested.)
+> 2. EvilTwin needs a second adapter connected to the internet (Not really an issue), to be able to reroute traffic 
 
 <h2><strong>Legal Note</strong></h2>
 
 > [!IMPORTANT]
 > Any malicious use of such features should be considered a crime, <br />
 > always assert permission to perform the penetration testing.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: 3way Version: 1.2.1 Summary: Freeway for network
+Metadata-Version: 2.1 Name: 3way Version: 1.2.2 Summary: Freeway for network
 pentesting Home-page: https://github.com/FLOCK4H/Freeway Author: FLOCK4H
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE
        [Freeway logo]$${\color{red}Freeway\ for\ Network\ Pentesting}$$
                  RReeaadd tthhee aarrttiiccllee aabboouutt FFrreeeewwaayy,, nnooww oonn _M_e_d_i_u_m
 
 > [!NOTE] > Before using the software, the user must agree to the EULA when
 prompted
@@ -105,18 +105,22 @@
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
 â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
-formatting in beacon_spam.py
+formatting in beacon_spam.py > 27.05 > 1. Added `updater.py` > 2. Added
+`evil_twin.py` > 3. Added `/templates` folder > 4. Added Evil Twin to actions
+list > 5. Updated README.md > 6. PyPi Release
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
-Android 11+, versions below Android 11 and above Android 5 were not tested.)
+Android 11+, versions below Android 11 and above Android 5 were not tested.) >
+2. EvilTwin needs a second adapter connected to the internet (Not really an
+issue), to be able to reroute traffic
 ********** LLeeggaall NNoottee **********
 > [!IMPORTANT] > Any malicious use of such features should be considered a
 crime,
 > always assert permission to perform the penetration testing.
 ********** LLiicceennssee **********
 The distribution of Freeway is regulated by the standard MIT license, users can
 feel free to use, share and contribute to the repository or report bugs.
```

### Comparing `3way-1.2.1/3way.egg-info/SOURCES.txt` & `3way-1.2.2/3way.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Freeway
 LICENSE
+MANIFEST.in
 README.md
 __init__.py
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 3way.egg-info/PKG-INFO
 3way.egg-info/SOURCES.txt
```

### Comparing `3way-1.2.1/Freeway` & `3way-1.2.2/Freeway`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/__init__.py` & `3way-1.2.2/FreewayTools/__init__.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/audit.py` & `3way-1.2.2/FreewayTools/audit.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/beacon_spam.py` & `3way-1.2.2/FreewayTools/beacon_spam.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/checkmac.py` & `3way-1.2.2/FreewayTools/checkmac.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/colors.py` & `3way-1.2.2/FreewayTools/colors.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/deauth.py` & `3way-1.2.2/FreewayTools/deauth.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/evil_twin.py` & `3way-1.2.2/FreewayTools/evil_twin.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/fuzzer.py` & `3way-1.2.2/FreewayTools/fuzzer.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/hopper.py` & `3way-1.2.2/FreewayTools/hopper.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/lists/ssid_list.txt` & `3way-1.2.2/FreewayTools/lists/ssid_list.txt`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/monitor.py` & `3way-1.2.2/FreewayTools/monitor.py`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/FreewayTools/updater.py` & `3way-1.2.2/FreewayTools/updater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import subprocess
 from FreewayTools.colors import *
-import time
+import time, os
 
 GITHUB_REPO = "FLOCK4H/Freeway"
 
 def get_latest_version():
     try:
         # This is an API created & hosted by github, not by me, 
         # it's the safest way of checking the most recent version of Freeway
@@ -17,30 +17,33 @@
         return latest_release["tag_name"]
     except ConnectionError:
         pass
     except Exception as e:
         wprint(str(e))
 
 def get_current_version():
-    return "1.2.1"
+    return "1.2.2"
 
 def update():
     cprint("Checking for updates..")
     
     current_version = get_current_version()
     latest_version = get_latest_version()
     if latest_version is None:
         wprint("You are not connected to any network, I can't fetch updates...")
         time.sleep(0.8)
         return
     
     if current_version != latest_version:
         cprint(f"New version available: {latest_version}")
         if cinput("Update Freeway? (y/n)") == "y":
-            subprocess.run(["git", "pull", "origin", "main"], check=True)
+            if os.path.exists("FreewayTools"):
+                subprocess.run(["git", "pull", "origin", "main"], check=True)
+            else:
+                subprocess.run(["sudo", "pip", "install", "--upgrade", "3way"])
             iprint("Update completed. Please restart Freeway.")
     else:
         iprint("You are using the latest version of Freeway.")
     time.sleep(0.8)
 
 if __name__ == "__main__":
-    update()
+    update()
```

### Comparing `3way-1.2.1/LICENSE` & `3way-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/PKG-INFO` & `3way-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 3way
-Version: 1.2.1
+Version: 1.2.2
 Summary: Freeway for network pentesting
 Home-page: https://github.com/FLOCK4H/Freeway
 Author: FLOCK4H
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -172,17 +172,26 @@
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
 
+> 27.05
+> 1. Added `updater.py`
+> 2. Added `evil_twin.py`
+> 3. Added `/templates` folder
+> 4. Added Evil Twin to actions list
+> 5. Updated README.md
+> 6. PyPi Release 
+
 <h2>Known Issues</h2>
 
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on Android 11+, versions below Android 11  and above Android 5 were not tested.)
+> 2. EvilTwin needs a second adapter connected to the internet (Not really an issue), to be able to reroute traffic 
 
 <h2><strong>Legal Note</strong></h2>
 
 > [!IMPORTANT]
 > Any malicious use of such features should be considered a crime, <br />
 > always assert permission to perform the penetration testing.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: 3way Version: 1.2.1 Summary: Freeway for network
+Metadata-Version: 2.1 Name: 3way Version: 1.2.2 Summary: Freeway for network
 pentesting Home-page: https://github.com/FLOCK4H/Freeway Author: FLOCK4H
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE
        [Freeway logo]$${\color{red}Freeway\ for\ Network\ Pentesting}$$
                  RReeaadd tthhee aarrttiiccllee aabboouutt FFrreeeewwaayy,, nnooww oonn _M_e_d_i_u_m
 
 > [!NOTE] > Before using the software, the user must agree to the EULA when
 prompted
@@ -105,18 +105,22 @@
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
 â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
-formatting in beacon_spam.py
+formatting in beacon_spam.py > 27.05 > 1. Added `updater.py` > 2. Added
+`evil_twin.py` > 3. Added `/templates` folder > 4. Added Evil Twin to actions
+list > 5. Updated README.md > 6. PyPi Release
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
-Android 11+, versions below Android 11 and above Android 5 were not tested.)
+Android 11+, versions below Android 11 and above Android 5 were not tested.) >
+2. EvilTwin needs a second adapter connected to the internet (Not really an
+issue), to be able to reroute traffic
 ********** LLeeggaall NNoottee **********
 > [!IMPORTANT] > Any malicious use of such features should be considered a
 crime,
 > always assert permission to perform the penetration testing.
 ********** LLiicceennssee **********
 The distribution of Freeway is regulated by the standard MIT license, users can
 feel free to use, share and contribute to the repository or report bugs.
```

### Comparing `3way-1.2.1/README.md` & `3way-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -162,17 +162,26 @@
 
 <h2>Changelog</h2>
 
 > 19.05
 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on dynamicly changing size dictionary
 > 2. Further improvements of beacon packet formatting in beacon_spam.py
 
+> 27.05
+> 1. Added `updater.py`
+> 2. Added `evil_twin.py`
+> 3. Added `/templates` folder
+> 4. Added Evil Twin to actions list
+> 5. Updated README.md
+> 6. PyPi Release 
+
 <h2>Known Issues</h2>
 
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on Android 11+, versions below Android 11  and above Android 5 were not tested.)
+> 2. EvilTwin needs a second adapter connected to the internet (Not really an issue), to be able to reroute traffic 
 
 <h2><strong>Legal Note</strong></h2>
 
 > [!IMPORTANT]
 > Any malicious use of such features should be considered a crime, <br />
 > always assert permission to perform the penetration testing.
```

#### html2text {}

```diff
@@ -102,18 +102,22 @@
 done on purpose to 'reserve' the name for the future official pip release as
 Freeway is taken.
 ********** TTOODDOO **********
 â Evil Twin attack â Version & update checker â PyPi Release
 ********** CChhaannggeelloogg **********
 > 19.05 > 1. Fixed rare RuntimeError in deauth.py caused by iterating on
 dynamicly changing size dictionary > 2. Further improvements of beacon packet
-formatting in beacon_spam.py
+formatting in beacon_spam.py > 27.05 > 1. Added `updater.py` > 2. Added
+`evil_twin.py` > 3. Added `/templates` folder > 4. Added Evil Twin to actions
+list > 5. Updated README.md > 6. PyPi Release
 ********** KKnnoowwnn IIssssuueess **********
 > 1. Android filters out fake beacon frames (works for Android 5, doesn't on
-Android 11+, versions below Android 11 and above Android 5 were not tested.)
+Android 11+, versions below Android 11 and above Android 5 were not tested.) >
+2. EvilTwin needs a second adapter connected to the internet (Not really an
+issue), to be able to reroute traffic
 ********** LLeeggaall NNoottee **********
 > [!IMPORTANT] > Any malicious use of such features should be considered a
 crime,
 > always assert permission to perform the penetration testing.
 ********** LLiicceennssee **********
 The distribution of Freeway is regulated by the standard MIT license, users can
 feel free to use, share and contribute to the repository or report bugs.
```

### Comparing `3way-1.2.1/setup.py` & `3way-1.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,22 +33,25 @@
                 shutil.copytree(f"{source}/{template}", f"{destination}/{template}")
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='3way',
-    version='1.2.1',
+    version='1.2.2',
     author='FLOCK4H',
     url='https://github.com/FLOCK4H/Freeway',
     description='Freeway for network pentesting',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
     install_requires=["scapy", "rich"],
-
     scripts=['Freeway'],
     cmdclass={
         'install': PostInstallCommand,
+    },
+    include_package_data=True,
+    package_data={
+        '': ['FreewayTools/lists/ssid_list.txt', 'templates/*'],
     }
 )
```

### Comparing `3way-1.2.1/templates/Valentines/index.html` & `3way-1.2.2/templates/Valentines/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/templates/google/index.html` & `3way-1.2.2/templates/google/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/templates/mcd/index.html` & `3way-1.2.2/templates/mcd/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/templates/mrhacker/index.html` & `3way-1.2.2/templates/mrhacker/index.html`

 * *Files identical despite different names*

### Comparing `3way-1.2.1/templates/mrhacker/static/mrhacker.png` & `3way-1.2.2/templates/mrhacker/static/mrhacker.png`

 * *Files identical despite different names*

