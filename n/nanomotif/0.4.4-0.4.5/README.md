# Comparing `tmp/nanomotif-0.4.4.tar.gz` & `tmp/nanomotif-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.4.4.tar", last modified: Mon May 27 13:18:00 2024, max compression
+gzip compressed data, was "nanomotif-0.4.5.tar", last modified: Wed May 29 08:37:28 2024, max compression
```

## Comparing `nanomotif-0.4.4.tar` & `nanomotif-0.4.5.tar`

### file list

```diff
@@ -1,72 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-27 13:17:48.000000 nanomotif-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-27 13:18:00.877487 nanomotif-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-27 13:17:48.000000 nanomotif-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.837487 nanomotif-0.4.4/nanomotif/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/bin_consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.841487 nanomotif-0.4.4/nanomotif/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/binnary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/dataload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.841487 nanomotif-0.4.4/nanomotif/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-27 13:17:48.000000 nanomotif-0.4.4/nanomotif/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20007 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.873487 nanomotif-0.4.4/nanomotif/mtase_linker/
--rw-r--r--   0 runner    (1001) docker     (127)     9801 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/MTase_linker.smk
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/mtase_linker/setup.smk
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/old_search_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/scoremotifs.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-27 13:17:49.000000 nanomotif-0.4.4/nanomotif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/nanomotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 13:18:00.000000 nanomotif-0.4.4/nanomotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:18:00.877487 nanomotif-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 13:17:49.000000 nanomotif-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.873487 nanomotif-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:18:00.877487 nanomotif-0.4.4/tests/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_data_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_generate_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/binnary/test_write_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_dataload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_motif_find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:17:49.000000 nanomotif-0.4.4/tests/test_motif_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 08:37:23.000000 nanomotif-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-29 08:37:28.235812 nanomotif-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-29 08:37:23.000000 nanomotif-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.191812 nanomotif-0.4.5/nanomotif/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/bin_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.195812 nanomotif-0.4.5/nanomotif/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/dataload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.195812 nanomotif-0.4.5/nanomotif/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20007 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.231812 nanomotif-0.4.5/nanomotif/mtase_linker/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/old_search_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/scoremotifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/nanomotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:37:28.235812 nanomotif-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 08:37:23.000000 nanomotif-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.231812 nanomotif-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/tests/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_data_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_generate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_write_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_dataload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_motif_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_motif_score.py
```

### Comparing `nanomotif-0.4.4/LICENSE` & `nanomotif-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/PKG-INFO` & `nanomotif-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.4
+Version: 0.4.5
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -16,16 +16,15 @@
 Requires-Dist: networkx>=3.1
 Requires-Dist: pyarrow>=15.0.2
 Requires-Dist: Bio>=1.6.2
 Requires-Dist: snakemake>=7.32.4
 Requires-Dist: progressbar2>=3.53.1
 
 # Nanomotif
-
-#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/nanomotif/badges/version.svg)](https://anaconda.org/bioconda/nanomotif)      [![PyPI version](https://badge.fury.io/py/nanomotif.svg)](https://badge.fury.io/py/nanomotif)
 
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.4/README.md` & `nanomotif-0.4.5/nanomotif.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,30 @@
-# Nanomotif
+Metadata-Version: 2.1
+Name: nanomotif
+Version: 0.4.5
+Summary: Identifying methlyation motifs in nanopore data
+Author: AAU_DarkScience
+Author-email: shei@bio.aau.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: wheel
+Requires-Dist: requests
+Requires-Dist: numpy>=1.24.4
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: polars>=0.19
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: networkx>=3.1
+Requires-Dist: pyarrow>=15.0.2
+Requires-Dist: Bio>=1.6.2
+Requires-Dist: snakemake>=7.32.4
+Requires-Dist: progressbar2>=3.53.1
 
