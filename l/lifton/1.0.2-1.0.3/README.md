# Comparing `tmp/lifton-1.0.2.tar.gz` & `tmp/lifton-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifton-1.0.2.tar", last modified: Wed May  8 22:06:44 2024, max compression
+gzip compressed data, was "lifton-1.0.3.tar", last modified: Wed May 29 14:32:18 2024, max compression
```

## Comparing `lifton-1.0.2.tar` & `lifton-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752896 lifton-1.0.2/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34599 2024-01-03 16:41:07.000000 lifton-1.0.2/LICENSE
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752298 lifton-1.0.2/Lifton.egg-info/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29602 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/PKG-INFO
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1336 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/SOURCES.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/dependency_links.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       46 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/entry_points.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      168 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/requires.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        7 2024-05-08 22:06:44.000000 lifton-1.0.2/Lifton.egg-info/top_level.txt
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29602 2024-05-08 22:06:44.752620 lifton-1.0.2/PKG-INFO
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    28941 2024-05-08 21:36:41.000000 lifton-1.0.2/README.md
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.745715 lifton-1.0.2/lifton/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       23 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     8659 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/align.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6640 2024-04-25 20:36:02.000000 lifton-1.0.2/lifton/annotation.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2620 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/extract_sequence.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1823 2024-04-24 16:55:38.000000 lifton-1.0.2/lifton/get_id_fraction.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      578 2024-01-17 14:20:47.000000 lifton-1.0.2/lifton/intervals.py
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.751541 lifton-1.0.2/lifton/liftoff/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        0 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    13175 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/align_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      597 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/aligned_seg.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    10276 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/extract_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      190 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/feature_hierarchy.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    19044 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/find_best_mapping.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9361 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/fix_overlapping_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5664 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/lift_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    15486 2024-04-24 10:49:54.000000 lifton-1.0.2/lifton/liftoff/liftoff_main.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4032 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/liftoff_utils.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5206 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/liftover_types.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     3945 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/merge_lifted_features.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      372 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/new_feature.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    14008 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/polish.py
-drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-08 22:06:44.752090 lifton-1.0.2/lifton/liftoff/tests/
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/__init__.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2058 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/test_advanced.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1895 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/tests/test_basic.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5428 2023-12-18 15:30:14.000000 lifton-1.0.2/lifton/liftoff/write_new_gff.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20403 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34486 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton_class.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20759 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/lifton_utils.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      233 2024-01-22 16:32:54.000000 lifton-1.0.2/lifton/logger.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     7585 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/protein_maximization.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5764 2024-04-23 23:08:43.000000 lifton-1.0.2/lifton/run_evaluation.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9031 2024-04-24 10:52:31.000000 lifton-1.0.2/lifton/run_liftoff.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6350 2024-05-08 21:36:41.000000 lifton-1.0.2/lifton/run_miniprot.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5595 2024-04-20 04:47:17.000000 lifton-1.0.2/lifton/stats.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4191 2024-04-23 23:08:43.000000 lifton-1.0.2/lifton/variants.py
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)       38 2024-05-08 22:06:44.752955 lifton-1.0.2/setup.cfg
--rw-r--r--   0 chaokuan-hao   (501) staff       (20)      865 2024-05-08 21:36:41.000000 lifton-1.0.2/setup.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-29 14:32:18.775534 lifton-1.0.3/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34599 2024-01-03 16:41:07.000000 lifton-1.0.3/LICENSE
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-29 14:32:18.774929 lifton-1.0.3/Lifton.egg-info/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29262 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/PKG-INFO
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1336 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/SOURCES.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/dependency_links.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       46 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/entry_points.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      182 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/requires.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        7 2024-05-29 14:32:18.000000 lifton-1.0.3/Lifton.egg-info/top_level.txt
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    29262 2024-05-29 14:32:18.775272 lifton-1.0.3/PKG-INFO
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    28572 2024-05-29 14:32:07.000000 lifton-1.0.3/README.md
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-29 14:32:18.769098 lifton-1.0.3/lifton/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       23 2024-05-29 14:32:07.000000 lifton-1.0.3/lifton/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     8659 2024-04-20 04:47:17.000000 lifton-1.0.3/lifton/align.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6640 2024-04-25 20:36:02.000000 lifton-1.0.3/lifton/annotation.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2620 2024-04-20 04:47:17.000000 lifton-1.0.3/lifton/extract_sequence.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1823 2024-04-24 16:55:38.000000 lifton-1.0.3/lifton/get_id_fraction.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      578 2024-01-17 14:20:47.000000 lifton-1.0.3/lifton/intervals.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-29 14:32:18.774217 lifton-1.0.3/lifton/liftoff/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        0 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    13175 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/align_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      597 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/aligned_seg.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    10276 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/extract_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      190 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/feature_hierarchy.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    19044 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/find_best_mapping.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9361 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/fix_overlapping_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5664 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/lift_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    15486 2024-04-24 10:49:54.000000 lifton-1.0.3/lifton/liftoff/liftoff_main.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4032 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/liftoff_utils.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5206 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/liftover_types.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     3945 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/merge_lifted_features.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      372 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/new_feature.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    14008 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/polish.py
+drwxr-xr-x   0 chaokuan-hao   (501) staff       (20)        0 2024-05-29 14:32:18.774726 lifton-1.0.3/lifton/liftoff/tests/
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)        1 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/tests/__init__.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     2058 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/tests/test_advanced.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     1895 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/tests/test_basic.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5428 2023-12-18 15:30:14.000000 lifton-1.0.3/lifton/liftoff/write_new_gff.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20486 2024-05-29 14:32:07.000000 lifton-1.0.3/lifton/lifton.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    34486 2024-05-08 21:36:41.000000 lifton-1.0.3/lifton/lifton_class.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)    20759 2024-05-08 21:36:41.000000 lifton-1.0.3/lifton/lifton_utils.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      233 2024-01-22 16:32:54.000000 lifton-1.0.3/lifton/logger.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     7585 2024-04-20 04:47:17.000000 lifton-1.0.3/lifton/protein_maximization.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5764 2024-04-23 23:08:43.000000 lifton-1.0.3/lifton/run_evaluation.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     9173 2024-05-29 14:32:07.000000 lifton-1.0.3/lifton/run_liftoff.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     6350 2024-05-08 21:36:41.000000 lifton-1.0.3/lifton/run_miniprot.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     5595 2024-04-20 04:47:17.000000 lifton-1.0.3/lifton/stats.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)     4191 2024-04-23 23:08:43.000000 lifton-1.0.3/lifton/variants.py
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)       38 2024-05-29 14:32:18.775582 lifton-1.0.3/setup.cfg
+-rw-r--r--   0 chaokuan-hao   (501) staff       (20)      882 2024-05-29 14:32:07.000000 lifton-1.0.3/setup.py
```

### Comparing `lifton-1.0.2/LICENSE` & `lifton-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/Lifton.egg-info/PKG-INFO` & `lifton-1.0.3/Lifton.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.2
+Version: 1.0.3
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: biopython>=1.76
 Requires-Dist: cigar>=0.1.3
 Requires-Dist: parasail>=1.2.4
 Requires-Dist: intervaltree>=3.1.0
 Requires-Dist: interlap>=0.2.6
