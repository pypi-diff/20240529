# Comparing `tmp/geopmdpy-3.0.1.tar.gz` & `tmp/geopmdpy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopmdpy-3.0.1.tar", last modified: Thu Dec  7 16:54:12 2023, max compression
+gzip compressed data, was "geopmdpy-3.1.0.tar", last modified: Wed May 29 18:29:41 2024, max compression
```

## Comparing `geopmdpy-3.0.1.tar` & `geopmdpy-3.1.0.tar`

### file list

```diff
@@ -1,31 +1,68 @@
-drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2023-12-07 16:54:12.837873 geopmdpy-3.0.1/
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1022 2023-11-07 21:40:27.000000 geopmdpy-3.0.1/AUTHORS
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1515 2023-11-07 21:40:27.000000 geopmdpy-3.0.1/COPYING
--rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)    13338 2023-12-07 16:54:12.837873 geopmdpy-3.0.1/PKG-INFO
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     9935 2023-11-07 22:03:25.000000 geopmdpy-3.0.1/README.rst
-drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2023-12-07 16:54:12.833873 geopmdpy-3.0.1/geopmdpy/
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      684 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/__init__.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1649 2023-11-16 00:07:13.000000 geopmdpy-3.0.1/geopmdpy/__main__.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    19558 2023-11-16 00:21:49.000000 geopmdpy-3.0.1/geopmdpy/access.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    25969 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/dbus_xml.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1875 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/error.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     2046 2023-11-08 01:32:20.000000 geopmdpy-3.0.1/geopmdpy/gffi.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5351 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/loop.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    26109 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/pio.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     3866 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/restorable_file_writer.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     2825 2023-12-07 16:33:57.000000 geopmdpy-3.0.1/geopmdpy/schemas.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    44022 2023-12-07 16:25:26.000000 geopmdpy-3.0.1/geopmdpy/service.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    11624 2023-12-05 23:59:22.000000 geopmdpy-3.0.1/geopmdpy/session.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1124 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/shmem.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    55405 2023-12-07 16:25:26.000000 geopmdpy-3.0.1/geopmdpy/system_files.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     8048 2023-10-20 16:44:46.000000 geopmdpy-3.0.1/geopmdpy/topo.py
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      114 2023-12-07 16:33:57.000000 geopmdpy-3.0.1/geopmdpy/version.py
-drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2023-12-07 16:54:12.837873 geopmdpy-3.0.1/geopmdpy.egg-info/
--rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)    13338 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/PKG-INFO
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      560 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/SOURCES.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        1 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/dependency_links.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      122 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/entry_points.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       78 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/requires.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        9 2023-12-07 16:54:12.000000 geopmdpy-3.0.1/geopmdpy.egg-info/top_level.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     2060 2023-12-07 16:50:20.000000 geopmdpy-3.0.1/pyproject.toml
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       38 2023-12-07 16:54:12.837873 geopmdpy-3.0.1/setup.cfg
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:29:41.461942 geopmdpy-3.1.0/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       96 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/.gitignore
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1101 2024-05-15 23:16:04.000000 geopmdpy-3.1.0/AUTHORS
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     3354 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5387 2024-05-21 00:55:39.000000 geopmdpy-3.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1527 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/LICENSE-BSD-3-Clause
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       24 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/MANIFEST.in
+-rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     5402 2024-05-29 18:29:41.461942 geopmdpy-3.1.0/PKG-INFO
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1862 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/README.md
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:29:41.453942 geopmdpy-3.1.0/debian/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      157 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/debian/changelog.in
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      775 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/debian/control
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5757 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/debian/copyright
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      119 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/debian/rules
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:29:41.457942 geopmdpy-3.1.0/geopmdpy/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        5 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy/VERSION
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      257 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/__init__.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1867 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/__main__.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    21632 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/access.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    25968 2024-05-21 17:46:17.000000 geopmdpy-3.1.0/geopmdpy/dbus_xml.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1874 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/error.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1676 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/gffi.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5350 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/loop.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    26108 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/pio.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     3865 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/restorable_file_writer.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     3536 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/schemas.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    45102 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/service.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    13576 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/session.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1123 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/shmem.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    55631 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/system_files.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     8047 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/topo.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      570 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/geopmdpy/version.py
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:29:41.461942 geopmdpy-3.1.0/geopmdpy.egg-info/
+-rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     5402 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/PKG-INFO
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1237 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        1 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      122 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/entry_points.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      142 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/requires.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        9 2024-05-29 18:29:41.000000 geopmdpy-3.1.0/geopmdpy.egg-info/top_level.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1591 2024-05-21 00:37:17.000000 geopmdpy-3.1.0/geopmdpy.spec.in
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      355 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/make_deb.sh
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      455 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/make_rpm.sh
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1287 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/make_sdist.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      146 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/make_sdist.sh
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     2356 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/pyproject.toml
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      197 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/requirements.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      353 2024-05-29 18:29:41.461942 geopmdpy-3.1.0/setup.cfg
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      461 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/setup.py
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:29:41.461942 geopmdpy-3.1.0/test/
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    17558 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestAccess.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    18874 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestAccessLists.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    39004 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestActiveSessions.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     3699 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestConfigPath.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     1172 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestDBusXML.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     2003 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestError.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      980 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestMSRDataFiles.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     1908 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestPIO.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    24860 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestPlatformService.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     2958 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestRequestQueue.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     5710 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestRestorableFileWriter.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    28448 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestSecureFiles.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     8894 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestSession.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     2559 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestTimedLoop.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     1711 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestTopo.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     4786 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/TestWriteLock.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       90 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/__init__.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      516 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/__main__.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      747 2024-05-15 17:46:43.000000 geopmdpy-3.1.0/test/geopmdpy_test.sh
```

### Comparing `geopmdpy-3.0.1/AUTHORS` & `geopmdpy-3.1.0/AUTHORS`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Steve Sylvester <steve.s.sylvester@intel.com>
 Christopher Cantalupo <christopher.m.cantalupo@intel.com>
 Jonathan Eastep <jonathan.m.eastep@intel.com>
-Stephanie Labasan <stephanie.labasan@intel.com>
+Stephanie Brink <brink2@llnl.gov>
 Brad Geltz <brad.geltz@intel.com>
 Baker Brandon <brandon.baker@intel.com>
 Diana Guttman <diana.r.guttman@intel.com>
 Daniel Wilson <daniel1.wilson@intel.com>
 Lowren Lawson <lowren.h.lawson@intel.com>
 Ali Mohammad <ali.mohammad@intel.com>
 Fuat Keceli <fuat.keceli@intel.com>
@@ -18,7 +18,9 @@
 Matthias Maiterth <matthias.maiterth@intel.com>
 Ethan Brown <ethan.w.brown@gmail.com>
 Aniruddha Marathe <marathe1@llnl.gov>
 Ben Allen <bsallen@alcf.anl.gov>
 Christian Wassermann <christian_wassermann@web.de>
 Reese Baird <reese.baird@intel.com>
 Kelly A. Livingston <kelly.a.livingston@intel.com>
+Siddhartha Jana <siddhartha.jana@intel.com>
+Taylor Jackle Spriggs <taylor.spriggs@intel.com>
```

