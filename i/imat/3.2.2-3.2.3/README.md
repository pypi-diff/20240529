# Comparing `tmp/imat-3.2.2.tar.gz` & `tmp/imat-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imat-3.2.2.tar", last modified: Tue Jul 25 17:26:47 2023, max compression
+gzip compressed data, was "imat-3.2.3.tar", last modified: Wed May 29 14:09:36 2024, max compression
```

## Comparing `imat-3.2.2.tar` & `imat-3.2.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.966630 imat-3.2.2/
--rw-rw-rw-   0        0        0     1096 2023-07-17 17:26:37.000000 imat-3.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0    15150 2023-07-25 17:26:47.964609 imat-3.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13941 2023-07-23 17:13:18.000000 imat-3.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.645465 imat-3.2.2/iMaT/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/__init__.py
--rw-rw-rw-   0        0        0     2430 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.652445 imat-3.2.2/iMaT/src/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.666416 imat-3.2.2/iMaT/src/analysis/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    58077 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/functions.py
--rw-rw-rw-   0        0        0     5213 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/analysis/main.py
--rw-rw-rw-   0        0        0     3630 2023-07-23 16:40:24.000000 imat-3.2.2/iMaT/src/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.674391 imat-3.2.2/iMaT/src/cli/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/cli/__init__.py
--rw-rw-rw-   0        0        0    31673 2023-07-25 17:21:31.000000 imat-3.2.2/iMaT/src/cli/menu_constructors.py
--rw-rw-rw-   0        0        0    23891 2023-07-23 17:04:10.000000 imat-3.2.2/iMaT/src/cli/menu_entries.py
--rw-rw-rw-   0        0        0     7837 2023-07-23 17:08:29.000000 imat-3.2.2/iMaT/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.708294 imat-3.2.2/iMaT/src/conversion/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/__init__.py
--rw-rw-rw-   0        0        0     5090 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/main.py
--rw-rw-rw-   0        0        0    12992 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.716277 imat-3.2.2/iMaT/src/m21_environment/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/m21_environment/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/m21_environment/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.740210 imat-3.2.2/iMaT/src/pattern_search/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/__init__.py
--rw-rw-rw-   0        0        0    15880 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/functions.py
--rw-rw-rw-   0        0        0    10903 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/main.py
--rw-rw-rw-   0        0        0    10307 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/pattern_search/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.761154 imat-3.2.2/iMaT/src/score_selection/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/__init__.py
--rw-rw-rw-   0        0        0    17704 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/main.py
--rw-rw-rw-   0        0        0    14028 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/name_parts.py
--rw-rw-rw-   0        0        0    12218 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/score_selection/select_parts_and_measures.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.796060 imat-3.2.2/iMaT/src/tokenization/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/__init__.py
--rw-rw-rw-   0        0        0    19526 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.833967 imat-3.2.2/iMaT/src/tokenization/refine_results/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/absolute_duration.py
--rw-rw-rw-   0        0        0     7020 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
--rw-rw-rw-   0        0        0     4966 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/remove_prefixes.py
--rw-rw-rw-   0        0        0     5447 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/refine_results/tokens_to_txt.py
--rw-rw-rw-   0        0        0    15349 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/tokenization/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.859889 imat-3.2.2/iMaT/src/utils/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3982 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/error_handling.py
--rw-rw-rw-   0        0        0     6787 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.911750 imat-3.2.2/iMaT/src/visualizations/
--rw-rw-rw-   0        0        0        0 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/__init__.py
--rw-rw-rw-   0        0        0    19214 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/analysis_results_graphs.py
--rw-rw-rw-   0        0        0    10926 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/m21_integrated.py
--rw-rw-rw-   0        0        0     3263 2023-07-17 17:26:37.000000 imat-3.2.2/iMaT/src/visualizations/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 17:26:47.961621 imat-3.2.2/imat.egg-info/
--rw-rw-rw-   0        0        0    15150 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      272 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 17:26:46.000000 imat-3.2.2/imat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 17:26:47.967618 imat-3.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2105 2023-07-25 17:25:27.000000 imat-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.889907 imat-3.2.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-18 16:54:24.000000 imat-3.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    15756 2024-05-29 14:09:36.888908 imat-3.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13946 2024-05-29 13:59:57.000000 imat-3.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.853902 imat-3.2.3/iMaT/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/__init__.py
+-rw-rw-rw-   0        0        0     2430 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.855902 imat-3.2.3/iMaT/src/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.858902 imat-3.2.3/iMaT/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    58077 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/analysis/functions.py
+-rw-rw-rw-   0        0        0     5213 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/analysis/main.py
+-rw-rw-rw-   0        0        0     3630 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.860906 imat-3.2.3/iMaT/src/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/cli/__init__.py
+-rw-rw-rw-   0        0        0    31673 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/cli/menu_constructors.py
+-rw-rw-rw-   0        0        0    23891 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/cli/menu_entries.py
+-rw-rw-rw-   0        0        0     7842 2024-05-29 14:01:30.000000 imat-3.2.3/iMaT/src/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.863905 imat-3.2.3/iMaT/src/conversion/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/conversion/__init__.py
+-rw-rw-rw-   0        0        0     5090 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/conversion/main.py
+-rw-rw-rw-   0        0        0    12992 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.864903 imat-3.2.3/iMaT/src/m21_environment/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/m21_environment/__init__.py
+-rw-rw-rw-   0        0        0    10306 2024-05-29 13:39:36.000000 imat-3.2.3/iMaT/src/m21_environment/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.867901 imat-3.2.3/iMaT/src/pattern_search/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/pattern_search/__init__.py
+-rw-rw-rw-   0        0        0    15880 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/pattern_search/functions.py
+-rw-rw-rw-   0        0        0    10903 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/pattern_search/main.py
+-rw-rw-rw-   0        0        0    10307 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/pattern_search/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.870904 imat-3.2.3/iMaT/src/score_selection/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/score_selection/__init__.py
+-rw-rw-rw-   0        0        0    17704 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/score_selection/main.py
+-rw-rw-rw-   0        0        0    14028 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/score_selection/name_parts.py
+-rw-rw-rw-   0        0        0    12218 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/score_selection/select_parts_and_measures.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.872905 imat-3.2.3/iMaT/src/tokenization/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/__init__.py
+-rw-rw-rw-   0        0        0    19526 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.876902 imat-3.2.3/iMaT/src/tokenization/refine_results/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/refine_results/__init__.py
+-rw-rw-rw-   0        0        0     6837 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/refine_results/absolute_duration.py
+-rw-rw-rw-   0        0        0     7020 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py
+-rw-rw-rw-   0        0        0     4966 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/refine_results/remove_prefixes.py
+-rw-rw-rw-   0        0        0     5447 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/refine_results/tokens_to_txt.py
+-rw-rw-rw-   0        0        0    15349 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/tokenization/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.878902 imat-3.2.3/iMaT/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3982 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/utils/error_handling.py
+-rw-rw-rw-   0        0        0     6787 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.881902 imat-3.2.3/iMaT/src/visualizations/
+-rw-rw-rw-   0        0        0        0 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/visualizations/__init__.py
+-rw-rw-rw-   0        0        0    19214 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/visualizations/analysis_results_graphs.py
+-rw-rw-rw-   0        0        0    10926 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/visualizations/m21_integrated.py
+-rw-rw-rw-   0        0        0     3263 2024-04-18 16:54:25.000000 imat-3.2.3/iMaT/src/visualizations/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:09:36.887907 imat-3.2.3/imat.egg-info/
+-rw-rw-rw-   0        0        0    15756 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      272 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-29 14:09:36.000000 imat-3.2.3/imat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:09:36.889907 imat-3.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2105 2024-05-29 13:55:17.000000 imat-3.2.3/setup.py
```

### Comparing `imat-3.2.2/LICENSE.txt` & `imat-3.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/PKG-INFO` & `imat-3.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.2.2
+Version: 3.2.3
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,16 +21,32 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 License-File: LICENSE.txt
+Requires-Dist: numpy~=1.23.5
+Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: pandas~=2.0.2
+Requires-Dist: music21~=8.3.0
+Requires-Dist: miditok~=2.0.6
+Requires-Dist: tokenizers~=0.13.3
+Requires-Dist: requests~=2.31.0
+Requires-Dist: openpyxl~=3.1.2
+Requires-Dist: tqdm~=4.65.0
+Requires-Dist: seaborn~=0.12.2
+Requires-Dist: scipy~=1.10.1
+Provides-Extra: doc
+Requires-Dist: sphinx<7.0.0; extra == "doc"
+Requires-Dist: sphinxcontrib-napoleon~=0.7; extra == "doc"
+Requires-Dist: sphinx-autobuild; extra == "doc"
+Requires-Dist: myst_parser; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=1.2.0; extra == "doc"
 
 # The Interactive Music Analysis Tool (I-MaT)
 
 I-MaT is an innovative tool designed to facilitate in-depth musical analysis through an easy-to-use interface. I-MaT offers a comprehensive set of functionalities allowing for the examination of musical pieces from a wide range of perspectives. The documentation (available on [readthedocs.io](https://i-mat.readthedocs.io/en/latest/)) serves as a comprehensive guide, aiming to provide you with insights into I-MaT's functionalities and its modular concept, and assist both first-time users and experienced researchers in using the tool effectively.
 
 The sections contained within the documentation provide detailed information on how to use the Interactive Music Analysis Tool, from [downloading and the installation](https://i-mat.readthedocs.io/en/latest/getting_started.html), to [contribution and code extension](https://i-mat.readthedocs.io/en/latest/contribute.html), to its application in music analysis. Furthermore, you will find a detailed descriptions of I-MaT's [source code](https://i-mat.readthedocs.io/en/latest/module_files/src.html), explaining the different packages' and modules' content that make up the tool.
 
@@ -80,19 +96,19 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.3, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
-MIT License, Copyright (c) 2023 S.O. Eck.
+MIT License, Copyright (c) 2023-2024 S.O. Eck.
 
 ----------------------------------------------------------------------
 
 LOCATION: Start Menu
 
 Please make a selection from the options below by entering the entry index number:
```

### Comparing `imat-3.2.2/README.md` & `imat-3.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,19 +50,19 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.3, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
-MIT License, Copyright (c) 2023 S.O. Eck.
+MIT License, Copyright (c) 2023-2024 S.O. Eck.
 
 ----------------------------------------------------------------------
 
 LOCATION: Start Menu
 
 Please make a selection from the options below by entering the entry index number:
```

### Comparing `imat-3.2.2/iMaT/__main__.py` & `imat-3.2.3/iMaT/__main__.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/analysis/functions.py` & `imat-3.2.3/iMaT/src/analysis/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/analysis/main.py` & `imat-3.2.3/iMaT/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/analysis/utils.py` & `imat-3.2.3/iMaT/src/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/cli/menu_constructors.py` & `imat-3.2.3/iMaT/src/cli/menu_constructors.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/cli/menu_entries.py` & `imat-3.2.3/iMaT/src/cli/menu_entries.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/constants.py` & `imat-3.2.3/iMaT/src/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 
 EXAMPLE_SCORES_DICT is a dictionary containing data about example scores. Each entry includes the title of the score,
 the URL where the score can be found, and the subcorpus the score belongs to. This dictionary is used to provide users
 with a selection of example scores for analysis.
 """
 
 TITLE_TEXT = (
-    '\nI-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"\n\n'
+    '\nI-MaT - Interactive Music Analysis Tool, v3.2.3, (2023). Project: "Computer-Assisted Music Analysis"\n\n'
     'Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany\n\n'
-    'MIT License, Copyright (c) 2023 S.O. Eck.\n\n'
+    'MIT License, Copyright (c) 2023-2024 S.O. Eck.\n\n'
     '----------------------------------------------------------------------\n'
 )
 
 KEYS_LIST = [
     ["C-Major", "C"],
     ["G-Major", "G"],
     ["D-Major", "D"],
```

### Comparing `imat-3.2.2/iMaT/src/conversion/main.py` & `imat-3.2.3/iMaT/src/conversion/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/conversion/utils.py` & `imat-3.2.3/iMaT/src/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/m21_environment/main.py` & `imat-3.2.3/iMaT/src/m21_environment/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                 ["Instructions",
                  "A new window will open after you press Enter. "
                  "In this window, navigate to the desired directory and select it."]
             ]
         }
         display_menu_print_textblock(directoryScratch_dict)
         directoryScratch = askdirectory()
+        directoryScratch = os.path.normpath(directoryScratch)
         us["directoryScratch"] = directoryScratch
         us["graphicsPath"] = directoryScratch
 
         # Prompt user for musescoreDirectPNGPath and musicxmlPath
         musescore_path_dict = {
             "menu_displayed_text": [
                 "-- File Selection for MuseScore --",
```

### Comparing `imat-3.2.2/iMaT/src/pattern_search/functions.py` & `imat-3.2.3/iMaT/src/pattern_search/functions.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/pattern_search/main.py` & `imat-3.2.3/iMaT/src/pattern_search/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/pattern_search/utils.py` & `imat-3.2.3/iMaT/src/pattern_search/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/score_selection/main.py` & `imat-3.2.3/iMaT/src/score_selection/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/score_selection/name_parts.py` & `imat-3.2.3/iMaT/src/score_selection/name_parts.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/score_selection/select_parts_and_measures.py` & `imat-3.2.3/iMaT/src/score_selection/select_parts_and_measures.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/main.py` & `imat-3.2.3/iMaT/src/tokenization/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/refine_results/absolute_duration.py` & `imat-3.2.3/iMaT/src/tokenization/refine_results/absolute_duration.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py` & `imat-3.2.3/iMaT/src/tokenization/refine_results/calculate_pitch_intervals.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/refine_results/remove_prefixes.py` & `imat-3.2.3/iMaT/src/tokenization/refine_results/remove_prefixes.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/refine_results/tokens_to_txt.py` & `imat-3.2.3/iMaT/src/tokenization/refine_results/tokens_to_txt.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/tokenization/utils.py` & `imat-3.2.3/iMaT/src/tokenization/utils.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/utils/error_handling.py` & `imat-3.2.3/iMaT/src/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/utils/misc.py` & `imat-3.2.3/iMaT/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/visualizations/analysis_results_graphs.py` & `imat-3.2.3/iMaT/src/visualizations/analysis_results_graphs.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/visualizations/m21_integrated.py` & `imat-3.2.3/iMaT/src/visualizations/m21_integrated.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/iMaT/src/visualizations/main.py` & `imat-3.2.3/iMaT/src/visualizations/main.py`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/imat.egg-info/PKG-INFO` & `imat-3.2.3/imat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imat
-Version: 3.2.2
+Version: 3.2.3
 Summary: Interactive Music Analysis Tool (I-MaT)
 Home-page: https://github.com/sebastian-eck/I-MaT
 Author: Sebastian Oliver Eck
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -21,16 +21,32 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Education
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Text Processing :: Linguistic
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 License-File: LICENSE.txt
+Requires-Dist: numpy~=1.23.5
+Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: pandas~=2.0.2
+Requires-Dist: music21~=8.3.0
+Requires-Dist: miditok~=2.0.6
+Requires-Dist: tokenizers~=0.13.3
+Requires-Dist: requests~=2.31.0
+Requires-Dist: openpyxl~=3.1.2
+Requires-Dist: tqdm~=4.65.0
+Requires-Dist: seaborn~=0.12.2
+Requires-Dist: scipy~=1.10.1
+Provides-Extra: doc
+Requires-Dist: sphinx<7.0.0; extra == "doc"
+Requires-Dist: sphinxcontrib-napoleon~=0.7; extra == "doc"
+Requires-Dist: sphinx-autobuild; extra == "doc"
+Requires-Dist: myst_parser; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=1.2.0; extra == "doc"
 
 # The Interactive Music Analysis Tool (I-MaT)
 
 I-MaT is an innovative tool designed to facilitate in-depth musical analysis through an easy-to-use interface. I-MaT offers a comprehensive set of functionalities allowing for the examination of musical pieces from a wide range of perspectives. The documentation (available on [readthedocs.io](https://i-mat.readthedocs.io/en/latest/)) serves as a comprehensive guide, aiming to provide you with insights into I-MaT's functionalities and its modular concept, and assist both first-time users and experienced researchers in using the tool effectively.
 
 The sections contained within the documentation provide detailed information on how to use the Interactive Music Analysis Tool, from [downloading and the installation](https://i-mat.readthedocs.io/en/latest/getting_started.html), to [contribution and code extension](https://i-mat.readthedocs.io/en/latest/contribute.html), to its application in music analysis. Furthermore, you will find a detailed descriptions of I-MaT's [source code](https://i-mat.readthedocs.io/en/latest/module_files/src.html), explaining the different packages' and modules' content that make up the tool.
 
@@ -80,19 +96,19 @@
 
 1. The first objective was to design an easily accessible tool with a well-structured interface, further lowering the barrier for musicology students to engage with methods from digital musicology.
 2. The second objective was to further refine and modularize I-MaT’s program code, to create a modular and flexible tool that could effortlessly be extended by either adding new functionalities offered by already integrated modules (such as music21 and MidiTok), or by incorporating new python packages related to digital musicology or other relevant fields, e.g., computational linguistics.
 
 ## I-MaT: Features and Accessibility
 
 ```
-I-MaT - Interactive Music Analysis Tool, v3.2.1, (2023). Project: "Computer-Assisted Music Analysis"
+I-MaT - Interactive Music Analysis Tool, v3.2.3, (2023). Project: "Computer-Assisted Music Analysis"
 
 Department of Musicology Weimar-Jena, University of Music Franz Liszt Weimar, Germany
 
-MIT License, Copyright (c) 2023 S.O. Eck.
+MIT License, Copyright (c) 2023-2024 S.O. Eck.
 
 ----------------------------------------------------------------------
 
 LOCATION: Start Menu
 
 Please make a selection from the options below by entering the entry index number:
```

### Comparing `imat-3.2.2/imat.egg-info/SOURCES.txt` & `imat-3.2.3/imat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imat-3.2.2/setup.py` & `imat-3.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     include_package_data=True,
     name='imat',
-    version='3.2.2',
+    version='3.2.3',
     author='Sebastian Oliver Eck',
     url="https://github.com/sebastian-eck/I-MaT",
     description='Interactive Music Analysis Tool (I-MaT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT License",
     packages=setuptools.find_packages(),
```