-Requires-Dist: networkx>=2.4
+Requires-Dist: networkx>=3.3
 Requires-Dist: pyfaidx>=0.5.8
 Requires-Dist: pysam>=0.19.1
 Requires-Dist: gffutils>=0.10.1
 Requires-Dist: ujson>=3.2.0
+Requires-Dist: pytest>=7.0.0
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/LiftOn/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 <a class="reference external image-reference" href="https://img.shields.io/badge/License-GPLv3-yellow.svg"><img alt="https://img.shields.io/badge/License-GPLv3-yellow.svg" src="https://img.shields.io/badge/License-GPLv3-yellow.svg"></a>
 <a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.1.0.0-blue"></a>
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
@@ -134,27 +135,14 @@
 </dl>
 </li>
 </ul>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
-<section id="cite-us" class="">
-<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
-<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv coming soon</b>.
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
-
-<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
-
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
-</a>
-</p><div class="line-block">
-<div class="line"><br></div>
-</div>
-</section>
 <section id="user-support" class="">
 <h2>User support<a class="headerlink" href="#user-support" title="Permalink to this heading">#</a></h2>
 <p>Please go through the <a class="reference internal" href="#table-of-contents"><span class="std std-ref">documentation</span></a> below first. If you have questions about using the package, a bug report, or a feature request, please use the GitHub issue tracker here:</p>
 <p><a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn/issues">https://github.com/Kuanhao-Chao/LiftOn/issues</a></p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
