# Comparing `tmp/spectrum_io-0.4.3.tar.gz` & `tmp/spectrum_io-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_io-0.4.3.tar", max compression
+gzip compressed data, was "spectrum_io-0.4.4.tar", max compression
```

## Comparing `spectrum_io-0.4.3.tar` & `spectrum_io-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1102 2024-04-27 15:10:51.928840 spectrum_io-0.4.3/LICENSE
--rw-r--r--   0        0        0     2409 2024-04-27 15:10:51.928840 spectrum_io-0.4.3/README.rst
--rw-r--r--   0        0        0     2370 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1051 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/__init__.py
--rw-r--r--   0        0        0      351 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/__main__.py
--rw-r--r--   0        0        0      133 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/__init__.py
--rw-r--r--   0        0        0     6872 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/bruker.py
--rw-r--r--   0        0        0     5690 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/masterPeak.py
--rw-r--r--   0        0        0    13238 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/masterSpectrum.py
--rw-r--r--   0        0        0     1919 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/d/peak.py
--rw-r--r--   0        0        0      104 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/__init__.py
--rw-r--r--   0        0        0      556 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/csv.py
--rw-r--r--   0        0        0     5912 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/file/hdf5.py
--rw-r--r--   0        0        0        0 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/py.typed
--rw-r--r--   0        0        0      105 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/__init__.py
--rw-r--r--   0        0        0    13364 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/msraw.py
--rw-r--r--   0        0        0     3897 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/raw/thermo_raw.py
--rw-r--r--   0        0        0      177 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/__init__.py
--rw-r--r--   0        0        0     4333 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/mascot.py
--rw-r--r--   0        0        0     6178 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/maxquant.py
--rw-r--r--   0        0        0     4143 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/msamanda.py
--rw-r--r--   0        0        0     2937 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/msfragger.py
--rw-r--r--   0        0        0     2542 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/sage.py
--rw-r--r--   0        0        0     2791 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/search_results.py
--rw-r--r--   0        0        0     5547 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/search_result/xisearch.py
--rw-r--r--   0        0        0      238 2024-04-27 15:10:51.932841 spectrum_io-0.4.3/spectrum_io/spectral_library/__init__.py
--rw-r--r--   0        0        0    21794 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/digest.py
--rw-r--r--   0        0        0    45056 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/dlib/myPrositLib.dlib
--rw-r--r--   0        0        0     8539 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/dlib.py
--rw-r--r--   0        0        0    98385 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/msp/myPrositLib.msp
--rw-r--r--   0        0        0     2319 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/msp.py
--rw-r--r--   0        0        0     3799 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectral_library.py
--rw-r--r--   0        0        0   565091 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
--rw-r--r--   0        0        0     2833 2024-04-27 15:10:51.936841 spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut.py
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 spectrum_io-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2409 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/README.rst
+-rw-r--r--   0        0        0     2378 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1051 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/spectrum_io/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/spectrum_io/__main__.py
+-rw-r--r--   0        0        0      133 2024-05-29 12:25:04.046663 spectrum_io-0.4.4/spectrum_io/d/__init__.py
+-rw-r--r--   0        0        0     6920 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/d/bruker.py
+-rw-r--r--   0        0        0     5690 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/d/masterPeak.py
+-rw-r--r--   0        0        0    13238 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/d/masterSpectrum.py
+-rw-r--r--   0        0        0     1919 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/d/peak.py
+-rw-r--r--   0        0        0      104 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/file/__init__.py
+-rw-r--r--   0        0        0      556 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/file/csv.py
+-rw-r--r--   0        0        0     5912 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/file/hdf5.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/py.typed
+-rw-r--r--   0        0        0      105 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/raw/__init__.py
+-rw-r--r--   0        0        0    13364 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/raw/msraw.py
+-rw-r--r--   0        0        0     3897 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/raw/thermo_raw.py
+-rw-r--r--   0        0        0      177 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/__init__.py
+-rw-r--r--   0        0        0     4333 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/mascot.py
+-rw-r--r--   0        0        0     6178 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/maxquant.py
+-rw-r--r--   0        0        0     4143 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/msamanda.py
+-rw-r--r--   0        0        0     2937 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/msfragger.py
+-rw-r--r--   0        0        0     2552 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/sage.py
+-rw-r--r--   0        0        0     2798 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/search_results.py
+-rw-r--r--   0        0        0     5547 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/search_result/xisearch.py
+-rw-r--r--   0        0        0      238 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/__init__.py
+-rw-r--r--   0        0        0    21794 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/digest.py
+-rw-r--r--   0        0        0    45056 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/dlib/myPrositLib.dlib
+-rw-r--r--   0        0        0     8539 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/dlib.py
+-rw-r--r--   0        0        0    98385 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/msp/myPrositLib.msp
+-rw-r--r--   0        0        0     2319 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/msp.py
+-rw-r--r--   0        0        0     3799 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/spectral_library.py
+-rw-r--r--   0        0        0   565091 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
+-rw-r--r--   0        0        0     2833 2024-05-29 12:25:04.050663 spectrum_io-0.4.4/spectrum_io/spectral_library/spectronaut.py
+-rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 spectrum_io-0.4.4/PKG-INFO
```

### Comparing `spectrum_io-0.4.3/LICENSE` & `spectrum_io-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/README.rst` & `spectrum_io-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/pyproject.toml` & `spectrum_io-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_io"
-version = "0.4.3"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.4"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "IO related functionalities for oktoberfest."
 authors = ["Wilhelmlab at Technical University of Munich"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_io"
 repository = "https://github.com/wilhelm-lab/spectrum_io"
 documentation = "https://spectrum_io.readthedocs.io"
@@ -24,16 +24,16 @@
 rich = ">=10.3.0"
 PyYAML = ">=5.4.1"
 numpy = "^1.18.1"
 pandas = "^1.3.0"
 h5py = "^3.1.0"
 pymzml = "^2.5.0"
 pyteomics = "^4.3.3"
-lxml= '^4.5.2'
-spectrum-fundamentals = ">=0.5.2,<0.6.0"
+lxml= '>=4.5.2,<6.0.0'
+spectrum-fundamentals = ">=0.5.4,<0.6.0"
 alphatims = "^1.0.8"
 sortedcontainers = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.3"
 coverage = {extras = ["toml"], version = ">=5.3"}
 safety = ">=1.9.0"
```

### Comparing `spectrum_io-0.4.3/spectrum_io/__init__.py` & `spectrum_io-0.4.4/spectrum_io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for spectrum_io."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.4.3"
+__version__ = "0.4.4"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 from . import d, file, raw
```

### Comparing `spectrum_io-0.4.3/spectrum_io/d/bruker.py` & `spectrum_io-0.4.4/spectrum_io/d/bruker.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,9 +180,10 @@
     """
     scan_to_precursor_map = pd.read_csv(tims_meta_file)
     raw_spectra = read_timstof(source, scan_to_precursor_map)
     df_combined = aggregate_timstof(raw_spectra)
     df_combined["RAW_FILE"] = source.stem
     df_combined["MASS_ANALYZER"] = "TOF"
     df_combined["FRAGMENTATION"] = "HCD"
+    df_combined["INSTRUMENT_TYPES"] = "TIMSTOF"
 
     return df_combined
```

### Comparing `spectrum_io-0.4.3/spectrum_io/d/masterPeak.py` & `spectrum_io-0.4.4/spectrum_io/d/masterPeak.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/d/masterSpectrum.py` & `spectrum_io-0.4.4/spectrum_io/d/masterSpectrum.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/d/peak.py` & `spectrum_io-0.4.4/spectrum_io/d/peak.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/file/csv.py` & `spectrum_io-0.4.4/spectrum_io/file/csv.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/file/hdf5.py` & `spectrum_io-0.4.4/spectrum_io/file/hdf5.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/raw/msraw.py` & `spectrum_io-0.4.4/spectrum_io/raw/msraw.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/raw/thermo_raw.py` & `spectrum_io-0.4.4/spectrum_io/raw/thermo_raw.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/mascot.py` & `spectrum_io-0.4.4/spectrum_io/search_result/mascot.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/maxquant.py` & `spectrum_io-0.4.4/spectrum_io/search_result/maxquant.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/msamanda.py` & `spectrum_io-0.4.4/spectrum_io/search_result/msamanda.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/msfragger.py` & `spectrum_io-0.4.4/spectrum_io/search_result/msfragger.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/sage.py` & `spectrum_io-0.4.4/spectrum_io/search_result/sage.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 "CALCMASS": "MASS",
                 "HYPERSCORE": "SCORE",
                 "LABEL": "REVERSE",
             }
         )
 
         # removing .mzML
-        df["RAW_FILE"] = df["RAW_FILE"].str.replace(".mzML", "", regex=True)
+        df["RAW_FILE"] = df["RAW_FILE"].str.replace(r"\.mz[M|m][l|L]", "", regex=True)
         # extracting only the scan number
         df["SCAN_NUMBER"] = [int(x.rsplit("=", 1)[-1]) for x in df["SCAN_NUMBER"]]
         # creating a column of decoys and targets
         df["REVERSE"] = df["REVERSE"] < 0
         # removing modification to create the unmodified sequences
         df["SEQUENCE"] = df["MODIFIED_SEQUENCE"].str.replace(r"\-|\[.*?\]", "", regex=True)
         # length of the peptide
```

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/search_results.py` & `spectrum_io-0.4.4/spectrum_io/search_result/search_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :param df: df to filter
     :return: df after filtering out unsupported peptides
     """
     logger.info(f"#sequences before filtering for valid prosit sequences: {len(df.index)}")
     # retain only peptides that fall within [7, 30] length supported by Prosit
     df = df[(df["PEPTIDE_LENGTH"] <= 30) & (df["PEPTIDE_LENGTH"] >= 7)]
     # remove unsupported mods to exclude
-    unsupported_mods = [r"Acetyl \(Protein N\-term\)", "ac", r"\[[0-9]+\]"]
+    unsupported_mods = [r"Acetyl \(Protein N\-term\)", "ac", r"\[[0-9]+\]", r"\+"]
     exclude_mods_pattern = re.compile("|".join(unsupported_mods))
     df = df[~df["MODIFIED_SEQUENCE"].str.contains(exclude_mods_pattern)]
     # remove non-canonical aas
     df = df[(~df["SEQUENCE"].str.contains("U|O"))]
     # remove precursor charges greater than 6
     df = df[df["PRECURSOR_CHARGE"] <= 6]
     logger.info(f"#sequences after filtering for valid prosit sequences: {len(df.index)}")
```

### Comparing `spectrum_io-0.4.3/spectrum_io/search_result/xisearch.py` & `spectrum_io-0.4.4/spectrum_io/search_result/xisearch.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/digest.py` & `spectrum_io-0.4.4/spectrum_io/spectral_library/digest.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/dlib/myPrositLib.dlib` & `spectrum_io-0.4.4/spectrum_io/spectral_library/dlib/myPrositLib.dlib`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/dlib.py` & `spectrum_io-0.4.4/spectrum_io/spectral_library/dlib.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/msp/myPrositLib.msp` & `spectrum_io-0.4.4/spectrum_io/spectral_library/msp/myPrositLib.msp`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/msp.py` & `spectrum_io-0.4.4/spectrum_io/spectral_library/msp.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/spectral_library.py` & `spectrum_io-0.4.4/spectrum_io/spectral_library/spectral_library.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut/myPrositLib.csv` & `spectrum_io-0.4.4/spectrum_io/spectral_library/spectronaut/myPrositLib.csv`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/spectrum_io/spectral_library/spectronaut.py` & `spectrum_io-0.4.4/spectrum_io/spectral_library/spectronaut.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.4.3/PKG-INFO` & `spectrum_io-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: spectrum_io
-Version: 0.4.3
+Version: 0.4.4
 Summary: IO related functionalities for oktoberfest.
 Home-page: https://github.com/wilhelm-lab/spectrum_io
 License: MIT
 Author: Wilhelmlab at Technical University of Munich
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: alphatims (>=1.0.8,<2.0.0)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: h5py (>=3.1.0,<4.0.0)
-Requires-Dist: lxml (>=4.5.2,<5.0.0)
+Requires-Dist: lxml (>=4.5.2,<6.0.0)
 Requires-Dist: numpy (>=1.18.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pymzml (>=2.5.0,<3.0.0)
 Requires-Dist: pyteomics (>=4.3.3,<5.0.0)
 Requires-Dist: rich (>=10.3.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
-Requires-Dist: spectrum-fundamentals (>=0.5.2,<0.6.0)
+Requires-Dist: spectrum-fundamentals (>=0.5.4,<0.6.0)
 Project-URL: Documentation, https://spectrum_io.readthedocs.io
 Project-URL: Repository, https://github.com/wilhelm-lab/spectrum_io
 Description-Content-Type: text/x-rst
 
 spectrum_io
 ===========================
```