### Comparing `geopmdpy-3.0.1/COPYING` & `geopmdpy-3.1.0/LICENSE-BSD-3-Clause`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-Copyright (c) 2015 - 2023, Intel Corporation
+Copyright (c) 2015 - 2024 Intel Corporation
 
 Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions
-are met:
+modification, are permitted provided that the following conditions are
+met:
 
-    * Redistributions of source code must retain the above copyright
-      notice, this list of conditions and the following disclaimer.
+    1. Redistributions of source code must retain the above copyright
+       notice, this list of conditions and the following disclaimer.
 
-    * Redistributions in binary form must reproduce the above copyright
-      notice, this list of conditions and the following disclaimer in
-      the documentation and/or other materials provided with the
-      distribution.
+    2. Redistributions in binary form must reproduce the above
+       copyright notice, this list of conditions and the following
+       disclaimer in the documentation and/or other materials provided
+       with the distribution.
 
-    * Neither the name of Intel Corporation nor the names of its
-      contributors may be used to endorse or promote products derived
-      from this software without specific prior written permission.
+    3. Neither the name of the copyright holder nor the names of its
+       contributors may be used to endorse or promote products derived
+       from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
 A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY LOG OF THE USE
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `geopmdpy-3.0.1/geopmdpy/__main__.py` & `geopmdpy-3.1.0/geopmdpy/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 from dasbus.loop import EventLoop
 from dasbus.connection import SystemMessageBus
 from signal import signal
 from signal import SIGTERM
 import sys
 import os
 from . import service
 from . import system_files
+from . import __version_str__
 from geopmdpy.restorable_file_writer import RestorableFileWriter
 
 ALLOW_WRITES_PATH = '/sys/module/msr/parameters/allow_writes'
 ALLOW_WRITES_BACKUP_PATH = os.path.join(system_files.GEOPM_SERVICE_RUN_PATH, 'msr-saved-allow-writes')
 
 _bus = None
 _loop = None
@@ -28,28 +29,33 @@
         _bus.disconnect()
         _bus = None
     if _loop is not None:
         _loop.quit()
 
 
 def main():
+    if len(sys.argv) > 1 and sys.argv[1] == '--version':
+        print(__version_str__)
+        return 0
     signal(SIGTERM, term_handler)
     global _bus, _loop
     system_files.secure_make_dirs(system_files.GEOPM_SERVICE_RUN_PATH,
                                   perm_mode=system_files.GEOPM_SERVICE_RUN_PATH_PERM)
     _loop = EventLoop()
     _bus = SystemMessageBus()
     with RestorableFileWriter(
         ALLOW_WRITES_PATH, ALLOW_WRITES_BACKUP_PATH,
         warning_handler=lambda warning: print('Warning <geopm-service>', warning,
                                               file=sys.stderr)) as writer:
         try:
             if not os.path.exists('/dev/cpu/msr_batch'):
                 writer.backup_and_try_update('on\n')
-            _bus.publish_object("/io/github/geopm", service.GEOPMService())
+            geopm_service = service.GEOPMService()
+            geopm_service.topo_rm_cache()
+            _bus.publish_object("/io/github/geopm", geopm_service)
             _bus.register_service("io.github.geopm")
             _loop.run()
         finally:
             stop()
 
 if __name__ == '__main__':
     main()
```