@@ -245,19 +233,27 @@
 <p>The LiftOn <em>chaining algorithm</em> now does not support multi-threading. This functionality stands as our next targeted feature on the development horizon!</p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 </section>
 
-        
 
-## <a name="citation"></a>Citation<a class="headerlink" href="#citation" title="Permalink to this heading">#</a>
+<section id="cite-us" class="">
+<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
+<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv</b>, doi: https://doi.org/10.1101/2024.05.16.593026, 2024.
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
 
+<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
 
-Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a tool to improve annotations for protein-coding genes during the lift-over process.", <i>bioRxiv</i> <b>2023.07.27.550754</b>, doi: [https://doi.org/10.1101/2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
+</a>
+</p><div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
 
 <br>
 <br>
 <br>
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/jhu-logo-dark.png">
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.2 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.3 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy>=1.22.0 Requires-Dist:
 biopython>=1.76 Requires-Dist: cigar>=0.1.3 Requires-Dist: parasail>=1.2.4
 Requires-Dist: intervaltree>=3.1.0 Requires-Dist: interlap>=0.2.6 Requires-
-Dist: networkx>=2.4 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
-Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0[My Logo]
+Dist: networkx>=3.3 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0 Requires-Dist:
+pytest>=7.0.0[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_o_w_n_l_o_a_d_s_/_K_u_a_n_h_a_o_-_C_h_a_o_/_l_i_f_t_o_n_/
 _t_o_t_a_l_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_g_i_t_h_u_b_&_l_a_b_e_l_=_D_o_w_n_l_o_a_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_p_l_a_t_f_o_r_m_-_m_a_c_O_S___/_L_i_n_u_x_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_l_a_b_._r_e_s_e_a_r_c_h_._g_o_o_g_l_e_._c_o_m_/
 _a_s_s_e_t_s_/_c_o_l_a_b_-_b_a_d_g_e_._s_v_g_]
@@ -100,21 +101,14 @@
                3. reference AAnnnnoottaattiioonn RA in GFF3 format.
     *   OOuuttppuutt:
                1. LiftOn annotation file, AAnnnnoottaattiioonn TA, in GFF3 format.
                2. Protein sequence identities & mutation types
                3. Features with extra copies
                4. Unmapped features
 
-********** CCiittee uuss_## **********
-Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
-Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
-improve genome annotation with LiftOn." bbiiooRRxxiivv ccoommiinngg ssoooonn.
-Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
-annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
-
 ********** UUsseerr ssuuppppoorrtt_## **********
 Please go through the _d_o_c_u_m_e_n_t_a_t_i_o_n below first. If you have questions about
 using the package, a bug report, or a feature request, please use the GitHub
 issue tracker here:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_K_u_a_n_h_a_o_-_C_h_a_o_/_L_i_f_t_O_n_/_i_s_s_u_e_s
 
 ********** KKeeyy ccoonnttrriibbuuttoorrss_## **********
@@ -169,14 +163,19 @@
 transcripts.
 DNA- and protein-based methods still have some limitations. We are developing a
 module to merge the LiftOn annotation with the released curated annotations to
 generate better annotations.
 The LiftOn cchhaaiinniinngg aallggoorriitthhmm now does not support multi-threading. This
 functionality stands as our next targeted feature on the development horizon!
 
-## Citation_# Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a
-tool to improve annotations for protein-coding genes during the lift-over
-process.", bioRxiv 22002233..0077..2277..555500775544, doi: [https://doi.org/10.1101/
-2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+********** CCiittee uuss_## **********
+Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
+Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
+improve genome annotation with LiftOn." bbiiooRRxxiivv, doi: https://doi.org/10.1101/
+2024.05.16.593026, 2024.
+Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
+annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
+
+
 
 
 [My Logo]