-#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+# Nanomotif
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/nanomotif/badges/version.svg)](https://anaconda.org/bioconda/nanomotif)      [![PyPI version](https://badge.fury.io/py/nanomotif.svg)](https://badge.fury.io/py/nanomotif)
 
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.4/nanomotif/argparser.py` & `nanomotif-0.4.5/nanomotif/argparser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/bin_consensus.py` & `nanomotif-0.4.5/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/analysis.py` & `nanomotif-0.4.5/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.5/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.5/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.5/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/logging.py` & `nanomotif-0.4.5/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/scoring.py` & `nanomotif-0.4.5/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/binnary/utils.py` & `nanomotif-0.4.5/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/candidate.py` & `nanomotif-0.4.5/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/constants.py` & `nanomotif-0.4.5/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/dataload.py` & `nanomotif-0.4.5/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/datasets.py` & `nanomotif-0.4.5/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/evaluate.py` & `nanomotif-0.4.5/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/feature.py` & `nanomotif-0.4.5/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/main.py` & `nanomotif-0.4.5/nanomotif/main.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/model.py` & `nanomotif-0.4.5/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.5/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.5/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/old_search_method.py` & `nanomotif-0.4.5/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/parallel.py` & `nanomotif-0.4.5/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/postprocess.py` & `nanomotif-0.4.5/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/scoremotifs.py` & `nanomotif-0.4.5/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/seq.py` & `nanomotif-0.4.5/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif/utils.py` & `nanomotif-0.4.5/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,9 @@
-Metadata-Version: 2.1
-Name: nanomotif
-Version: 0.4.4
-Summary: Identifying methlyation motifs in nanopore data
-Author: AAU_DarkScience
-Author-email: shei@bio.aau.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: wheel
-Requires-Dist: requests
-Requires-Dist: numpy>=1.24.4
-Requires-Dist: pandas>=2.0.2
-Requires-Dist: polars>=0.19
-Requires-Dist: scipy>=1.10.1
-Requires-Dist: networkx>=3.1
-Requires-Dist: pyarrow>=15.0.2
-Requires-Dist: Bio>=1.6.2
-Requires-Dist: snakemake>=7.32.4
-Requires-Dist: progressbar2>=3.53.1
-
 # Nanomotif
-
-#### *OBS: Bioconda is currently down for pushing new versions, we therefore recommend using pip for installing Nanomotif, see [here](https://nanomotif.readthedocs.io/en/latest/installation.html#local-environment)*
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/nanomotif/badges/version.svg)](https://anaconda.org/bioconda/nanomotif)      [![PyPI version](https://badge.fury.io/py/nanomotif.svg)](https://badge.fury.io/py/nanomotif)
 
 Nanomotif is a Python package designed to explore methylation in prokaryotic genomes using Nanopore sequencing. Nanomotif is a fast, scalable, and sensitive tool for identification and utilization of methylation motifs in monocultures and metagenomic samples.
   - [Overview](#nanomotif-offers)
   - [Documentation](#documentation)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Citation](#citation)
```

### Comparing `nanomotif-0.4.4/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.5/nanomotif.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,19 +35,17 @@
 nanomotif/binnary/include_contigs.py
 nanomotif/binnary/logging.py
 nanomotif/binnary/scoring.py
 nanomotif/binnary/utils.py
 nanomotif/datasets/geobacillus-contig-bin.tsv
 nanomotif/datasets/geobacillus-plasmids.assembly.fasta
 nanomotif/datasets/geobacillus-plasmids.pileup.bed
-nanomotif/mtase_linker/MTase_linker.smk
 nanomotif/mtase_linker/__init__.py
 nanomotif/mtase_linker/command.py
 nanomotif/mtase_linker/dependencies.py
-nanomotif/mtase_linker/setup.smk
 tests/__init__.py
 tests/test_candidate.py
 tests/test_dataload.py
 tests/test_motif_find.py
 tests/test_motif_score.py
 tests/binnary/__init__.py
 tests/binnary/conftest.py
```

### Comparing `nanomotif-0.4.4/setup.py` & `nanomotif-0.4.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     author='AAU_DarkScience',
     author_email='shei@bio.aau.com',
     license='MIT',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
-    package_data={'nanomotif': ['datasets/*'], '':['*.smk']},
+    package_data={'nanomotif': ['datasets/*'], '':['*.smk'], '':['*.yaml']},
     zip_safe=False,
     install_requires=[
         "wheel",
         "requests",
         "numpy>=1.24.4",
         "pandas>=2.0.2",
         "polars>=0.19",
```

### Comparing `nanomotif-0.4.4/tests/binnary/conftest.py` & `nanomotif-0.4.5/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.5/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.5/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.5/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.5/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_generate_output.py` & `nanomotif-0.4.5/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.5/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_scoring.py` & `nanomotif-0.4.5/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_utils.py` & `nanomotif-0.4.5/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/binnary/test_write_bins.py` & `nanomotif-0.4.5/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/test_candidate.py` & `nanomotif-0.4.5/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/test_dataload.py` & `nanomotif-0.4.5/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.4/tests/test_motif_find.py` & `nanomotif-0.4.5/tests/test_motif_find.py`

 * *Files identical despite different names*