### Comparing `geopmdpy-3.0.1/geopmdpy/access.py` & `geopmdpy-3.1.0/geopmdpy/access.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """Implementation for the geopmaccess command line tool.
 
 """
 
@@ -10,14 +10,23 @@
 import os
 import tempfile
 import subprocess # nosec
 from argparse import ArgumentParser
 from dasbus.connection import SystemMessageBus
 from dasbus.error import DBusError
 from geopmdpy import system_files
+from . import gffi
+from . import error
+from . import __version_str__
+
+gffi.gffi.cdef("""
+int geopm_allowlist(size_t result_max,
+                    char *result);
+""")
+_dl = gffi.get_dl_geopmd()
 
 
 class DirectAccessProxy:
     """A proxy for access-related GEOPM service interactions that attempts
     in-process operations instead of issuing D-Bus calls.
     """
 
@@ -297,16 +306,34 @@
 
         Parse list of signals or controls from standard input or edit
         existing list.
 
         """
         return [ll.strip() for ll in fid.readlines() if ll.strip()]
 
+    def get_msr_safe_allowlist(self):
+        """Generate an allowlist for msr-safe
+
+        Generates the minimal msr-safe allowlist required for
+        GEOPM to access all the expected signals and controls.
+
+        Returns:
+            str: msr-safe allowlist string.
+
+        """
+        global _dl
+        data_max = 2097152 # 2 MiB
+        allowlist_cstr = gffi.gffi.new("char[]", data_max)
+        err = _dl.geopm_allowlist(data_max, allowlist_cstr)
+        if err < 0:
+            raise RuntimeError('geopm_allowlist() failed: {}'.format(error.message(err)))
+        return gffi.gffi.string(allowlist_cstr).decode()
+
     def run(self, is_write, is_all, is_control, group, is_default, is_delete,
-            is_dry_run, is_force, is_edit):
+            is_dry_run, is_force, is_edit, is_log, is_msr_safe):
         """Execute geopmaccess command line interface
 
         The inputs to this method are parsed from the command line
         interface of geopmaccess.  All of the features of the
         geopmaccess tool are implemented with this method.
 
         Args:
@@ -331,35 +358,43 @@
             is_default (bool): True if the default user access list
                                should be printed rather than the calling
                                process' access list.
             is_delete (bool): True to remove an access list file.
             is_dry_run (bool): True to run error checking without file
                                modification
             is_force (bool): True if error checking is disabled
+            is_log (bool): True if log user requested a log of requests
+                           since service restart
+            is_msr_safe (bool): True if user requested msr-safe allowlist
 
         """
         output = None
         # Determine if user provided -g option
         if group is None:
             is_group = False
-            # Empty string is for default access list
-            group = ''
+            if is_log:
+                group = system_files.GEOPM_SERVICE_LOG_REQUEST
+            else:
+                # Empty string is for default access list
+                group = ''
         else:
             is_group = True
 
-        if is_all and (is_write or is_edit or is_delete):
-            raise RuntimeError('Option -a/--all is not valid when writing a configuration')
+        if (is_all or is_log or is_msr_safe) and (is_write or is_edit or is_delete):
+            raise RuntimeError('Option -a/--all or -l/--log or -s/--msr-safe are not valid when '
+                               'writing a configuration')
         if is_dry_run and (is_edit or is_delete):
             raise RuntimeError('Option -n/--dry-run not valid with -e/--edit or -D/--delete')
         if is_force and is_edit:
             raise RuntimeError('Option -F/--force is not valid with -e/--edit')
-        if is_group and (is_default or is_all):
-            raise RuntimeError('Option -g/--group is not valid with -u/--default or -a/--all')
+        if is_group and (is_default or is_all or is_log or is_msr_safe):
+            raise RuntimeError('Option -g/--group is not valid with -u/--default or -a/--all or -l/--log '
+                               ' or -s/--msr-safe')
         if not (is_edit or is_write or is_delete) and (is_dry_run or is_force):
-            raise RuntimeError('-n/--dry-run, and -F/--force not valid when reading')
+            raise RuntimeError('-n/--dry-run or -F/--force not valid when reading')
 
 
         names = None
         if is_edit:
             names = self.edited_names(is_control, group)
         elif is_write:
             names = self.read_names(sys.stdin)