```

### Comparing `lifton-1.0.2/Lifton.egg-info/SOURCES.txt` & `lifton-1.0.3/Lifton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/PKG-INFO` & `lifton-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: lifton
-Version: 1.0.2
+Version: 1.0.3
 Summary: Combining DNA and protein alignments to improve genome annotation with LiftOn
 Home-page: https://github.com/Kuanhao-Chao/Lifton
 Author: Kuan-Hao Chao
 Author-email: kh.chao@cs.jhu.edu
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: biopython>=1.76
 Requires-Dist: cigar>=0.1.3
 Requires-Dist: parasail>=1.2.4
 Requires-Dist: intervaltree>=3.1.0
 Requires-Dist: interlap>=0.2.6
-Requires-Dist: networkx>=2.4
+Requires-Dist: networkx>=3.3
 Requires-Dist: pyfaidx>=0.5.8
 Requires-Dist: pysam>=0.19.1
 Requires-Dist: gffutils>=0.10.1
 Requires-Dist: ujson>=3.2.0
+Requires-Dist: pytest>=7.0.0
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/LiftOn/LiftOn_color.png" style="width:90%">
 
 <div class="content">
 <a class="reference external image-reference" href="https://img.shields.io/badge/License-GPLv3-yellow.svg"><img alt="https://img.shields.io/badge/License-GPLv3-yellow.svg" src="https://img.shields.io/badge/License-GPLv3-yellow.svg"></a>
 <a class="reference external image-reference" href="https://img.shields.io/badge/version-v.0.0.1-blue"><img alt="https://img.shields.io/badge/version-v.0.0.1-blue" src="https://img.shields.io/badge/version-v.1.0.0-blue"></a>
 <a class="reference external image-reference" href="https://pepy.tech/project/lifton"><img alt="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads" src="https://static.pepy.tech/personalized-badge/lifton?period=total&amp;units=abbreviation&amp;left_color=grey&amp;right_color=blue&amp;left_text=PyPi%20downloads"></a>
@@ -134,27 +135,14 @@
 </dl>
 </li>
 </ul>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
-<section id="cite-us" class="">
-<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
-<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv coming soon</b>.
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
-
-<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
-
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
-</a>
-</p><div class="line-block">
-<div class="line"><br></div>
-</div>
-</section>
 <section id="user-support" class="">
 <h2>User support<a class="headerlink" href="#user-support" title="Permalink to this heading">#</a></h2>
 <p>Please go through the <a class="reference internal" href="#table-of-contents"><span class="std std-ref">documentation</span></a> below first. If you have questions about using the package, a bug report, or a feature request, please use the GitHub issue tracker here:</p>
 <p><a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn/issues">https://github.com/Kuanhao-Chao/LiftOn/issues</a></p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
@@ -245,19 +233,27 @@
 <p>The LiftOn <em>chaining algorithm</em> now does not support multi-threading. This functionality stands as our next targeted feature on the development horizon!</p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 </section>
 
-        
 
-## <a name="citation"></a>Citation<a class="headerlink" href="#citation" title="Permalink to this heading">#</a>
+<section id="cite-us" class="">
+<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
+<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv</b>, doi: https://doi.org/10.1101/2024.05.16.593026, 2024.
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
 
+<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
 
-Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a tool to improve annotations for protein-coding genes during the lift-over process.", <i>bioRxiv</i> <b>2023.07.27.550754</b>, doi: [https://doi.org/10.1101/2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
+</a>
+</p><div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
 
 <br>
 <br>
 <br>
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/jhu-logo-dark.png">
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: lifton Version: 1.0.2 Summary: Combining DNA and
+Metadata-Version: 2.1 Name: lifton Version: 1.0.3 Summary: Combining DNA and
 protein alignments to improve genome annotation with LiftOn Home-page: https://
 github.com/Kuanhao-Chao/Lifton Author: Kuan-Hao Chao Author-email:
 kh.chao@cs.jhu.edu Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy>=1.22.0 Requires-Dist:
 biopython>=1.76 Requires-Dist: cigar>=0.1.3 Requires-Dist: parasail>=1.2.4
 Requires-Dist: intervaltree>=3.1.0 Requires-Dist: interlap>=0.2.6 Requires-
