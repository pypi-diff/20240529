# Comparing `tmp/trust_plutus_namematch-1.tar.gz` & `tmp/trust_plutus_namematch-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trust_plutus_namematch-1.tar", max compression
+gzip compressed data, was "trust_plutus_namematch-2.tar", max compression
```

## Comparing `trust_plutus_namematch-1.tar` & `trust_plutus_namematch-2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-1/LICENSE
--rw-r--r--   0        0        0      489 2024-05-17 05:49:46.267215 trust_plutus_namematch-1/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-1/README.md
--rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-1/trust_plutus_namematch/__init__.py
--rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-1/trust_plutus_namematch/match.py
--rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-1/trust_plutus_namematch/utils/__init__.py
--rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-1/trust_plutus_namematch/utils/logs.py
--rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 trust_plutus_namematch-1/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-03-20 09:06:41.708383 trust_plutus_namematch-2/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-29 11:23:33.283157 trust_plutus_namematch-2/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-10 06:55:13.290252 trust_plutus_namematch-2/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 10:32:15.022349 trust_plutus_namematch-2/trust_plutus_namematch/__init__.py
+-rw-r--r--   0        0        0     1515 2024-05-10 06:28:57.924280 trust_plutus_namematch-2/trust_plutus_namematch/match.py
+-rw-r--r--   0        0        0        0 2024-02-12 07:49:10.008013 trust_plutus_namematch-2/trust_plutus_namematch/utils/__init__.py
+-rw-r--r--   0        0        0      425 2024-05-09 10:37:36.797518 trust_plutus_namematch-2/trust_plutus_namematch/utils/logs.py
+-rw-r--r--   0        0        0     1047 1970-01-01 00:00:00.000000 trust_plutus_namematch-2/PKG-INFO
```

### Comparing `trust_plutus_namematch-1/LICENSE` & `trust_plutus_namematch-2/LICENSE`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-1/trust_plutus_namematch/match.py` & `trust_plutus_namematch-2/trust_plutus_namematch/match.py`

 * *Files identical despite different names*

### Comparing `trust_plutus_namematch-1/PKG-INFO` & `trust_plutus_namematch-2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trust-plutus-namematch
-Version: 1
+Version: 2
 Summary: Name match for fund names from ICRA and MILES
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
 Author: Rolf Lobo
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