@@ -374,19 +409,21 @@
         else:
             # Get access list
             if is_all:
                 if is_control:
                     output = self.get_all_controls()
                 else:
                     output = self.get_all_signals()
-            elif is_default or is_group:
+            elif is_default or is_group or is_log:
                 if is_control:
                     output = self.get_group_controls(group)
                 else:
                     output = self.get_group_signals(group)
+            elif is_msr_safe:
+                output = self.get_msr_safe_allowlist()
             else:
                 if is_control:
                     output = self.get_user_controls()
                 else:
                     output = self.get_user_signals()
         return output
 
@@ -396,23 +433,29 @@
     Command line tool for reading and writing the access management
     lists for the GEOPM Service signals and controls.
 
     """
 
     err = 0
     parser = ArgumentParser(description=main.__doc__)
+    parser.add_argument('-v', '--version', dest='version', action='store_true',
+                        help='Print version and exit')
     parser.add_argument('-c', '--controls', dest='controls', action='store_true', default=False,
                         help='Command applies to controls not signals')
-    parser_group_uga = parser.add_mutually_exclusive_group(required=False)
-    parser_group_uga.add_argument('-u', '--default', dest='default', action='store_true', default=False,
-                                  help='Print the default user access list')
-    parser_group_uga.add_argument('-g', '--group', dest='group', type=str, default=None,
-                                 help='Read or write the access list for a specific Unix GROUP')
-    parser_group_uga.add_argument('-a', '--all', dest='all', action='store_true', default=False,
-                                  help='Print all signals or controls supported by the service system')
+    parser_group_ugals = parser.add_mutually_exclusive_group(required=False)
+    parser_group_ugals.add_argument('-u', '--default', dest='default', action='store_true', default=False,
+                                    help='Print the default user access list')
+    parser_group_ugals.add_argument('-g', '--group', dest='group', type=str, default=None,
+                                    help='Read or write the access list for a specific Unix GROUP')
+    parser_group_ugals.add_argument('-a', '--all', dest='all', action='store_true', default=False,
+                                    help='Print all signals or controls supported by the service system')
+    parser_group_ugals.add_argument('-l', '--log', action='store_true', default=False,
+                                    help='Print list of used signals or controls used since last restart of the service')
+    parser_group_ugals.add_argument('-s', '--msr-safe', dest='msr_safe', action='store_true', default=False,
+                                    help='Generate an allowlist for msr-safe')
     parser_group_weD = parser.add_mutually_exclusive_group(required=False)
     parser_group_weD.add_argument('-w', '--write', dest='write', action='store_true', default=False,
                                   help='Use standard input to write an access list. Implies -u unless -g is provided.')
     parser_group_weD.add_argument('-e', '--edit', dest='edit', action='store_true', default=False,
                                   help='Edit an access list using EDITOR environment variable, default vi')
     parser_group_weD.add_argument('-D', '--delete', dest='delete', action='store_true', default=False,
                                   help='Remove an access list for default user or a particular Unix Group')
@@ -427,20 +470,23 @@
     if args.direct and not (args.group or args.default):
         # This option is intended for early admin access list management before
         # the GEOPM service is running. The option does not have a meaningful
         # use case when run for the root user.
         parser.error('Must specify either --group or --default with --direct.')
 
     try:
+        if args.version:
+            print(__version_str__)
+            return 0
         geopm_proxy = (DirectAccessProxy() if args.direct
                        else SystemMessageBus().get_proxy('io.github.geopm', '/io/github/geopm'))
         acc = Access(geopm_proxy)
         output = acc.run(args.write, args.all, args.controls, args.group,
                          args.default, args.delete, args.dry_run, args.force,
-                         args.edit)
+                         args.edit, args.log, args.msr_safe)
         if output:
             print(output)
     except RuntimeError as ee:
         if 'GEOPM_DEBUG' in os.environ:
             # Do not handle exception if GEOPM_DEBUG is set
             raise ee
         sys.stderr.write('Error: {}\n\n'.format(ee))
```

### Comparing `geopmdpy-3.0.1/geopmdpy/dbus_xml.py` & `geopmdpy-3.1.0/geopmdpy/dbus_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 
 """The GEOPM DBus API enables a client to make measurements from the
 hardware platform and set hardware control parameters.  Fine grained
 permissions management for both measurements (signals) and controls is
```

### Comparing `geopmdpy-3.0.1/geopmdpy/error.py` & `geopmdpy-3.1.0/geopmdpy/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 
 import sys
 from . import gffi