-Dist: networkx>=2.4 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
-Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0[My Logo]
+Dist: networkx>=3.3 Requires-Dist: pyfaidx>=0.5.8 Requires-Dist: pysam>=0.19.1
+Requires-Dist: gffutils>=0.10.1 Requires-Dist: ujson>=3.2.0 Requires-Dist:
+pytest>=7.0.0[My Logo]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_G_P_L_v_3_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_v_e_r_s_i_o_n_-_v_._0_._0_._1_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
 _l_i_f_t_o_n_?_p_e_r_i_o_d_=_t_o_t_a_l_&_u_n_i_t_s_=_a_b_b_r_e_v_i_a_t_i_o_n_&_l_e_f_t___c_o_l_o_r_=_g_r_e_y_&_r_i_g_h_t___c_o_l_o_r_=_b_l_u_e_&_l_e_f_t___t_e_x_t_=_P_y_P_i_%_2_0_d_o_w_n_l_o_a_d_s_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_o_w_n_l_o_a_d_s_/_K_u_a_n_h_a_o_-_C_h_a_o_/_l_i_f_t_o_n_/
 _t_o_t_a_l_._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_g_i_t_h_u_b_&_l_a_b_e_l_=_D_o_w_n_l_o_a_d_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_p_l_a_t_f_o_r_m_-_m_a_c_O_S___/_L_i_n_u_x_-_g_r_e_e_n_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_l_a_b_._r_e_s_e_a_r_c_h_._g_o_o_g_l_e_._c_o_m_/
 _a_s_s_e_t_s_/_c_o_l_a_b_-_b_a_d_g_e_._s_v_g_]
@@ -100,21 +101,14 @@
                3. reference AAnnnnoottaattiioonn RA in GFF3 format.
     *   OOuuttppuutt:
                1. LiftOn annotation file, AAnnnnoottaattiioonn TA, in GFF3 format.
                2. Protein sequence identities & mutation types
                3. Features with extra copies
                4. Unmapped features
 
-********** CCiittee uuss_## **********
-Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
-Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
-improve genome annotation with LiftOn." bbiiooRRxxiivv ccoommiinngg ssoooonn.
-Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
-annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
-
 ********** UUsseerr ssuuppppoorrtt_## **********
 Please go through the _d_o_c_u_m_e_n_t_a_t_i_o_n below first. If you have questions about
 using the package, a bug report, or a feature request, please use the GitHub
 issue tracker here:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_K_u_a_n_h_a_o_-_C_h_a_o_/_L_i_f_t_O_n_/_i_s_s_u_e_s
 
 ********** KKeeyy ccoonnttrriibbuuttoorrss_## **********
@@ -169,14 +163,19 @@
 transcripts.
 DNA- and protein-based methods still have some limitations. We are developing a
 module to merge the LiftOn annotation with the released curated annotations to
 generate better annotations.
 The LiftOn cchhaaiinniinngg aallggoorriitthhmm now does not support multi-threading. This
 functionality stands as our next targeted feature on the development horizon!
 
-## Citation_# Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a
-tool to improve annotations for protein-coding genes during the lift-over
-process.", bioRxiv 22002233..0077..2277..555500775544, doi: [https://doi.org/10.1101/
-2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+********** CCiittee uuss_## **********
+Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
+Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
+improve genome annotation with LiftOn." bbiiooRRxxiivv, doi: https://doi.org/10.1101/
+2024.05.16.593026, 2024.
+Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
+annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
+
+
 
 
 [My Logo]
```

### Comparing `lifton-1.0.2/README.md` & `lifton-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,27 +112,14 @@
 </dl>
 </li>
 </ul>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
