# Comparing `tmp/neurocaps-0.9.4.tar.gz` & `tmp/neurocaps-0.9.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.4.tar", last modified: Tue May 28 05:05:57 2024, max compression
+gzip compressed data, was "neurocaps-0.9.4.post1.tar", last modified: Wed May 29 01:05:21 2024, max compression
```

## Comparing `neurocaps-0.9.4.tar` & `neurocaps-0.9.4.post1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.191095 neurocaps-0.9.4/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.4/LICENSE.md
--rw-rw-rw-   0        0        0    16839 2024-05-28 05:05:57.191095 neurocaps-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0    15453 2024-05-28 03:26:11.000000 neurocaps-0.9.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:56.985672 neurocaps-0.9.4/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.009633 neurocaps-0.9.4/neurocaps/_utils/
--rw-rw-rw-   0        0        0      363 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.040401 neurocaps-0.9.4/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.4/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.084978 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2187 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.130895 neurocaps-0.9.4/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    72959 2024-05-28 03:26:54.000000 neurocaps-0.9.4/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4791 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1626 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.141551 neurocaps-0.9.4/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    33356 2024-05-27 23:20:35.000000 neurocaps-0.9.4/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.191095 neurocaps-0.9.4/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    16839 2024-05-28 05:05:56.000000 neurocaps-0.9.4/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-28 05:05:56.000000 neurocaps-0.9.4/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:05:56.000000 neurocaps-0.9.4/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-05-28 05:05:56.000000 neurocaps-0.9.4/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-28 05:05:56.000000 neurocaps-0.9.4/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1572 2024-05-28 05:02:04.000000 neurocaps-0.9.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 05:05:57.191095 neurocaps-0.9.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 05:05:57.191095 neurocaps-0.9.4/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.4/tests/test_CAP.py
--rw-rw-rw-   0        0        0     4687 2024-05-27 23:20:35.000000 neurocaps-0.9.4/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-27 23:20:35.000000 neurocaps-0.9.4/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.4/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.4/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.4.post1/LICENSE.md
+-rw-rw-rw-   0        0        0    17016 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    15453 2024-05-28 18:55:10.000000 neurocaps-0.9.4.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.086144 neurocaps-0.9.4.post1/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.116421 neurocaps-0.9.4.post1/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.119165 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.126961 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.131695 neurocaps-0.9.4.post1/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    72959 2024-05-28 18:55:10.000000 neurocaps-0.9.4.post1/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.133604 neurocaps-0.9.4.post1/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33356 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.140702 neurocaps-0.9.4.post1/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    17016 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 01:05:21.000000 neurocaps-0.9.4.post1/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1731 2024-05-29 00:57:01.000000 neurocaps-0.9.4.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 01:05:21.143163 neurocaps-0.9.4.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 01:05:21.140702 neurocaps-0.9.4.post1/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.4.post1/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-27 18:25:53.000000 neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.4.post1/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.4.post1/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.4/LICENSE.md` & `neurocaps-0.9.4.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/PKG-INFO` & `neurocaps-0.9.4.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.4
+Version: 0.9.4.post1
 Summary: Co-activation Patterns (CAPs) Python package
