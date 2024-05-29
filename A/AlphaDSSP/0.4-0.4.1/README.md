# Comparing `tmp/AlphaDSSP-0.4.tar.gz` & `tmp/AlphaDSSP-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlphaDSSP-0.4.tar", last modified: Mon May 27 02:42:33 2024, max compression
+gzip compressed data, was "AlphaDSSP-0.4.1.tar", last modified: Wed May 29 04:09:30 2024, max compression
```

## Comparing `AlphaDSSP-0.4.tar` & `AlphaDSSP-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-27 02:42:33.439047 AlphaDSSP-0.4/
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-27 02:42:33.438047 AlphaDSSP-0.4/AlphaDSSP.egg-info/
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2616 2024-05-27 02:42:33.000000 AlphaDSSP-0.4/AlphaDSSP.egg-info/PKG-INFO
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      235 2024-05-27 02:42:33.000000 AlphaDSSP-0.4/AlphaDSSP.egg-info/SOURCES.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)        1 2024-05-27 02:42:33.000000 AlphaDSSP-0.4/AlphaDSSP.egg-info/dependency_links.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       21 2024-05-27 02:42:33.000000 AlphaDSSP-0.4/AlphaDSSP.egg-info/requires.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       10 2024-05-27 02:42:33.000000 AlphaDSSP-0.4/AlphaDSSP.egg-info/top_level.txt
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    35129 2024-04-27 00:47:33.000000 AlphaDSSP-0.4/LICENSE
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2616 2024-05-27 02:42:33.439047 AlphaDSSP-0.4/PKG-INFO
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2197 2024-05-14 20:01:58.000000 AlphaDSSP-0.4/README.md
-drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-27 02:42:33.438047 AlphaDSSP-0.4/alphadssp/
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       36 2024-05-14 19:12:55.000000 AlphaDSSP-0.4/alphadssp/__init__.py
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    11936 2024-05-27 02:36:37.000000 AlphaDSSP-0.4/alphadssp/alphadssp.py
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       38 2024-05-27 02:42:33.439047 AlphaDSSP-0.4/setup.cfg
--rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      656 2024-05-27 02:41:41.000000 AlphaDSSP-0.4/setup.py
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-29 04:09:30.294370 AlphaDSSP-0.4.1/
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-29 04:09:30.294370 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2618 2024-05-29 04:09:30.000000 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/PKG-INFO
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      235 2024-05-29 04:09:30.000000 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/SOURCES.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)        1 2024-05-29 04:09:30.000000 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/dependency_links.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       21 2024-05-29 04:09:30.000000 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/requires.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       10 2024-05-29 04:09:30.000000 AlphaDSSP-0.4.1/AlphaDSSP.egg-info/top_level.txt
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    35129 2024-04-27 00:47:33.000000 AlphaDSSP-0.4.1/LICENSE
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2618 2024-05-29 04:09:30.294370 AlphaDSSP-0.4.1/PKG-INFO
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)     2197 2024-05-14 20:01:58.000000 AlphaDSSP-0.4.1/README.md
+drwxr-xr-x   0 tiltwolf  (1000) tiltwolf  (1000)        0 2024-05-29 04:09:30.294370 AlphaDSSP-0.4.1/alphadssp/
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       36 2024-05-14 19:12:55.000000 AlphaDSSP-0.4.1/alphadssp/__init__.py
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)    11918 2024-05-29 04:08:27.000000 AlphaDSSP-0.4.1/alphadssp/alphadssp.py
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)       38 2024-05-29 04:09:30.294370 AlphaDSSP-0.4.1/setup.cfg
+-rw-r--r--   0 tiltwolf  (1000) tiltwolf  (1000)      658 2024-05-29 04:08:41.000000 AlphaDSSP-0.4.1/setup.py
```

### Comparing `AlphaDSSP-0.4/AlphaDSSP.egg-info/PKG-INFO` & `AlphaDSSP-0.4.1/AlphaDSSP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlphaDSSP
-Version: 0.4
+Version: 0.4.1
 Summary: Tool for converting Alphafold tar shards to a database of DSSP secondary structure information.
 Home-page: https://github.com/noelgarber/AlphaDSSP
 Author: Noel Garber
 Author-email: ngarber93@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `AlphaDSSP-0.4/LICENSE` & `AlphaDSSP-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AlphaDSSP-0.4/PKG-INFO` & `AlphaDSSP-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlphaDSSP
-Version: 0.4
+Version: 0.4.1
 Summary: Tool for converting Alphafold tar shards to a database of DSSP secondary structure information.
 Home-page: https://github.com/noelgarber/AlphaDSSP
 Author: Noel Garber
 Author-email: ngarber93@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `AlphaDSSP-0.4/README.md` & `AlphaDSSP-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `AlphaDSSP-0.4/alphadssp/alphadssp.py` & `AlphaDSSP-0.4.1/alphadssp/alphadssp.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,35 +232,35 @@
             pool.join()
     else:
         max_hcf_len = max([value[0].shape[0] for value in accession_results.values()])
         print(f"Models were not fragmented; longest model was {max_hcf_len}")
 
     return accession_results
 
-def generate_dssp(tar_dir = None, dssp_executable="/usr/bin/dssp", forbidden_codes = ("H","B","E","G","I","T"), plddt_thres=70):
+def generate_dssp(tar_dir = None, dssp_executable="/usr/bin/dssp", forbidden_codes = ("H","B","E","G","I","T"),
+                  plddt_thres=70, use_cached=True):
     '''
     Main function to generate DSSP results and an exclusion mask based on confident forbidden codes
 
     Args:
         tar_dir (str|None):           AlphaFold tar shards directory
         dssp_executable (str):        path to locally installed DSSP executable
         forbidden_codes (list|tuple): disallowed DSSP codes that will be used for generating the exclusion mask
         plddt_thres (int):            threshold for pLDDT such that only confident disallowed DSSP codes are used
+        use_cached (bool):            whether to use cached (pickled) AlphaDSSP data; if no, it is rebuilt
 
     Returns:
         results (dict): dictionary of full entry name --> tuple of (high_confidence_forbidden, dssp_codes_str)
     '''
 
     # Reload from previous build if desired
     if os.path.exists(alphadssp_path):
-        use_again = input(f"Previously built results exist (alphadssp_excluded_results.pkl); use them again? (Y/N)  ")
-        if use_again == "Y":
-            with open(alphadssp_path, "rb") as file:
-                results = pickle.load(file)
-                return results
+        with open(alphadssp_path, "rb") as file:
+            results = pickle.load(file)
+            return results
 
     if tar_dir is None:
         tar_dir = input("Enter the path to the folder containing tar shards of Alphafold structures:  ")
     tar_paths = [os.path.join(tar_dir, filename) for filename in os.listdir(tar_dir)]
     results = run_dssp_parallel(tar_paths, dssp_executable, forbidden_codes, plddt_thres)
     results = parse_fragments(results)
     with open("../alphadssp_excluded_results.pkl", "wb") as file:
```

### Comparing `AlphaDSSP-0.4/setup.py` & `AlphaDSSP-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AlphaDSSP",
-    version="0.4",
+    version="0.4.1",
     packages=find_packages(),
     description="Tool for converting Alphafold tar shards to a database of DSSP secondary structure information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noel Garber",
     author_email="ngarber93@gmail.com",
     url="https://github.com/noelgarber/AlphaDSSP",
```