-<section id="cite-us" class="">
-<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
-<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv coming soon</b>.
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
-
-<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
-
-<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
-</a>
-</p><div class="line-block">
-<div class="line"><br></div>
-</div>
-</section>
 <section id="user-support" class="">
 <h2>User support<a class="headerlink" href="#user-support" title="Permalink to this heading">#</a></h2>
 <p>Please go through the <a class="reference internal" href="#table-of-contents"><span class="std std-ref">documentation</span></a> below first. If you have questions about using the package, a bug report, or a feature request, please use the GitHub issue tracker here:</p>
 <p><a class="reference external" href="https://github.com/Kuanhao-Chao/LiftOn/issues">https://github.com/Kuanhao-Chao/LiftOn/issues</a></p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
@@ -223,19 +210,27 @@
 <p>The LiftOn <em>chaining algorithm</em> now does not support multi-threading. This functionality stands as our next targeted feature on the development horizon!</p>
 <div class="line-block">
 <div class="line"><br></div>
 </div>
 </section>
 </section>
 
-        
 
-## <a name="citation"></a>Citation<a class="headerlink" href="#citation" title="Permalink to this heading">#</a>
+<section id="cite-us" class="">
+<h2>Cite us<a class="headerlink" href="#cite-us" title="Permalink to this heading">#</a></h2>
+<p>Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela Pertea, and Steven L. Salzberg. <i>"Combining DNA and protein alignments to improve genome annotation with LiftOn."</i> <b>bioRxiv</b>, doi: https://doi.org/10.1101/2024.05.16.593026, 2024.
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg> </a> </p>
 
+<p>Alaina Shumate, and Steven L. Salzberg. <i>"Liftoff: accurate mapping of gene annotations."</i> <b>Bioinformatics</b> 37.12 (2021): 1639-1643.
 
-Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a tool to improve annotations for protein-coding genes during the lift-over process.", <i>bioRxiv</i> <b>2023.07.27.550754</b>, doi: [https://doi.org/10.1101/2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+<a href="https://doi.org/10.1093/bioinformatics/btaa1016" target="_blank"> <svg xmlns="http://www.w3.org/2000/svg" aria-hidden="true" x="0px" y="0px" viewBox="0 0 100 100" width="15" height="15" class="icon outbound"><path fill="currentColor" d="M18.8,85.1h56l0,0c2.2,0,4-1.8,4-4v-32h-8v28h-48v-48h28v-8h-32l0,0c-2.2,0-4,1.8-4,4v56C14.8,83.3,16.6,85.1,18.8,85.1z"></path> <polygon fill="currentColor" points="45.7,48.7 51.3,54.3 77.2,28.5 77.2,37.2 85.2,37.2 85.2,14.9 62.8,14.9 62.8,22.9 71.5,22.9"></polygon></svg>
+</a>
+</p><div class="line-block">
+<div class="line"><br></div>
+</div>
+</section>
 
 <br>
 <br>
 <br>
 
 <img alt="My Logo" class="logo header-image only-light align-center" src="https://storage.googleapis.com/storage.khchao.com/figures/jhu-logo-dark.png">
```

#### html2text {}

```diff
@@ -92,21 +92,14 @@
                3. reference AAnnnnoottaattiioonn RA in GFF3 format.
     *   OOuuttppuutt:
                1. LiftOn annotation file, AAnnnnoottaattiioonn TA, in GFF3 format.
                2. Protein sequence identities & mutation types
                3. Features with extra copies
                4. Unmapped features
 
-********** CCiittee uuss_## **********
-Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
-Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
-improve genome annotation with LiftOn." bbiiooRRxxiivv ccoommiinngg ssoooonn.
-Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
-annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
-
 ********** UUsseerr ssuuppppoorrtt_## **********
 Please go through the _d_o_c_u_m_e_n_t_a_t_i_o_n below first. If you have questions about
 using the package, a bug report, or a feature request, please use the GitHub
 issue tracker here:
 _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_K_u_a_n_h_a_o_-_C_h_a_o_/_L_i_f_t_O_n_/_i_s_s_u_e_s
 
 ********** KKeeyy ccoonnttrriibbuuttoorrss_## **********
@@ -161,14 +154,19 @@
 transcripts.
 DNA- and protein-based methods still have some limitations. We are developing a
 module to merge the LiftOn annotation with the released curated annotations to
 generate better annotations.
 The LiftOn cchhaaiinniinngg aallggoorriitthhmm now does not support multi-threading. This
 functionality stands as our next targeted feature on the development horizon!
 