-Author-email: Donisha Smith <dsmit216@fiu.edu>
+Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
+Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `neurocaps-0.9.4/README.md` & `neurocaps-0.9.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.4.post1/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.4.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/analysis/cap.py` & `neurocaps-0.9.4.post1/neurocaps/analysis/cap.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/analysis/merge.py` & `neurocaps-0.9.4.post1/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/analysis/standardize.py` & `neurocaps-0.9.4.post1/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.4.post1/neurocaps/extraction/timeseriesextractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.4.post1/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.4
+Version: 0.9.4.post1
 Summary: Co-activation Patterns (CAPs) Python package
-Author-email: Donisha Smith <dsmit216@fiu.edu>
+Author-email: Donisha Smith <donishasmith@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Project-URL: Issues, https://github.com/donishadsmith/neurocaps/issues
+Project-URL: Changelog, https://github.com/donishadsmith/neurocaps/blob/main/CHANGELOG.md
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `neurocaps-0.9.4/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.4.post1/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/pyproject.toml` & `neurocaps-0.9.4.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,98 +2,108 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e34 220d  rsion = "0.9.4".
-00000090: 0a6c 6963 656e 7365 203d 207b 7465 7874  .license = {text
-000000a0: 203d 2022 4d49 5420 4c69 6365 6e73 6522   = "MIT License"
-000000b0: 7d0d 0a61 7574 686f 7273 203d 205b 7b6e  }..authors = [{n
-000000c0: 616d 6520 3d20 2244 6f6e 6973 6861 2053  ame = "Donisha S
-000000d0: 6d69 7468 222c 2065 6d61 696c 203d 2022  mith", email = "
-000000e0: 6473 6d69 7432 3136 4066 6975 2e65 6475  dsmit216@fiu.edu
-000000f0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
-00000100: 203d 2022 436f 2d61 6374 6976 6174 696f   = "Co-activatio
-00000110: 6e20 5061 7474 6572 6e73 2028 4341 5073  n Patterns (CAPs
-00000120: 2920 5079 7468 6f6e 2070 6163 6b61 6765  ) Python package
-00000130: 220d 0a72 6561 646d 6520 3d20 2252 4541  "..readme = "REA
-00000140: 444d 452e 6d64 220d 0a72 6571 7569 7265  DME.md"..require
-00000150: 732d 7079 7468 6f6e 203d 2022 3e3d 332e  s-python = ">=3.
-00000160: 392e 3022 0d0a 6b65 7977 6f72 6473 203d  9.0"..keywords =
-00000170: 205b 2270 7974 686f 6e22 2c20 2243 6f2d   ["python", "Co-
-00000180: 4163 7469 7661 7469 6f6e 2050 6174 7465  Activation Patte
-00000190: 726e 7322 2c20 2243 4150 7322 2c20 226e  rns", "CAPs", "n
-000001a0: 6575 726f 696d 6167 696e 6722 2c20 2266  euroimaging", "f
-000001b0: 6d72 6922 2c20 2264 6663 222c 2022 6479  mri", "dfc", "dy
-000001c0: 6e61 6d69 6320 6675 6e63 7469 6f6e 616c  namic functional
-000001d0: 2063 6f6e 6e65 6374 6976 6974 7922 2c20   connectivity", 
-000001e0: 2266 4d52 4950 7265 7022 5d0d 0a63 6c61  "fMRIPrep"]..cla
-000001f0: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
-00000200: 2020 2249 6e74 656e 6465 6420 4175 6469    "Intended Audi
-00000210: 656e 6365 203a 3a20 4564 7563 6174 696f  ence :: Educatio
-00000220: 6e22 2c0d 0a20 2020 2022 496e 7465 6e64  n",..    "Intend
-00000230: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
-00000240: 6369 656e 6365 2f52 6573 6561 7263 6822  cience/Research"
-00000250: 2c0d 0a20 2020 2022 546f 7069 6320 3a3a  ,..    "Topic ::
-00000260: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
-00000270: 6e65 6572 696e 6722 2c0d 0a20 2020 2022  neering",..    "
-00000280: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000290: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
-000002a0: 6963 656e 7365 222c 0d0a 2020 2020 2250  icense",..    "P
-000002b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002d0: 2033 2e39 222c 0d0a 2020 2020 2250 726f   3.9",..    "Pro
-000002e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000300: 2e31 3022 2c0d 0a20 2020 2022 5072 6f67  .10",..    "Prog
-00000310: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000320: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000330: 3131 222c 0d0a 2020 2020 2250 726f 6772  11",..    "Progr
-00000340: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000350: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000360: 3222 2c0d 0a20 2020 2022 4f70 6572 6174  2",..    "Operat
-00000370: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
-00000380: 634f 5320 3a3a 204d 6163 4f53 2058 222c  cOS :: MacOS X",
-00000390: 0d0a 2020 2020 224f 7065 7261 7469 6e67  ..    "Operating
-000003a0: 2053 7973 7465 6d20 3a3a 2050 4f53 4958   System :: POSIX
-000003b0: 203a 3a20 4c69 6e75 7822 2c0d 0a20 2020   :: Linux",..   
-000003c0: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-000003d0: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-000003e0: 3a3a 2057 696e 646f 7773 203a 3a20 5769  :: Windows :: Wi
-000003f0: 6e64 6f77 7320 3131 222c 0d0a 2020 2020  ndows 11",..    
-00000400: 2244 6576 656c 6f70 6d65 6e74 2053 7461  "Development Sta
-00000410: 7475 7320 3a3a 2034 202d 2042 6574 6122  tus :: 4 - Beta"
-00000420: 0d0a 5d0d 0a64 6570 656e 6465 6e63 6965  ..]..dependencie
-00000430: 7320 3d20 5b22 6e75 6d70 7922 2c0d 0a20  s = ["numpy",.. 
-00000440: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000450: 7061 6e64 6173 222c 0d0a 2020 2020 2020  pandas",..      
-00000460: 2020 2020 2020 2020 2020 226d 6174 706c            "matpl
-00000470: 6f74 6c69 6222 2c0d 0a20 2020 2020 2020  otlib",..       
-00000480: 2020 2020 2020 2020 2022 7365 6162 6f72           "seabor
-00000490: 6e22 2c0d 0a20 2020 2020 2020 2020 2020  n",..           
-000004a0: 2020 2020 2022 6b6e 6565 6422 2c0d 0a20       "kneed",.. 
-000004b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000004c0: 6e69 6261 6265 6c22 2c0d 0a20 2020 2020  nibabel",..     
-000004d0: 2020 2020 2020 2020 2020 2022 6e69 6c65             "nile
-000004e0: 6172 6e3e 3d30 2e31 302e 312c 2021 3d30  arn>=0.10.1, !=0
-000004f0: 2e31 302e 3322 2c0d 0a20 2020 2020 2020  .10.3",..       
-00000500: 2020 2020 2020 2020 2022 7363 696b 6974           "scikit
-00000510: 2d6c 6561 726e 3e3d 312e 342e 3022 2c0d  -learn>=1.4.0",.
-00000520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000530: 2022 7375 7266 706c 6f74 222c 0d0a 2020   "surfplot",..  
-00000540: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00000550: 6575 726f 6d61 7073 222c 0d0a 2020 2020  euromaps",..    
-00000560: 2020 2020 2020 2020 2020 2020 2270 7962              "pyb
-00000570: 6964 733b 2070 6c61 7466 6f72 6d5f 7379  ids; platform_sy
-00000580: 7374 656d 2021 3d20 2757 696e 646f 7773  stem != 'Windows
-00000590: 2722 0d0a 2020 2020 2020 2020 2020 2020  '"..            
-000005a0: 2020 2020 5d0d 0a0d 0a5b 7072 6f6a 6563      ]....[projec
-000005b0: 742e 7572 6c73 5d0d 0a48 6f6d 6570 6167  t.urls]..Homepag
-000005c0: 6520 3d20 2268 7474 7073 3a2f 2f67 6974  e = "https://git
-000005d0: 6875 622e 636f 6d2f 646f 6e69 7368 6164  hub.com/donishad
-000005e0: 736d 6974 682f 6e65 7572 6f63 6170 7322  smith/neurocaps"
-000005f0: 2020 0d0a 0d0a 5b74 6f6f 6c2e 6469 7374    ....[tool.dist
-00000600: 7574 696c 732e 6264 6973 745f 7768 6565  utils.bdist_whee
-00000610: 6c5d 0d0a 756e 6976 6572 7361 6c20 3d20  l]..universal = 
-00000620: 7472 7565                                true
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e34 2e70  rsion = "0.9.4.p
+00000090: 6f73 7431 220d 0a6c 6963 656e 7365 203d  ost1"..license =
+000000a0: 207b 7465 7874 203d 2022 4d49 5420 4c69   {text = "MIT Li
+000000b0: 6365 6e73 6522 7d0d 0a61 7574 686f 7273  cense"}..authors
+000000c0: 203d 205b 7b6e 616d 6520 3d20 2244 6f6e   = [{name = "Don
+000000d0: 6973 6861 2053 6d69 7468 222c 2065 6d61  isha Smith", ema
+000000e0: 696c 203d 2022 646f 6e69 7368 6173 6d69  il = "donishasmi
+000000f0: 7468 406f 7574 6c6f 6f6b 2e63 6f6d 227d  th@outlook.com"}
+00000100: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
+00000110: 2022 436f 2d61 6374 6976 6174 696f 6e20   "Co-activation 
+00000120: 5061 7474 6572 6e73 2028 4341 5073 2920  Patterns (CAPs) 
+00000130: 5079 7468 6f6e 2070 6163 6b61 6765 220d  Python package".
+00000140: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
+00000150: 452e 6d64 220d 0a72 6571 7569 7265 732d  E.md"..requires-
+00000160: 7079 7468 6f6e 203d 2022 3e3d 332e 392e  python = ">=3.9.
+00000170: 3022 0d0a 6b65 7977 6f72 6473 203d 205b  0"..keywords = [
+00000180: 2270 7974 686f 6e22 2c20 2243 6f2d 4163  "python", "Co-Ac
+00000190: 7469 7661 7469 6f6e 2050 6174 7465 726e  tivation Pattern
+000001a0: 7322 2c20 2243 4150 7322 2c20 226e 6575  s", "CAPs", "neu
+000001b0: 726f 696d 6167 696e 6722 2c20 2266 6d72  roimaging", "fmr
+000001c0: 6922 2c20 2264 6663 222c 2022 6479 6e61  i", "dfc", "dyna
+000001d0: 6d69 6320 6675 6e63 7469 6f6e 616c 2063  mic functional c
+000001e0: 6f6e 6e65 6374 6976 6974 7922 2c20 2266  onnectivity", "f
+000001f0: 4d52 4950 7265 7022 5d0d 0a63 6c61 7373  MRIPrep"]..class
+00000200: 6966 6965 7273 203d 205b 0d0a 2020 2020  ifiers = [..    
+00000210: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
+00000220: 6365 203a 3a20 4564 7563 6174 696f 6e22  ce :: Education"
+00000230: 2c0d 0a20 2020 2022 496e 7465 6e64 6564  ,..    "Intended
+00000240: 2041 7564 6965 6e63 6520 3a3a 2053 6369   Audience :: Sci
+00000250: 656e 6365 2f52 6573 6561 7263 6822 2c0d  ence/Research",.
+00000260: 0a20 2020 2022 546f 7069 6320 3a3a 2053  .    "Topic :: S
+00000270: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000280: 6572 696e 6722 2c0d 0a20 2020 2022 4c69  ering",..    "Li
+00000290: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000002a0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+000002b0: 656e 7365 222c 0d0a 2020 2020 2250 726f  ense",..    "Pro
+000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002e0: 2e39 222c 0d0a 2020 2020 2250 726f 6772  .9",..    "Progr
+000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000300: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+00000310: 3022 2c0d 0a20 2020 2022 5072 6f67 7261  0",..    "Progra
+00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000340: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
+00000350: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000360: 2050 7974 686f 6e20 3a3a 2033 2e31 3222   Python :: 3.12"
+00000370: 2c0d 0a20 2020 2022 4f70 6572 6174 696e  ,..    "Operatin
+00000380: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000390: 5320 3a3a 204d 6163 4f53 2058 222c 0d0a  S :: MacOS X",..
+000003a0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
+000003b0: 7973 7465 6d20 3a3a 2050 4f53 4958 203a  ystem :: POSIX :
+000003c0: 3a20 4c69 6e75 7822 2c0d 0a20 2020 2022  : Linux",..    "
+000003d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000003e0: 203a 3a20 4d69 6372 6f73 6f66 7420 3a3a   :: Microsoft ::
+000003f0: 2057 696e 646f 7773 203a 3a20 5769 6e64   Windows :: Wind
+00000400: 6f77 7320 3131 222c 0d0a 2020 2020 2244  ows 11",..    "D
+00000410: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000420: 7320 3a3a 2034 202d 2042 6574 6122 0d0a  s :: 4 - Beta"..
+00000430: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
+00000440: 3d20 5b22 6e75 6d70 7922 2c0d 0a20 2020  = ["numpy",..   
+00000450: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
+00000460: 6e64 6173 222c 0d0a 2020 2020 2020 2020  ndas",..        
+00000470: 2020 2020 2020 2020 226d 6174 706c 6f74          "matplot
+00000480: 6c69 6222 2c0d 0a20 2020 2020 2020 2020  lib",..         
+00000490: 2020 2020 2020 2022 7365 6162 6f72 6e22         "seaborn"
+000004a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000004b0: 2020 2022 6b6e 6565 6422 2c0d 0a20 2020     "kneed",..   
+000004c0: 2020 2020 2020 2020 2020 2020 2022 6e69               "ni
+000004d0: 6261 6265 6c22 2c0d 0a20 2020 2020 2020  babel",..       
+000004e0: 2020 2020 2020 2020 2022 6e69 6c65 6172           "nilear
+000004f0: 6e3e 3d30 2e31 302e 312c 2021 3d30 2e31  n>=0.10.1, !=0.1
+00000500: 302e 3322 2c0d 0a20 2020 2020 2020 2020  0.3",..         
+00000510: 2020 2020 2020 2022 7363 696b 6974 2d6c         "scikit-l
+00000520: 6561 726e 3e3d 312e 342e 3022 2c0d 0a20  earn>=1.4.0",.. 
+00000530: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000540: 7375 7266 706c 6f74 222c 0d0a 2020 2020  surfplot",..    
+00000550: 2020 2020 2020 2020 2020 2020 226e 6575              "neu
+00000560: 726f 6d61 7073 222c 0d0a 2020 2020 2020  romaps",..      
+00000570: 2020 2020 2020 2020 2020 2270 7962 6964            "pybid
+00000580: 733b 2070 6c61 7466 6f72 6d5f 7379 7374  s; platform_syst
+00000590: 656d 2021 3d20 2757 696e 646f 7773 2722  em != 'Windows'"
+000005a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000005b0: 2020 5d0d 0a0d 0a5b 7072 6f6a 6563 742e    ]....[project.
+000005c0: 7572 6c73 5d0d 0a48 6f6d 6570 6167 6520  urls]..Homepage 
+000005d0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+000005e0: 622e 636f 6d2f 646f 6e69 7368 6164 736d  b.com/donishadsm
+000005f0: 6974 682f 6e65 7572 6f63 6170 7322 2020  ith/neurocaps"  
+00000600: 0d0a 4973 7375 6573 203d 2022 6874 7470  ..Issues = "http
+00000610: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000620: 6f6e 6973 6861 6473 6d69 7468 2f6e 6575  onishadsmith/neu
+00000630: 726f 6361 7073 2f69 7373 7565 7322 2020  rocaps/issues"  
+00000640: 0d0a 4368 616e 6765 6c6f 6720 3d20 2268  ..Changelog = "h
+00000650: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000660: 6d2f 646f 6e69 7368 6164 736d 6974 682f  m/donishadsmith/
+00000670: 6e65 7572 6f63 6170 732f 626c 6f62 2f6d  neurocaps/blob/m
+00000680: 6169 6e2f 4348 414e 4745 4c4f 472e 6d64  ain/CHANGELOG.md
+00000690: 220d 0a0d 0a5b 746f 6f6c 2e64 6973 7475  "....[tool.distu
+000006a0: 7469 6c73 2e62 6469 7374 5f77 6865 656c  tils.bdist_wheel
+000006b0: 5d0d 0a75 6e69 7665 7273 616c 203d 2074  ]..universal = t
+000006c0: 7275 65                                  rue
```

### Comparing `neurocaps-0.9.4/tests/test_CAP.py` & `neurocaps-0.9.4.post1/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.4.post1/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/tests/test_merge_dicts.py` & `neurocaps-0.9.4.post1/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.4/tests/test_standardize.py` & `neurocaps-0.9.4.post1/tests/test_standardize.py`

 * *Files identical despite different names*

