# Comparing `tmp/rapid_pe-0.1.2.dev20240527.tar.gz` & `tmp/rapid_pe-0.1.2.dev20240528.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapid_pe-0.1.2.dev20240527.tar", last modified: Mon May 27 05:03:24 2024, max compression
+gzip compressed data, was "rapid_pe-0.1.2.dev20240528.tar", last modified: Tue May 28 05:03:21 2024, max compression
```

## Comparing `rapid_pe-0.1.2.dev20240527.tar` & `rapid_pe-0.1.2.dev20240528.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:03:24.387206 rapid_pe-0.1.2.dev20240527/
--rw-rw-rw-   0 root         (0) root         (0)    18022 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/COPYING
--rw-r--r--   0 root         (0) root         (0)     1665 2024-05-27 05:03:24.386206 rapid_pe-0.1.2.dev20240527/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:03:24.376205 rapid_pe-0.1.2.dev20240527/bin/
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_calculate_overlap
--rw-rw-rw-   0 root         (0) root         (0)    16683 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_compute_intrinsic_fisher
--rw-rw-rw-   0 root         (0) root         (0)    37924 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_compute_intrinsic_grid
--rw-rw-rw-   0 root         (0) root         (0)    13261 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_create_event_dag
--rw-rw-rw-   0 root         (0) root         (0)    26192 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_integrate_extrinsic_likelihood
--rw-rw-rw-   0 root         (0) root         (0)     5035 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/bin/rapidpe_triangulation
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:03:24.383206 rapid_pe-0.1.2.dev20240527/rapid_pe/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32921 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/amrlib.py
--rw-rw-rw-   0 root         (0) root         (0)    12507 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/common_cl.py
--rw-rw-rw-   0 root         (0) root         (0)    15311 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/dagutils.py
--rw-rw-rw-   0 root         (0) root         (0)    23687 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/effectiveFisher.py
--rw-rw-rw-   0 root         (0) root         (0)    20243 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/factored_likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)    57880 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/lalsimutils.py
--rw-rw-rw-   0 root         (0) root         (0)    33626 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/mcsampler.py
--rw-rw-rw-   0 root         (0) root         (0)    11383 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/sph_harmonics.py
--rw-rw-rw-   0 root         (0) root         (0)    10345 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/statutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/synchlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:03:24.386206 rapid_pe-0.1.2.dev20240527/rapid_pe/tests/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      342 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/tests/test_common_cl.py
--rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/rapid_pe/xmlutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 05:03:24.386206 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1665 2024-05-27 05:03:24.000000 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      724 2024-05-27 05:03:24.000000 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 05:03:24.000000 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-27 05:03:24.000000 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-27 05:03:24.000000 rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 05:03:24.387206 rapid_pe-0.1.2.dev20240527/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2966 2024-05-25 05:03:28.000000 rapid_pe-0.1.2.dev20240527/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:03:21.934193 rapid_pe-0.1.2.dev20240528/
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/COPYING
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-28 05:03:21.934193 rapid_pe-0.1.2.dev20240528/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:03:21.930193 rapid_pe-0.1.2.dev20240528/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_calculate_overlap
+-rw-rw-rw-   0 root         (0) root         (0)    16683 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_compute_intrinsic_fisher
+-rw-rw-rw-   0 root         (0) root         (0)    37924 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_compute_intrinsic_grid
+-rw-rw-rw-   0 root         (0) root         (0)    13261 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_create_event_dag
+-rw-rw-rw-   0 root         (0) root         (0)    26192 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_integrate_extrinsic_likelihood
+-rw-rw-rw-   0 root         (0) root         (0)     5035 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/bin/rapidpe_triangulation
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:03:21.932193 rapid_pe-0.1.2.dev20240528/rapid_pe/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32921 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/amrlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12507 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/common_cl.py
+-rw-rw-rw-   0 root         (0) root         (0)    15311 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/dagutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    23687 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/effectiveFisher.py
+-rw-rw-rw-   0 root         (0) root         (0)    20243 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/factored_likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)    57880 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/lalsimutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    33626 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/mcsampler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11383 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/sph_harmonics.py
+-rw-rw-rw-   0 root         (0) root         (0)    10345 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/statutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/synchlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:03:21.933193 rapid_pe-0.1.2.dev20240528/rapid_pe/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      342 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/tests/test_common_cl.py
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/rapid_pe/xmlutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 05:03:21.934193 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1665 2024-05-28 05:03:21.000000 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2024-05-28 05:03:21.000000 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 05:03:21.000000 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-28 05:03:21.000000 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-28 05:03:21.000000 rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 05:03:21.934193 rapid_pe-0.1.2.dev20240528/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2966 2024-05-28 05:03:12.000000 rapid_pe-0.1.2.dev20240528/setup.py
```

### Comparing `rapid_pe-0.1.2.dev20240527/COPYING` & `rapid_pe-0.1.2.dev20240528/COPYING`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/PKG-INFO` & `rapid_pe-0.1.2.dev20240528/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid_pe
-Version: 0.1.2.dev20240527
+Version: 0.1.2.dev20240528
 Summary: RapidPE: The original low-latency gravitational wave parameter estimation code.
 Home-page: https://git.ligo.org/rapidpe-rift/rapidpe/
 License: GPL-2+
 Project-URL: Bug Tracker, https://git.ligo.org/rapidpe-rift/rapidpe/-/issues/
 Project-URL: Source Code, https://git.ligo.org/rapidpe-rift/rapidpe/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `rapid_pe-0.1.2.dev20240527/README.md` & `rapid_pe-0.1.2.dev20240528/README.md`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_calculate_overlap` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_calculate_overlap`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_compute_intrinsic_fisher` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_compute_intrinsic_fisher`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_compute_intrinsic_grid` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_compute_intrinsic_grid`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_create_event_dag` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_create_event_dag`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_integrate_extrinsic_likelihood` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_integrate_extrinsic_likelihood`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/bin/rapidpe_triangulation` & `rapid_pe-0.1.2.dev20240528/bin/rapidpe_triangulation`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/amrlib.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/amrlib.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/common_cl.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/common_cl.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/dagutils.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/dagutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/effectiveFisher.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/factored_likelihood.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/lalsimutils.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/lalsimutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/mcsampler.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/mcsampler.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/sph_harmonics.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/sph_harmonics.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/statutils.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/statutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/synchlib.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/synchlib.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe/xmlutils.py` & `rapid_pe-0.1.2.dev20240528/rapid_pe/xmlutils.py`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/PKG-INFO` & `rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid_pe
-Version: 0.1.2.dev20240527
+Version: 0.1.2.dev20240528
 Summary: RapidPE: The original low-latency gravitational wave parameter estimation code.
 Home-page: https://git.ligo.org/rapidpe-rift/rapidpe/
 License: GPL-2+
 Project-URL: Bug Tracker, https://git.ligo.org/rapidpe-rift/rapidpe/-/issues/
 Project-URL: Source Code, https://git.ligo.org/rapidpe-rift/rapidpe/
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `rapid_pe-0.1.2.dev20240527/rapid_pe.egg-info/SOURCES.txt` & `rapid_pe-0.1.2.dev20240528/rapid_pe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapid_pe-0.1.2.dev20240527/setup.py` & `rapid_pe-0.1.2.dev20240528/setup.py`

 * *Files identical despite different names*