-## Citation_# Kuan-Hao Chao*, Mihaela Pertea, Steven L Salzberg*, "LiftOn: a
-tool to improve annotations for protein-coding genes during the lift-over
-process.", bioRxiv 22002233..0077..2277..555500775544, doi: [https://doi.org/10.1101/
-2023.07.27.550754](https://doi.org/10.1101/2023.07.27.550754), 2023
+********** CCiittee uuss_## **********
+Kua-Hao Chao, Jakob M. Heinz, Celine Hoh, Alan Mao, Alaina Shumate, Mihaela
+Pertea, and Steven L. Salzberg. "Combining DNA and protein alignments to
+improve genome annotation with LiftOn." bbiiooRRxxiivv, doi: https://doi.org/10.1101/
+2024.05.16.593026, 2024.
+Alaina Shumate, and Steven L. Salzberg. "Liftoff: accurate mapping of gene
+annotations." BBiiooiinnffoorrmmaattiiccss 37.12 (2021): 1639-1643.
+
+
 
 
 [My Logo]
```

### Comparing `lifton-1.0.2/lifton/align.py` & `lifton-1.0.3/lifton/align.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/annotation.py` & `lifton-1.0.3/lifton/annotation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/extract_sequence.py` & `lifton-1.0.3/lifton/extract_sequence.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/get_id_fraction.py` & `lifton-1.0.3/lifton/get_id_fraction.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/intervals.py` & `lifton-1.0.3/lifton/intervals.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/align_features.py` & `lifton-1.0.3/lifton/liftoff/align_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/aligned_seg.py` & `lifton-1.0.3/lifton/liftoff/aligned_seg.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/extract_features.py` & `lifton-1.0.3/lifton/liftoff/extract_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/find_best_mapping.py` & `lifton-1.0.3/lifton/liftoff/find_best_mapping.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/fix_overlapping_features.py` & `lifton-1.0.3/lifton/liftoff/fix_overlapping_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/lift_features.py` & `lifton-1.0.3/lifton/liftoff/lift_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/liftoff_main.py` & `lifton-1.0.3/lifton/liftoff/liftoff_main.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/liftoff_utils.py` & `lifton-1.0.3/lifton/liftoff/liftoff_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/liftover_types.py` & `lifton-1.0.3/lifton/liftoff/liftover_types.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/merge_lifted_features.py` & `lifton-1.0.3/lifton/liftoff/merge_lifted_features.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/polish.py` & `lifton-1.0.3/lifton/liftoff/polish.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/tests/test_advanced.py` & `lifton-1.0.3/lifton/liftoff/tests/test_advanced.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/tests/test_basic.py` & `lifton-1.0.3/lifton/liftoff/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/liftoff/write_new_gff.py` & `lifton-1.0.3/lifton/liftoff/write_new_gff.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/lifton.py` & `lifton-1.0.3/lifton/lifton.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 def parse_args(arglist):
     parser = argparse.ArgumentParser(description='Lift features from one genome assembly to another')
     parser.add_argument('target', help='target fasta genome to lift genes to')
     parser.add_argument('reference', help='reference fasta genome to lift genes from')
     parser.add_argument('-E', '--evaluation', help='Run LiftOn in evaluation mode', action='store_true', default = False)
     parser.add_argument('-EL', '--evaluation-liftoff-chm13', help='Run LiftOn in evaluation mode', action='store_true', default = False)
     parser.add_argument('-c', '--write_chains', help='Write chaining files', action='store_true', default = True)
+    parser.add_argument('--no-orf-search', help='Do not perform open reading frame search', action='store_true', default = False)
     parser_outgrp = args_outgrp(parser)
     parser_aligngrp = args_aligngrp(parser)
     args_optional(parser)
     referencegrp = parser.add_argument_group('* Required input (Reference annotation)')    
     referencegrp.add_argument(
         '-g', '--reference-annotation', metavar='GFF',  required=True,
         help='the reference annotation file to lift over in GFF or GTF format (or) '
@@ -341,12 +342,11 @@
     ██║     ██║██╔════╝╚══██╔══╝██╔═══██╗████╗  ██║
     ██║     ██║█████╗     ██║   ██║   ██║██╔██╗ ██║
     ██║     ██║██╔══╝     ██║   ██║   ██║██║╚██╗██║
     ███████╗██║██║        ██║   ╚██████╔╝██║ ╚████║
     ╚══════╝╚═╝╚═╝        ╚═╝    ╚═════╝ ╚═╝  ╚═══╝
     '''
     print(banner, file=sys.stderr)
-    print(f"{__version__}\n", file=sys.stderr)
     args = parse_args(arglist)
     if not run_miniprot.check_miniprot_installed(): 
         sys.exit("miniprot is not installed. Please install miniprot before running LiftOn.")
     run_all_lifton_steps(args)
```

### Comparing `lifton-1.0.2/lifton/lifton_class.py` & `lifton-1.0.3/lifton/lifton_class.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/lifton_utils.py` & `lifton-1.0.3/lifton/lifton_utils.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/protein_maximization.py` & `lifton-1.0.3/lifton/protein_maximization.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/run_evaluation.py` & `lifton-1.0.3/lifton/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/run_liftoff.py` & `lifton-1.0.3/lifton/run_liftoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,18 @@
     else:
         if ENTRY_FEATURE: # Gene (1st) features with direct exons 
             ref_trans_id = ref_gene_id
         else: # Transcript features with direct exons 
             ref_gene_id, ref_trans_id = lifton_utils.get_ref_ids_liftoff(ref_features_dict, lifton_gene.entry.id, locus.id)
         lifton_status = lifton_class.Lifton_Status()
         lifton_status.annotation = "Liftoff"
+        try: # Test if the reference transcript exists. Skip if not.
+            ref_db[ref_trans_id]
+        except:
+            return None
         lifton_trans, cds_num = lifton_add_trans_exon_cds(lifton_gene, locus, ref_db, l_feature_db, ref_trans_id)
         if cds_num > 0:
             process_liftoff_with_protein(locus, lifton_gene, lifton_trans,
                                         ref_id_2_m_id_trans_dict, m_feature_db, tree_dict,
                                         tgt_fai, ref_trans_id, ref_proteins, ref_trans,
                                         fw_chain, args.write_chains, lifton_status, args.debug)
         lifton_trans_aln, lifton_aa_aln = lifton_gene.orf_search_protein(lifton_trans.entry.id, ref_trans_id, tgt_fai, ref_proteins, ref_trans, lifton_status)
```

### Comparing `lifton-1.0.2/lifton/run_miniprot.py` & `lifton-1.0.3/lifton/run_miniprot.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/stats.py` & `lifton-1.0.3/lifton/stats.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/lifton/variants.py` & `lifton-1.0.3/lifton/variants.py`

 * *Files identical despite different names*

### Comparing `lifton-1.0.2/setup.py` & `lifton-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 from pathlib import Path
 
 this_directory = Path(__file__).resolve().parent
 long_description = (this_directory / "./README.md").read_text()
 setuptools.setup(
 	name="lifton",
-	version="1.0.2",
+	version="1.0.3",
 	author="Kuan-Hao Chao",
 	author_email="kh.chao@cs.jhu.edu",
 	description="Combining DNA and protein alignments to improve genome annotation with LiftOn",
 	url="https://github.com/Kuanhao-Chao/Lifton",
-	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=2.4', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0'],
+	install_requires=['numpy>= 1.22.0', "biopython>=1.76", "cigar>=0.1.3", "parasail>=1.2.4", 'intervaltree>=3.1.0', 'interlap>=0.2.6', 'networkx>=3.3', 'pyfaidx>=0.5.8', 'pysam>=0.19.1', 'gffutils>=0.10.1', 'ujson>=3.2.0', 'pytest>=7.0.0'],
 	python_requires='>=3.6',
 	packages=setuptools.find_packages(),
 	entry_points={'console_scripts': ['lifton = lifton.lifton:main'], },
         long_description=long_description,
         long_description_content_type='text/markdown'
 )
```