```

### Comparing `geopmdpy-3.0.1/geopmdpy/gffi.py` & `geopmdpy-3.1.0/geopmdpy/gffi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 '''The gffi module provides a wrapper around the cffi interface
 
 This module enables a single cffi.FFI() object to be used throughout
 all of the GEOPM python modules and also enables us to enforce that
@@ -46,29 +46,19 @@
     global _dl_geopm
     if type(_dl_geopm) is OSError:
         raise _dl_geopm
     return _dl_geopm
 
 # Enforce load order of libgeopm.so and libgeopmd.so by loading
 # them together in this module.
-
-# Set GEOPM_PROGRAM_FILTER to empty string to avoid registering for
-# profiling upon calling dlopen() on libgeopm.so
-_orig_filter = os.environ.get('GEOPM_PROGRAM_FILTER')
-os.environ['GEOPM_PROGRAM_FILTER'] = ''
 try:
     _dl_geopm = gffi.dlopen('libgeopm.so.2',
                             gffi.RTLD_GLOBAL|gffi.RTLD_LAZY)
 except OSError as err:
     _dl_geopm = err
-finally:
-    if _orig_filter is not None:
-        os.environ['GEOPM_PROGRAM_FILTER'] = _orig_filter
-    else:
-        os.environ.pop('GEOPM_PROGRAM_FILTER')
 
 # Load libgeopmd.so after libgeopm.so
 try:
     _dl_geopmd =  gffi.dlopen('libgeopmd.so.2',
                               gffi.RTLD_GLOBAL|gffi.RTLD_LAZY)
 except OSError as err:
     _dl_geopmd = err
```

### Comparing `geopmdpy-3.0.1/geopmdpy/loop.py` & `geopmdpy-3.1.0/geopmdpy/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """Classes to support timer based loops
 
 """
```

### Comparing `geopmdpy-3.0.1/geopmdpy/pio.py` & `geopmdpy-3.1.0/geopmdpy/pio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """The pio module provides python bindings for the geopm_pio(3) C
 interfaces.  This interface provides an abstraction for reading
 signals and writing controls from system components.
```

### Comparing `geopmdpy-3.0.1/geopmdpy/restorable_file_writer.py` & `geopmdpy-3.1.0/geopmdpy/restorable_file_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 import os
 from typing import Union, Callable
 from geopmdpy import system_files
```

### Comparing `geopmdpy-3.0.1/geopmdpy/service.py` & `geopmdpy-3.1.0/geopmdpy/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """Module containing the implementations of the DBus interfaces
 exposed by geopmd."""
 
 import os
@@ -44,14 +44,16 @@
         """
         self._pio = pio
         self._RUN_PATH = system_files.GEOPM_SERVICE_RUN_PATH
         self._SAVE_DIR = 'SAVE_FILES'
         self._WATCH_INTERVAL_SEC = 1
         self._active_sessions = system_files.ActiveSessions(self._RUN_PATH)
         self._access_lists = system_files.AccessLists(system_files.get_config_path())
+        self._accessed_signals = set()
+        self._accessed_controls = set()
         for client_pid in self._active_sessions.get_clients():
             is_active = self.check_client(client_pid)
             if is_active:
                 watch_id = self._watch_client(client_pid)
                 self._active_sessions.set_watch_id(client_pid, watch_id)
         with system_files.WriteLock(self._RUN_PATH) as lock:
             write_pid = lock.try_lock()
@@ -78,15 +80,19 @@
         Returns:
             list(str), list(str): Signal and control allowed lists, both in sorted order.
 
         Raises:
             RuntimeError: The group name is not valid on the system.
 
         """
-        return self._access_lists.get_group_access(group)
+        if group == system_files.GEOPM_SERVICE_LOG_REQUEST:
+            result = (sorted(self._accessed_signals), sorted(self._accessed_controls))
+        else:
+            result = self._access_lists.get_group_access(group)
+        return result
 
     def set_group_access(self, group, allowed_signals, allowed_controls):
         """Set signals and controls in the allowed lists
 
         Write the list of allowed signals and controls for the
         specified group.  If the group is None or the empty string
         then the default lists of allowed signals and controls are
@@ -601,14 +607,18 @@
         if len(control_config) != 0:
             self._write_mode(client_pid)
         batch_pid = self._active_sessions.get_batch_server(client_pid)
         if batch_pid is not None:
             raise RuntimeError(f'Client {client_pid} has already started a batch server: {batch_pid}')
         batch_pid , batch_key = self._pio.start_batch_server(client_pid, signal_config, control_config)
         self._active_sessions.set_batch_server(client_pid, batch_pid)
+        for (_, _, sn) in signal_config:
+            self._accessed_signals.add(sn)
+        for (_, _, cn) in control_config:
+            self._accessed_controls.add(cn)
         return batch_pid, batch_key
 
     def stop_batch(self, client_pid, server_pid):
         """End a batch server previously started by the client.
 
         Terminate the batch server process and free up all resources
         associated with the batch server.  Any future calls by the
@@ -672,14 +682,15 @@
         if not self._check_client_active(client_pid, 'PlatformReadSignal'):
             return result
         signal_avail = self._active_sessions.get_signals(client_pid)
         if not signal_name in signal_avail:
             sys.stderr.write(f"Warning: <geopm-service>: Requested signal that is not in allowed list: '{signal_name}'\n")
         else:
             result = self._pio.read_signal(signal_name, domain, domain_idx)
+            self._accessed_signals.add(signal_name)
         return result
 
     def write_control(self, client_pid, control_name, domain, domain_idx, setting):
         """Write a control value to a particular domain.
 
         Select a control by name and write a new setting for the
         domain type and index specified.  The written control setting
@@ -716,14 +727,15 @@
         if not self._check_client_active(client_pid, 'PlatformWriteControl'):
             return
         control_avail = self._active_sessions.get_controls(client_pid)
         if not control_name in control_avail:
             raise RuntimeError('Requested control that is not in allowed list: {}'.format(control_name))
         self._write_mode(client_pid)
         self._pio.write_control(control_name, domain, domain_idx, setting)
+        self._accessed_controls.add(control_name)
 
     def restore_control(self, client_pid):
         """Restore all controls recorded at the start of a session.
 
         For the session associated to the given process, restore the state
         of all controls, which is recorded at the beginning of the session.
 
@@ -880,14 +892,15 @@
 
     """
     def __init__(self, topo=topo):
         """TopoService constructor that initializes all private members.
 
         """
         self._topo = topo
+        self._topo_path = os.path.join(system_files.GEOPM_SERVICE_RUN_PATH, 'geopm-topo-cache')
 
     def get_cache(self):
         """Return the contents of the PlatformTopo cache file.
 
         Create the PlatformTopo cache file if it does not exist and
         then return the contents of the file as a string.  This
         provides all the information required to associate all domains
@@ -895,18 +908,26 @@
 
         Returns:
             (str): Contents of the topology cache file that defines
                    the system topology.
 
         """
         self._topo.create_cache()
-        with open(os.path.join(system_files.GEOPM_SERVICE_RUN_PATH, 'geopm-topo-cache')) as fid:
+        with open(self._topo_path) as fid:
             result = fid.read()
         return result
 
+    def rm_cache(self):
+        """Remove an existing cache file if it exists
+
+        """
+        try:
+            os.unlink(self._topo_path)
+        except FileNotFoundError:
+            pass
 
 class GEOPMService(object):
     """The dasbus service object that is published.
 
     Object used by dasbus to map GEOPM service DBus APIs to their
     implementation.  A GEOPMService object is published by geopmd
     using the publish_object() method of dasbus.SystemMessageBus
@@ -928,15 +949,18 @@
         self._platform = PlatformService()
         self._dbus_proxy = SystemMessageBus().get_proxy('org.freedesktop.DBus',
                                                         '/org/freedesktop/DBus')
 
     def TopoGetCache(self):
         return self._topo.get_cache()
 
-    def PlatformGetGroupAccess(self, group):
+    @accepts_additional_arguments
+    def PlatformGetGroupAccess(self, group, **call_info):
+        if group == '0.GEOPM_SERVICE_LOG_REQUEST':
+            self._check_cap_sys_admin(call_info, "PlatformGetGroupAccess")
         return self._platform.get_group_access(group)
 
     @accepts_additional_arguments
     def PlatformSetGroupAccess(self, group, allowed_signals, allowed_controls, **call_info):
         self._check_cap_sys_admin(call_info, "PlatformSetGroupAccess")
         self._platform.set_group_access(group, allowed_signals, allowed_controls)
 
@@ -1022,14 +1046,20 @@
     def PlatformGetProfilePids(self, profile_name):
         return self._platform.get_profile_pids(profile_name)
 
     # TODO: This method should check credentials
     def PlatformPopProfileRegionNames(self, profile_name):
         return self._platform.pop_profile_region_names(profile_name)
 
+    def topo_rm_cache(self):
+        """Remove an existing topo cache file if it exists
+
+        """
+        self._topo.rm_cache()
+
     def _get_user(self, call_info):
         """Use DBus proxy object to derive the user name that owns the client
            process.
 
         Args:
            call_info (dict): The dictionary provided by the dasbus
                              @accepts_additional_arguments decorator.
```

### Comparing `geopmdpy-3.0.1/geopmdpy/session.py` & `geopmdpy-3.1.0/geopmdpy/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """Implementation for the geopmsession command line tool
 
 """
 
 import sys
 import os
+import errno
 import math
 from argparse import ArgumentParser
 from . import topo
 from . import pio
 from . import loop
+from . import __version_str__
 
 
 class Session:
     """Object responsible for creating a GEOPM batch read session
 
     This object's run() method is the main entry point for
     geopmsession command line tool.  The inputs to run() are derived
@@ -52,15 +54,15 @@
         if len(signals) != len(signal_format):
             raise RuntimeError(
                 'Number of signal values does not match the number of requests')
         result = [pio.format_signal(ss, ff) for (ss, ff) in
                   zip(signals, signal_format)]
         return '{}\n'.format(','.join(result))
 
-    def run_read(self, requests, duration, period, out_stream):
+    def run_read(self, requests, duration, period, pid, out_stream):
         """Run a read mode session
 
         Periodically read the requested signals. A line of text will
         be printed to the output stream for each period of time.  The
         line will contain a comma separated list of the read values,
         one for each request.
 
@@ -78,14 +80,17 @@
             duration (float): The user specified minimum length of time
                               for the samples to span in units of
                               seconds.
 
             period (float): The user specified period between samples
                             in units of seconds.
 
+            pid (int or None): If not None, stop monitoring when the
+                                      given process finishes.
+
             out_stream (typing.IO): Object with write() method where output
                                will be printed (typically sys.stdout).
 
         """
         num_period = 0
         if period != 0:
             num_period = math.ceil(duration / period)
@@ -94,14 +99,28 @@
             signal_handles.append(pio.push_signal(name, dom, dom_idx))
 
         for sample_idx in loop.TimedLoop(period, num_period):
             pio.read_batch()
             signals = [pio.sample(handle) for handle in signal_handles]
             line = self.format_signals(signals, requests.get_formats())
             out_stream.write(line)
+            if pid is not None:
+                try:
+                    os.kill(pid, 0)
+                except OSError as e:
+                    if e.errno == errno.ESRCH:
+                        # No such process. Stop watching.
+                        break
+                    elif e.errno == errno.EPERM:
+                        # There's a still a process, but we aren't allowed to
+                        # signal it. Since there's still a process, keep going.
+                        pass
+                    else:
+                        # Any other error. Bubble up the exception.
+                        raise
 
     def check_read_args(self, run_time, period):
         """Check that the run time and period are valid for a read session
 
         Args:
             run_time (float): Time duration of the session open in
                               seconds.
@@ -117,39 +136,50 @@
         if period > run_time:
             raise RuntimeError('Specified a period that is greater than the total run time')
         if period > 86400:
             raise RuntimeError('Specified a period greater than 24 hours')
         if period < 0.0 or run_time < 0.0:
             raise RuntimeError('Specified a negative run time or period')
 
-    def run(self, run_time, period,
+    def run(self, run_time, period, pid, print_header,
             request_stream=sys.stdin, out_stream=sys.stdout):
         """"Create a GEOPM session with values parsed from the command line
 
         The implementation for the geopmsession command line tool.
         The inputs to this method are derived from the parsed command
         line provided by the user.
 
         Args:
             run_time (float): Time duration of the session in seconds.
 
             period (float): Time interval for each line of output for.
                             Value must be zero for a write mode
                             session.
 
+            pid (int or None): If not None, stop monitoring when the
+                                      given process finishes.
+
+            print_header (bool): Whether to print a row of headers before printing
+                                 CSV data.
+
             request_stream (typing.IO): Input from user describing the
                                    requests to read.
 
             out_stream (typing.IO): Stream where output from will be
                                printed.
 
         """
         requests = ReadRequestQueue(request_stream)
         self.check_read_args(run_time, period)
-        self.run_read(requests, run_time, period, out_stream)
+        if print_header:
+            header_names = [f'"{name}-{topo.domain_name(domain)}-{domain_idx}"'
+                            if topo.domain_name(domain) != 'board' else f'"{name}"'
+                            for name, domain, domain_idx in requests]
+            print(','.join(header_names), file=out_stream)
+        self.run_read(requests, run_time, period, pid, out_stream)
 
 
 class RequestQueue:
     """Object derived from user input that provides request information
 
     The geopmsession command line tool parses requests for reading
     from standard input.  The RequestQueue object holds the logic for
@@ -298,22 +328,31 @@
 
     This command can be used to read signals by opening a session with
     the geopm service.
 
     """
     err = 0
     parser = ArgumentParser(description=main.__doc__)
+    parser.add_argument('-v', '--version', dest='version', action='store_true',
+                        help='Print version and exit')
     parser.add_argument('-t', '--time', dest='time', type=float, default=0.0,
                         help='Total run time of the session to be opened in seconds')
     parser.add_argument('-p', '--period', dest='period', type=float, default = 0.0,
                         help='When used with a read mode session reads all values out periodically with the specified period in seconds')
+    parser.add_argument('--pid', type=int,
+                        help='Stop the session when the given process PID ends')
+    parser.add_argument('--print-header', action='store_true',
+                        help='Print a CSV header before printing any sampled values')
     args = parser.parse_args()
     try:
+        if args.version:
+            print(__version_str__)
+            return 0
         sess = Session()
-        sess.run(args.time, args.period)
+        sess.run(run_time=args.time, period=args.period, pid=args.pid, print_header=args.print_header)
     except RuntimeError as ee:
         if 'GEOPM_DEBUG' in os.environ:
             # Do not handle exception if GEOPM_DEBUG is set
             raise ee
         sys.stderr.write('Error: {}\n\n'.format(ee))
         err = -1
     return err
```

### Comparing `geopmdpy-3.0.1/geopmdpy/shmem.py` & `geopmdpy-3.1.0/geopmdpy/shmem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 from . import gffi
 from . import error
 
 gffi.gffi.cdef("""
```

### Comparing `geopmdpy-3.0.1/geopmdpy/system_files.py` & `geopmdpy-3.1.0/geopmdpy/system_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 """Manage system files used by the geopm service
 
 Provides secure interfaces for manipulating the files in
 
@@ -37,14 +37,17 @@
 from . import schemas
 from . import shmem
 
 GEOPM_SERVICE_RUN_PATH = '/run/geopm'
 GEOPM_SERVICE_CONFIG_PATH = '/etc/geopm'
 # Deprecated since 3.0. May remove in a future release.
 LEGACY_GEOPM_SERVICE_CONFIG_PATH = '/etc/geopm-service'
+# Special strings used in place of user "group"
+GEOPM_SERVICE_LOG_REQUEST = '0.LOG_REQUEST'
+GEOPM_SERVICE_DEFAULT_ACCESS = '0.DEFAULT_ACCESS'
 
 GEOPM_SERVICE_RUN_PATH_PERM = 0o711
 """Default permissions for the GEOPM service run path
 
 """
 
 GEOPM_SERVICE_CONFIG_PATH_PERM = 0o700
@@ -1013,21 +1016,20 @@
 class AccessLists(object):
     """Class that manages the access list files
 
     """
     def __init__(self, config_path):
         self._CONFIG_PATH = config_path
         secure_make_dirs(self._CONFIG_PATH)
-        self._DEFAULT_ACCESS = '0.DEFAULT_ACCESS'
         self._signal_names = _get_names('/usr/bin/geopmread', quiet=False)
         self._control_names = _get_names('/usr/bin/geopmwrite')
 
     def _validate_group(self, group):
         if group is None or group == '':
-            group = self._DEFAULT_ACCESS
+            group = GEOPM_SERVICE_DEFAULT_ACCESS
         else:
             group = str(group)
             if group[0].isdigit():
                 raise RuntimeError('Linux group name cannot begin with a digit: group = "{}"'.format(group))
             try:
                 grp.getgrnam(group)
             except KeyError:
@@ -1450,7 +1452,12 @@
     cap_sys_admin = 0x00200000
     status_path = f'/proc/{pid}/status'
     with open(status_path) as fid:
         for line in fid.readlines():
             if line.startswith('CapEff:'):
                 cap = int(line.split(':')[1], 16)
     return (cap & cap_sys_admin != 0)
+
+def is_log_request(request):
+    if len(request) == 1 and request[0] == '0_LOG_REQUEST':
+        return True
+    return False
```

### Comparing `geopmdpy-3.0.1/geopmdpy/topo.py` & `geopmdpy-3.1.0/geopmdpy/topo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright (c) 2015 - 2023, Intel Corporation
+#  Copyright (c) 2015 - 2024 Intel Corporation
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 
 
 from . import gffi
 from . import error
```

### Comparing `geopmdpy-3.0.1/pyproject.toml` & `geopmdpy-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=59.6", "setuptools-scm>=6.4.2" ]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["geopmdpy"]
+
+[tool.setuptools.package-data]
+geopmdpy = ["VERSION"]
+
+[tool.setuptools_scm]
+root = ".."
+
 [project]
 name = "geopmdpy"
-version = "3.0.1"
+dynamic = ["version"]
 description = "GEOPM - Global Extensible Open Power Manager Daemon"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.6"
-license = {file = "COPYING"}
+license = {file = "LICENSE-BSD-3-Clause"}
 keywords = ["service", "hardware", "telemetry", "configuration"]
 authors = [
     {name = "Christopher Cantalupo", email = "christopher.m.cantalupo@intel.com"},
     {name = "Brad Geltz", email = "brad.geltz@intel.com"},
 ]
 maintainers = [
     {name = "Christopher Cantalupo", email = "christopher.m.cantalupo@intel.com"},
@@ -32,18 +41,21 @@
                "Programming Language :: Python :: 3.8",
                "Programming Language :: Python :: 3.9",
                "Programming Language :: Python :: 3.10",
                "Programming Language :: Python :: 3.11",
                "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = ["cffi>=1.14.5",
-                "setuptools>=53.0.0",
+                "setuptools>=59.6.0",
                 "psutil>=5.8.0",
-                "dasbus>=1.6.0",
+                "dasbus>=1.6",
                 "jsonschema>=3.2.0",
+                "pygobject>=3.42.0",
+                "docstring-parser>0.13",
+                "importlib_metadata>=4.0.0",
 ]
 
 [project.scripts]
 geopmd = "geopmdpy.__main__:main"
 geopmaccess = "geopmdpy.access:main"
 geopmsession = "geopmdpy.session:main"
```

