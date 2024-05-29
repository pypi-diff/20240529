# Comparing `tmp/geopmpy-3.0.1.tar.gz` & `tmp/geopmpy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopmpy-3.0.1.tar", last modified: Thu Dec  7 16:56:39 2023, max compression
+gzip compressed data, was "geopmpy-3.1.0.tar", last modified: Wed May 29 18:30:03 2024, max compression
```

## Comparing `geopmpy-3.0.1.tar` & `geopmpy-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,53 @@
-drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2023-12-07 16:56:39.651548 geopmpy-3.0.1/
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1022 2023-11-07 22:08:55.000000 geopmpy-3.0.1/AUTHORS
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1515 2023-11-07 22:09:00.000000 geopmpy-3.0.1/COPYING
--rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     9894 2023-12-07 16:56:39.651548 geopmpy-3.0.1/PKG-INFO
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     6345 2023-11-07 22:08:42.000000 geopmpy-3.0.1/README.md
-drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2023-12-07 16:56:39.651548 geopmpy-3.0.1/geopmpy.egg-info/
--rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     9894 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/PKG-INFO
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      228 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/SOURCES.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        1 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/dependency_links.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       54 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/entry_points.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      141 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/requires.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        1 2023-12-07 16:56:39.000000 geopmpy-3.0.1/geopmpy.egg-info/top_level.txt
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     2150 2023-12-07 16:55:26.000000 geopmpy-3.0.1/pyproject.toml
--rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       38 2023-12-07 16:56:39.651548 geopmpy-3.0.1/setup.cfg
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:30:03.970018 geopmpy-3.1.0/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       93 2024-05-15 17:46:43.000000 geopmpy-3.1.0/.gitignore
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1101 2024-05-15 23:16:04.000000 geopmpy-3.1.0/AUTHORS
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     3354 2024-05-15 17:46:43.000000 geopmpy-3.1.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5387 2024-05-21 00:55:39.000000 geopmpy-3.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1527 2024-05-15 17:46:43.000000 geopmpy-3.1.0/LICENSE-BSD-3-Clause
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       24 2024-05-15 17:46:43.000000 geopmpy-3.1.0/MANIFEST.in
+-rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     5593 2024-05-29 18:30:03.970018 geopmpy-3.1.0/PKG-INFO
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     2019 2024-05-15 17:46:43.000000 geopmpy-3.1.0/README.md
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:30:03.970018 geopmpy-3.1.0/debian/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      157 2024-05-15 17:46:43.000000 geopmpy-3.1.0/debian/changelog.in
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      949 2024-05-21 23:56:09.000000 geopmpy-3.1.0/debian/control
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     5238 2024-05-15 17:46:43.000000 geopmpy-3.1.0/debian/copyright
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      118 2024-05-15 17:46:43.000000 geopmpy-3.1.0/debian/rules
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      231 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmlaunch
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:30:03.970018 geopmpy-3.1.0/geopmpy/
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        5 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy/VERSION
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      257 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/__init__.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     7286 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/agent.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     9221 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/endpoint.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      668 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/hash.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    44408 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/io.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    76523 2024-05-15 23:16:04.000000 geopmpy-3.1.0/geopmpy/launcher.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     4163 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/policy_store.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      570 2024-05-15 17:46:43.000000 geopmpy-3.1.0/geopmpy/version.py
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:30:03.970018 geopmpy-3.1.0/geopmpy.egg-info/
+-rw-r--r--   0 cmcantal  (1001) cmcantal  (1001)     5593 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/PKG-INFO
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      884 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        1 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)       54 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/entry_points.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      141 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/requires.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)        8 2024-05-29 18:30:03.000000 geopmpy-3.1.0/geopmpy.egg-info/top_level.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1445 2024-05-21 23:56:09.000000 geopmpy-3.1.0/geopmpy.spec.in
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      356 2024-05-15 17:46:43.000000 geopmpy-3.1.0/make_deb.sh
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      454 2024-05-15 17:46:43.000000 geopmpy-3.1.0/make_rpm.sh
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)     1287 2024-05-15 17:46:43.000000 geopmpy-3.1.0/make_sdist.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      146 2024-05-15 17:46:43.000000 geopmpy-3.1.0/make_sdist.sh
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     2324 2024-05-15 17:46:43.000000 geopmpy-3.1.0/pyproject.toml
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      155 2024-05-15 17:46:43.000000 geopmpy-3.1.0/requirements.txt
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      279 2024-05-29 18:30:03.970018 geopmpy-3.1.0/setup.cfg
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      460 2024-05-15 17:46:43.000000 geopmpy-3.1.0/setup.py
+drwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)        0 2024-05-29 18:30:03.970018 geopmpy-3.1.0/test/
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    28144 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestAffinity.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     1542 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestAgent.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     5866 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestEndpoint.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)      694 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestHash.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)    48678 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestIO.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     8378 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestLauncher.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     3445 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestPolicyStore.py
+-rwxrwxr-x   0 cmcantal  (1001) cmcantal  (1001)     1837 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/TestPolicyStoreIntegration.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      386 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/__init__.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)      516 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/__main__.py
+-rw-rw-r--   0 cmcantal  (1001) cmcantal  (1001)    22157 2024-05-15 17:46:43.000000 geopmpy-3.1.0/test/test_io_experiment.report
```

### Comparing `geopmpy-3.0.1/AUTHORS` & `geopmpy-3.1.0/AUTHORS`

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

### Comparing `geopmpy-3.0.1/COPYING` & `geopmpy-3.1.0/LICENSE-BSD-3-Clause`

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

### Comparing `geopmpy-3.0.1/pyproject.toml` & `geopmpy-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=59.6", "setuptools-scm>=6.4.2" ]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["geopmpy"]
+
+[tool.setuptools.package-data]
+geopmpy = ["VERSION"]
+
+[tool.setuptools_scm]
+root = ".."
+
 [project]
 name = "geopmpy"
-version = "3.0.1"
+dynamic = ["version"]
 description = "GEOPM - Global Extensible Open Power Manager Runtime Tools"
 readme = "README.md"
 requires-python = ">=3.6"
-license = {file = "COPYING"}
+license = {file = "LICENSE-BSD-3-Clause"}
 keywords = ["runtime", "hardware", "telemetry", "configuration"]
 authors = [
     {name = "Christopher Cantalupo", email = "christopher.m.cantalupo@intel.com"},
     {name = "Brad Geltz", email = "brad.geltz@intel.com"},
 ]
 maintainers = [
     {name = "Christopher Cantalupo", email = "christopher.m.cantalupo@intel.com"},
```

