# Comparing `tmp/alphabase-1.2.3.tar.gz` & `tmp/alphabase-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphabase-1.2.3.tar", last modified: Fri Mar 22 19:16:57 2024, max compression
+gzip compressed data, was "alphabase-1.2.4.tar", last modified: Wed May 29 14:36:44 2024, max compression
```

## Comparing `alphabase-1.2.3.tar` & `alphabase-1.2.4.tar`

### file list

```diff
@@ -1,105 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.559087 alphabase-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 19:16:39.000000 alphabase-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-03-22 19:16:39.000000 alphabase-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 19:16:39.000000 alphabase-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-22 19:16:57.555087 alphabase-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-03-22 19:16:39.000000 alphabase-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.539087 alphabase-1.2.3/alphabase/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.539087 alphabase-1.2.3/alphabase/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)    36454 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.539087 alphabase-1.2.3/alphabase/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/aa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/atom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.543087 alphabase-1.2.3/alphabase/constants/const_files/
--rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/__emass_element.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   542725 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/__used_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/amino_acid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/common_constants.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)   153267 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/contaminants.fasta
--rw-r--r--   0 runner    (1001) docker     (127)   262552 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/modification.tsv
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/nist_element.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/protease.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/psm_reader.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    21208 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/const_files/quant_reader_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/isotope.py
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/constants/modification.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.543087 alphabase-1.2.3/alphabase/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18953 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/hdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.547087 alphabase-1.2.3/alphabase/io/psm_reader/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/alphapept_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/dia_psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/dia_search_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/maxquant_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/msfragger_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/pfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/psm_reader/psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/io/tempmmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.547087 alphabase-1.2.3/alphabase/peptide/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/peptide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48481 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/peptide/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/peptide/mass_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/peptide/mobility.py
--rw-r--r--   0 runner    (1001) docker     (127)    19936 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/peptide/precursor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.547087 alphabase-1.2.3/alphabase/protein/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46941 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/protein/fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/protein/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/protein/lcp_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/protein/protein_level_decoy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.547087 alphabase-1.2.3/alphabase/psm_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/alphapept_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/dia_psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/maxquant_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/msfragger_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/pfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19355 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6631 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/psm_reader/sage_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.535087 alphabase-1.2.3/alphabase/quantification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.547087 alphabase-1.2.3/alphabase/quantification/quant_reader/
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/config_dict_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/longformat_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/plexdia_reformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/quant_reader_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/quantreader_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/table_reformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/quantification/quant_reader/wideformat_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.551087 alphabase-1.2.3/alphabase/scoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/scoring/fdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/scoring/feature_extraction_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/scoring/ml_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.551087 alphabase-1.2.3/alphabase/spectral_library/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26758 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/decoy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15950 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/spectral_library/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.551087 alphabase-1.2.3/alphabase/statistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/statistics/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-22 19:16:39.000000 alphabase-1.2.3/alphabase/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.539087 alphabase-1.2.3/alphabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13959 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 19:16:57.000000 alphabase-1.2.3/alphabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 19:16:57.559087 alphabase-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-22 19:16:39.000000 alphabase-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:57.551087 alphabase-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 19:16:39.000000 alphabase-1.2.3/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.359095 alphabase-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 14:36:19.000000 alphabase-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-29 14:36:19.000000 alphabase-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 14:36:19.000000 alphabase-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14553 2024-05-29 14:36:44.359095 alphabase-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-29 14:36:19.000000 alphabase-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.339094 alphabase-1.2.4/alphabase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.343094 alphabase-1.2.4/alphabase/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.343094 alphabase-1.2.4/alphabase/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/aa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/atom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.347094 alphabase-1.2.4/alphabase/constants/const_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/__emass_element.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   542725 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/__used_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/amino_acid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/common_constants.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   153267 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/contaminants.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)   262552 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/modification.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/nist_element.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/protease.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/psm_reader.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21079 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/const_files/quant_reader_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12370 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/constants/modification.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.347094 alphabase-1.2.4/alphabase/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18528 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/io/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/io/tempmmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.347094 alphabase-1.2.4/alphabase/peptide/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/peptide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48911 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/peptide/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/peptide/mass_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/peptide/mobility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20507 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/peptide/precursor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.347094 alphabase-1.2.4/alphabase/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46937 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/protein/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/protein/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/protein/lcp_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/protein/protein_level_decoy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.347094 alphabase-1.2.4/alphabase/psm_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/alphapept_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/dia_psm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/maxquant_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/msfragger_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/pfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/psm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/psm_reader/sage_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.339094 alphabase-1.2.4/alphabase/quantification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.351095 alphabase-1.2.4/alphabase/quantification/quant_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/config_dict_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/longformat_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/plexdia_reformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/quant_reader_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/quantreader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/table_reformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/quantification/quant_reader/wideformat_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.351095 alphabase-1.2.4/alphabase/spectral_library/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25977 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/decoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/spectral_library/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 14:36:19.000000 alphabase-1.2.4/alphabase/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.351095 alphabase-1.2.4/alphabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14553 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 14:36:44.000000 alphabase-1.2.4/alphabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 14:36:19.000000 alphabase-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 14:36:44.359095 alphabase-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-29 14:36:19.000000 alphabase-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:44.351095 alphabase-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 14:36:19.000000 alphabase-1.2.4/tests/test_gui.py
```

### Comparing `alphabase-1.2.3/LICENSE` & `alphabase-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/LICENSE.txt` & `alphabase-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/PKG-INFO` & `alphabase-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabase
-Version: 1.2.3
+Version: 1.2.4
 Summary: An infrastructure Python package of the AlphaX ecosystem
 Home-page: https://github.com/MannLabs/alphabase
 Author: Mann Labs
 Author-email: jalew188@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -33,22 +33,23 @@
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 Requires-Dist: regex
 Requires-Dist: dask
 Requires-Dist: dask_expr
 Requires-Dist: pyahocorasick
+Requires-Dist: pyteomics
+Requires-Dist: lxml
 Requires-Dist: pywin32; sys_platform == "win32"
 Provides-Extra: development-stable
 Requires-Dist: jupyter; extra == "development-stable"
 Requires-Dist: twine; extra == "development-stable"
 Requires-Dist: bumpversion; extra == "development-stable"
 Requires-Dist: pipdeptree; extra == "development-stable"
 Requires-Dist: ipykernel; extra == "development-stable"
-Requires-Dist: nbdev; extra == "development-stable"
 Requires-Dist: pyteomics; extra == "development-stable"
 Requires-Dist: scikit-learn; extra == "development-stable"
 Requires-Dist: matplotlib; extra == "development-stable"
 Requires-Dist: autodocsumm; extra == "development-stable"
 Requires-Dist: myst_parser; extra == "development-stable"
 Requires-Dist: sphinx; extra == "development-stable"
 Requires-Dist: nbsphinx; extra == "development-stable"
@@ -65,21 +66,22 @@
 Requires-Dist: h5py; extra == "development-stable"
 Requires-Dist: contextlib2; extra == "development-stable"
 Requires-Dist: xxhash; extra == "development-stable"
 Requires-Dist: regex; extra == "development-stable"
 Requires-Dist: pydivsufsort; extra == "development-stable"
 Requires-Dist: pyahocorasick; extra == "development-stable"
 Requires-Dist: pytest; extra == "development-stable"
+Requires-Dist: pre-commit==3.7.0; extra == "development-stable"
+Requires-Dist: nbmake==1.5.3; extra == "development-stable"
 Provides-Extra: development
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
-Requires-Dist: nbdev; extra == "development"
 Requires-Dist: pyteomics; extra == "development"
 Requires-Dist: scikit-learn; extra == "development"
 Requires-Dist: matplotlib; extra == "development"
 Requires-Dist: autodocsumm; extra == "development"
 Requires-Dist: myst_parser; extra == "development"
 Requires-Dist: sphinx; extra == "development"
 Requires-Dist: nbsphinx; extra == "development"
@@ -96,14 +98,16 @@
 Requires-Dist: h5py; extra == "development"
 Requires-Dist: contextlib2; extra == "development"
 Requires-Dist: xxhash; extra == "development"
 Requires-Dist: regex; extra == "development"
 Requires-Dist: pydivsufsort; extra == "development"
 Requires-Dist: pyahocorasick; extra == "development"
 Requires-Dist: pytest; extra == "development"
+Requires-Dist: pre-commit; extra == "development"
+Requires-Dist: nbmake; extra == "development"
 Provides-Extra: stable
 Requires-Dist: numba; extra == "stable"
 Requires-Dist: numpy; extra == "stable"
 Requires-Dist: pyyaml; extra == "stable"
 Requires-Dist: pandas; extra == "stable"
 Requires-Dist: h5py; extra == "stable"
 Requires-Dist: contextlib2; extra == "stable"
@@ -112,14 +116,16 @@
 Requires-Dist: psutil; extra == "stable"
 Requires-Dist: tqdm; extra == "stable"
 Requires-Dist: scikit-learn; extra == "stable"
 Requires-Dist: regex; extra == "stable"
 Requires-Dist: dask; extra == "stable"
 Requires-Dist: dask_expr; extra == "stable"
 Requires-Dist: pyahocorasick; extra == "stable"
+Requires-Dist: pyteomics; extra == "stable"
+Requires-Dist: lxml; extra == "stable"
 
 # AlphaBase
 
 ![Pip installation](https://github.com/MannLabs/alphabase/workflows/Default%20installation%20and%20tests/badge.svg)
 ![PyPi releases](https://github.com/MannLabs/alphabase/workflows/Publish%20on%20PyPi%20and%20release%20on%20GitHub/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/alphabase/badge/?version=latest)](https://alphabase.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/alphabase)](https://pypi.org/project/alphabase)
@@ -311,13 +317,27 @@
 a new [issue](https://github.com/MannLabs/alphabase/issues) or clone the
 repository and create a [pull
 request](https://github.com/MannLabs/alphabase/pulls) with a new branch.
 For an even more interactive participation, check out the
 [discussions](https://github.com/MannLabs/alphabase/discussions) and the
 [the Contributors License Agreement](misc/CLA.md).
 
+### Notes for developers
+#### pre-commit hooks
+It is highly recommended to use the provided pre-commit hooks, as the CI pipeline enforces all checks therein to
+pass in order to merge a branch.
+
+The hooks need to be installed once by
+```bash
+pre-commit install
+```
+You can run the checks yourself using:
+```bash
+pre-commit run --all-files
+```
+
 ------------------------------------------------------------------------
 
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made
 in each version.
```

### Comparing `alphabase-1.2.3/README.md` & `alphabase-1.2.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -192,13 +192,27 @@
 a new [issue](https://github.com/MannLabs/alphabase/issues) or clone the
 repository and create a [pull
 request](https://github.com/MannLabs/alphabase/pulls) with a new branch.
 For an even more interactive participation, check out the
 [discussions](https://github.com/MannLabs/alphabase/discussions) and the
 [the Contributors License Agreement](misc/CLA.md).
 
+### Notes for developers
+#### pre-commit hooks
+It is highly recommended to use the provided pre-commit hooks, as the CI pipeline enforces all checks therein to
+pass in order to merge a branch.
+
+The hooks need to be installed once by
+```bash
+pre-commit install
+```
+You can run the checks yourself using:
+```bash
+pre-commit run --all-files
+```
+
 ------------------------------------------------------------------------
 
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made
 in each version.
```

### Comparing `alphabase-1.2.3/alphabase/__init__.py` & `alphabase-1.2.4/alphabase/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 
 
 __project__ = "alphabase"
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __license__ = "Apache"
 __description__ = "An infrastructure Python package of the AlphaX ecosystem"
 __author__ = "Mann Labs"
 __author_email__ = "jalew188@gmail.com"
 __github__ = "https://github.com/MannLabs/alphabase"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphabase-1.2.3/alphabase/__pycache__/__init__.cpython-39.pyc` & `alphabase-1.2.4/alphabase/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar 22 19:16:39 2024 UTC, .py size: 1394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 17d9 fd65 7205 0000  a..........er...
+00000000: 610d 0d0a 0000 0000 633d 5766 7205 0000  a.......c=Wfr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6700 6407 a201  Z.d.Z.d.Z.g.d...
 00000050: 5a07 6408 5a08 6700 6409 a201 5a09 640a  Z.d.Z.g.d...Z.d.
 00000060: 6701 5a0a 640b 640c 6506 640d 640e 640f  g.Z.d.d.e.d.d.d.
 00000070: 9c05 5a0b 6410 6411 6901 5a0c 6412 5300  ..Z.d.d.i.Z.d.S.
 00000080: 2913 da09 616c 7068 6162 6173 657a 0531  )...alphabasez.1
-00000090: 2e32 2e33 5a06 4170 6163 6865 7a38 416e  .2.3Z.Apachez8An
+00000090: 2e32 2e34 5a06 4170 6163 6865 7a38 416e  .2.4Z.Apachez8An
 000000a0: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
 000000b0: 5079 7468 6f6e 2070 6163 6b61 6765 206f  Python package o
 000000c0: 6620 7468 6520 416c 7068 6158 2065 636f  f the AlphaX eco
 000000d0: 7379 7374 656d 7a09 4d61 6e6e 204c 6162  systemz.Mann Lab
 000000e0: 737a 126a 616c 6577 3138 3840 676d 6169  sz.jalew188@gmai
 000000f0: 6c2e 636f 6d7a 2568 7474 7073 3a2f 2f67  l.comz%https://g
 00000100: 6974 6875 622e 636f 6d2f 4d61 6e6e 4c61  ithub.com/MannLa
```

### Comparing `alphabase-1.2.3/alphabase/constants/_const.py` & `alphabase-1.2.4/alphabase/constants/_const.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import os
 import numpy as np
 
 from alphabase.yaml_utils import load_yaml
 
-CONST_FILE_FOLDER = os.path.join(
-    os.path.dirname(__file__),
-    "const_files"
-)
+CONST_FILE_FOLDER = os.path.join(os.path.dirname(__file__), "const_files")
 
-common_const_dict:dict = load_yaml(
+common_const_dict: dict = load_yaml(
     os.path.join(CONST_FILE_FOLDER, "common_constants.yaml")
 )
 
-# Only applied in peak and fragment dataframes to save RAM. 
+# Only applied in peak and fragment dataframes to save RAM.
 # Using float32 still keeps 0.1 ppm precision in any value range.
 # Default float dtype is "float64" for value calculation and other senarios.
-PEAK_MZ_DTYPE:np.dtype = np.dtype(
-    common_const_dict["PEAK_MZ_DTYPE"]
-).type
-PEAK_INTENSITY_DTYPE:np.dtype = np.dtype(
+PEAK_MZ_DTYPE: np.dtype = np.dtype(common_const_dict["PEAK_MZ_DTYPE"]).type
+PEAK_INTENSITY_DTYPE: np.dtype = np.dtype(
     common_const_dict["PEAK_INTENSITY_DTYPE"]
-).type
+).type
```

### Comparing `alphabase-1.2.3/alphabase/constants/atom.py` & `alphabase-1.2.4/alphabase/constants/atom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 import os
 import numpy as np
 import numba
 import typing
 
 from alphabase.yaml_utils import load_yaml
 
-from alphabase.constants._const import (
-    CONST_FILE_FOLDER,
-    common_const_dict
-)
+from alphabase.constants._const import CONST_FILE_FOLDER, common_const_dict
 
-MASS_PROTON:float = common_const_dict['MASS_PROTON']
-MASS_ISOTOPE:float = common_const_dict['MASS_ISOTOPE']
+MASS_PROTON: float = common_const_dict["MASS_PROTON"]
+MASS_ISOTOPE: float = common_const_dict["MASS_ISOTOPE"]
 
-MAX_ISOTOPE_LEN:int = common_const_dict['MAX_ISOTOPE_LEN']
-EMPTY_DIST:np.ndarray = np.zeros(MAX_ISOTOPE_LEN)
+MAX_ISOTOPE_LEN: int = common_const_dict["MAX_ISOTOPE_LEN"]
+EMPTY_DIST: np.ndarray = np.zeros(MAX_ISOTOPE_LEN)
 EMPTY_DIST[0] = 1
 
+
 @numba.njit
-def truncate_isotope(
-    isotopes: np.ndarray, mono_idx: int
-)->tuple:
-    '''
-    For a given isotope distribution (intensity patterns), 
-    this function truncates the distribution by top 
-    `MAX_ISOTOPE_LEN` neighbors those contain the monoisotopic 
+def truncate_isotope(isotopes: np.ndarray, mono_idx: int) -> tuple:
+    """
+    For a given isotope distribution (intensity patterns),
+    this function truncates the distribution by top
+    `MAX_ISOTOPE_LEN` neighbors those contain the monoisotopic
     peak pointed by `mono_idx`.
 
     Parameters
     ----------
     isotopes : np.ndarray
 
         Isotope patterns with size > `MAX_ISOTOPE_LEN`.
 
     mono_idx : int
 
         Monoisotopic peak position (index) in the isotope patterns
-            
+
     Returns
     -------
     int
-    
+
         the new position of `mono_idx`
 
     int
-    
+
         the start position of the truncated isotopes
 
     int
-    
+
         the end position of the truncated isotopes
-    '''
+    """
     trunc_start = mono_idx - 1
     trunc_end = mono_idx + 1
-    while trunc_start >= 0 and trunc_end < len(isotopes) and (trunc_end-trunc_start-1)<MAX_ISOTOPE_LEN:
+    while (
+        trunc_start >= 0
+        and trunc_end < len(isotopes)
+        and (trunc_end - trunc_start - 1) < MAX_ISOTOPE_LEN
+    ):
         if isotopes[trunc_end] >= isotopes[trunc_start]:
             trunc_end += 1
         else:
             trunc_start -= 1
-    if trunc_end-trunc_start-1 < MAX_ISOTOPE_LEN:
+    if trunc_end - trunc_start - 1 < MAX_ISOTOPE_LEN:
         if trunc_start == -1:
             trunc_end = MAX_ISOTOPE_LEN
         elif trunc_end == len(isotopes):
-            trunc_start = len(isotopes)-MAX_ISOTOPE_LEN-1
-    return mono_idx-trunc_start-1, trunc_start+1, trunc_end
+            trunc_start = len(isotopes) - MAX_ISOTOPE_LEN - 1
+    return mono_idx - trunc_start - 1, trunc_start + 1, trunc_end
+
 
 #: chemical element information in dict defined by `nist_element.yaml`
 CHEM_INFO_DICT = {}
 
 #: {element: mass}
 CHEM_MONO_MASS = {}
 
 #: {element: np.ndarray of abundance distribution}
-CHEM_ISOTOPE_DIST:numba.typed.Dict = numba.typed.Dict.empty(
-    key_type=numba.types.unicode_type,
-    value_type=numba.types.float64[:]
+CHEM_ISOTOPE_DIST: numba.typed.Dict = numba.typed.Dict.empty(
+    key_type=numba.types.unicode_type, value_type=numba.types.float64[:]
 )
 
 #: {element: int (mono position)}
-CHEM_MONO_IDX:numba.typed.Dict = numba.typed.Dict.empty(
-    key_type=numba.types.unicode_type,
-    value_type=numba.types.int64
+CHEM_MONO_IDX: numba.typed.Dict = numba.typed.Dict.empty(
+    key_type=numba.types.unicode_type, value_type=numba.types.int64
 )
 
-MASS_H:int = None
-MASS_C:int = None
-MASS_O:int = None
-MASS_N:int = None
-MASS_H2O:int = None #raise errors if the value is not reset
-MASS_NH3:int = None
+MASS_H: int = None
+MASS_C: int = None
+MASS_O: int = None
+MASS_N: int = None
+MASS_H2O: int = None  # raise errors if the value is not reset
+MASS_NH3: int = None
+
 
-def update_atom_infos(new_atom_info:typing.Dict):
+def update_atom_infos(new_atom_info: typing.Dict):
     """
     Args:
         atom_dict (Dict): Example, replacing N with 15N
           {"N":
             {"abundance": [0.01,0.99]},
             {"mass": [14.00307400443, 15.00010889888]},
           }
     """
     for atom, info in new_atom_info.items():
         CHEM_INFO_DICT[atom] = info
 
     reset_elements()
 
-def reset_elements():
 
+def reset_elements():
     global MASS_C, MASS_H, MASS_O, MASS_N
     global MASS_H2O, MASS_NH3
 
     for elem, items in CHEM_INFO_DICT.items():
-        isotopes = np.array(items['abundance'])
-        masses = np.array(items['mass'])
+        isotopes = np.array(items["abundance"])
+        masses = np.array(items["mass"])
         _sort_idx = np.argsort(masses)
         masses = masses[_sort_idx]
         isotopes = isotopes[_sort_idx]
         _mass_pos = np.round(masses).astype(int)
         _mass_pos = _mass_pos - _mass_pos[0]
         if _mass_pos[-1] - _mass_pos[0] + 1 <= MAX_ISOTOPE_LEN:
             _isos = np.zeros(MAX_ISOTOPE_LEN)
@@ -135,77 +135,68 @@
             mono_idx = np.argmax(_isos)
             CHEM_MONO_MASS[elem] = _masses[mono_idx]
 
             _mono_idx, start, end = truncate_isotope(_isos, mono_idx)
 
             CHEM_ISOTOPE_DIST[elem] = _isos[start:end]
             CHEM_MONO_IDX[elem] = _mono_idx
-    
-    MASS_C = CHEM_MONO_MASS['C']
-    MASS_H = CHEM_MONO_MASS['H']
-    MASS_N = CHEM_MONO_MASS['N']
-    MASS_O = CHEM_MONO_MASS['O']
-    MASS_H2O = CHEM_MONO_MASS['H']*2 + CHEM_MONO_MASS['O']
-    MASS_NH3 = CHEM_MONO_MASS['H']*3 + CHEM_MONO_MASS['N']
-
-def load_elem_yaml(yaml_file:str):
-    '''Load built-in or user-defined element yaml file. Default yaml is: 
-        os.path.join(_base_dir, 'nist_element.yaml')
-    '''
+
+    MASS_C = CHEM_MONO_MASS["C"]
+    MASS_H = CHEM_MONO_MASS["H"]
+    MASS_N = CHEM_MONO_MASS["N"]
+    MASS_O = CHEM_MONO_MASS["O"]
+    MASS_H2O = CHEM_MONO_MASS["H"] * 2 + CHEM_MONO_MASS["O"]
+    MASS_NH3 = CHEM_MONO_MASS["H"] * 3 + CHEM_MONO_MASS["N"]
+
+
+def load_elem_yaml(yaml_file: str):
+    """Load built-in or user-defined element yaml file. Default yaml is:
+    os.path.join(_base_dir, 'nist_element.yaml')
+    """
     global CHEM_INFO_DICT
     global CHEM_MONO_MASS
     global CHEM_ISOTOPE_DIST
     global CHEM_MONO_IDX
 
     CHEM_INFO_DICT = load_yaml(yaml_file)
 
     CHEM_MONO_MASS = {}
     CHEM_ISOTOPE_DIST = numba.typed.Dict.empty(
-        key_type=numba.types.unicode_type,
-        value_type=numba.types.float64[:]
+        key_type=numba.types.unicode_type, value_type=numba.types.float64[:]
     )
-    
+
     CHEM_MONO_IDX = numba.typed.Dict.empty(
-        key_type=numba.types.unicode_type,
-        value_type=numba.types.int64
+        key_type=numba.types.unicode_type, value_type=numba.types.int64
     )
 
     reset_elements()
 
-load_elem_yaml(
-    os.path.join(CONST_FILE_FOLDER,
-        'nist_element.yaml'
-    )
-)
 
-def parse_formula(
-    formula:str
-)->list:
-    '''
-    Given a formula (str, e.g. `H(1)C(2)O(3)`), 
+load_elem_yaml(os.path.join(CONST_FILE_FOLDER, "nist_element.yaml"))
+
+
+def parse_formula(formula: str) -> list:
+    """
+    Given a formula (str, e.g. `H(1)C(2)O(3)`),
     it generates `[('H', 2), ('C', 2), ('O', 1)]`
-    '''
-    if not formula: return []
-    items = [item.split('(') for item in 
-        formula.strip(')').split(')')
-    ]
+    """
+    if not formula:
+        return []
+    items = [item.split("(") for item in formula.strip(")").split(")")]
     return [(elem, int(n)) for elem, n in items]
 
 
-def calc_mass_from_formula(formula:str):
-    '''
+def calc_mass_from_formula(formula: str):
+    """
     Calculates the mass of the formula`
 
     Parameters
     ----------
     formula : str
         e.g. `H(1)C(2)O(3)`
-    
+
     Returns
     -------
     float
         mass of the formula
-    '''
-    return np.sum([
-        CHEM_MONO_MASS[elem]*n 
-        for elem, n in parse_formula(formula)
-    ])
+    """
+    return np.sum([CHEM_MONO_MASS[elem] * n for elem, n in parse_formula(formula)])
```

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/__emass_element.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/__emass_element.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/__used_mod.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/__used_mod.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/amino_acid.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/amino_acid.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 U: 'C(3)H(5)N(1)O(1)Se(1)'
 V: 'C(5)H(9)N(1)O(1)S(0)'
 W: 'C(11)H(10)N(2)O(1)S(0)'
 X: 'C(1000000)'
 Y: 'C(9)H(9)N(1)O(2)S(0)'
 Z: 'C(1000000)'
 # Any other ASCII chars could be the placeholders for future usage.
-# For example: 
+# For example:
 # phospho site-specific search (only lower case 'sty' can be modified)
 # s is S
 s: 'C(3)H(5)N(1)O(2)S(0)'
 # t is T
 t: 'C(4)H(8)N(1)O(5)P(1)'
 # y is Y
-y: 'C(9)H(9)N(1)O(2)S(0)'
+y: 'C(9)H(9)N(1)O(2)S(0)'
```

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/contaminants.fasta` & `alphabase-1.2.4/alphabase/constants/const_files/contaminants.fasta`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/modification.tsv` & `alphabase-1.2.4/alphabase/constants/const_files/modification.tsv`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/nist_element.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/nist_element.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/protease.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/protease.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 thrombin:  '((?<=G)R(?=G))|((?<=[AFGILTVM][AFGILTVWA]P)R(?=[^DE][^DE]))'
 trypsin_full:  '([KR](?=[^P]))|((?<=W)K(?=P))|((?<=M)R(?=P))'
 trypsin_exception:  '((?<=[CD])K(?=D))|((?<=C)K(?=[HY]))|((?<=C)R(?=K))|((?<=R)R(?=[HR]))'
 trypsin_not_p:  '([KR](?=[^P]))'
 trypsin:  '([KR])'
 trypsin/p:  '([KR])'
 non-specific:  '()'
-no-cleave: '_'
+no-cleave: '_'
```

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/psm_reader.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/psm_reader.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,61 +26,61 @@
   rt_unit: minute
   fixed_C57: True
   column_mapping:
     'sequence': 'Sequence'
     'charge': 'Charge'
     'rt': 'Retention time'
     'ccs': 'CCS'
-    'mobility': 
+    'mobility':
       - 'Mobility'
       - 'IonMobility'
       - 'K0' # Bug in MaxQuant? It should be 1/K0
       - '1/K0'
-    'scan_num': 
+    'scan_num':
       - 'Scan number'
       - 'MS/MS scan number'
       - 'Scan index'
     'raw_name': 'Raw file'
     'precursor_mz': 'm/z'
     'score': 'Score'
     'proteins': 'Proteins'
     'genes': ['Gene Names','Gene names']
     'decoy': 'Reverse'
     'intensity': 'Intensity'
 
   modification_mapping:
-    'Dimethyl@K': 
+    'Dimethyl@K':
       - 'K(Dimethyl)'
     'Dimethyl@R':
       - 'R(Dimethyl)'
     'Dimethyl@Any N-term':
       - '(Dimethyl)'
-    'Acetyl@Protein N-term': 
+    'Acetyl@Protein N-term':
       - '_(Acetyl (Protein N-term))'
       - '_(ac)'
-    'Carbamidomethyl@C': 
+    'Carbamidomethyl@C':
       - 'C(Carbamidomethyl (C))'
       - 'C(Carbamidomethyl)'
-    'Oxidation@M': 
+    'Oxidation@M':
       - 'M(Oxidation)'
       - 'M(Oxidation (M))'
       - 'M(ox)'
-    'Phospho@S': 
+    'Phospho@S':
       - 'S(Phospho (S))'
       - 'S(Phospho (ST))'
       - 'S(Phospho (STY))'
       - 'S(ph)'
       - 'pS'
-    'Phospho@T': 
+    'Phospho@T':
       - 'T(Phospho (T))'
       - 'T(Phospho (ST))'
       - 'T(Phospho (STY))'
       - 'T(ph)'
       - 'pT'
-    'Phospho@Y': 
+    'Phospho@Y':
       - 'Y(Phospho (Y))'
       - 'Y(Phospho (STY))'
       - 'Y(ph)'
       - 'pY'
     'Deamidated@N': ['N(Deamidation (NQ))','N(de)']
     'Deamidated@Q': ['Q(Deamidation (NQ))','Q(de)']
     'GlyGly@K': ['K(GlyGly (K))', 'K(gl)']
@@ -183,15 +183,15 @@
     'ccs': 'CCS'
     'precursor_mz': 'PrecursorMz'
     'mobility': ['Mobility','IonMobility','PrecursorIonMobility']
     'proteins': ['Protein Name','ProteinId','ProteinID','ProteinName','ProteinGroup','ProteinGroups']
     'uniprot_ids': ['UniProtIds','UniProtID','UniprotId']
     'genes': ['Genes','Gene','GeneName','GeneNames']
   modification_mapping: 'maxquant'
-  
+
 library_reader_base:
   reader_type: library_reader_base
   rt_unit: irt
   fixed_C57: False
   csv_sep: "\t"
   mod_seq_columns:
     - 'ModifiedPeptideSequence'
@@ -232,8 +232,8 @@
     'raw_name': 'filename'
     'scannr': 'scannr'
     'score': 'sage_discriminant_score'
     'proteins': 'proteins'
     'fdr': 'spectrum_q'
     'peptide_fdr': 'peptide_q'
     'protein_fdr': 'protein_q'
-    'decoy': 'is_decoy'
+    'decoy': 'is_decoy'
```

### Comparing `alphabase-1.2.3/alphabase/constants/const_files/quant_reader_config.yaml` & `alphabase-1.2.4/alphabase/constants/const_files/quant_reader_config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -10,34 +10,34 @@
     precursor_intensity: int_sum
   protein_cols:
    - protein_group
   ion_hierarchy:
     precursor_intensity:
       order: [SEQ, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - naked_sequence
-        CHARGE: 
+        CHARGE:
          - charge
-         
+
   use_iontree: False
 
 
 maxquant_peptides_leading_razor_protein:
   format: widetable
   quant_pre_or_suffix: "Intensity "
   protein_cols:
    - Leading razor protein
   ion_cols:
    - Sequence
   ion_hierarchy:
     sequence_int:
       order: [SEQ, MOD]
       mapping:
-        SEQ: 
+        SEQ:
           - Sequence
         MOD:
           - Mass
   filters:
     reverse:
       param: Reverse
       comparator: "!="
@@ -108,15 +108,15 @@
    - Modifications
    - Charge
 
 
 
 diann_fragion_isotopes_mDIA_raw:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     fragion: Fragment.Quant.Raw
     #Fragment.Quant.Raw
     ms1iso: Ms1.Area
@@ -124,41 +124,41 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Raw: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Raw
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
 
 diann_fragion_isotopes_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     fragion: Fragment.Quant.Corrected
     #Fragment.Quant.Raw
     ms1iso: Ms1.Area
@@ -166,199 +166,199 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Corrected: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Corrected
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
 diann_precursors_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     precursor: Precursor.Quantity
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 diann_precursors_translated_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     precursor: Precursor.Translated
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
 diann_precursors_normalised_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     precursor: Precursor.Normalised
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 diann_precursors_and_ms1_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     precursor: Precursor.Quantity
     ms1iso: Ms1.Area
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1:
           - Stripped.Sequence
   use_iontree: True
   ml_level: CHARGE
 
 
 
 diann_precursors_and_ms1_normalised_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     precursor: Precursor.Normalised
     ms1iso: Ms1.Area
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1:
           - Stripped.Sequence
   use_iontree: True
   ml_level: CHARGE
 
 
 diann_ms1_mDIA:
   format: longtable
-  channel_ID: 
+  channel_ID:
    - Channel.0
    - Channel.4
   sample_ID: Run
   quant_ID:
     ms1iso: Ms1.Area
   protein_cols:
    - Protein.Group
   ion_hierarchy:
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1:
           - Stripped.Sequence
 
 diann_fragion_isotopes:
   format: longtable
   sample_ID: Run
@@ -370,30 +370,30 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Corrected: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Corrected
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
@@ -408,30 +408,30 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Raw: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Raw
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
@@ -446,30 +446,30 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Raw: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Raw
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 
@@ -482,21 +482,21 @@
    - Protein.Group
   split_cols:
     Fragment.Quant.Corrected: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Corrected
   use_iontree: True
   ml_level: CHARGE
 
 
 diann_precursor:
   format: longtable
@@ -587,32 +587,32 @@
    - F.Charge
   split_cols:
     FG.MS1IsotopeIntensities (Measured): ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - ptm_mapped_modseq
-        CHARGE: 
+        CHARGE:
          - FG.Charge
-        FRGION: 
+        FRGION:
          - F.FrgIon
          - F.FrgLossType
          - F.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - ptm_mapped_modseq
-        CHARGE: 
+        CHARGE:
          - FG.Charge
         MS1ISOTOPES:
          - FG.MS1IsotopeIntensities (Measured)
   filters:
     fragion_intensity:
       param: F.PeakArea
       comparator: ">"
@@ -637,32 +637,32 @@
    - F.Charge
   split_cols:
     FG.MS1IsotopeIntensities (Measured): ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
-        FRGION: 
+        FRGION:
          - F.FrgIon
          - F.FrgLossType
          - F.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
         MS1ISOTOPES:
          - FG.MS1IsotopeIntensities (Measured)
   filters:
     fragion_intensity:
       param: F.PeakArea
       comparator: ">"
@@ -670,15 +670,15 @@
   use_iontree: True
   ml_level: CHARGE
   # filters:
   #   decoy_filt:
   #     param: EG.IsDecoy
   #     comparator: "=="
   #     value: False
-  #   shape_quality: 
+  #   shape_quality:
   #     param: FG.ShapeQualityScore (MS2)
   #     comparator: ">"
   #     value: 0.4
   #   fragion_interference:
   #     param: F.PossibleInterference
   #     comparator: "=="
   #     value: False
@@ -699,32 +699,32 @@
    - F.Charge
   split_cols:
     FG.MS1IsotopeIntensities (Measured): ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
-        FRGION: 
+        FRGION:
          - F.FrgIon
          - F.FrgLossType
          - F.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
         MS1ISOTOPES:
          - FG.MS1IsotopeIntensities (Measured)
   filters:
     fragion_intensity:
       param: F.PeakHeight
       comparator: ">"
@@ -749,32 +749,32 @@
    - F.Charge
   split_cols:
     FG.MS1IsotopeIntensities (Measured): ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
-        FRGION: 
+        FRGION:
          - F.FrgIon
          - F.FrgLossType
          - F.Charge
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
         MS1ISOTOPES:
          - FG.MS1IsotopeIntensities (Measured)
   filters:
     fragion_intensity:
       param: F.PeakArea
       comparator: ">"
@@ -783,30 +783,30 @@
       param: EG.UsedForPeptideQuantity
       comparator: "=="
       value: True
     decoy_filt:
       param: EG.IsDecoy
       comparator: "=="
       value: False
-    shape_quality: 
+    shape_quality:
       param: FG.ShapeQualityScore
       comparator: ">"
       value: 0.4
     fragion_interference:
       param: F.PossibleInterference
       comparator: "=="
       value: False
   use_iontree: True
   ml_level: CHARGE
   # filters:
   #   decoy_filt:
   #     param: EG.IsDecoy
   #     comparator: "=="
   #     value: False
-  #   shape_quality: 
+  #   shape_quality:
   #     param: FG.ShapeQualityScore (MS2)
   #     comparator: ">"
   #     value: 0.4
   #   fragion_interference:
   #     param: F.PossibleInterference
   #     comparator: "=="
   #     value: False
@@ -826,21 +826,21 @@
    - F.Charge
   split_cols:
     FG.MS1IsotopeIntensities (Measured): ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - PEP.StrippedSequence
-        MOD: 
+        MOD:
          - EG.ModifiedSequence
-        CHARGE: 
+        CHARGE:
          - FG.Charge
-        FRGION: 
+        FRGION:
          - F.FrgIon
          - F.FrgLossType
   filters:
     used_for_quant:
       param: F.ExcludedFromQuantification
       comparator: "=="
       value: False
@@ -873,15 +873,15 @@
   ion_cols:
    - FG.Id
   filters:
     decoy_filt:
       param: EG.IsDecoy
       comparator: "=="
       value: False
-    shape_quality: 
+    shape_quality:
       param: FG.ShapeQualityScore (MS2)
       comparator: ">"
       value: 0.4
 
 spectronaut_sequence:
   format: longtable
   sample_ID: R.Label
@@ -920,15 +920,15 @@
   ion_cols:
    - EG.ModifiedSequence
    - FG.Charge
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
           - PEP.StrippedSequence
         MOD:
           - EG.ModifiedSequence
         CHARGE:
           - FG.Charge
   use_iontree: True
   ml_level: CHARGE
@@ -940,15 +940,15 @@
     precursor: FG.Quantity
   protein_cols:
    - PG.ProteinGroups
   ion_hierarchy:
     precursor:
       order: [SEQ, MOD, CHARGE]
       mapping:
-        SEQ: 
+        SEQ:
           - PEP.StrippedSequence
         MOD:
           - EG.ModifiedSequence
         CHARGE:
           - FG.Charge
   use_iontree: True
   ml_level: CHARGE
@@ -1012,15 +1012,15 @@
    - Stripped.Sequence
    - Modified.Sequence
    - Precursor.Charge
   ion_hierarchy:
     sequence_int:
       order: [SEQ, MOD]
       mapping:
-        SEQ: 
+        SEQ:
           - Stripped.Sequence
         MOD:
           - Modified.Sequence
         CH:
           - Precursor.Charge
   ml_level: SEQ
   use_iontree: False
@@ -1037,30 +1037,30 @@
    - Genes
   split_cols:
     Fragment.Quant.Raw: ";"
   ion_hierarchy:
     fragion:
       order: [SEQ, MOD, CHARGE, FRGION]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
-        FRGION: 
+        FRGION:
          - Fragment.Quant.Raw
     ms1iso:
       order: [SEQ, MOD, CHARGE, MS1ISOTOPES]
       mapping:
-        SEQ: 
+        SEQ:
          - Stripped.Sequence
-        MOD: 
+        MOD:
          - Modified.Sequence
-        CHARGE: 
+        CHARGE:
          - Precursor.Charge
         MS1ISOTOPES:
          - Precursor.Charge
   use_iontree: True
   ml_level: CHARGE
 
 fragpipe_precursors:
@@ -1070,10 +1070,10 @@
    - Protein
   ion_hierarchy:
     sequence_int:
       order: [SEQ, MOD]
       mapping:
         SEQ:
           - Peptide Sequence
-        MOD: 
+        MOD:
           - Modified Sequence
-  use_iontree: False
+  use_iontree: False
```

### Comparing `alphabase-1.2.3/alphabase/constants/isotope.py` & `alphabase-1.2.4/alphabase/constants/isotope.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 import numba
 import numpy as np
 import typing
 
-from alphabase.constants.element import (
-    MAX_ISOTOPE_LEN, EMPTY_DIST,
-    CHEM_ISOTOPE_DIST, CHEM_MONO_IDX, CHEM_MONO_MASS,
-    truncate_isotope, parse_formula
+from alphabase.constants.atom import (
+    MAX_ISOTOPE_LEN,
+    EMPTY_DIST,
+    CHEM_ISOTOPE_DIST,
+    CHEM_MONO_IDX,
+    truncate_isotope,
+    parse_formula,
 )
 
+
 @numba.njit
 def abundance_convolution(
-    d1:np.ndarray,
-    mono1:int,
-    d2:np.ndarray,
-    mono2:int,
-)->typing.Tuple[np.ndarray, int]:
-    '''
-    If we have two isotope distributions, 
-    we can convolute them into one distribution. 
-    
+    d1: np.ndarray,
+    mono1: int,
+    d2: np.ndarray,
+    mono2: int,
+) -> typing.Tuple[np.ndarray, int]:
+    """
+    If we have two isotope distributions,
+    we can convolute them into one distribution.
+
     Parameters
     ----------
     d1 : np.ndarray
         isotope distribution to convolute
 
     mono1 : int
         mono position of d1.
 
     d2 : np.ndarray
         isotope distribution to convolute
 
     mono2 : int
         mono position of d2
-        
+
     Returns
     -------
     tuple[np.ndarray,int]
         np.ndarray, convoluted isotope distribution
         int, new mono position.
-    '''
+    """
     mono_idx = mono1 + mono2
-    ret = np.zeros(MAX_ISOTOPE_LEN*2-1)
+    ret = np.zeros(MAX_ISOTOPE_LEN * 2 - 1)
     for i in range(len(d1)):
         for j in range(len(d2)):
-            ret[i+j] += d1[i]*d2[j]
+            ret[i + j] += d1[i] * d2[j]
 
     mono_idx, start, end = truncate_isotope(ret, mono_idx)
     return ret[start:end], mono_idx
 
+
 @numba.njit
 def one_element_dist(
     elem: str,
     n: int,
     chem_isotope_dist: numba.typed.Dict,
     chem_mono_idx: numba.typed.Dict,
-)->typing.Tuple[np.ndarray, int]:
-    '''
-    Calculate the isotope distribution for 
+) -> typing.Tuple[np.ndarray, int]:
+    """
+    Calculate the isotope distribution for
     an element and its numbers.
-    
+
     Parameters
     ----------
     elem : str
         element.
 
     n : int
         element number.
@@ -74,203 +79,206 @@
         use `CHEM_MONO_IDX` as parameter.
 
     Returns
     -------
     tuple[np.ndarray, int]
         np.ndarray, isotope distribution of the element.
         int, mono position in the distribution
-    '''
-    if n == 0: return EMPTY_DIST.copy(), 0
-    elif n == 1: return chem_isotope_dist[elem], chem_mono_idx[elem]
-    tmp_dist, mono_idx = one_element_dist(elem, n//2, chem_isotope_dist, chem_mono_idx)
+    """
+    if n == 0:
+        return EMPTY_DIST.copy(), 0
+    elif n == 1:
+        return chem_isotope_dist[elem], chem_mono_idx[elem]
+    tmp_dist, mono_idx = one_element_dist(
+        elem, n // 2, chem_isotope_dist, chem_mono_idx
+    )
     tmp_dist, mono_idx = abundance_convolution(tmp_dist, mono_idx, tmp_dist, mono_idx)
-    if n%2 == 0:
+    if n % 2 == 0:
         return tmp_dist, mono_idx
     else:
-        return abundance_convolution(tmp_dist, mono_idx, chem_isotope_dist[elem], chem_mono_idx[elem])
+        return abundance_convolution(
+            tmp_dist, mono_idx, chem_isotope_dist[elem], chem_mono_idx[elem]
+        )
+
 
-def formula_dist(
-    formula: typing.Union[list, str]
-)->typing.Tuple[np.ndarray, int]:
-    '''
-    Generate the isotope distribution and the mono index for 
+def formula_dist(formula: typing.Union[list, str]) -> typing.Tuple[np.ndarray, int]:
+    """
+    Generate the isotope distribution and the mono index for
     a given formula (as a list, e.g. `[('H', 2), ('C', 2), ('O', 1)]`).
 
     Parameters
     ----------
     formula : Union[list, str]
         chemical formula, could be str or list.
         If str: "H(1)N(2)O(3)".
         If list: "[('H',1),('H',2),('H',3)]".
-            
+
     Returns
     -------
     tuple[np.ndarray,int]
         np.ndarray, isotope distribution
         int, mono position
-    '''
+    """
     if isinstance(formula, str):
         formula = parse_formula(formula)
     calc_dist = EMPTY_DIST.copy()
     mono_idx = 0
     for elem, n in formula:
         _dist, _mono = one_element_dist(elem, n, CHEM_ISOTOPE_DIST, CHEM_MONO_IDX)
         calc_dist, mono_idx = abundance_convolution(calc_dist, mono_idx, _dist, _mono)
     return calc_dist, mono_idx
 
-def _calc_one_elem_cum_dist(
-    element_cum_dist:np.ndarray, 
-    element_cum_mono:np.ndarray
-):
+
+def _calc_one_elem_cum_dist(element_cum_dist: np.ndarray, element_cum_mono: np.ndarray):
     """Pre-build isotope abundance distribution for an element for fast calculation.
     Internel function.
-    
+
     Added information inplace into element_cum_dist and element_cum_mono
 
     Parameters
     ----------
     element_cum_dist : np.ndarray
         Cumulated element abundance distribution
 
     element_cum_mono : np.ndarray
         Cumulated element mono position in the distribution
     """
     for n in range(2, len(element_cum_dist)):
-        (
-            element_cum_dist[n], 
-            element_cum_mono[n]
-        ) = abundance_convolution(
-            element_cum_dist[n-1],
-            element_cum_mono[n-1],
+        (element_cum_dist[n], element_cum_mono[n]) = abundance_convolution(
+            element_cum_dist[n - 1],
+            element_cum_mono[n - 1],
             element_cum_dist[1],
-            element_cum_mono[1]
+            element_cum_mono[1],
         )
 
+
 class IsotopeDistribution:
-    def __init__(self, 
-        max_elem_num_dict:dict = {
-            'C': 2000,
-            'H': 5000,
-            'N': 1000,
-            'O': 1000,
-            'S': 200,
-            'P': 200,
-        }
+    def __init__(
+        self,
+        max_elem_num_dict: dict = {
+            "C": 2000,
+            "H": 5000,
+            "N": 1000,
+            "O": 1000,
+            "S": 200,
+            "P": 200,
+        },
     ):
         """Faster calculation of isotope abundance distribution by pre-building
         isotope distribution tables for most common elements.
 
         We have considered large enough number of elements for shotgun proteomics.
-        We can increase `max_elem_num_dict` to support larger peptide or top-down 
+        We can increase `max_elem_num_dict` to support larger peptide or top-down
         in the future. However, current `MAX_ISOTOPE_LEN` is not suitable for top-down,
         it must be extended to a larger number (100?).
         Note that non-standard amino acids have 1000000 C elements in AlphaBase,
         We clip 1000000 C to the maximal number of C in `max_elem_num_dict`.
         As they have very large masses thus impossible to identify,
         their isotope distributions do not matter.
 
         Parameters
         ----------
         max_elem_num_dict : dict, optional
-            Define the maximal number of the elements. 
-            Defaults to { 'C': 2000, 'H': 5000, 'N': 1000, 'O': 1000, 'S': 200, 'P': 200, } 
-        
+            Define the maximal number of the elements.
+            Defaults to { 'C': 2000, 'H': 5000, 'N': 1000, 'O': 1000, 'S': 200, 'P': 200, }
+
         Attributes
         ----------
-        element_to_cum_dist_dict : dict 
+        element_to_cum_dist_dict : dict
             {element: cumulated isotope distribution array},
-            and the cumulated isotope distribution array is a 2-D float np.ndarray with 
+            and the cumulated isotope distribution array is a 2-D float np.ndarray with
             shape (element_max_number, MAX_ISOTOPE_LEN).
 
         element_to_cum_mono_idx : dict
             {element: mono position array of cumulated isotope distribution},
             and mono position array is a 1-D int np.ndarray.
         """
         self.element_to_cum_dist_dict = {}
         self.element_to_cum_mono_idx = {}
         for elem, n in max_elem_num_dict.items():
-            if n < 2: n = 2
+            if n < 2:
+                n = 2
             self.element_to_cum_dist_dict[elem] = np.zeros((n, MAX_ISOTOPE_LEN))
-            self.element_to_cum_mono_idx[elem] = -np.ones(n,dtype=np.int64)
-            self.element_to_cum_dist_dict[elem][0,:] = EMPTY_DIST
+            self.element_to_cum_mono_idx[elem] = -np.ones(n, dtype=np.int64)
+            self.element_to_cum_dist_dict[elem][0, :] = EMPTY_DIST
             self.element_to_cum_mono_idx[elem][0] = 0
-            self.element_to_cum_dist_dict[elem][1,:] = CHEM_ISOTOPE_DIST[elem]
+            self.element_to_cum_dist_dict[elem][1, :] = CHEM_ISOTOPE_DIST[elem]
             self.element_to_cum_mono_idx[elem][1] = CHEM_MONO_IDX[elem]
             _calc_one_elem_cum_dist(
-                self.element_to_cum_dist_dict[elem],
-                self.element_to_cum_mono_idx[elem]
+                self.element_to_cum_dist_dict[elem], self.element_to_cum_mono_idx[elem]
             )
 
-    def calc_formula_distribution(self,
-        formula: typing.List[typing.Tuple[str,int]],
-    )->typing.Tuple[np.ndarray, int]:
+    def calc_formula_distribution(
+        self,
+        formula: typing.List[typing.Tuple[str, int]],
+    ) -> typing.Tuple[np.ndarray, int]:
         """Calculate isotope abundance distribution for a given formula
 
         Parameters
         ----------
         formula : List[tuple(str,int)]
             chemical formula: "[('H',1),('C',2),('O',3)]".
 
         Returns
         -------
         tuple[np.ndarray, int]
             np.ndarray, isotope abundance distribution
             int, monoisotope position in the distribution array
-    
+
         Examples
         --------
         >>> from alphabase.constants import IsotopeDistribution, parse_formula
         >>> iso = IsotopeDistribution()
         >>> formula = 'C(100)H(100)O(10)Na(1)Fe(1)'
         >>> formula = parse_formula(formula)
         >>> dist, mono = iso.calc_formula_distribution(formula)
         >>> dist
         array([1.92320044e-02, 2.10952666e-02, 3.13753566e-01, 3.42663681e-01,
                 1.95962632e-01, 7.69157517e-02, 2.31993814e-02, 5.71948249e-03,
                 1.19790438e-03, 2.18815385e-04])
-        >>> # Fe's mono position is 2 Da larger than its smallest mass, 
+        >>> # Fe's mono position is 2 Da larger than its smallest mass,
         >>> # so the mono position of this formula shifts by +2 (Da).
-        >>> mono 
+        >>> mono
         2
 
-        >>> formula = 'C(100)H(100)O(10)13C(1)Na(1)' 
+        >>> formula = 'C(100)H(100)O(10)13C(1)Na(1)'
         >>> formula = parse_formula(formula)
         >>> dist, mono = iso.calc_formula_distribution(formula)
         >>> dist
         array([3.29033438e-03, 3.29352217e-01, 3.59329960e-01, 2.01524592e-01,
                 7.71395498e-02, 2.26229845e-02, 5.41229894e-03, 1.09842389e-03,
                 1.94206388e-04, 3.04911585e-05])
         >>> # 13C's mono position is +1 Da shifted
         >>> mono
         1
 
-        >>> formula = 'C(100)H(100)O(10)Na(1)' 
+        >>> formula = 'C(100)H(100)O(10)Na(1)'
         >>> formula = parse_formula(formula)
         >>> dist, mono = iso.calc_formula_distribution(formula)
         >>> dist
         array([3.29033438e-01, 3.60911319e-01, 2.02775462e-01, 7.76884706e-02,
                 2.27963906e-02, 5.45578135e-03, 1.10754072e-03, 1.95857410e-04,
                 3.07552058e-05, 4.35047710e-06])
         >>> # mono position is normal (=0) for regular formulas
         >>> mono
         0
-            
+
         """
         mono = 0
         dist = EMPTY_DIST.copy()
         for elem, n in formula:
             if elem in self.element_to_cum_dist_dict:
                 if n >= len(self.element_to_cum_mono_idx[elem]):
-                    n = len(self.element_to_cum_mono_idx[elem])-1
+                    n = len(self.element_to_cum_mono_idx[elem]) - 1
                 dist, mono = abundance_convolution(
-                    dist, mono,
+                    dist,
+                    mono,
                     self.element_to_cum_dist_dict[elem][n],
                     self.element_to_cum_mono_idx[elem][n],
                 )
             else:
                 dist, mono = abundance_convolution(
-                    dist, mono, *one_element_dist(
-                        elem,n,CHEM_ISOTOPE_DIST, CHEM_MONO_IDX
-                    )
+                    dist,
+                    mono,
+                    *one_element_dist(elem, n, CHEM_ISOTOPE_DIST, CHEM_MONO_IDX),
                 )
         return dist, mono
-
```

### Comparing `alphabase-1.2.3/alphabase/constants/modification.py` & `alphabase-1.2.4/alphabase/constants/modification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,403 +1,411 @@
 import os
 import numba
 import numpy as np
 import pandas as pd
 from typing import Union, List
 
-from alphabase.constants.element import (
-    calc_mass_from_formula, parse_formula,
+from alphabase.constants.atom import (
+    calc_mass_from_formula,
+    parse_formula,
 )
 
 from alphabase.constants._const import CONST_FILE_FOLDER
 
 
 #: Main entry of modification infomation (DataFrame fotmat).
-MOD_DF:pd.DataFrame = pd.DataFrame()
+MOD_DF: pd.DataFrame = pd.DataFrame()
 
 
-MOD_INFO_DICT:dict = {}
+MOD_INFO_DICT: dict = {}
 #: Modification to formula str dict. {mod_name: formula str ('H(1)C(2)O(3)')}
-MOD_CHEM:dict = {}
+MOD_CHEM: dict = {}
 #: Modification to mass dict.
-MOD_MASS:dict = {}
+MOD_MASS: dict = {}
 #: Modification to modification neutral loss dict.
-MOD_LOSS_MASS:dict = {}
-#Modification to formula dict of dict, i.e. {modname: {'C': n, 'H': m, ...}}
-MOD_Composition:dict = {}
+MOD_LOSS_MASS: dict = {}
+# Modification to formula dict of dict, i.e. {modname: {'C': n, 'H': m, ...}}
+MOD_Composition: dict = {}
 #: Modification loss importance
-MOD_LOSS_IMPORTANCE:dict = {}
+MOD_LOSS_IMPORTANCE: dict = {}
+
 
 def update_all_by_MOD_DF():
     """
-    As DataFrame is more conveneint in data operation, 
-    we can also process MOD_DF and then update all global 
+    As DataFrame is more conveneint in data operation,
+    we can also process MOD_DF and then update all global
     modification variables from MOD_DF
     """
-    
+
     MOD_INFO_DICT.clear()
-    MOD_INFO_DICT.update(MOD_DF.to_dict(orient='index'))
+    MOD_INFO_DICT.update(MOD_DF.to_dict(orient="index"))
     MOD_CHEM.clear()
-    MOD_CHEM.update(MOD_DF['composition'].to_dict())
+    MOD_CHEM.update(MOD_DF["composition"].to_dict())
     MOD_MASS.clear()
-    MOD_MASS.update(MOD_DF['mass'].to_dict())
+    MOD_MASS.update(MOD_DF["mass"].to_dict())
     MOD_LOSS_MASS.clear()
-    MOD_LOSS_MASS.update(MOD_DF['modloss'].to_dict())
+    MOD_LOSS_MASS.update(MOD_DF["modloss"].to_dict())
     MOD_LOSS_IMPORTANCE.clear()
-    MOD_LOSS_IMPORTANCE.update(MOD_DF['modloss_importance'].to_dict())
+    MOD_LOSS_IMPORTANCE.update(MOD_DF["modloss_importance"].to_dict())
 
     MOD_Composition.clear()
     for mod, chem in MOD_CHEM.items():
         MOD_Composition[mod] = dict(parse_formula(chem))
 
+
 def add_modifications_for_lower_case_AA():
-    """ Add modifications for lower-case AAs for advanced usages """
+    """Add modifications for lower-case AAs for advanced usages"""
     global MOD_DF
     lower_case_df = MOD_DF.copy()
-    
+
     def _mod_lower_case(modname):
-        modname, site = modname.split('@')
+        modname, site = modname.split("@")
         if len(site) == 1:
-            return modname+'@'+site.lower()
-        elif '^' in site:
-            site = site[0].lower()+site[1:]
-            return modname+'@'+site
+            return modname + "@" + site.lower()
+        elif "^" in site:
+            site = site[0].lower() + site[1:]
+            return modname + "@" + site
         else:
-            return ''
-    lower_case_df['mod_name'] = lower_case_df['mod_name'].apply(_mod_lower_case)
-    lower_case_df = lower_case_df[lower_case_df['mod_name']!='']
-    lower_case_df.set_index('mod_name', drop=False, inplace=True)
-    lower_case_df['lower_case_AA'] = True
-    MOD_DF['lower_case_AA'] = False
+            return ""
+
+    lower_case_df["mod_name"] = lower_case_df["mod_name"].apply(_mod_lower_case)
+    lower_case_df = lower_case_df[lower_case_df["mod_name"] != ""]
+    lower_case_df.set_index("mod_name", drop=False, inplace=True)
+    lower_case_df["lower_case_AA"] = True
+    MOD_DF["lower_case_AA"] = False
     MOD_DF = pd.concat([MOD_DF, lower_case_df])
     update_all_by_MOD_DF()
 
-def keep_modloss_by_importance(modloss_importance_level:float=1.0):
-    MOD_DF['modloss'] = MOD_DF['modloss_original']
-    MOD_DF.loc[MOD_DF.modloss_importance<modloss_importance_level,"modloss"] = 0
+
+def keep_modloss_by_importance(modloss_importance_level: float = 1.0):
+    MOD_DF["modloss"] = MOD_DF["modloss_original"]
+    MOD_DF.loc[MOD_DF.modloss_importance < modloss_importance_level, "modloss"] = 0
     MOD_LOSS_MASS.clear()
-    MOD_LOSS_MASS.update(MOD_DF['modloss'].to_dict())
+    MOD_LOSS_MASS.update(MOD_DF["modloss"].to_dict())
+
 
 def load_mod_df(
-    tsv:str=os.path.join(CONST_FILE_FOLDER, 'modification.tsv'),
+    tsv: str = os.path.join(CONST_FILE_FOLDER, "modification.tsv"),
     *,
     modloss_importance_level=1,
 ):
     global MOD_DF
-    MOD_DF = pd.read_table(tsv,keep_default_na=False)
-    _df = MOD_DF[MOD_DF.mod_name.str.contains(' ', regex=False)].copy()
-    _df["mod_name"] = MOD_DF.mod_name.str.replace(' ', '_', regex=False)
-    MOD_DF = pd.concat(
-        [MOD_DF, _df], ignore_index=True
-    ).drop_duplicates("mod_name")
-    MOD_DF.fillna('',inplace=True)
-    MOD_DF['unimod_id'] = MOD_DF.unimod_id.astype(np.int32)
-    MOD_DF.set_index('mod_name', drop=False, inplace=True)
-    MOD_DF['mass'] = MOD_DF.composition.apply(calc_mass_from_formula)
-    MOD_DF['modloss_original'] = MOD_DF.modloss_composition.apply(calc_mass_from_formula)
-    MOD_DF['modloss'] = MOD_DF['modloss_original']
+    MOD_DF = pd.read_table(tsv, keep_default_na=False)
+    _df = MOD_DF[MOD_DF.mod_name.str.contains(" ", regex=False)].copy()
+    _df["mod_name"] = MOD_DF.mod_name.str.replace(" ", "_", regex=False)
+    MOD_DF = pd.concat([MOD_DF, _df], ignore_index=True).drop_duplicates("mod_name")
+    MOD_DF.fillna("", inplace=True)
+    MOD_DF["unimod_id"] = MOD_DF.unimod_id.astype(np.int32)
+    MOD_DF.set_index("mod_name", drop=False, inplace=True)
+    MOD_DF["mass"] = MOD_DF.composition.apply(calc_mass_from_formula)
+    MOD_DF["modloss_original"] = MOD_DF.modloss_composition.apply(
+        calc_mass_from_formula
+    )
+    MOD_DF["modloss"] = MOD_DF["modloss_original"]
     keep_modloss_by_importance(modloss_importance_level)
     update_all_by_MOD_DF()
-    
+
+
 load_mod_df()
 
+
 def calc_modification_mass(
-    nAA:int, 
-    mod_names:List[str], 
-    mod_sites:List[int]
-)->np.ndarray:
-    '''
-    Calculate modification masses for the given peptide length (`nAA`), 
+    nAA: int, mod_names: List[str], mod_sites: List[int]
+) -> np.ndarray:
+    """
+    Calculate modification masses for the given peptide length (`nAA`),
     and modified site list.
-    
+
     Parameters
     ----------
     nAA : int
         Peptide length
 
     mod_names : list
         List[str]. Modification name list
 
     mod_sites : list
         List[int]. Modification site list corresponding to `mod_names`.
         * `site=0` refers to an N-term modification
         * `site=-1` refers to a C-term modification
         * `1<=site<=peplen` refers to a normal modification
-    
+
     Returns
     -------
     np.ndarray
-        1-D array with length=`nAA`. 
-        Masses of modifications through the peptide, 
+        1-D array with length=`nAA`.
+        Masses of modifications through the peptide,
         `0` if sites has no modifications
-    '''
+    """
     masses = np.zeros(nAA)
     for site, mod in zip(mod_sites, mod_names):
         if site == 0:
             masses[site] += MOD_MASS[mod]
         elif site == -1:
             masses[site] += MOD_MASS[mod]
         else:
-            masses[site-1] += MOD_MASS[mod]
+            masses[site - 1] += MOD_MASS[mod]
     return masses
 
+
 def calc_mod_masses_for_same_len_seqs(
-    nAA:int, 
-    mod_names_list:List[List[str]], 
-    mod_sites_list:List[List[int]]
-)->np.ndarray:
-    '''
+    nAA: int, mod_names_list: List[List[str]], mod_sites_list: List[List[int]]
+) -> np.ndarray:
+    """
     Calculate modification masses for the given peptides with same peptide length (`nAA`).
-    
+
     Parameters
     ----------
     nAA : int
-    
+
         Peptide length
 
     mod_names_list : List[List[str]]
         List (pep_count) of modification list (n_mod on each peptide)
 
     mod_sites_list : List[List[int]]
         List of modification site list corresponding to `mod_names_list`.
         * `site=0` refers to an N-term modification
         * `site=-1` refers to a C-term modification
         * `1<=site<=peplen` refers to a normal modification
-    
+
     Returns
     -------
     np.ndarray
-        2-D array with shape=`(nAA, pep_count or len(mod_names_list)))`. 
-        Masses of modifications through all the peptides, 
+        2-D array with shape=`(nAA, pep_count or len(mod_names_list)))`.
+        Masses of modifications through all the peptides,
         `0` if sites without modifications.
-    '''
-    masses = np.zeros((len(mod_names_list),nAA))
-    for i, (mod_names, mod_sites) in enumerate(
-        zip(mod_names_list, mod_sites_list)
-    ):
-        for mod, site in zip(mod_names, mod_sites): 
+    """
+    masses = np.zeros((len(mod_names_list), nAA))
+    for i, (mod_names, mod_sites) in enumerate(zip(mod_names_list, mod_sites_list)):
+        for mod, site in zip(mod_names, mod_sites):
             if site == 0:
-                masses[i,site] += MOD_MASS[mod]
+                masses[i, site] += MOD_MASS[mod]
             elif site == -1:
-                masses[i,site] += MOD_MASS[mod]
+                masses[i, site] += MOD_MASS[mod]
             else:
-                masses[i,site-1] += MOD_MASS[mod]
+                masses[i, site - 1] += MOD_MASS[mod]
     return masses
 
-def calc_modification_mass_sum(
-    mod_names:List[str]
-)->float:
+
+def calc_modification_mass_sum(mod_names: List[str]) -> float:
     """
-    Calculate summed mass of the given modification 
+    Calculate summed mass of the given modification
     without knowing the sites and peptide length.
     It is useful to calculate peptide mass.
-    
+
     Parameters
     ----------
     mod_names : List[str]
         Modification name list
 
     Returns
     -------
     float
         Total mass
     """
-    return np.sum([
-        MOD_MASS[mod] for mod in mod_names
-    ])
+    return np.sum([MOD_MASS[mod] for mod in mod_names])
 
 
 @numba.jit(nopython=True, nogil=True)
 def _calc_modloss_with_importance(
-    mod_losses: np.ndarray, 
-    _loss_importance: np.ndarray
-)->np.ndarray:
-    '''
-    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T). 
-    Modification with higher `_loss_importance` has higher priorities. 
+    mod_losses: np.ndarray, _loss_importance: np.ndarray
+) -> np.ndarray:
+    """
+    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T).
+    Modification with higher `_loss_importance` has higher priorities.
     For example, `AM(Oxidation@M)S(Phospho@S)...`,
-    importance of Phospho@S > importance of Oxidation@M, so the modloss of 
+    importance of Phospho@S > importance of Oxidation@M, so the modloss of
     b3 ion will be -98 Da, not -64 Da.
-    
+
     Parameters
     ----------
     mod_losses : np.ndarray
         Mod loss masses of each AA position
 
     _loss_importance : np.ndarray
         Mod loss importance of each AA position
-    
+
     Returns
     -------
     np.ndarray
         New mod_loss masses selected by `_loss_importance`
-    '''
+    """
     prev_importance = _loss_importance[0]
     prev_most = 0
-    for i, _curr_imp in enumerate(_loss_importance[1:],1):
+    for i, _curr_imp in enumerate(_loss_importance[1:], 1):
         if _curr_imp > prev_importance:
             prev_most = i
             prev_importance = _curr_imp
         else:
             mod_losses[i] = mod_losses[prev_most]
     return mod_losses
 
+
 def calc_modloss_mass_with_importance(
-    nAA: int, 
-    mod_names: List, 
+    nAA: int,
+    mod_names: List,
     mod_sites: List,
     for_nterm_frag: bool,
-)->np.ndarray:
-    '''
-    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T, 
-    -64 Da for Oxidation@M). Modifications with higher `MOD_LOSS_IMPORTANCE` 
+) -> np.ndarray:
+    """
+    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T,
+    -64 Da for Oxidation@M). Modifications with higher `MOD_LOSS_IMPORTANCE`
     have higher priorities. For example, `AS(Phospho@S)M(Oxidation@M)...`,
-    importance of Phospho@S > importance of Oxidation@M, so the modloss of 
+    importance of Phospho@S > importance of Oxidation@M, so the modloss of
     b3 ion will be -98 Da, not -64 Da.
-    
+
     Parameters
     ----------
     nAA : int
         Peptide length
 
     mod_names : List[str]
         Modification name list
 
     mod_sites : List[int]
-        Modification site list  
+        Modification site list
 
     for_nterm_frag : bool
-        If `True`, the loss will be on the 
-        N-term fragments (mainly `b` ions); 
-        If `False`, the loss will be on the 
+        If `True`, the loss will be on the
+        N-term fragments (mainly `b` ions);
+        If `False`, the loss will be on the
         C-term fragments (mainly `y` ions)
-    
+
     Returns
     -------
     np.ndarray
         mod_loss masses
-    '''
-    if not mod_names: return np.zeros(nAA-1)
-    mod_losses = np.zeros(nAA+2)
+    """
+    if not mod_names:
+        return np.zeros(nAA - 1)
+    mod_losses = np.zeros(nAA + 2)
     mod_losses[mod_sites] = [MOD_LOSS_MASS[mod] for mod in mod_names]
-    _loss_importance = np.zeros(nAA+2)
+    _loss_importance = np.zeros(nAA + 2)
     _loss_importance[mod_sites] = [
-        MOD_LOSS_IMPORTANCE[mod] if mod in MOD_LOSS_IMPORTANCE else 0 
+        MOD_LOSS_IMPORTANCE[mod] if mod in MOD_LOSS_IMPORTANCE else 0
         for mod in mod_names
     ]
-    
+
     # Will not consider the modloss if the corresponding modloss_importance is 0
-    mod_losses[_loss_importance==0] = 0
+    mod_losses[_loss_importance == 0] = 0
 
     if for_nterm_frag:
         return _calc_modloss_with_importance(mod_losses, _loss_importance)[1:-2]
     else:
-        return _calc_modloss_with_importance(mod_losses[::-1], _loss_importance[::-1])[-3:0:-1]
+        return _calc_modloss_with_importance(mod_losses[::-1], _loss_importance[::-1])[
+            -3:0:-1
+        ]
+
 
 @numba.njit
-def _calc_modloss(
-    mod_losses: np.ndarray
-)->np.ndarray:
-    '''
-    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T). 
-    
+def _calc_modloss(mod_losses: np.ndarray) -> np.ndarray:
+    """
+    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T).
+
     Parameters
     ----------
     mod_losses : np.ndarray
         Mod loss masses of each AA position
-    
+
     Returns
     -------
     np.ndarray
-        New mod_loss masses 
-    '''
-    for i, _curr_loss in enumerate(mod_losses[1:],1):
+        New mod_loss masses
+    """
+    for i, _curr_loss in enumerate(mod_losses[1:], 1):
         if _curr_loss == 0:
-            mod_losses[i] = mod_losses[i-1]
+            mod_losses[i] = mod_losses[i - 1]
         else:
             mod_losses[i] = _curr_loss
     return mod_losses
-    
+
+
 def calc_modloss_mass(
-    nAA: int, 
-    mod_names: List, 
+    nAA: int,
+    mod_names: List,
     mod_sites: List,
     for_nterm_frag: bool,
-)->np.ndarray:
-    '''
-    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T, 
+) -> np.ndarray:
+    """
+    Calculate modification loss masses (e.g. -98 Da for Phospho@S/T,
     -64 Da for Oxidation@M). The mod loss mass is calculated by the
-    modification closer to the fragment sites. For example, 
+    modification closer to the fragment sites. For example,
     the modloss of the b3 ion for `AS(Phospho@S)M(Oxidation@M)...`
     will be -64 Da.
-    
+
     Parameters
     ----------
     nAA : int
         Peptide length
 
     mod_names : List[str]
         Modification name list
 
     mod_sites : List[int]
-        Modification site list corresponding 
+        Modification site list corresponding
 
     for_nterm_frag : bool
-        If `True`, the loss will be on the 
-        N-term fragments (mainly `b` ions); 
-        If `False`, the loss will be on the 
+        If `True`, the loss will be on the
+        N-term fragments (mainly `b` ions);
+        If `False`, the loss will be on the
         C-term fragments (mainly `y` ions)
-    
+
     Returns
     -------
     np.ndarray
         mod_loss masses
-    '''
-    if len(mod_names) == 0: return np.zeros(nAA-1)
-    mod_losses = np.zeros(nAA+2)
+    """
+    if len(mod_names) == 0:
+        return np.zeros(nAA - 1)
+    mod_losses = np.zeros(nAA + 2)
     mod_losses[mod_sites] = [MOD_LOSS_MASS[mod] for mod in mod_names]
 
     if for_nterm_frag:
         return _calc_modloss(mod_losses)[1:-2]
     else:
         return _calc_modloss(mod_losses[::-1])[-3:0:-1]
 
+
 def _add_a_new_modification(
-    mod_name:str, composition:str,
-    modloss_composition:str=''
+    mod_name: str, composition: str, modloss_composition: str = ""
 ):
     """
     Add a new modification into :data:`MOD_DF`.
     """
-    MOD_DF.loc[mod_name,[
-        'mod_name','composition','modloss_composition',
-        'classification','unimod_id'
-    ]] = [
-        mod_name, composition, modloss_composition,
-        'User-added', 0
-    ]
-    MOD_DF.loc[mod_name,['mass','modloss']] = (
+    MOD_DF.loc[
+        mod_name,
+        [
+            "mod_name",
+            "composition",
+            "modloss_composition",
+            "classification",
+            "unimod_id",
+        ],
+    ] = [mod_name, composition, modloss_composition, "User-added", 0]
+    MOD_DF.loc[mod_name, ["mass", "modloss"]] = (
         calc_mass_from_formula(composition),
-        calc_mass_from_formula(modloss_composition)
+        calc_mass_from_formula(modloss_composition),
     )
-    if MOD_DF.loc[mod_name, 'modloss'] > 0:
-        MOD_DF.loc[mod_name, 'modloss_importance'] = 1e10
+    if MOD_DF.loc[mod_name, "modloss"] > 0:
+        MOD_DF.loc[mod_name, "modloss_importance"] = 1e10
     MOD_DF.fillna(0, inplace=True)
     # update_all_by_MOD_DF()
 
-def add_new_modifications(new_mods:Union[list,dict]):
+
+def add_new_modifications(new_mods: Union[list, dict]):
     """Add new modifications into :data:`MOD_DF`.
 
     Parameters
     ----------
     new_mods : list or dict
         list of tuples example:
         ```
         [(
-        mod@site:str (e.g. Mod@S), 
+        mod@site:str (e.g. Mod@S),
         composition:str (e.g. "H(4)O(2)"),
         [optional] modloss composition:str (e.g. "H(2)O(1)"),
         ), ...]
         ```,
         dict example:
         ```
         {
```

### Comparing `alphabase-1.2.3/alphabase/io/hdf.py` & `alphabase-1.2.4/alphabase/io/hdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import h5py
 import numpy as np
 import pandas as pd
 import re
 import contextlib
 import time
-import warnings
 
 
 class HDF_Object(object):
-    '''
+    """
     A generic class to access HDF components.
-    '''
+    """
 
     @property
     def read_only(self):
         return self._read_only
 
     @property
     def truncate(self):
@@ -25,26 +24,18 @@
         return self._file_name
 
     @property
     def name(self):
         return self._name
 
     def __eq__(self, other):
-        return (
-            self.file_name == other.self.file_name
-        ) and (
-            self.name == other.name
-        )
+        return (self.file_name == other.self.file_name) and (self.name == other.name)
 
     @contextlib.contextmanager
-    def editing_mode(
-        self,
-        read_only: bool = False,
-        truncate: bool = True
-    ):
+    def editing_mode(self, read_only: bool = False, truncate: bool = True):
         original_read_only = self.read_only
         original_truncate = self.truncate
         try:
             self.set_read_only(read_only)
             self.set_truncate(truncate)
             yield self
         finally:
@@ -78,34 +69,31 @@
         object.__setattr__(self, "_truncate", truncate)
 
     def __setattr__(self, name, value):
         if self.read_only:
             raise AttributeError("Cannot set read-only attributes")
         elif not isinstance(name, str):
             raise KeyError(f"Attribute name '{name}' is not a string")
-        elif not bool(re.match(r'^[a-zA-Z_][\w.-]*$', name)):
+        elif not bool(re.match(r"^[a-zA-Z_][\w.-]*$", name)):
             raise KeyError(f"Invalid attribute name: {name}")
         if (not self.truncate) and (name in self.metadata):
-            raise KeyError(
-                f"Attribute '{name}' cannot be truncated"
-            )
+            raise KeyError(f"Attribute '{name}' cannot be truncated")
         if isinstance(value, (str, bool, int, float)):
             with h5py.File(self.file_name, "a") as hdf_file:
                 hdf_object = hdf_file[self.name]
                 hdf_object.attrs[name] = value
                 object.__setattr__(self, name, value)
         else:
             raise NotImplementedError(
                 f"Type '{type(name)}' is invalid for attribute {name}. "
                 "Only (str, bool, int, float) types are accepted."
             )
 
 
 class HDF_Group(HDF_Object):
-
     def __init__(
         self,
         *,
         file_name: str,
         name: str,
         read_only: bool = True,
         truncate: bool = False,
@@ -154,43 +142,40 @@
 
     @property
     def dataframe_names(self):
         return self.components[2]
 
     @property
     def groups(self):
-        return [
-            self.__getattribute__(name) for name in self.group_names
-        ]
+        return [self.__getattribute__(name) for name in self.group_names]
 
     @property
     def datasets(self):
-        return [
-            self.__getattribute__(name) for name in self.dataset_names
-        ]
+        return [self.__getattribute__(name) for name in self.dataset_names]
 
     @property
     def dataframes(self):
-        return [
-            self.__getattribute__(name) for name in self.dataframe_names
-        ]
+        return [self.__getattribute__(name) for name in self.dataframe_names]
 
     @property
     def components(self):
         group_names = []
         dataset_names = []
         datafame_names = []
         with h5py.File(self.file_name, "a") as hdf_file:
             hdf_object = hdf_file[self.name]
             for name in sorted(hdf_object):
                 if isinstance(hdf_object[name], h5py.Dataset):
                     if not name.endswith("_mmap"):
                         dataset_names.append(name)
                 else:
-                    if name.endswith('_df') or "is_pd_dataframe" in hdf_object[name].attrs:
+                    if (
+                        name.endswith("_df")
+                        or "is_pd_dataframe" in hdf_object[name].attrs
+                    ):
                         datafame_names.append(name)
                     else:
                         group_names.append(name)
         return group_names, dataset_names, datafame_names
 
     def set_read_only(self, read_only: bool = True):
         super().__setattr__(self, "_read_only", read_only)
@@ -212,35 +197,29 @@
 
     def __setattr__(self, name, value):
         try:
             super().__setattr__(name, value)
         except NotImplementedError:
             if not self.truncate:
                 if name in self.group_names:
-                    raise KeyError(
-                        f"Group name '{name}' cannot be truncated"
-                    )
+                    raise KeyError(f"Group name '{name}' cannot be truncated")
                 elif name in self.dataset_names:
-                    raise KeyError(
-                        f"Dataset name '{name}' cannot be truncated"
-                    )
+                    raise KeyError(f"Dataset name '{name}' cannot be truncated")
                 elif name in self.dataframe_names:
-                    raise KeyError(
-                        f"Dataframe name '{name}' cannot be truncated"
-                    )
+                    raise KeyError(f"Dataframe name '{name}' cannot be truncated")
             if isinstance(value, (np.ndarray, pd.core.series.Series)):
                 self.add_dataset(name, value)
             elif isinstance(value, (dict, pd.DataFrame)):
                 self.add_group(name, value)
             else:
                 raise NotImplementedError(
                     f"Type '{type(value)}' is invalid for attribute {name}",
                     "Only (str, bool, int, float, np.ndarray, "
                     "pd.core.series.Series, dict pd.DataFrame) types are "
-                    "accepted."
+                    "accepted.",
                 )
 
     def add_dataset(
         self,
         name: str,
         array: np.ndarray,
     ):
@@ -294,15 +273,15 @@
     ):
         with h5py.File(self.file_name, "a") as hdf_file:
             hdf_object = hdf_file[self.name]
             if name in hdf_object:
                 del hdf_object[name]
             hdf_object.create_group(name)
         if isinstance(group, pd.DataFrame):
-            if not name.endswith('_df'):
+            if not name.endswith("_df"):
                 raise TypeError(f"DataFrame group name `{name}` must end with `_df`")
             group = dict(group)
             # group["is_pd_dataframe"] = True
             new_group = HDF_Dataframe(
                 file_name=self.file_name,
                 name=f"{self.name}/{name}",
                 read_only=self.read_only,
@@ -318,15 +297,14 @@
         for key, value in group.items():
             new_group.__setattr__(key, value)
         new_group.last_updated = time.asctime()
         object.__setattr__(self, name, new_group)
 
 
 class HDF_Dataset(HDF_Object):
-
     def __init__(
         self,
         *,
         file_name: str,
         name: str,
         read_only: bool = True,
         truncate: bool = False,
@@ -367,17 +345,15 @@
             return hdf_object[keys]
 
     def append(self, data):
         if self.read_only:
             raise AttributeError("Cannot append read-only dataset")
         with h5py.File(self.file_name, "a") as hdf_file:
             hdf_object = hdf_file[self.name]
-            new_shape = tuple(
-                [i + j for i, j in zip(self.shape, data.shape)]
-            )
+            new_shape = tuple([i + j for i, j in zip(self.shape, data.shape)])
             old_size = len(self)
             hdf_object.resize(new_shape)
             hdf_object[old_size:] = data
 
     def set_slice(self, slice_selection, values):
         if self.read_only:
             raise AttributeError("Cannot set slice of read-only dataset")
@@ -417,30 +393,23 @@
         if not self.mmap_exists:
             self.create_mmap()
         with h5py.File(self.file_name, "r") as hdf_file:
             subgroup = hdf_file[self.mmap_name]
             offset = subgroup.id.get_offset()
             shape = subgroup.shape
             import mmap
+
             with open(self.file_name, "rb") as raw_hdf_file:
-                mmap_obj = mmap.mmap(
-                    raw_hdf_file.fileno(),
-                    0,
-                    access=mmap.ACCESS_READ
-                )
+                mmap_obj = mmap.mmap(raw_hdf_file.fileno(), 0, access=mmap.ACCESS_READ)
                 return np.frombuffer(
-                    mmap_obj,
-                    dtype=subgroup.dtype,
-                    count=np.prod(shape),
-                    offset=offset
+                    mmap_obj, dtype=subgroup.dtype, count=np.prod(shape), offset=offset
                 ).reshape(shape)
 
 
 class HDF_Dataframe(HDF_Group):
-
     @property
     def dtype(self):
         dtypes = []
         for column_name in self.dataset_names:
             dtype = self.__getattribute__(column_name).dtype
             dtypes.append(dtype)
         return list(dtypes)
@@ -486,27 +455,27 @@
         read_only: bool = True,
         truncate: bool = False,
         delete_existing: bool = False,
     ):
         """HDF file object to load/save the hdf file. It also provides convenient
         attribute-like accesses to operate the data in the HDF object.
 
-        Instead of relying directly on the `h5py` interface, we will use an HDF wrapper 
-        file to provide consistent access to only those specific HDF features we want. 
-        Since components of an HDF file come in three shapes `datasets`, `groups` and `attributes`, 
-        we will first define a generic HDF wrapper object to handle these components. 
-        Once this is done, the HDF wrapper file can be treated as such an object with additional 
+        Instead of relying directly on the `h5py` interface, we will use an HDF wrapper
+        file to provide consistent access to only those specific HDF features we want.
+        Since components of an HDF file come in three shapes `datasets`, `groups` and `attributes`,
+        we will first define a generic HDF wrapper object to handle these components.
+        Once this is done, the HDF wrapper file can be treated as such an object with additional
         features to open and close the initial connection.
 
         Args:
             file_name (str): file path.
             read_only (bool, optional): If hdf is read-only. Defaults to True.
-            truncate (bool, optional): If existing groups and datasets can be 
+            truncate (bool, optional): If existing groups and datasets can be
                 truncated (i.e. are overwitten). Defaults to False.
-            delete_existing (bool, optional): If the file already exists, 
+            delete_existing (bool, optional): If the file already exists,
                 delete it completely and create a new one. Defaults to False.
 
         Examples::
             >>> # create a hdf file to write
             >>> hdf_file = HDF_File(hdf_file_path, read_only=False, truncate=True, delete_existing=True)
             >>> # create an empty group as "dfs"
             >>> hdf_file.dfs = {}
@@ -526,15 +495,15 @@
             >>> hdf_file.dfs.df1.data_from
             "colleagues"
         """
         if delete_existing:
             mode = "w"
         else:
             mode = "a"
-        with h5py.File(file_name, mode):#, swmr=True):
+        with h5py.File(file_name, mode):  # , swmr=True):
             pass
         super().__init__(
             file_name=file_name,
             name="/",
             read_only=read_only,
             truncate=truncate,
         )
```

### Comparing `alphabase-1.2.3/alphabase/io/tempmmap.py` & `alphabase-1.2.4/alphabase/io/tempmmap.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,22 +9,31 @@
 # external
 import numpy as np
 import mmap
 import h5py
 import tempfile
 import shutil
 
+# TODO initialize temp_dir not on import but when it is first needed
 _TEMP_DIR = tempfile.TemporaryDirectory(prefix="temp_mmap_")
 TEMP_DIR_NAME = _TEMP_DIR.name
 
-logging.warning(
-    f"Temp mmap arrays are written to {TEMP_DIR_NAME}. "
-    "Cleanup of this folder is OS dependant, "
-    "and might need to be triggered manually!"
-)
+is_cleanup_info_logged = False
+
+
+def _log_cleanup_info_once() -> None:
+    """Logs a info on temp array cleanup once."""
+    global is_cleanup_info_logged
+    if not is_cleanup_info_logged:
+        logging.info(
+            f"Temp mmap arrays are written to {TEMP_DIR_NAME}. "
+            "Cleanup of this folder is OS dependent and might need to be triggered manually!"
+        )
+        is_cleanup_info_logged = True
+
 
 def redefine_temp_location(path):
     """
     Redfine the location where the temp arrays are written to.
 
     Parameters
     ----------
@@ -34,26 +43,31 @@
     ------
     str
         the location of the new temporary directory.
 
     """
 
     global _TEMP_DIR, _TEMP_DIR, TEMP_DIR_NAME
-    logging.warning(f'''Folder {TEMP_DIR_NAME} with temp mmap arrays is being deleted.All existing temp mmapp arrays will be unusable!''')
-    
-    #cleaup old temporary directory
-    shutil.rmtree(TEMP_DIR_NAME, ignore_errors = True)
+    logging.warning(
+        f"""Folder {TEMP_DIR_NAME} with temp mmap arrays is being deleted.All existing temp mmapp arrays will be unusable!"""
+    )
+
+    # cleaup old temporary directory
+    shutil.rmtree(TEMP_DIR_NAME, ignore_errors=True)
     del _TEMP_DIR
 
-    #create new tempfile at desired location
-    _TEMP_DIR = tempfile.TemporaryDirectory(prefix = os.path.join(path, 'temp_mmap'))
+    # create new tempfile at desired location
+    _TEMP_DIR = tempfile.TemporaryDirectory(prefix=os.path.join(path, "temp_mmap"))
     TEMP_DIR_NAME = _TEMP_DIR.name
-    logging.warning(f'''New temp folder location. Temp mmap arrays are written to {TEMP_DIR_NAME}. Cleanup of this folder is OS dependant, and might need to be triggered manually!''')
+    logging.warning(
+        f"""New temp folder location. Temp mmap arrays are written to {TEMP_DIR_NAME}. Cleanup of this folder is OS dependant, and might need to be triggered manually!"""
+    )
     return TEMP_DIR_NAME
 
+
 def array(shape: tuple, dtype: np.dtype) -> np.ndarray:
     """Create a writable temporary mmapped array.
 
     Parameters
     ----------
     shape : tuple
         A tuple with the shape of the array.
@@ -61,37 +75,114 @@
         The np.dtype of the array.
 
     Returns
     -------
     type
         A writable temporary mmapped array.
     """
+    _log_cleanup_info_once()
+
     temp_file_name = os.path.join(
-        TEMP_DIR_NAME,
-        f"temp_mmap_{np.random.randint(2**63)}.hdf"
+        TEMP_DIR_NAME, f"temp_mmap_{np.random.randint(2**63)}.hdf"
     )
+
     with h5py.File(temp_file_name, "w") as hdf_file:
-        array = hdf_file.create_dataset(
-            "array",
-            shape=shape,
-            dtype=dtype
-        )
+        array = hdf_file.create_dataset("array", shape=shape, dtype=dtype)
         array[0] = 0
         offset = array.id.get_offset()
+
     with open(temp_file_name, "rb+") as raw_hdf_file:
-        mmap_obj = mmap.mmap(
-            raw_hdf_file.fileno(),
-            0,
-            access=mmap.ACCESS_WRITE
+        mmap_obj = mmap.mmap(raw_hdf_file.fileno(), 0, access=mmap.ACCESS_WRITE)
+        return np.frombuffer(
+            mmap_obj, dtype=dtype, count=np.prod(shape), offset=offset
+        ).reshape(shape)
+
+
+def create_empty_mmap(shape: tuple, dtype: np.dtype, path: str = None, overwrite=False):
+    """Initialize a new HDF5 file compatible with mmap. Returns the path to the initialized file.
+    File can be mapped using the mmap_array_from_path function.
+
+    Parameters
+    ----------
+    shape : tuple
+        A tuple with the shape of the array.
+    dtype : type
+        The np.dtype of the array.
+    path : str, optional
+        The path to the file that should be created.
+        Defaults to None.
+        If None a random file name will be generated.
+    overwrite : bool , optional
+        If True the file will be overwritten if it already exists.
+        Defaults to False.
+
+    Returns
+    -------
+    str
+        path to the newly created file.
+    """
+    _log_cleanup_info_once()
+
+    # if path does not exist generate a random file name in the TEMP directory
+    if path is None:
+        temp_file_name = os.path.join(
+            TEMP_DIR_NAME, f"temp_mmap_{np.random.randint(2**63)}.hdf"
         )
+    else:
+        # check that if overwrite is false the file does not already exist
+        if not overwrite:
+            if os.path.exists(path):
+                raise ValueError(
+                    "The file already exists. Set overwrite to True to overwrite the file or choose a different name."
+                )
+        if not os.path.basename.endswith(".hdf"):
+            raise ValueError("The chosen file name needs to end with .hdf")
+        if os.path.isdir(os.path.commonpath(path)):
+            temp_file_name = path
+        else:
+            raise ValueError(
+                "The directory in which the file should be created does not exist."
+            )
+
+    with h5py.File(temp_file_name, "w") as hdf_file:
+        array = hdf_file.create_dataset("array", shape=shape, dtype=dtype)
+        array[0] = 0
+
+    return temp_file_name
+
+
+def mmap_array_from_path(hdf_file: str) -> np.ndarray:
+    """reconnect to an exisiting HDF5 file to generate a writable temporary mmapped array.
+
+    Parameters
+    ----------
+    hdf_file : str
+        path to the array that should be reconnected to.
+
+    Returns
+    -------
+    type
+        A writable temporary mmapped array.
+    """
+    _log_cleanup_info_once()
+
+    path = os.path.join(hdf_file)
+
+    # read parameters required to reinitialize the mmap object
+    with h5py.File(path, "r") as hdf_file:
+        array = hdf_file["array"]
+        offset = array.id.get_offset()
+        shape = array.shape
+        dtype = array.dtype
+
+    # reinitialize the mmap object
+    with open(path, "rb+") as raw_hdf_file:
+        mmap_obj = mmap.mmap(raw_hdf_file.fileno(), 0, access=mmap.ACCESS_WRITE)
         return np.frombuffer(
-            mmap_obj,
-            dtype=dtype,
-            count=np.prod(shape),
-            offset=offset
+            mmap_obj, dtype=dtype, count=np.prod(shape), offset=offset
         ).reshape(shape)
 
 
 def zeros(shape: tuple, dtype: np.dtype) -> np.ndarray:
     """Create a writable temporary mmapped array filled with zeros.
 
     Parameters
```

### Comparing `alphabase-1.2.3/alphabase/peptide/fragment.py` & `alphabase-1.2.4/alphabase/peptide/fragment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,277 +1,266 @@
 import numpy as np
 import pandas as pd
-from typing import List, Union, Tuple, Dict, TYPE_CHECKING
-import warnings
+from typing import List, Union, Tuple, Dict
 import numba as nb
-import logging
 
-from alphabase.constants._const import (
-    PEAK_MZ_DTYPE, PEAK_INTENSITY_DTYPE
-)
-from alphabase.peptide.mass_calc import *
-from alphabase.constants.modification import (
-    calc_modloss_mass
-)
-from alphabase.constants.element import (
-    MASS_H2O, MASS_PROTON, 
-    MASS_NH3, MASS_H, MASS_C, MASS_O,
-)
+from alphabase.constants._const import PEAK_MZ_DTYPE, PEAK_INTENSITY_DTYPE
 
+from alphabase.constants.modification import calc_modloss_mass
+from alphabase.constants.atom import (
+    MASS_PROTON,
+)
+from alphabase.peptide.mass_calc import calc_b_y_and_peptide_masses_for_same_len_seqs
 from alphabase.peptide.precursor import (
     refine_precursor_df,
-    update_precursor_mz,
-    is_precursor_sorted
+    is_precursor_refined,
 )
 
-from alphabase.constants.element import (
-    calc_mass_from_formula
-)
+from alphabase.constants.atom import calc_mass_from_formula
 
 frag_type_representation_dict = {
-    'c': 'b+N(1)H(3)',
-    'z': 'y+N(-1)H(-2)',
-    'a': 'b+C(-1)O(-1)',
-    'x': 'y+C(1)O(1)H(-2)',
-    'b_H2O': 'b+H(-2)O(-1)',
-    'y_H2O': 'y+H(-2)O(-1)',
-    'b_NH3': 'b+N(-1)H(-3)',
-    'y_NH3': 'y+N(-1)H(-3)',
-    'c_lossH': 'b+N(1)H(2)',
-    'z_addH': 'y+N(-1)H(-1)',
+    "c": "b+N(1)H(3)",
+    "z": "y+N(-1)H(-2)",
+    "a": "b+C(-1)O(-1)",
+    "x": "y+C(1)O(1)H(-2)",
+    "b_H2O": "b+H(-2)O(-1)",
+    "y_H2O": "y+H(-2)O(-1)",
+    "b_NH3": "b+N(-1)H(-3)",
+    "y_NH3": "y+N(-1)H(-3)",
+    "c_lossH": "b+N(1)H(2)",
+    "z_addH": "y+N(-1)H(-1)",
 }
 """
 Represent fragment ion types from b/y ions.
-Modification neutral losses (i.e. modloss) are not here 
+Modification neutral losses (i.e. modloss) are not here
 as they have variable atoms added to b/y ions.
 """
 
 frag_mass_from_ref_ion_dict = {}
 """
 Masses parsed from :data:`frag_type_representation_dict`.
 """
 
-def add_new_frag_type(frag_type:str, representation:str):
+
+def add_new_frag_type(frag_type: str, representation: str):
     """Add new modifications into :data:`frag_type_representation_dict`
     and update :data:`frag_mass_from_ref_ion_dict`.
 
     Parameters
     ----------
     frag_type : str
         New fragment type
     representation : str
         The representation similar to :data:`frag_type_representation_dict`
     """
     frag_type_representation_dict[frag_type] = representation
-    ref_ion, formula = representation.split('+')
+    ref_ion, formula = representation.split("+")
     frag_mass_from_ref_ion_dict[frag_type] = dict(
-        ref_ion=ref_ion, 
-        add_mass=calc_mass_from_formula(formula)
+        ref_ion=ref_ion, add_mass=calc_mass_from_formula(formula)
     )
 
+
 def parse_all_frag_type_representation():
     for frag, representation in frag_type_representation_dict.items():
         add_new_frag_type(frag, representation)
 
-parse_all_frag_type_representation()
 
+parse_all_frag_type_representation()
 
 
 def get_charged_frag_types(
-    frag_types:List[str], 
-    max_frag_charge:int = 2
-)->List[str]:
-    '''
+    frag_types: List[str], max_frag_charge: int = 2
+) -> List[str]:
+    """
     Combine fragment types and charge states.
 
     Parameters
     ----------
     frag_types : List[str]
         e.g. ['b','y','b_modloss','y_modloss']
 
     max_frag_charge : int
         max fragment charge. (default: 2)
-    
+
     Returns
     -------
     List[str]
         charged fragment types
-    
+
     Examples
     --------
     >>> frag_types=['b','y','b_modloss','y_modloss']
     >>> get_charged_frag_types(frag_types, 2)
     ['b_z1','b_z2','y_z1','y_z2','b_modloss_z1','b_modloss_z2','y_modloss_z1','y_modloss_z2']
-    '''
+    """
     charged_frag_types = []
     for _type in frag_types:
-        for _ch in range(1, max_frag_charge+1):
+        for _ch in range(1, max_frag_charge + 1):
             charged_frag_types.append(f"{_type}_z{_ch}")
     return charged_frag_types
 
-def parse_charged_frag_type(
-    charged_frag_type: str
-)->Tuple[str,int]:
-    '''
+
+def parse_charged_frag_type(charged_frag_type: str) -> Tuple[str, int]:
+    """
     Oppsite to `get_charged_frag_types`.
-    
+
     Parameters
     ----------
     charged_frag_type : str
         e.g. 'y_z1', 'b_modloss_z1'
 
     Returns
     -------
     tuple
         str. Fragment type, e.g. 'b','y'
 
         int. Charge state
-    '''
-    _type, _ch = charged_frag_type.split('_z')
+    """
+    _type, _ch = charged_frag_type.split("_z")
     return _type, int(_ch)
 
+
 def init_zero_fragment_dataframe(
-    peplen_array:np.ndarray,
-    charged_frag_types:List[str], 
-    dtype=PEAK_MZ_DTYPE
-)->Tuple[pd.DataFrame, np.ndarray, np.ndarray]: 
-    '''Initialize a zero dataframe based on peptide length 
+    peplen_array: np.ndarray, charged_frag_types: List[str], dtype=PEAK_MZ_DTYPE
+) -> Tuple[pd.DataFrame, np.ndarray, np.ndarray]:
+    """Initialize a zero dataframe based on peptide length
     (nAA) array (peplen_array) and charge_frag_types (column number).
     The row number of returned dataframe is np.sum(peplen_array-1).
 
     Parameters
     ----------
     peplen_array : np.ndarray
         peptide lengths for the fragment dataframe
-        
+
     charged_frag_types : List[str]
         `['b_z1','b_z2','y_z1','y_z2','b_modloss_z1','y_H2O_z1'...]`
-    
+
     Returns
     -------
     tuple
         pd.DataFrame, `fragment_df` with zero values
 
         np.ndarray (int64), the start indices point to the `fragment_df` for each peptide
 
         np.ndarray (int64), the end indices point to the `fragment_df` for each peptide
-    '''
-    indices = np.zeros(len(peplen_array)+1, dtype=np.int64)
-    indices[1:] = peplen_array-1
+    """
+    indices = np.zeros(len(peplen_array) + 1, dtype=np.int64)
+    indices[1:] = peplen_array - 1
     indices = np.cumsum(indices)
     fragment_df = pd.DataFrame(
-        np.zeros((indices[-1],len(charged_frag_types)), dtype=dtype),
-        columns = charged_frag_types
+        np.zeros((indices[-1], len(charged_frag_types)), dtype=dtype),
+        columns=charged_frag_types,
     )
     return fragment_df, indices[:-1], indices[1:]
 
+
 def init_fragment_dataframe_from_other(
-    reference_fragment_df: pd.DataFrame,
-    dtype=PEAK_MZ_DTYPE
+    reference_fragment_df: pd.DataFrame, dtype=PEAK_MZ_DTYPE
 ):
-    '''
+    """
     Init zero fragment dataframe from the `reference_fragment_df` (same rows and same columns)
-    '''
+    """
     return pd.DataFrame(
         np.zeros_like(reference_fragment_df.values, dtype=dtype),
-        columns = reference_fragment_df.columns
+        columns=reference_fragment_df.columns,
     )
 
+
 def init_fragment_by_precursor_dataframe(
     precursor_df,
     charged_frag_types: List[str],
     *,
     reference_fragment_df: pd.DataFrame = None,
-    dtype:np.dtype=PEAK_MZ_DTYPE,
-    inplace_in_reference:bool=False,
+    dtype: np.dtype = PEAK_MZ_DTYPE,
+    inplace_in_reference: bool = False,
 ):
-    '''
-    Init zero fragment dataframe for the `precursor_df`. If 
-    the `reference_fragment_df` is provided, the result dataframe's 
-    length will be the same as reference_fragment_df. Otherwise it 
+    """
+    Init zero fragment dataframe for the `precursor_df`. If
+    the `reference_fragment_df` is provided, the result dataframe's
+    length will be the same as reference_fragment_df. Otherwise it
     generates the dataframe from scratch.
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursors to generate fragment masses,
-        if `precursor_df` contains the 'frag_start_idx' column, 
-        it is better to provide `reference_fragment_df` as 
-        `precursor_df.frag_start_idx` and `precursor.frag_stop_idx` 
+        if `precursor_df` contains the 'frag_start_idx' column,
+        it is better to provide `reference_fragment_df` as
+        `precursor_df.frag_start_idx` and `precursor.frag_stop_idx`
         point to the indices in `reference_fragment_df`
 
     charged_frag_types : List
         `['b_z1','b_z2','y_z1','y_z2','b_modloss_z1','y_H2O_z1'...]`
 
     reference_fragment_df : pd.DataFrame
         init zero fragment_mz_df based
-        on this reference. If None, fragment_mz_df will be 
+        on this reference. If None, fragment_mz_df will be
         initialized by :func:`alphabase.peptide.fragment.init_zero_fragment_dataframe`.
         Defaults to None.
 
     dtype: np.dtype
         dtype of fragment mz values, Defaults to :data:`PEAK_MZ_DTYPE`.
 
     inplace_in_reference : bool, optional
-        if calculate the fragment mz 
+        if calculate the fragment mz
         inplace in the reference_fragment_df (default: False)
 
     Returns
     -------
     pd.DataFrame
         zero `fragment_df` with given `charged_frag_types` columns
-    '''
-    if 'frag_start_idx' not in precursor_df.columns:
-        (
-            fragment_df, start_indices, end_indices
-        ) = init_zero_fragment_dataframe(
-            precursor_df.nAA.values,
-            charged_frag_types,
-            dtype=dtype
+    """
+    if "frag_start_idx" not in precursor_df.columns:
+        (fragment_df, start_indices, end_indices) = init_zero_fragment_dataframe(
+            precursor_df.nAA.values, charged_frag_types, dtype=dtype
         )
-        precursor_df['frag_start_idx'] = start_indices
-        precursor_df['frag_stop_idx'] = end_indices
+        precursor_df["frag_start_idx"] = start_indices
+        precursor_df["frag_stop_idx"] = end_indices
     else:
         if reference_fragment_df is None:
             # raise ValueError(
             #     "`precursor_df` contains 'frag_start_idx' column, "\
             #     "please provide `reference_fragment_df` argument"
             # )
             fragment_df = pd.DataFrame(
-                np.zeros((
-                    precursor_df.frag_stop_idx.max(), 
-                    len(charged_frag_types)
-                ), dtype=dtype),
-                columns = charged_frag_types
+                np.zeros(
+                    (precursor_df.frag_stop_idx.max(), len(charged_frag_types)),
+                    dtype=dtype,
+                ),
+                columns=charged_frag_types,
             )
         else:
-            if inplace_in_reference: 
-                fragment_df = reference_fragment_df[[
-                    _fr for _fr in charged_frag_types 
-                    if _fr in reference_fragment_df.columns
-                ]]
+            if inplace_in_reference:
+                fragment_df = reference_fragment_df[
+                    [
+                        _fr
+                        for _fr in charged_frag_types
+                        if _fr in reference_fragment_df.columns
+                    ]
+                ]
             else:
                 fragment_df = pd.DataFrame(
-                    np.zeros((
-                        len(reference_fragment_df), 
-                        len(charged_frag_types)
-                    ), dtype=dtype),
-                    columns = charged_frag_types
+                    np.zeros(
+                        (len(reference_fragment_df), len(charged_frag_types)),
+                        dtype=dtype,
+                    ),
+                    columns=charged_frag_types,
                 )
     return fragment_df
 
+
 def update_sliced_fragment_dataframe(
     fragment_df: pd.DataFrame,
     fragment_df_vals: np.ndarray,
     values: np.ndarray,
-    frag_start_end_list: List[Tuple[int,int]],
-    charged_frag_types: List[str]=None,
+    frag_start_end_list: List[Tuple[int, int]],
+    charged_frag_types: List[str] = None,
 ):
-    '''
-    Set the values of the slices `frag_start_end_list=[(start,end),(start,end),...]` 
+    """
+    Set the values of the slices `frag_start_end_list=[(start,end),(start,end),...]`
     of fragment_df.
 
     Parameters
     ----------
     fragment_df : pd.DataFrame
         fragment dataframe to set the values
 
@@ -283,183 +272,202 @@
 
     frag_start_end_list : List[Tuple[int,int]]
         e.g. `[(start,end),(start,end),...]`
 
     charged_frag_types : List[str], optional
         e.g. `['b_z1','b_z2','y_z1','y_z2']`.
         If None, the columns of values should be the same as fragment_df's columns.
-        It is much faster if charged_frag_types is None as we use numpy slicing, 
+        It is much faster if charged_frag_types is None as we use numpy slicing,
         otherwise we use pd.loc (much slower).
         Defaults to None.
-    '''
-    frag_slice_list = [slice(start,end) for start,end in frag_start_end_list]
+    """
+    frag_slice_list = [slice(start, end) for start, end in frag_start_end_list]
     frag_slices = np.r_[tuple(frag_slice_list)]
-    if charged_frag_types is None or len(charged_frag_types)==0:
+    if charged_frag_types is None or len(charged_frag_types) == 0:
         fragment_df_vals[frag_slices, :] = values.astype(fragment_df_vals.dtype)
     else:
-        charged_frag_idxes = [fragment_df.columns.get_loc(c) for c in charged_frag_types]
-        fragment_df.iloc[
-            frag_slices, charged_frag_idxes
-        ] = values.astype(fragment_df_vals.dtype)
+        charged_frag_idxes = [
+            fragment_df.columns.get_loc(c) for c in charged_frag_types
+        ]
+        fragment_df.iloc[frag_slices, charged_frag_idxes] = values.astype(
+            fragment_df_vals.dtype
+        )
         fragment_df_vals[frag_slices] = fragment_df.values[frag_slices]
 
+
 def get_sliced_fragment_dataframe(
     fragment_df: pd.DataFrame,
-    frag_start_end_list:Union[List,np.ndarray],
-    charged_frag_types:List = None,
-)->pd.DataFrame:
-    '''
+    frag_start_end_list: Union[List, np.ndarray],
+    charged_frag_types: List = None,
+) -> pd.DataFrame:
+    """
     Get the sliced fragment_df from `frag_start_end_list=[(start,end),(start,end),...]`.
-    
+
     Parameters
     ----------
     fragment_df : pd.DataFrame
         fragment dataframe to get values
 
     frag_start_end_list : Union
         List[Tuple[int,int]], e.g. `[(start,end),(start,end),...]` or np.ndarray
 
     charged_frag_types : List[str]
         e.g. `['b_z1','b_z2','y_z1','y_z2']`.
         if None, all columns will be considered
-    
+
     Returns
     -------
     pd.DataFrame
-    
-        sliced fragment_df. If `charged_frag_types` is None, 
+
+        sliced fragment_df. If `charged_frag_types` is None,
         return fragment_df with all columns
-    '''
-    frag_slice_list = [slice(start,end) for start,end in frag_start_end_list]
+    """
+    frag_slice_list = [slice(start, end) for start, end in frag_start_end_list]
     frag_slices = np.r_[tuple(frag_slice_list)]
-    if charged_frag_types is None or len(charged_frag_types)==0:
+    if charged_frag_types is None or len(charged_frag_types) == 0:
         charged_frag_idxes = slice(None)
     else:
-        charged_frag_idxes = [fragment_df.columns.get_loc(c) for c in charged_frag_types]
+        charged_frag_idxes = [
+            fragment_df.columns.get_loc(c) for c in charged_frag_types
+        ]
     return fragment_df.iloc[frag_slices, charged_frag_idxes]
 
+
 def concat_precursor_fragment_dataframes(
     precursor_df_list: List[pd.DataFrame],
     fragment_df_list: List[pd.DataFrame],
-    *other_fragment_df_lists
-)->Tuple[pd.DataFrame,...]:
-    '''
-    Since fragment_df is indexed by precursor_df, when we concatenate multiple 
-    fragment_df, the indexed positions will change for in precursor_dfs,  
-    this function keeps the correct indexed positions of precursor_df when 
+    *other_fragment_df_lists,
+) -> Tuple[pd.DataFrame, ...]:
+    """
+    Since fragment_df is indexed by precursor_df, when we concatenate multiple
+    fragment_df, the indexed positions will change for in precursor_dfs,
+    this function keeps the correct indexed positions of precursor_df when
     concatenating multiple fragment_df dataframes.
-    
+
     Parameters
     ----------
     precursor_df_list : List[pd.DataFrame]
         precursor dataframe list to concatenate
 
     fragment_df_list : List[pd.DataFrame]
         fragment dataframe list to concatenate
 
     other_fragment_df_lists
-        arbitray other fragment dataframe list to concatenate, 
+        arbitray other fragment dataframe list to concatenate,
         e.g. fragment_mass_df, fragment_inten_df, ...
-    
+
     Returns
     -------
     Tuple[pd.DataFrame,...]
         concatenated precursor_df, fragment_df, other_fragment_dfs ...
-    '''
+    """
     fragment_df_lens = [len(fragment_df) for fragment_df in fragment_df_list]
     precursor_df_list = [precursor_df.copy() for precursor_df in precursor_df_list]
     cum_frag_df_lens = np.cumsum(fragment_df_lens)
-    for i,precursor_df in enumerate(precursor_df_list[1:]):
-        precursor_df[['frag_start_idx','frag_stop_idx']] += cum_frag_df_lens[i]
+    for i, precursor_df in enumerate(precursor_df_list[1:]):
+        precursor_df[["frag_start_idx", "frag_stop_idx"]] += cum_frag_df_lens[i]
     return (
         pd.concat(precursor_df_list, ignore_index=True),
         pd.concat(fragment_df_list, ignore_index=True),
-        *[pd.concat(other_list, ignore_index=True)
+        *[
+            pd.concat(other_list, ignore_index=True)
             for other_list in other_fragment_df_lists
-        ]
+        ],
     )
 
+
 def calc_fragment_mz_values_for_same_nAA(
-    df_group:pd.DataFrame, 
-    nAA:int, 
-    charged_frag_types:list
+    df_group: pd.DataFrame, nAA: int, charged_frag_types: list
 ):
-    mod_list = df_group.mods.str.split(';').apply(
-        lambda x: [m for m in x if len(m)>0]
-    ).values
-    site_list = df_group.mod_sites.str.split(';').apply(
-        lambda x: [int(s) for s in x if len(s)>0]
-    ).values
-
-    if 'aa_mass_diffs' in df_group.columns:
-        mod_diff_list = df_group.aa_mass_diffs.str.split(';').apply(
-            lambda x: [float(m) for m in x if len(m)>0]
-        ).values
-        mod_diff_site_list = df_group.aa_mass_diff_sites.str.split(';').apply(
-            lambda x: [int(s) for s in x if len(s)>0]
-        ).values
+    mod_list = (
+        df_group.mods.str.split(";")
+        .apply(lambda x: [m for m in x if len(m) > 0])
+        .values
+    )
+    site_list = (
+        df_group.mod_sites.str.split(";")
+        .apply(lambda x: [int(s) for s in x if len(s) > 0])
+        .values
+    )
+
+    if "aa_mass_diffs" in df_group.columns:
+        mod_diff_list = (
+            df_group.aa_mass_diffs.str.split(";")
+            .apply(lambda x: [float(m) for m in x if len(m) > 0])
+            .values
+        )
+        mod_diff_site_list = (
+            df_group.aa_mass_diff_sites.str.split(";")
+            .apply(lambda x: [int(s) for s in x if len(s) > 0])
+            .values
+        )
     else:
         mod_diff_list = None
         mod_diff_site_list = None
-    (
-        b_mass, y_mass, pepmass
-    ) = calc_b_y_and_peptide_masses_for_same_len_seqs(
-        df_group.sequence.values.astype('U'), 
-        mod_list, site_list,
+    (b_mass, y_mass, pepmass) = calc_b_y_and_peptide_masses_for_same_len_seqs(
+        df_group.sequence.values.astype("U"),
+        mod_list,
+        site_list,
         mod_diff_list,
-        mod_diff_site_list
+        mod_diff_site_list,
     )
     b_mass = b_mass.reshape(-1)
     y_mass = y_mass.reshape(-1)
 
     for charged_frag_type in charged_frag_types:
-        if charged_frag_type.startswith('b_modloss'):
-            b_modloss = np.concatenate([
-                calc_modloss_mass(nAA, mods, sites, True)
-                for mods, sites in zip(mod_list, site_list)
-            ])
+        if charged_frag_type.startswith("b_modloss"):
+            b_modloss = np.concatenate(
+                [
+                    calc_modloss_mass(nAA, mods, sites, True)
+                    for mods, sites in zip(mod_list, site_list)
+                ]
+            )
             break
     for charged_frag_type in charged_frag_types:
-        if charged_frag_type.startswith('y_modloss'):
-            y_modloss = np.concatenate([
-                calc_modloss_mass(nAA, mods, sites, False)
-                for mods, sites in zip(mod_list, site_list)
-            ])
+        if charged_frag_type.startswith("y_modloss"):
+            y_modloss = np.concatenate(
+                [
+                    calc_modloss_mass(nAA, mods, sites, False)
+                    for mods, sites in zip(mod_list, site_list)
+                ]
+            )
             break
 
     mz_values = []
     add_proton = MASS_PROTON
     for charged_frag_type in charged_frag_types:
         # Neutral masses also considered for future uses
-        if charged_frag_type == 'b':
+        if charged_frag_type == "b":
             mz_values.append(b_mass)
             continue
-        elif charged_frag_type == 'y':
+        elif charged_frag_type == "y":
             mz_values.append(y_mass)
             continue
         frag_type, charge = parse_charged_frag_type(charged_frag_type)
-        if frag_type == 'b':
-            _mass = b_mass/charge + add_proton
-        elif frag_type == 'y':
-            _mass = y_mass/charge + add_proton
-        elif frag_type == 'b_modloss':
-            _mass = (b_mass-b_modloss)/charge + add_proton
+        if frag_type == "b":
+            _mass = b_mass / charge + add_proton
+        elif frag_type == "y":
+            _mass = y_mass / charge + add_proton
+        elif frag_type == "b_modloss":
+            _mass = (b_mass - b_modloss) / charge + add_proton
             _mass[b_modloss == 0] = 0
-        elif frag_type == 'y_modloss':
-            _mass = (y_mass-y_modloss)/charge + add_proton
+        elif frag_type == "y_modloss":
+            _mass = (y_mass - y_modloss) / charge + add_proton
             _mass[y_modloss == 0] = 0
         elif frag_type in frag_mass_from_ref_ion_dict:
-            ref_ion = frag_mass_from_ref_ion_dict[frag_type]['ref_ion']
-            add_mass = frag_mass_from_ref_ion_dict[frag_type]['add_mass']
-            if ref_ion == 'b':
-                _mass = (b_mass+add_mass)/charge + add_proton
-            elif ref_ion == 'y':
-                _mass = (y_mass+add_mass)/charge + add_proton
+            ref_ion = frag_mass_from_ref_ion_dict[frag_type]["ref_ion"]
+            add_mass = frag_mass_from_ref_ion_dict[frag_type]["add_mass"]
+            if ref_ion == "b":
+                _mass = (b_mass + add_mass) / charge + add_proton
+            elif ref_ion == "y":
+                _mass = (y_mass + add_mass) / charge + add_proton
             else:
-                raise KeyError(f"ref_ion only allows `b` and `y`, but {ref_ion} is given")
+                raise KeyError(
+                    f"ref_ion only allows `b` and `y`, but {ref_ion} is given"
+                )
         # elif frag_type == 'b_H2O':
         #     _mass = (b_mass-MASS_H2O)/charge + add_proton
         # elif frag_type == 'y_H2O':
         #     _mass = (y_mass-MASS_H2O)/charge + add_proton
         # elif frag_type == 'b_NH3':
         #     _mass = (b_mass-MASS_NH3)/charge + add_proton
         # elif frag_type == 'y_NH3':
@@ -473,53 +481,48 @@
         # elif frag_type == 'z_addH': # H rearrangement: z+1
         #     _mass = (MASS_H*2-MASS_NH3+y_mass)/charge + add_proton
         # elif frag_type == 'a':
         #     _mass = (-MASS_C-MASS_O+b_mass)/charge + add_proton
         # elif frag_type == 'x':
         #     _mass = (MASS_C+MASS_O-MASS_H*2+y_mass)/charge + add_proton
         else:
-            raise KeyError(
-                f'Fragment type "{frag_type}" is not in fragment_mz_df.'
-            )
+            raise KeyError(f'Fragment type "{frag_type}" is not in fragment_mz_df.')
         mz_values.append(_mass)
     return np.array(mz_values).T
 
+
 def mask_fragments_for_charge_greater_than_precursor_charge(
-    fragment_df:pd.DataFrame, 
-    precursor_charge_array:np.ndarray,
-    nAA_array:np.ndarray,
+    fragment_df: pd.DataFrame,
+    precursor_charge_array: np.ndarray,
+    nAA_array: np.ndarray,
     *,
-    candidate_fragment_charges:list = [2,3,4],
+    candidate_fragment_charges: list = [2, 3, 4],
 ):
-    """Mask the fragment dataframe when 
+    """Mask the fragment dataframe when
     the fragment charge is larger than the precursor charge"""
-    precursor_charge_array = np.repeat(
-        precursor_charge_array, nAA_array-1
-    )
+    precursor_charge_array = np.repeat(precursor_charge_array, nAA_array - 1)
     for col in fragment_df.columns:
         for charge in candidate_fragment_charges:
-            if col.endswith(f'z{charge}'):
-                fragment_df.loc[
-                    precursor_charge_array<charge,col
-                ] = 0
+            if col.endswith(f"z{charge}"):
+                fragment_df.loc[precursor_charge_array < charge, col] = 0
     return fragment_df
 
 
-
 @nb.njit(parallel=True)
 def fill_in_indices(
-    frag_start_idxes:np.ndarray,
-    frag_stop_idxes: np.ndarray, 
-    indices:np.ndarray, 
-    max_indices:np.ndarray, 
-    excluded_indices:np.ndarray, 
-    top_k: int, 
-    flattened_intensity:np.ndarray, 
-    number_of_fragment_types:int, 
-    max_frag_per_peptide:int = 300) -> None:
+    frag_start_idxes: np.ndarray,
+    frag_stop_idxes: np.ndarray,
+    indices: np.ndarray,
+    max_indices: np.ndarray,
+    excluded_indices: np.ndarray,
+    top_k: int,
+    flattened_intensity: np.ndarray,
+    number_of_fragment_types: int,
+    max_frag_per_peptide: int = 300,
+) -> None:
     """
     Fill in indices, max indices and excluded indices for each peptide.
     indices: index of fragment per peptide (from 0 to max_index-1)
     max_indices: max index of fragments per peptide (number of fragments per peptide)
     excluded_indices: not top k excluded indices per peptide
 
     Parameters
@@ -548,34 +551,46 @@
     number_of_fragment_types : int
         number of types of fragments (e.g. b,y,b_modloss,y_modloss, ...) equals to the number of columns in fragment mz dataframe
 
     max_frag_per_peptide : int, optional
         maximum number of fragments per peptide, Defaults to 300
 
     """
-    array = np.arange(0,max_frag_per_peptide).reshape(-1,1)
-    ones = np.ones(max_frag_per_peptide).reshape(-1,1)
+    array = np.arange(0, max_frag_per_peptide).reshape(-1, 1)
+    ones = np.ones(max_frag_per_peptide).reshape(-1, 1)
     length = len(frag_start_idxes)
 
     for i in nb.prange(length):
         frag_start = frag_start_idxes[i]
         frag_end = frag_stop_idxes[i]
-        max_index = frag_end-frag_start
+        max_index = frag_end - frag_start
         indices[frag_start:frag_end] = array[:max_index]
-        max_indices[frag_start:frag_end] = ones[:max_index]*max_index
-        if flattened_intensity is None or top_k >= max_index*number_of_fragment_types: continue
-        idxes = np.argsort(flattened_intensity[frag_start*number_of_fragment_types:frag_end*number_of_fragment_types])
+        max_indices[frag_start:frag_end] = ones[:max_index] * max_index
+        if flattened_intensity is None or top_k >= max_index * number_of_fragment_types:
+            continue
+        idxes = np.argsort(
+            flattened_intensity[
+                frag_start * number_of_fragment_types : frag_end
+                * number_of_fragment_types
+            ]
+        )
         _excl = np.ones_like(idxes, dtype=np.bool_)
         _excl[idxes[-top_k:]] = False
-        excluded_indices[frag_start*number_of_fragment_types:frag_end*number_of_fragment_types] = _excl
-            
+        excluded_indices[
+            frag_start * number_of_fragment_types : frag_end * number_of_fragment_types
+        ] = _excl
 
 
-@nb.vectorize([nb.uint32(nb.int8, nb.uint32, nb.uint32, nb.uint32)],target='parallel')
-def calculate_fragment_numbers(frag_direction:np.int8, frag_number:np.uint32, index:np.uint32, max_index:np.uint32):
+@nb.vectorize([nb.uint32(nb.int8, nb.uint32, nb.uint32, nb.uint32)], target="parallel")
+def calculate_fragment_numbers(
+    frag_direction: np.int8,
+    frag_number: np.uint32,
+    index: np.uint32,
+    max_index: np.uint32,
+):
     """
     Calculate fragment numbers for each fragment based on the fragment direction.
 
     Parameters
     ----------
     frag_direction : np.int8
         directions of fragments for each peptide
@@ -583,35 +598,34 @@
     frag_number : np.uint32
         fragment numbers for each peptide
 
     index : np.uint32
         index of fragment per peptide (from 0 to max_index-1)
 
     max_index : np.uint32
-        max index of fragments per peptide (number of fragments per peptide) 
+        max index of fragments per peptide (number of fragments per peptide)
     """
     if frag_direction == 1:
         frag_number = index + 1
     elif frag_direction == -1:
-        frag_number = max_index - index        
+        frag_number = max_index - index
     return frag_number
 
 
-
 def parse_fragment(
-    frag_directions:np.ndarray, 
-    frag_start_idxes:np.ndarray, 
-    frag_stop_idxes: np.ndarray, 
-    top_k: int, 
-    intensities:np.ndarray, 
-    number_of_fragment_types:int
+    frag_directions: np.ndarray,
+    frag_start_idxes: np.ndarray,
+    frag_stop_idxes: np.ndarray,
+    top_k: int,
+    intensities: np.ndarray,
+    number_of_fragment_types: int,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
-    Parse fragments to get fragment numbers, fragment positions and not top k excluded indices in one hit 
-    faster than doing each operation individually, and makes the most of the operations that are done in parallel. 
+    Parse fragments to get fragment numbers, fragment positions and not top k excluded indices in one hit
+    faster than doing each operation individually, and makes the most of the operations that are done in parallel.
 
     Parameters
     ----------
     frag_directions : np.ndarray
         directions of fragments for each peptide
 
     frag_start_idxes : np.ndarray
@@ -624,496 +638,514 @@
         top k highest peaks to keep
 
     intensities : np.ndarray
         Flattened fragment intensities
 
     number_of_fragment_types : int
         number of types of fragments (e.g. b,y,b_modloss,y_modloss, ...) equals to the number of columns in fragment mz dataframe
-    
+
     Returns
     -------
     Tuple[np.ndarray, np.ndarray, np.ndarray]
         Tuple of fragment numbers, fragment positions and not top k excluded indices
 
     """
     # Allocate memory for fragment numbers, indices, max indices and excluded indices
     frag_numbers = np.empty_like(frag_directions, dtype=np.uint32)
     indices = np.empty_like(frag_directions, dtype=np.uint32)
     max_indices = np.empty_like(frag_directions, dtype=np.uint32)
-    excluded_indices = np.zeros(frag_directions.shape[0]*frag_directions.shape[1], dtype=np.bool_)
+    excluded_indices = np.zeros(
+        frag_directions.shape[0] * frag_directions.shape[1], dtype=np.bool_
+    )
 
     # Fill in indices, max indices and excluded indices
-    fill_in_indices(frag_start_idxes, frag_stop_idxes,indices,max_indices, excluded_indices,top_k,intensities, number_of_fragment_types)
- 
+    fill_in_indices(
+        frag_start_idxes,
+        frag_stop_idxes,
+        indices,
+        max_indices,
+        excluded_indices,
+        top_k,
+        intensities,
+        number_of_fragment_types,
+    )
+
     # Calculate fragment numbers
-    frag_numbers = calculate_fragment_numbers(frag_directions, frag_numbers, indices, max_indices)
+    frag_numbers = calculate_fragment_numbers(
+        frag_directions, frag_numbers, indices, max_indices
+    )
     return frag_numbers, indices, excluded_indices
 
-   
+
 def flatten_fragments(
-    precursor_df: pd.DataFrame, 
+    precursor_df: pd.DataFrame,
     fragment_mz_df: pd.DataFrame,
     fragment_intensity_df: pd.DataFrame,
     min_fragment_intensity: float = -1,
     keep_top_k_fragments: int = 1000,
-    custom_columns : list = [
-        'type','number','position','charge','loss_type'
-    ],
-    custom_df : Dict[str, pd.DataFrame] = {}
-)->Tuple[pd.DataFrame, pd.DataFrame]:
+    custom_columns: list = ["type", "number", "position", "charge", "loss_type"],
+    custom_df: Dict[str, pd.DataFrame] = {},
+) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """
-    Converts the tabular fragment format consisting of 
-    the `fragment_mz_df` and the `fragment_intensity_df` 
+    Converts the tabular fragment format consisting of
+    the `fragment_mz_df` and the `fragment_intensity_df`
     into a linear fragment format.
-    The linear fragment format will only retain fragments 
-    above a given intensity treshold with `mz > 0`. 
-    It consists of columns: `mz`, `intensity`, 
-    `type`, `number`, `charge` and `loss_type`,  
+    The linear fragment format will only retain fragments
+    above a given intensity treshold with `mz > 0`.
+    It consists of columns: `mz`, `intensity`,
+    `type`, `number`, `charge` and `loss_type`,
     where each column refers to:
 
     - mz:        :data:`PEAK_MZ_DTYPE`, fragment mz value
     - intensity: :data:`PEAK_INTENSITY_DTYPE`, fragment intensity value
     - type:      uint8, ASCII code of the ion type. Small caps are for regular scoring ions used during search: (97=a, 98=b, 99=c, 120=x, 121=y, 122=z).
                         Small caps subtracted by 64 are used for ions only quantified and not scored: (33=a, 34=b, 35=c, 56=x, 57=y, 58=z).
                         By default all ions are scored and quantified. It is left to the user or search engine to decide which ions to use.
     - number:    uint32, fragment series number
     - position:  uint32, fragment position in sequence (from left to right, starts with 0)
     - charge:    uint8, fragment charge
     - loss_type: int16, fragment loss type, 0=noloss, 17=NH3, 18=H2O, 98=H3PO4 (phos), ...
-    
-    The fragment pointers `frag_start_idx` and `frag_stop_idx` 
+
+    The fragment pointers `frag_start_idx` and `frag_stop_idx`
     will be reannotated to the new fragment format.
 
     For ASCII code `type`, we can convert it into byte-str by using `frag_df.type.values.view('S1')`.
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
         input precursor dataframe which contains the frag_start_idx and frag_stop_idx columns
-    
+
     fragment_mz_df : pd.DataFrame
         input fragment mz dataframe of shape (N, T) which contains N * T fragment mzs.
         Fragments with mz==0 will be excluded.
-    
+
     fragment_intensity_df : pd.DataFrame
         input fragment intensity dataframe of shape (N, T) which contains N * T fragment mzs.
         Could be empty (len==0) to exclude intensity values.
-    
+
     min_fragment_intensity : float, optional
         minimum intensity which should be retained. Defaults to -1
-    
+
     custom_columns : list, optional
-        'mz' and 'intensity' columns are required. Others could be customized. 
+        'mz' and 'intensity' columns are required. Others could be customized.
         Defaults to ['type','number','position','charge','loss_type']
 
     custom_df : Dict[str, pd.DataFrame], optional
         Append custom columns by providing additional dataframes of the same shape as fragment_mz_df and fragment_intensity_df. Defaults to {}.
-    
+
     Returns
     -------
     pd.DataFrame
         precursor dataframe with added `flat_frag_start_idx` and `flat_frag_stop_idx` columns
     pd.DataFrame
-        fragment dataframe with columns: `mz`, `intensity`, `type`, `number`, 
+        fragment dataframe with columns: `mz`, `intensity`, `type`, `number`,
         `charge` and `loss_type`, where each column refers to:
-        
+
         - mz:        :data:`PEAK_MZ_DTYPE`, fragment mz value
         - intensity: :data:`PEAK_INTENSITY_DTYPE`, fragment intensity value
         - type:      uint8, ASCII code of the ion type. Small caps are for regular scoring ions used during search: (97=a, 98=b, 99=c, 120=x, 121=y, 122=z).
                             Small caps subtracted by 64 are used for ions only quantified and not scored: (33=a, 34=b, 35=c, 56=x, 57=y, 58=z).
                             By default all ions are scored and quantified. It is left to the user or search engine to decide which ions to use.
         - number:    uint32, fragment series number
         - position:  uint32, fragment position in sequence (from left to right, starts with 0)
         - charge:    uint8, fragment charge
         - loss_type: int16, fragment loss type, 0=noloss, 17=NH3, 18=H2O, 98=H3PO4 (phos), ...
     """
     if len(precursor_df) == 0:
         return precursor_df, pd.DataFrame()
     # new dataframes for fragments and precursors are created
     frag_df = {}
-    frag_df['mz'] = fragment_mz_df.values.reshape(-1)
+    frag_df["mz"] = fragment_mz_df.values.reshape(-1)
     if len(fragment_intensity_df) > 0:
-        frag_df['intensity'] = fragment_intensity_df.values.astype(
+        frag_df["intensity"] = fragment_intensity_df.values.astype(
             PEAK_INTENSITY_DTYPE
         ).reshape(-1)
         use_intensity = True
     else:
         use_intensity = False
     # add additional columns to the fragment dataframe
     # each column in the flat fragment dataframe is a whole pandas dataframe in the dense representation
     for col_name, df in custom_df.items():
         frag_df[col_name] = df.values.reshape(-1)
-    
+
     frag_types = []
     frag_loss_types = []
     frag_charges = []
-    frag_directions = [] # 'abc': direction=1, 'xyz': direction=-1, otherwise 0
-    
+    frag_directions = []  # 'abc': direction=1, 'xyz': direction=-1, otherwise 0
+
     for col in fragment_mz_df.columns.values:
-        _types = col.split('_')
-        frag_types.append(ord(_types[0])) # using ASCII code
+        _types = col.split("_")
+        frag_types.append(ord(_types[0]))  # using ASCII code
         frag_charges.append(int(_types[-1][1:]))
         if len(_types) == 2:
             frag_loss_types.append(0)
         else:
-            if _types[1] == 'NH3':
+            if _types[1] == "NH3":
                 frag_loss_types.append(17)
-            elif _types[1] == 'H2O':
+            elif _types[1] == "H2O":
                 frag_loss_types.append(18)
             else:
                 frag_loss_types.append(98)
-        if ord(_types[0]) >= 97 and ord(_types[0]) <= 109: # a-m
+        if ord(_types[0]) >= 97 and ord(_types[0]) <= 109:  # a-m
             frag_directions.append(1)
-        elif ord(_types[0]) >= 110 and ord(_types[0]) <= 122: #n-z
+        elif ord(_types[0]) >= 110 and ord(_types[0]) <= 122:  # n-z
             frag_directions.append(-1)
         else:
             frag_directions.append(0)
-    
-    if 'type' in custom_columns:
-        frag_df['type'] = np.array(np.tile(frag_types, len(fragment_mz_df)), dtype=np.int8)
-    if 'loss_type' in custom_columns:    
-        frag_df['loss_type'] = np.array(np.tile(frag_loss_types, len(fragment_mz_df)), dtype=np.int16)
-    if 'charge' in custom_columns:
-        frag_df['charge'] = np.array(np.tile(frag_charges, len(fragment_mz_df)), dtype=np.int8)
-    
-    frag_directions = np.array(np.tile(frag_directions,(len(fragment_mz_df),1)), dtype=np.int8)
+
+    if "type" in custom_columns:
+        frag_df["type"] = np.array(
+            np.tile(frag_types, len(fragment_mz_df)), dtype=np.int8
+        )
+    if "loss_type" in custom_columns:
+        frag_df["loss_type"] = np.array(
+            np.tile(frag_loss_types, len(fragment_mz_df)), dtype=np.int16
+        )
+    if "charge" in custom_columns:
+        frag_df["charge"] = np.array(
+            np.tile(frag_charges, len(fragment_mz_df)), dtype=np.int8
+        )
+
+    frag_directions = np.array(
+        np.tile(frag_directions, (len(fragment_mz_df), 1)), dtype=np.int8
+    )
 
     numbers, positions, excluded_indices = parse_fragment(
-        frag_directions, 
-        precursor_df.frag_start_idx.values, 
+        frag_directions,
+        precursor_df.frag_start_idx.values,
         precursor_df.frag_stop_idx.values,
         keep_top_k_fragments,
-        frag_df['intensity'] if use_intensity else None,
-        len(fragment_mz_df.columns)
+        frag_df["intensity"] if use_intensity else None,
+        len(fragment_mz_df.columns),
     )
-   
-    if 'number' in custom_columns:
 
-        frag_df['number'] = numbers.reshape(-1)
-   
-    if 'position' in custom_columns:
-        frag_df['position'] = positions.reshape(-1)
-    
-
-    precursor_df['flat_frag_start_idx'] = precursor_df.frag_start_idx
-    precursor_df['flat_frag_stop_idx'] = precursor_df.frag_stop_idx
-    precursor_df[['flat_frag_start_idx','flat_frag_stop_idx']] *= len(fragment_mz_df.columns)
+    if "number" in custom_columns:
+        frag_df["number"] = numbers.reshape(-1)
 
- 
-    if use_intensity:
-        frag_df['intensity'][frag_df['mz'] == 0.0] = 0.0
+    if "position" in custom_columns:
+        frag_df["position"] = positions.reshape(-1)
 
+    precursor_df["flat_frag_start_idx"] = precursor_df.frag_start_idx
+    precursor_df["flat_frag_stop_idx"] = precursor_df.frag_stop_idx
+    precursor_df[["flat_frag_start_idx", "flat_frag_stop_idx"]] *= len(
+        fragment_mz_df.columns
+    )
+
+    if use_intensity:
+        frag_df["intensity"][frag_df["mz"] == 0.0] = 0.0
 
     excluded = (
-        frag_df['mz'] == 0 if not use_intensity else
-        (
-            frag_df['intensity'] < min_fragment_intensity
-        ) | (
-            frag_df['mz'] == 0
-        ) | (
-            excluded_indices
-            )
-        )
+        frag_df["mz"] == 0
+        if not use_intensity
+        else (frag_df["intensity"] < min_fragment_intensity)
+        | (frag_df["mz"] == 0)
+        | (excluded_indices)
+    )
 
     frag_df = pd.DataFrame(frag_df)
     frag_df = frag_df[~excluded]
     frag_df = frag_df.reset_index(drop=True)
 
-    # cumulative sum counts the number of fragments before the given fragment which were removed. 
+    # cumulative sum counts the number of fragments before the given fragment which were removed.
     # This sum does not include the fragment at the index position and has therefore len N +1
-    cum_sum_tresh = np.zeros(shape=len(excluded)+1, dtype=np.int64)
+    cum_sum_tresh = np.zeros(shape=len(excluded) + 1, dtype=np.int64)
     cum_sum_tresh[1:] = np.cumsum(excluded)
 
-    precursor_df['flat_frag_start_idx'] -= cum_sum_tresh[precursor_df.flat_frag_start_idx.values]
-    precursor_df['flat_frag_stop_idx'] -= cum_sum_tresh[precursor_df.flat_frag_stop_idx.values]
+    precursor_df["flat_frag_start_idx"] -= cum_sum_tresh[
+        precursor_df.flat_frag_start_idx.values
+    ]
+    precursor_df["flat_frag_stop_idx"] -= cum_sum_tresh[
+        precursor_df.flat_frag_stop_idx.values
+    ]
 
     return precursor_df, frag_df
 
+
 @nb.njit()
 def compress_fragment_indices(frag_idx):
     """
     recalculates fragment indices to remove unused fragments. Can be used to compress a fragment library.
     Expects fragment indices to be ordered by increasing values (!!!).
     It should be O(N) runtime with N being the number of fragment rows.
-    
+
     >>> frag_idx = [[6,  10],
                 [12, 14],
                 [20, 22]]
-    
+
     >>> frag_idx = [[0, 4],
                 [4, 6],
                 [6, 8]]
     >>> fragment_pointer = [6,7,8,9,12,13,20,21]
     """
-    frag_idx_len = frag_idx[:,1]-frag_idx[:,0]
-
+    frag_idx_len = frag_idx[:, 1] - frag_idx[:, 0]
 
     # This sum does not include the fragment at the index position and has therefore len N +1
-    frag_idx_cumsum = np.zeros(shape=len(frag_idx_len)+1, dtype='int64')
+    frag_idx_cumsum = np.zeros(shape=len(frag_idx_len) + 1, dtype="int64")
     frag_idx_cumsum[1:] = np.cumsum(frag_idx_len)
 
-    fragment_pointer = np.zeros(np.sum(frag_idx_len), dtype='int64')
+    fragment_pointer = np.zeros(np.sum(frag_idx_len), dtype="int64")
 
     for i in range(len(frag_idx)):
-
         start_index = frag_idx_cumsum[i]
 
-        for j,k in enumerate(range(frag_idx[i,0],frag_idx[i,1])):
-            fragment_pointer[start_index+j]=k
-
+        for j, k in enumerate(range(frag_idx[i, 0], frag_idx[i, 1])):
+            fragment_pointer[start_index + j] = k
 
-    new_frag_idx = np.column_stack((frag_idx_cumsum[:-1],frag_idx_cumsum[1:]))
+    new_frag_idx = np.column_stack((frag_idx_cumsum[:-1], frag_idx_cumsum[1:]))
     return new_frag_idx, fragment_pointer
 
+
 def remove_unused_fragments(
-        precursor_df: pd.DataFrame, 
-        fragment_df_list: Tuple[pd.DataFrame, ...],
-        frag_start_col:str = 'frag_start_idx',
-        frag_stop_col:str = 'frag_stop_idx',
-    ) -> Tuple[pd.DataFrame, Tuple[pd.DataFrame, ...]]:
-    """Removes unused fragments of removed precursors, 
+    precursor_df: pd.DataFrame,
+    fragment_df_list: Tuple[pd.DataFrame, ...],
+    frag_start_col: str = "frag_start_idx",
+    frag_stop_col: str = "frag_stop_idx",
+) -> Tuple[pd.DataFrame, Tuple[pd.DataFrame, ...]]:
+    """Removes unused fragments of removed precursors,
     reannotates the `frag_start_col` and `frag_stop_col`
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
         Precursor dataframe which contains frag_start_idx and frag_stop_idx columns
-    
+
     fragment_df_list : List[pd.DataFrame]
         A list of fragment dataframes which should be compressed by removing unused fragments.
-        Multiple fragment dataframes can be provided which will all be sliced in the same way. 
-        This allows to slice both the fragment_mz_df and fragment_intensity_df. 
-        At least one fragment dataframe needs to be provided. 
+        Multiple fragment dataframes can be provided which will all be sliced in the same way.
+        This allows to slice both the fragment_mz_df and fragment_intensity_df.
+        At least one fragment dataframe needs to be provided.
 
     frag_start_col : str, optional
         Fragment start idx column in `precursor_df`, such as "frag_start_idx" and "peak_start_idx".
         Defaults to "frag_start_idx".
 
     frag_stop_col : str, optional
         Fragment stop idx column in `precursor_df`, such as "frag_stop_idx" and "peak_stop_idx".
         Defaults to "frag_stop_idx".
-    
+
     Returns
     -------
     pd.DataFrame, List[pd.DataFrame]
         returns the reindexed precursor DataFrame and the sliced fragment DataFrames
     """
 
     precursor_df = precursor_df.sort_values([frag_start_col], ascending=True)
-    frag_idx = precursor_df[[frag_start_col,frag_stop_col]].values
+    frag_idx = precursor_df[[frag_start_col, frag_stop_col]].values
 
     new_frag_idx, fragment_pointer = compress_fragment_indices(frag_idx)
 
-    precursor_df[[frag_start_col,frag_stop_col]] = new_frag_idx
+    precursor_df[[frag_start_col, frag_stop_col]] = new_frag_idx
     precursor_df = precursor_df.sort_index()
 
     output_tuple = []
 
     for i in range(len(fragment_df_list)):
         output_tuple.append(
-            fragment_df_list[i].iloc[
-                fragment_pointer
-            ].copy().reset_index(drop=True)
+            fragment_df_list[i].iloc[fragment_pointer].copy().reset_index(drop=True)
         )
 
     return precursor_df, tuple(output_tuple)
 
+
 def create_fragment_mz_dataframe_by_sort_precursor(
     precursor_df: pd.DataFrame,
-    charged_frag_types:List,
-    batch_size:int=500000,
-    dtype:np.dtype=PEAK_MZ_DTYPE,
-)->pd.DataFrame:
+    charged_frag_types: List,
+    batch_size: int = 500000,
+    dtype: np.dtype = PEAK_MZ_DTYPE,
+) -> pd.DataFrame:
     """Sort nAA in precursor_df for faster fragment mz dataframe creation.
-    
+
     Because the fragment mz values are continous in memory, so it is faster
     when setting values in pandas.
-    
+
     Note that this function will change the order and index of precursor_df
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursor dataframe
-    
+
     charged_frag_types : List
         fragment types list
-    
+
     batch_size : int, optional
-        Calculate fragment mz values in batch. 
+        Calculate fragment mz values in batch.
         Defaults to 500000.
     """
-    if 'frag_start_idx' in precursor_df.columns:
-        precursor_df.drop(columns=[
-            'frag_start_idx','frag_stop_idx'
-        ], inplace=True)
+    if "frag_start_idx" in precursor_df.columns:
+        precursor_df.drop(columns=["frag_start_idx", "frag_stop_idx"], inplace=True)
 
     refine_precursor_df(precursor_df)
 
     fragment_mz_df = init_fragment_by_precursor_dataframe(
-        precursor_df, charged_frag_types, 
+        precursor_df,
+        charged_frag_types,
         dtype=dtype,
     )
 
-    _grouped = precursor_df.groupby('nAA')
+    _grouped = precursor_df.groupby("nAA")
     for nAA, big_df_group in _grouped:
         for i in range(0, len(big_df_group), batch_size):
-            batch_end = i+batch_size
-            
-            df_group = big_df_group.iloc[i:batch_end,:]
+            batch_end = i + batch_size
+
+            df_group = big_df_group.iloc[i:batch_end, :]
 
             mz_values = calc_fragment_mz_values_for_same_nAA(
                 df_group, nAA, charged_frag_types
             )
 
             fragment_mz_df.iloc[
-                df_group.frag_start_idx.values[0]:
-                df_group.frag_stop_idx.values[-1], :
+                df_group.frag_start_idx.values[0] : df_group.frag_stop_idx.values[-1], :
             ] = mz_values.astype(PEAK_MZ_DTYPE)
     return mask_fragments_for_charge_greater_than_precursor_charge(
-            fragment_mz_df,
-            precursor_df.charge.values,
-            precursor_df.nAA.values,
-        )
+        fragment_mz_df,
+        precursor_df.charge.values,
+        precursor_df.nAA.values,
+    )
+
 
 def create_fragment_mz_dataframe(
     precursor_df: pd.DataFrame,
-    charged_frag_types:List,
+    charged_frag_types: List,
     *,
     reference_fragment_df: pd.DataFrame = None,
-    inplace_in_reference:bool = False,
-    batch_size:int=500000,
-    dtype:np.dtype=PEAK_MZ_DTYPE,
-)->pd.DataFrame:
-    '''
-    Generate fragment mass dataframe for the precursor_df. If 
-    the `reference_fragment_df` is provided and precursor_df contains `frag_start_idx`, 
-    it will generate  the mz dataframe based on the reference. Otherwise it 
+    inplace_in_reference: bool = False,
+    batch_size: int = 500000,
+    dtype: np.dtype = PEAK_MZ_DTYPE,
+) -> pd.DataFrame:
+    """
+    Generate fragment mass dataframe for the precursor_df. If
+    the `reference_fragment_df` is provided and precursor_df contains `frag_start_idx`,
+    it will generate  the mz dataframe based on the reference. Otherwise it
     generates the mz dataframe from scratch.
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursors to generate fragment masses,
-        if `precursor_df` contains the 'frag_start_idx' column, 
+        if `precursor_df` contains the 'frag_start_idx' column,
         `reference_fragment_df` must be provided
-        
+
     charged_frag_types : List
         `['b_z1','b_z2','y_z1','y_z2','b_modloss_1','y_H2O_z1'...]`
-    
+
     reference_fragment_df : pd.DataFrame
-        kwargs only. Generate fragment_mz_df based on this reference, 
-        as `precursor_df.frag_start_idx` and 
-        `precursor.frag_stop_idx` point to the indices in 
+        kwargs only. Generate fragment_mz_df based on this reference,
+        as `precursor_df.frag_start_idx` and
+        `precursor.frag_stop_idx` point to the indices in
         `reference_fragment_df`.
         Defaults to None
-    
+
     inplace_in_reference : bool
         kwargs only. Change values in place in the `reference_fragment_df`.
         Defaults to False
-    
+
     batch_size: int
         Number of peptides for each batch, to save RAM.
-    
+
     Returns
     -------
     pd.DataFrame
         `fragment_mz_df` with given `charged_frag_types`
-    '''
+    """
     if reference_fragment_df is None:
-        if 'frag_start_idx' in precursor_df.columns:
+        if "frag_start_idx" in precursor_df.columns:
             # raise ValueError(
             #     "`precursor_df` contains 'frag_start_idx' column, "\
             #     "please provide `reference_fragment_df` argument"
             # )
             fragment_mz_df = init_fragment_by_precursor_dataframe(
-                precursor_df, charged_frag_types,
+                precursor_df,
+                charged_frag_types,
                 dtype=dtype,
             )
             return create_fragment_mz_dataframe(
-                precursor_df=precursor_df, 
+                precursor_df=precursor_df,
                 charged_frag_types=charged_frag_types,
                 reference_fragment_df=fragment_mz_df,
                 inplace_in_reference=True,
                 batch_size=batch_size,
                 dtype=dtype,
             )
-    if 'nAA' not in precursor_df.columns:
+    if "nAA" not in precursor_df.columns:
         # fast
         return create_fragment_mz_dataframe_by_sort_precursor(
-            precursor_df, charged_frag_types, 
-            batch_size, dtype=dtype,
+            precursor_df,
+            charged_frag_types,
+            batch_size,
+            dtype=dtype,
         )
 
-    if (is_precursor_sorted(precursor_df) and 
-        reference_fragment_df is None
-    ):
+    if is_precursor_refined(precursor_df) and reference_fragment_df is None:
         # fast
         return create_fragment_mz_dataframe_by_sort_precursor(
-            precursor_df, charged_frag_types, 
-            batch_size, dtype=dtype
+            precursor_df, charged_frag_types, batch_size, dtype=dtype
         )
 
     else:
         # slow
         if reference_fragment_df is not None:
             if inplace_in_reference:
-                fragment_mz_df = reference_fragment_df.loc[:,[
-                    _fr for _fr in charged_frag_types 
-                    if _fr in reference_fragment_df.columns
-                ]]
+                fragment_mz_df = reference_fragment_df.loc[
+                    :,
+                    [
+                        _fr
+                        for _fr in charged_frag_types
+                        if _fr in reference_fragment_df.columns
+                    ],
+                ]
             else:
                 fragment_mz_df = pd.DataFrame(
-                    np.zeros((
-                        len(reference_fragment_df), 
-                        len(charged_frag_types)
-                    ), dtype=dtype),
-                    columns = charged_frag_types
+                    np.zeros(
+                        (len(reference_fragment_df), len(charged_frag_types)),
+                        dtype=dtype,
+                    ),
+                    columns=charged_frag_types,
                 )
         else:
             fragment_mz_df = init_fragment_by_precursor_dataframe(
-                precursor_df, charged_frag_types,
+                precursor_df,
+                charged_frag_types,
                 dtype=dtype,
             )
 
         frag_mz_values = fragment_mz_df.to_numpy(copy=True)
 
-        _grouped = precursor_df.groupby('nAA')
+        _grouped = precursor_df.groupby("nAA")
         for nAA, big_df_group in _grouped:
             for i in range(0, len(big_df_group), batch_size):
-                batch_end = i+batch_size
-                
-                df_group = big_df_group.iloc[i:batch_end,:]
+                batch_end = i + batch_size
+
+                df_group = big_df_group.iloc[i:batch_end, :]
 
                 mz_values = calc_fragment_mz_values_for_same_nAA(
                     df_group, nAA, fragment_mz_df.columns
                 )
-                
+
                 update_sliced_fragment_dataframe(
-                    fragment_mz_df, frag_mz_values, mz_values, 
-                    df_group[['frag_start_idx','frag_stop_idx']].values, 
+                    fragment_mz_df,
+                    frag_mz_values,
+                    mz_values,
+                    df_group[["frag_start_idx", "frag_stop_idx"]].values,
                 )
 
     fragment_mz_df.iloc[:] = frag_mz_values
 
     return mask_fragments_for_charge_greater_than_precursor_charge(
-            fragment_mz_df,
-            precursor_df.charge.values,
-            precursor_df.nAA.values,
-        )
+        fragment_mz_df,
+        precursor_df.charge.values,
+        precursor_df.nAA.values,
+    )
 
 
-# %% ../../nbdev_nbs/peptide/fragment.ipynb 38
 @nb.njit(nogil=True)
-def join_left(
-    left: np.ndarray, 
-    right: np.ndarray
-    ):
-    """joins all values in the left array to the values in the right array. 
-    The index to the element in the right array is returned. 
+def join_left(left: np.ndarray, right: np.ndarray):
+    """joins all values in the left array to the values in the right array.
+    The index to the element in the right array is returned.
     If the value wasn't found, -1 is returned. If the element appears more than once, the last appearance is used.
 
     Parameters
     ----------
 
     left: numpy.ndarray
         left array which should be matched
@@ -1129,82 +1161,81 @@
     """
     left_indices = np.argsort(left)
     left_sorted = left[left_indices]
 
     right_indices = np.argsort(right)
     right_sorted = right[right_indices]
 
-    joined_index = -np.ones(len(left), dtype='int64')
-    
+    joined_index = -np.ones(len(left), dtype="int64")
+
     # from hereon sorted arrays are expected
     lower_right = 0
 
     for i in range(len(joined_index)):
-
         for k in range(lower_right, len(right)):
-
             if left_sorted[i] >= right_sorted[k]:
                 if left_sorted[i] == right_sorted[k]:
                     joined_index[i] = k
                     lower_right = k
             else:
                 break
 
     # the joined_index_sorted connects indices from the sorted left array with the sorted right array
     # to get the original indices, the order of both sides needs to be restored
     # First, the indices pointing to the right side are restored by masking the array for hits and looking up the right side
     joined_index[joined_index >= 0] = right_indices[joined_index[joined_index >= 0]]
 
     # Next, the left side is restored by arranging the items
-    joined_index[left_indices] =  joined_index
+    joined_index[left_indices] = joined_index
 
     return joined_index
 
-def calc_fragment_count(
-        precursor_df : pd.DataFrame, 
-        fragment_intensity_df : pd.DataFrame
-    ):
 
+def calc_fragment_count(
+    precursor_df: pd.DataFrame, fragment_intensity_df: pd.DataFrame
+):
     """
     Calculates the number of fragments for each precursor.
 
     Parameters
     ----------
 
     precursor_df : pd.DataFrame
         precursor dataframe which contains the frag_start_idx and frag_stop_idx columns
 
     fragment_intensity_df : pd.DataFrame
         fragment intensity dataframe which contains the fragment intensities
 
     Returns
-    ------- 
+    -------
     numpy.ndarray
         array with the number of fragments for each precursor
     """
-    if not set(['frag_start_idx', 'frag_stop_idx']).issubset(precursor_df.columns):
-        raise KeyError('frag_start_idx and frag_stop_idx not in dataframe')
-    
+    if not set(["frag_start_idx", "frag_stop_idx"]).issubset(precursor_df.columns):
+        raise KeyError("frag_start_idx and frag_stop_idx not in dataframe")
+
     n_fragments = []
-    
-    for start, stop in zip(precursor_df['frag_start_idx'].values, precursor_df['frag_stop_idx'].values):
+
+    for start, stop in zip(
+        precursor_df["frag_start_idx"].values, precursor_df["frag_stop_idx"].values
+    ):
         n_fragments += [np.sum(fragment_intensity_df.iloc[start:stop].values > 0)]
 
     return np.array(n_fragments)
-  
-def filter_fragment_number(
-        precursor_df : pd.DataFrame, 
-        fragment_intensity_df : pd.DataFrame,
-        n_fragments_allowed_column_name : str = 'n_fragments_allowed',
-        n_allowed : int = 999
-    ):
 
+
+def filter_fragment_number(
+    precursor_df: pd.DataFrame,
+    fragment_intensity_df: pd.DataFrame,
+    n_fragments_allowed_column_name: str = "n_fragments_allowed",
+    n_allowed: int = 999,
+):
     """
     Filters the number of fragments for each precursor.
-        
+
     Parameters
     ----------
 
     precursor_df : pd.DataFrame
 
         precursor dataframe which contains the frag_start_idx and frag_stop_idx columns
 
@@ -1218,134 +1249,151 @@
         number of fragments which should be allowed
 
     Returns
     -------
     None
     """
 
-    if not set(['frag_start_idx', 'frag_stop_idx']).issubset(precursor_df.columns):
-        raise KeyError('frag_start_idx and frag_stop_idx not in dataframe')
+    if not set(["frag_start_idx", "frag_stop_idx"]).issubset(precursor_df.columns):
+        raise KeyError("frag_start_idx and frag_stop_idx not in dataframe")
 
     for i, (start_idx, stop_idx, n_allowed_lib) in enumerate(
         zip(
-            precursor_df['frag_start_idx'].values, 
-            precursor_df['frag_stop_idx'].values, 
-            precursor_df[n_fragments_allowed_column_name].values
-            )
-        ):
-
+            precursor_df["frag_start_idx"].values,
+            precursor_df["frag_stop_idx"].values,
+            precursor_df[n_fragments_allowed_column_name].values,
+        )
+    ):
         _allowed = min(n_allowed_lib, n_allowed)
 
         intensies = fragment_intensity_df.iloc[start_idx:stop_idx].values
         flat_intensities = np.sort(intensies.flatten())[::-1]
         intensies[intensies <= flat_intensities[_allowed]] = 0
         fragment_intensity_df.iloc[start_idx:stop_idx] = intensies
-        
-def calc_fragment_cardinality(
-        precursor_df,
-        fragment_mz_df,
-        group_column = 'elution_group_idx',
-        split_target_decoy = True
-    ):
 
+
+def calc_fragment_cardinality(
+    precursor_df,
+    fragment_mz_df,
+    group_column="elution_group_idx",
+    split_target_decoy=True,
+):
     """
     Calculate the cardinality for a given fragment across a group of precursors.
     The cardinality is the number of precursors that have a given fragment at a given position.
 
-    All precursors within a group are expected to have the same number of fragments.    
+    All precursors within a group are expected to have the same number of fragments.
     The precursor dataframe.
 
     fragment_mz_df : pd.DataFrame
         The fragment mz dataframe.
 
     group_column : str
         The column to group the precursors by. Integer column is expected.
 
     split_target_decoy : bool
         If True, the cardinality is calculated for the target and decoy precursors separately.
 
     """
-    
+
     if len(precursor_df) == 0:
-        raise ValueError('Precursor dataframe is empty.')
-    
+        raise ValueError("Precursor dataframe is empty.")
+
     if len(fragment_mz_df) == 0:
-        raise ValueError('Fragment dataframe is empty.')
-    
+        raise ValueError("Fragment dataframe is empty.")
+
     if group_column not in precursor_df.columns:
-        raise KeyError('Group column not in precursor dataframe.')
-    
-    if ('frag_start_idx' not in precursor_df.columns) or ('frag_stop_idx' not in precursor_df.columns):
-        raise KeyError('Precursor dataframe does not contain fragment indices.')
-    
+        raise KeyError("Group column not in precursor dataframe.")
+
+    if ("frag_start_idx" not in precursor_df.columns) or (
+        "frag_stop_idx" not in precursor_df.columns
+    ):
+        raise KeyError("Precursor dataframe does not contain fragment indices.")
+
     precursor_df = precursor_df.sort_values(group_column)
     fragment_mz = fragment_mz_df.values
     fragment_cardinality = np.ones(fragment_mz.shape, dtype=np.uint8)
 
     @nb.njit
     def _calc_fragment_cardinality(
         elution_group_idx,
         start_idx,
         stop_idx,
         fragment_mz,
         fragment_cardinality,
     ):
-        elution_group = elution_group_idx[0]
+        if len(elution_group_idx) == 0:
+            return
+        elution_group_idx[0]  # noqa TODO check for potential bug
         elution_group_start = 0
 
         for i in range(len(elution_group_idx)):
-            if i == len(elution_group_idx)-1 or elution_group_idx[i] != elution_group_idx[i+1]:
-                elution_group_stop = i+1
+            if (
+                i == len(elution_group_idx) - 1
+                or elution_group_idx[i] != elution_group_idx[i + 1]
+            ):
+                elution_group_stop = i + 1
 
             # check if whole elution group is covered
             n_precursor = elution_group_stop - elution_group_start
-            
+
             # Check that all precursors within a group have the same number of fragments.
-            nAA = stop_idx[elution_group_start:elution_group_stop] - start_idx[elution_group_start:elution_group_stop]
+            nAA = (
+                stop_idx[elution_group_start:elution_group_stop]
+                - start_idx[elution_group_start:elution_group_stop]
+            )
             if not np.all(nAA[0] == nAA):
-                raise ValueError('All precursors within a group must have the same number of fragments.')
+                raise ValueError(
+                    "All precursors within a group must have the same number of fragments."
+                )
 
             # within a group, check for each precursor if it has the same fragment as another precursor
             for i in range(n_precursor):
-
                 precursor_start_idx = start_idx[elution_group_start + i]
                 precursor_stop_idx = stop_idx[elution_group_start + i]
 
-                precursor_fragment_mz = fragment_mz[precursor_start_idx:precursor_stop_idx]
+                precursor_fragment_mz = fragment_mz[
+                    precursor_start_idx:precursor_stop_idx
+                ]
 
                 for j in range(n_precursor):
                     if i == j:
                         continue
 
                     other_precursor_start_idx = start_idx[elution_group_start + j]
                     other_precursor_stop_idx = stop_idx[elution_group_start + j]
-                    other_precursor_fragment_mz = fragment_mz[other_precursor_start_idx:other_precursor_stop_idx]
-                    
-                    binary_mask = np.abs(precursor_fragment_mz - other_precursor_fragment_mz) < 0.00001
-                    
-                    fragment_cardinality[precursor_start_idx:precursor_stop_idx] += binary_mask.astype(np.uint8)
-                    
+                    other_precursor_fragment_mz = fragment_mz[
+                        other_precursor_start_idx:other_precursor_stop_idx
+                    ]
+
+                    binary_mask = (
+                        np.abs(precursor_fragment_mz - other_precursor_fragment_mz)
+                        < 0.00001
+                    )
+
+                    fragment_cardinality[precursor_start_idx:precursor_stop_idx] += (
+                        binary_mask.astype(np.uint8)
+                    )
+
             elution_group_start = elution_group_stop
-    if ('decoy' in precursor_df.columns) and (split_target_decoy):
-        decoy_classes = precursor_df['decoy'].unique()
+
+    if ("decoy" in precursor_df.columns) and (split_target_decoy):
+        decoy_classes = precursor_df["decoy"].unique()
         for decoy_class in decoy_classes:
-            df = precursor_df[precursor_df['decoy'] == decoy_class]
+            df = precursor_df[precursor_df["decoy"] == decoy_class]
             _calc_fragment_cardinality(
                 df[group_column].values,
-                df['frag_start_idx'].values,
-                df['frag_stop_idx'].values,
+                df["frag_start_idx"].values,
+                df["frag_stop_idx"].values,
                 fragment_mz,
                 fragment_cardinality,
             )
     else:
         _calc_fragment_cardinality(
             precursor_df[group_column].values,
-            precursor_df['frag_start_idx'].values,
-            precursor_df['frag_stop_idx'].values,
+            precursor_df["frag_start_idx"].values,
+            precursor_df["frag_stop_idx"].values,
             fragment_mz,
             fragment_cardinality,
         )
 
-    return pd.DataFrame(
-        fragment_cardinality, 
-        columns = fragment_mz_df.columns
-    )
+    return pd.DataFrame(fragment_cardinality, columns=fragment_mz_df.columns)
```

### Comparing `alphabase-1.2.3/alphabase/peptide/mass_calc.py` & `alphabase-1.2.4/alphabase/peptide/mass_calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,254 +1,244 @@
 import numpy as np
 from typing import List, Tuple
 
 from alphabase.constants.aa import (
-    calc_AA_masses, 
+    calc_AA_masses,
     calc_AA_masses_for_same_len_seqs,
-    calc_sequence_masses_for_same_len_seqs
+    calc_sequence_masses_for_same_len_seqs,
 )
 from alphabase.constants.modification import (
     calc_modification_mass,
     calc_modification_mass_sum,
-    calc_mod_masses_for_same_len_seqs
+    calc_mod_masses_for_same_len_seqs,
 )
-from alphabase.constants.element import MASS_H2O
+from alphabase.constants.atom import MASS_H2O
+
 
 def calc_diff_modification_mass(
-    pep_len:int,
-    mass_diffs:List[float],
-    mass_diff_sites:List[int]
-)->np.ndarray:
-    '''
-    For open-search, we may also get modification 
+    pep_len: int, mass_diffs: List[float], mass_diff_sites: List[int]
+) -> np.ndarray:
+    """
+    For open-search, we may also get modification
     mass diffs other than mod names. This function calculate
     modification masses from these diff masses.
-    
+
     Parameters
     ----------
     pep_len : int
         nAA
-    
+
     mass_diffs : List[float]
         mass diffs on the peptide
 
     mass_diff_sites : List[int]
         localized sites of corresponding mass diffs
 
     Returns
     -------
     np.ndarray
         1-D array with length=`peplen`.
         Masses of modifications (mass diffs) through the peptide,
         `0` if sites has no modifications
-    '''
+    """
     masses = np.zeros(pep_len)
     for site, mass in zip(mass_diff_sites, mass_diffs):
         if site == 0:
             masses[site] += mass
         elif site == -1:
             masses[site] += mass
         else:
-            masses[site-1] += mass
+            masses[site - 1] += mass
     return masses
 
+
 def calc_mod_diff_masses_for_same_len_seqs(
-    nAA:int, 
-    aa_mass_diffs_list:List[List[float]], 
-    mod_sites_list:List[List[int]]
-)->np.ndarray:
-    '''
-    Calculate diff modification masses for the given peptide length (`nAA`), 
-    For open-search, we may also get modification 
+    nAA: int, aa_mass_diffs_list: List[List[float]], mod_sites_list: List[List[int]]
+) -> np.ndarray:
+    """
+    Calculate diff modification masses for the given peptide length (`nAA`),
+    For open-search, we may also get modification
     mass diffs other than mod names. This function calculate
     modification masses from these diff masses.
-    
+
     Parameters
     ----------
     nAA : int
         peptide length
 
     mod_names_list : List[List[str]]
         list of modification list
 
     mod_sites_list : List[List[int]]
-        list of modification site list corresponding 
+        list of modification site list corresponding
         to `mod_names_list`.
         * `site=0` refers to an N-term modification
         * `site=-1` refers to a C-term modification
         * `1<=site<=peplen` refers to a normal modification
-    
+
     Returns
     -------
     np.ndarray
-        2-D array with shape=`(nAA, pep_count or len(mod_names_list)))`. 
-        Masses of modifications through all the peptides, 
+        2-D array with shape=`(nAA, pep_count or len(mod_names_list)))`.
+        Masses of modifications through all the peptides,
         `0` if sites has no modifications
-    '''
-    masses = np.zeros((len(aa_mass_diffs_list),nAA))
+    """
+    masses = np.zeros((len(aa_mass_diffs_list), nAA))
     for i, (aa_mass_diffs, mod_sites) in enumerate(
         zip(aa_mass_diffs_list, mod_sites_list)
     ):
-        for mod_diff, site in zip(aa_mass_diffs, mod_sites): 
+        for mod_diff, site in zip(aa_mass_diffs, mod_sites):
             if site == 0:
-                masses[i,site] += mod_diff
+                masses[i, site] += mod_diff
             elif site == -1:
-                masses[i,site] += mod_diff
+                masses[i, site] += mod_diff
             else:
-                masses[i,site-1] += mod_diff
+                masses[i, site - 1] += mod_diff
     return masses
 
+
 def calc_b_y_and_peptide_mass(
     sequence: str,
     mod_names: List[str],
     mod_sites: List[int],
     aa_mass_diffs: List[float] = None,
     aa_mass_diff_sites: List[int] = None,
-)->Tuple[np.ndarray,np.ndarray,float]:
-    '''
-    It is highly recommend to use 
+) -> Tuple[np.ndarray, np.ndarray, float]:
+    """
+    It is highly recommend to use
     `calc_b_y_and_peptide_masses_for_same_len_seqs`
     as it is much faster
-    '''
+    """
     residue_masses = calc_AA_masses(sequence)
-    mod_masses = calc_modification_mass(
-        len(sequence), mod_names, mod_sites
-    )
+    mod_masses = calc_modification_mass(len(sequence), mod_names, mod_sites)
     residue_masses += mod_masses
     if aa_mass_diffs is not None:
         mod_masses = calc_diff_modification_mass(
             len(sequence), aa_mass_diffs, aa_mass_diff_sites
         )
         residue_masses += mod_masses
-    #residue_masses = residue_masses[np.newaxis, ...]
+    # residue_masses = residue_masses[np.newaxis, ...]
     b_masses = np.cumsum(residue_masses)
     b_masses, pepmass = b_masses[:-1], b_masses[-1]
-        
+
     pepmass += MASS_H2O
     y_masses = pepmass - b_masses
     return b_masses, y_masses, pepmass
 
+
 def calc_peptide_masses_for_same_len_seqs(
-    sequences: np.ndarray,
-    mod_list: List[str],
-    mod_diff_list: List[str]=None
-)->np.ndarray:
-    '''
+    sequences: np.ndarray, mod_list: List[str], mod_diff_list: List[str] = None
+) -> np.ndarray:
+    """
     Calculate peptide masses for peptide sequences with same lengths.
-    We need 'same_len' here because numpy can process AA sequences 
-    with same length very fast. 
+    We need 'same_len' here because numpy can process AA sequences
+    with same length very fast.
     See `alphabase.aa.calc_sequence_masses_for_same_len_seqs`
 
     Parameters
     ----------
     mod_list : List[str]
 
-        list of modifications, 
+        list of modifications,
         e.g. `['Oxidation@M;Phospho@S','Phospho@S;Deamidated@N']`
 
     mass_diff_list : List[str]
-    
+
         List of modifications as mass diffs,
         e.g. `['15.9xx;79.9xxx','79.9xx;0.98xx']`
-    
+
     Returns
     -------
         np.ndarray
-            
+
             peptide masses (1-D array, H2O already added)
-    '''
-    seq_masses = calc_sequence_masses_for_same_len_seqs(
-        sequences
-    )
+    """
+    seq_masses = calc_sequence_masses_for_same_len_seqs(sequences)
     mod_masses = np.zeros_like(seq_masses)
     for i, mods in enumerate(mod_list):
         if len(mods) > 0:
-            mod_masses[i] = calc_modification_mass_sum(
-                mods.split(';')
-            )
+            mod_masses[i] = calc_modification_mass_sum(mods.split(";"))
     if mod_diff_list is not None:
         for i, mass_diffs in enumerate(mod_diff_list):
             if len(mass_diffs) > 0:
-                mod_masses[i] += np.sum([
-                    float(mass) for mass in mass_diffs.split(';')
-                ])
-    return seq_masses+mod_masses
-    
+                mod_masses[i] += np.sum([float(mass) for mass in mass_diffs.split(";")])
+    return seq_masses + mod_masses
+
 
 def calc_b_y_and_peptide_masses_for_same_len_seqs(
     sequences: np.ndarray,
     mod_list: List[List[str]],
     site_list: List[List[int]],
-    mod_diff_list: List[List[float]]=None,
-    mod_diff_site_list: List[List[int]]=None,
-)->Tuple[np.ndarray,np.ndarray,np.ndarray]:
-    '''
-    Calculate b/y fragment masses and peptide masses 
+    mod_diff_list: List[List[float]] = None,
+    mod_diff_site_list: List[List[int]] = None,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """
+    Calculate b/y fragment masses and peptide masses
     for peptide sequences with same lengths.
-    We need 'same_len' here because numpy can process AA sequences 
+    We need 'same_len' here because numpy can process AA sequences
     with same length very fast.
 
     Parameters
     ----------
     sequence : np.ndarray of str
         np.ndarray of peptie sequences with same length.
 
     mod_list : List[List[str]]
-        list of modifications , 
-        e.g. `[['Oxidation@M','Phospho@S'],['Phospho@S','Deamidated@N']]` 
+        list of modifications ,
+        e.g. `[['Oxidation@M','Phospho@S'],['Phospho@S','Deamidated@N']]`
 
     site_list : List[List[int]]
         list of modification sites
         corresponding to `mod_list`, e.g. `[[3,6],[4,17]]`
 
     mod_diff_list : List[List[float]]
-        list of modifications, 
-        e.g. `[[15.994915,79.966331],[79.966331,0.984016]]` 
+        list of modifications,
+        e.g. `[[15.994915,79.966331],[79.966331,0.984016]]`
 
     mod_diff_site_list : List[List[int]]
         list of modification mass diff sites
         corresponding to `mod_list`, e.g. `[[3,6],[4,17]]`
-    
+
     Returns
     -------
     np.ndarray
         neutral b fragment masses (2-D array)
 
     np.ndarray
         neutral y fragmnet masses (2-D array)
 
     np.ndarray
         neutral peptide masses (1-D array)
-    '''
+    """
     aa_masses = calc_AA_masses_for_same_len_seqs(sequences)
     nAA = len(sequences[0])
 
     # mod_masses = np.zeros_like(aa_masses)
     # for i, (mods, sites) in enumerate(zip(mod_list, site_list)):
     #     if len(mods) != 0:
     #         mod_masses[i,:] = calc_modification_mass(
-    #             seq_len, 
-    #             mods, 
+    #             seq_len,
+    #             mods,
     #             sites,
     #         )
     mod_masses = calc_mod_masses_for_same_len_seqs(nAA, mod_list, site_list)
     if mod_diff_list is not None:
         mod_masses += calc_mod_diff_masses_for_same_len_seqs(
             nAA, mod_diff_list, mod_diff_site_list
         )
         # for i, (mass_diffs, sites) in enumerate(zip(
         #     mass_diff_list, mass_diff_site_list
         # )):
         #     if len(mass_diffs) != 0:
         #         mod_masses[i,:] += calc_diff_modification_mass(
-        #             seq_len, 
-        #             mass_diffs, 
+        #             seq_len,
+        #             mass_diffs,
         #             sites,
         #         )
     aa_masses += mod_masses
 
     b_masses = np.cumsum(aa_masses, axis=1)
-    b_masses, pepmass = b_masses[:,:-1], b_masses[:,-1:]
-        
+    b_masses, pepmass = b_masses[:, :-1], b_masses[:, -1:]
+
     pepmass += MASS_H2O
     y_masses = pepmass - b_masses
     return b_masses, y_masses, pepmass.flatten()
```

### Comparing `alphabase-1.2.3/alphabase/peptide/mobility.py` & `alphabase-1.2.4/alphabase/peptide/mobility.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,107 @@
 import numpy as np
 import pandas as pd
 
-from alphabase.peptide.fragment import update_precursor_mz
-from alphabase.constants.element import common_const_dict
+from alphabase.peptide.precursor import update_precursor_mz
+from alphabase.constants.atom import common_const_dict
 
-CCS_IM_COEF = common_const_dict['MOBILITY']['CCS_IM_COEF']
-IM_GAS_MASS = common_const_dict['MOBILITY']['IM_GAS_MASS']
+CCS_IM_COEF = common_const_dict["MOBILITY"]["CCS_IM_COEF"]
+IM_GAS_MASS = common_const_dict["MOBILITY"]["IM_GAS_MASS"]
+
+
+def get_reduced_mass(precursor_mzs: np.ndarray, charges: np.ndarray) -> np.ndarray:
+    """Reduced mass for CCS and mobility calculation"""
+    reduced_masses = precursor_mzs * charges
+    return reduced_masses * IM_GAS_MASS / (reduced_masses + IM_GAS_MASS)
 
-def get_reduced_mass(
-    precursor_mzs: np.ndarray, 
-    charges: np.ndarray
-)->np.ndarray:
-    """ Reduced mass for CCS and mobility calculation """
-    reduced_masses = precursor_mzs*charges
-    return reduced_masses*IM_GAS_MASS/(reduced_masses+IM_GAS_MASS)
 
 def ccs_to_mobility_bruker(
-    ccs_values: np.ndarray, 
-    charges: np.ndarray, 
-    precursor_mzs: np.ndarray
-)->np.ndarray:
-    """ Convert CCS to mobility for Bruker (timsTOF) """
+    ccs_values: np.ndarray, charges: np.ndarray, precursor_mzs: np.ndarray
+) -> np.ndarray:
+    """Convert CCS to mobility for Bruker (timsTOF)"""
     reduced_masses = get_reduced_mass(precursor_mzs, charges)
-    return ccs_values*np.sqrt(reduced_masses)/charges/CCS_IM_COEF
+    return ccs_values * np.sqrt(reduced_masses) / charges / CCS_IM_COEF
+
 
 def mobility_to_ccs_bruker(
-    im_values: np.ndarray, 
-    charges: np.ndarray, 
-    precursor_mzs: np.ndarray
-)->np.ndarray:
-    """ Convert mobility to CCS for Bruker (timsTOF) """
+    im_values: np.ndarray, charges: np.ndarray, precursor_mzs: np.ndarray
+) -> np.ndarray:
+    """Convert mobility to CCS for Bruker (timsTOF)"""
     reduced_masses = get_reduced_mass(precursor_mzs, charges)
-    return im_values*charges*CCS_IM_COEF/np.sqrt(reduced_masses)
+    return im_values * charges * CCS_IM_COEF / np.sqrt(reduced_masses)
+
 
 def ccs_to_mobility_for_df(
-    precursor_df:pd.DataFrame,
-    ccs_column:str,
-    *,
-    vendor="bruker"
-)->np.ndarray:
+    precursor_df: pd.DataFrame, ccs_column: str, *, vendor="bruker"
+) -> np.ndarray:
     """
 
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursor_df
 
     ccs_column : str
         CCS column name in precursor_df
 
     vendor : str, optional
-        Different vender may have different IM calculation. 
+        Different vender may have different IM calculation.
         Defaults to "bruker".
         Note that other vendors are not implemented currently.
 
     Returns
     -------
     np.ndarray
         mobility values
     """
-    if 'precursor_mz' not in precursor_df.columns:
+    if "precursor_mz" not in precursor_df.columns:
         precursor_df = update_precursor_mz(precursor_df)
     return ccs_to_mobility_bruker(
-        precursor_df[ccs_column].values, 
+        precursor_df[ccs_column].values,
         precursor_df.charge.values,
-        precursor_df.precursor_mz.values
+        precursor_df.precursor_mz.values,
     )
 
+
 def mobility_to_ccs_for_df(
-    precursor_df:pd.DataFrame,
-    mobility_column:str,
-    *,
-    vendor="bruker"
-)->np.ndarray:
+    precursor_df: pd.DataFrame, mobility_column: str, *, vendor="bruker"
+) -> np.ndarray:
     """
 
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursor_df
 
     mobility_column : str
         mobility column name in precursor_df
 
     vendor : str, optional
-        Different vender may have different IM calculation. 
+        Different vender may have different IM calculation.
         Defaults to "bruker".
         Note that other vendors are not implemented currently.
 
     Returns
     -------
     np.ndarray
         CCS values
     """
-    
-    if 'precursor_mz' not in precursor_df.columns:
+
+    if "precursor_mz" not in precursor_df.columns:
         precursor_df = update_precursor_mz(precursor_df)
     if precursor_df[mobility_column].isna().any():
         print(f"NA/nan is detected in the `{mobility_column}` column, fillna with 0.0")
-        precursor_df[mobility_column] = precursor_df[mobility_column].fillna(0.0).astype(np.float64)
-    if (precursor_df[mobility_column]=="").any():
-        print(f"Empty string is detected in the `{mobility_column}` column, fill with 0.0")
-        precursor_df[mobility_column] = precursor_df[mobility_column].replace("",0.0).astype(np.float64)
+        precursor_df[mobility_column] = (
+            precursor_df[mobility_column].fillna(0.0).astype(np.float64)
+        )
+    if (precursor_df[mobility_column] == "").any():
+        print(
+            f"Empty string is detected in the `{mobility_column}` column, fill with 0.0"
+        )
+        precursor_df[mobility_column] = (
+            precursor_df[mobility_column].replace("", 0.0).astype(np.float64)
+        )
     return mobility_to_ccs_bruker(
         precursor_df[mobility_column].values,
         precursor_df.charge.values,
-        precursor_df.precursor_mz.values
+        precursor_df.precursor_mz.values,
     )
```

### Comparing `alphabase-1.2.3/alphabase/peptide/precursor.py` & `alphabase-1.2.4/alphabase/peptide/precursor.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,312 +4,327 @@
 import typing
 import multiprocessing as mp
 from tqdm import tqdm
 
 from xxhash import xxh64_intdigest
 from functools import partial
 
-from alphabase.constants.element import (
-    MASS_PROTON, MASS_ISOTOPE
-)
+from alphabase.constants.atom import MASS_PROTON, MASS_ISOTOPE
 from alphabase.constants.aa import AA_Composition
 from alphabase.constants.modification import MOD_Composition
-from alphabase.constants.isotope import (
-    IsotopeDistribution
-)
-from alphabase.peptide.mass_calc import (
-    calc_peptide_masses_for_same_len_seqs
-)
+from alphabase.constants.isotope import IsotopeDistribution
+from alphabase.peptide.mass_calc import calc_peptide_masses_for_same_len_seqs
+
 
 def refine_precursor_df(
-    df:pd.DataFrame, 
-    drop_frag_idx = False,
-    ensure_data_validity = False,
-)->pd.DataFrame:
-    """ 
+    df: pd.DataFrame,
+    drop_frag_idx=False,
+    ensure_data_validity=False,
+) -> pd.DataFrame:
+    """
     Refine df inplace for faster precursor/fragment calculation.
     """
     if ensure_data_validity:
-        df.fillna('', inplace=True)
-        if 'charge' in df.columns:
+        df.fillna("", inplace=True)
+        if "charge" in df.columns:
             if df.charge.dtype not in [
-                'int','int8','int64','int32',
+                "int",
+                "int8",
+                "int64",
+                "int32",
                 # np.int64, np.int32, np.int8,
             ]:
-                df['charge'] = df['charge'].astype(np.int8)
-        if 'mod_sites' in df.columns:
-            if df.mod_sites.dtype not in ['O','U']:
-                df['mod_sites'] = df.mod_sites.astype('U')
-
-    if 'nAA' not in df.columns:
-        df['nAA']= df.sequence.str.len().astype(np.int32)
-
-    if drop_frag_idx and 'frag_start_idx' in df.columns:
-        df.drop(columns=[
-            'frag_start_idx','frag_stop_idx'
-        ], inplace=True)
+                df["charge"] = df["charge"].astype(np.int8)
+        if "mod_sites" in df.columns:
+            if df.mod_sites.dtype not in ["O", "U"]:
+                df["mod_sites"] = df.mod_sites.astype("U")
+
+    if "nAA" not in df.columns:
+        df["nAA"] = df.sequence.str.len().astype(np.int32)
+
+    if drop_frag_idx and "frag_start_idx" in df.columns:
+        df.drop(columns=["frag_start_idx", "frag_stop_idx"], inplace=True)
 
     if not is_precursor_refined(df):
-        df.sort_values('nAA', inplace=True)
+        df.sort_values("nAA", inplace=True)
         df.reset_index(drop=True, inplace=True)
 
     return df
 
+
 reset_precursor_df = refine_precursor_df
 
+
 def is_precursor_refined(precursor_df: pd.DataFrame):
-    return (
-        (len(precursor_df) == 0) or (
-            (precursor_df.index.values[0] == 0) and
-            precursor_df.nAA.is_monotonic_increasing and
-            np.all(
-                np.diff(precursor_df.index.values)==1
-            )
-        )
+    return (len(precursor_df) == 0) or (
+        (precursor_df.index.values[0] == 0)
+        and precursor_df.nAA.is_monotonic_increasing
+        and np.all(np.diff(precursor_df.index.values) == 1)
+    )
+
+
+def is_precursor_sorted(precursor_df: pd.DataFrame):
+    import warnings
+
+    warnings.warn(
+        "`alphabase.peptide.precursor.is_precursor_sorted()` is deprecated, "
+        "it will be removed in alphabse>=1.3.0. "
+        "Please use `alphabase.peptide.precursor.is_precursor_refined()` instead.",
+        FutureWarning,
     )
+    return is_precursor_refined(precursor_df)
 
-is_precursor_sorted = is_precursor_refined
 
 def update_precursor_mz(
     precursor_df: pd.DataFrame,
-    batch_size = 500000,
-)->pd.DataFrame:
+    batch_size=500000,
+) -> pd.DataFrame:
     """
     Calculate precursor_mz inplace in the precursor_df
-    
+
     Parameters
     ----------
     precursor_df : pd.DataFrame
 
         precursor_df with the 'charge' column
 
     Returns
     -------
     pd.DataFrame
-        
+
         precursor_df with 'precursor_mz'
     """
 
-    if 'nAA' not in precursor_df:
+    if "nAA" not in precursor_df:
         reset_precursor_df(precursor_df)
         _calc_in_order = True
-    elif is_precursor_sorted(precursor_df):
+    elif is_precursor_refined(precursor_df):
         _calc_in_order = True
     else:
         _calc_in_order = False
-    precursor_df['precursor_mz'] = 0.
+    precursor_df["precursor_mz"] = 0.0
     precursor_mzs = np.zeros(len(precursor_df))
-    _grouped = precursor_df.groupby('nAA')
+    _grouped = precursor_df.groupby("nAA")
     # precursor_mz_idx = precursor_df.columns.get_loc(
     #     'precursor_mz'
     # )
     for nAA, big_df_group in _grouped:
         for i in range(0, len(big_df_group), batch_size):
-            batch_end = i+batch_size
-            
-            df_group = big_df_group.iloc[i:batch_end,:]
-
-            pep_mzs = calc_peptide_masses_for_same_len_seqs(
-                df_group.sequence.values.astype('U'),
-                df_group.mods.values,
-                df_group.aa_mass_diffs.values if 
-                'aa_mass_diffs' in df_group.columns else None
-            )/df_group.charge + MASS_PROTON
+            batch_end = i + batch_size
+
+            df_group = big_df_group.iloc[i:batch_end, :]
+
+            pep_mzs = (
+                calc_peptide_masses_for_same_len_seqs(
+                    df_group.sequence.values.astype("U"),
+                    df_group.mods.values,
+                    df_group.aa_mass_diffs.values
+                    if "aa_mass_diffs" in df_group.columns
+                    else None,
+                )
+                / df_group.charge
+                + MASS_PROTON
+            )
             if _calc_in_order:
                 precursor_mzs[
-                    df_group.index.values[0]:
-                    df_group.index.values[-1]+1
+                    df_group.index.values[0] : df_group.index.values[-1] + 1
                 ] = pep_mzs
             else:
-                precursor_df.loc[
-                    df_group.index, 'precursor_mz'
-                ] = pep_mzs
+                precursor_df.loc[df_group.index, "precursor_mz"] = pep_mzs
     if _calc_in_order:
         precursor_df["precursor_mz"] = precursor_mzs
     return precursor_df
 
-calc_precursor_mz = update_precursor_mz
+
+def calc_precursor_mz(precursor_df: pd.DataFrame, batch_size: int = 500000):
+    import warnings
+
+    warnings.warn(
+        "`alphabase.peptide.precursor.calc_precursor_mz()` is deprecated, "
+        "it will be removed in alphabse>=2.0.0. "
+        "Please use `alphabase.peptide.precursor.update_precursor_mz()` instead.",
+        FutureWarning,
+    )
+    return update_precursor_mz(precursor_df, batch_size)
+
 
 def get_mod_seq_hash(
-    sequence:str, mods:str, 
-    mod_sites:str,
-    *, seed:int=0
-)->np.uint64:
+    sequence: str, mods: str, mod_sites: str, *, seed: int = 0
+) -> np.uint64:
     """Get hash code value for a peptide:
       (sequence, mods, mod_sites)
 
     Parameters
     ----------
         sequence : str
-            
+
             Amino acid sequence
 
         mods : str
-            
+
             Modification names in AlphaBase format
 
         mod_sites : str
-        
+
             Modification sites in AlphaBase format
 
         seed : int
-            
+
             Seed for hashing.
             Optional, by default 0
 
     Returns
     -------
     np.uint64
 
         64-bit hash code value
     """
-    return np.array([
-        xxh64_intdigest(sequence, seed=seed),
-        xxh64_intdigest(mods, seed=seed),
-        xxh64_intdigest(mod_sites, seed=seed),
-    ],dtype=np.uint64).sum() # use np.sum to prevent overflow
+    return np.array(
+        [
+            xxh64_intdigest(sequence, seed=seed),
+            xxh64_intdigest(mods, seed=seed),
+            xxh64_intdigest(mod_sites, seed=seed),
+        ],
+        dtype=np.uint64,
+    ).sum()  # use np.sum to prevent overflow
+
 
 def get_mod_seq_charge_hash(
-    sequence:str, mods:str, 
-    mod_sites:str, charge:int,
-    *, seed=0
+    sequence: str, mods: str, mod_sites: str, charge: int, *, seed=0
 ):
     """Get hash code value for a precursor:
       (sequence, mods, mod_sites, charge)
 
     Parameters
     ----------
     sequence : str
 
         Amino acid sequence
 
     mods : str
-        
+
         Modification names in AlphaBase format
 
     mod_sites : str
-    
+
         Modification sites in AlphaBase format
 
     charge : int
-    
+
         Precursor charge state
 
     seed : int
-    
+
         Seed for hashing.
         Optional, by default 0
 
     Returns
     -------
     np.uint64
-    
+
         64-bit hash code value
     """
-    return np.array([
-        get_mod_seq_hash(
-            sequence, mods, mod_sites, 
-            seed=seed
-        ),
-        charge,
-    ],dtype=np.uint64).sum() # use np.sum to prevent overflow 
-
-def hash_mod_seq_df(
-    precursor_df:pd.DataFrame,
-    *, seed=0
-):
-    """ Internal function """
+    return np.array(
+        [
+            get_mod_seq_hash(sequence, mods, mod_sites, seed=seed),
+            charge,
+        ],
+        dtype=np.uint64,
+    ).sum()  # use np.sum to prevent overflow
+
+
+def hash_mod_seq_df(precursor_df: pd.DataFrame, *, seed=0):
+    """Internal function"""
     hash_vals = precursor_df.sequence.apply(
         lambda x: xxh64_intdigest(x, seed=seed)
     ).to_numpy(copy=True, dtype=np.uint64)
-    hash_vals += precursor_df.mods.apply(
-        lambda x: xxh64_intdigest(x, seed=seed)
-    ).astype(np.uint64).values
-    hash_vals += precursor_df.mod_sites.apply(
-        lambda x: xxh64_intdigest(x, seed=seed)
-    ).astype(np.uint64).values
+    hash_vals += (
+        precursor_df.mods.apply(lambda x: xxh64_intdigest(x, seed=seed))
+        .astype(np.uint64)
+        .values
+    )
+    hash_vals += (
+        precursor_df.mod_sites.apply(lambda x: xxh64_intdigest(x, seed=seed))
+        .astype(np.uint64)
+        .values
+    )
 
-    precursor_df[
-        "mod_seq_hash"
-    ] = hash_vals
+    precursor_df["mod_seq_hash"] = hash_vals
     return precursor_df
 
-def hash_mod_seq_charge_df(
-    precursor_df:pd.DataFrame,
-    *, seed=0
-):
-    """ Internal function """
+
+def hash_mod_seq_charge_df(precursor_df: pd.DataFrame, *, seed=0):
+    """Internal function"""
     if "mod_seq_hash" not in precursor_df.columns:
         hash_mod_seq_df(precursor_df, seed=seed)
     if "charge" not in precursor_df.columns:
         return precursor_df
-    
-    precursor_df["mod_seq_charge_hash"] = (
-        precursor_df["mod_seq_hash"].values
-        + precursor_df["charge"].values.astype(np.uint64)
-    )
+
+    precursor_df["mod_seq_charge_hash"] = precursor_df[
+        "mod_seq_hash"
+    ].values + precursor_df["charge"].values.astype(np.uint64)
     return precursor_df
 
-def hash_precursor_df(
-    precursor_df:pd.DataFrame,
-    *, seed:int=0
-)->pd.DataFrame:
+
+def hash_precursor_df(precursor_df: pd.DataFrame, *, seed: int = 0) -> pd.DataFrame:
     """Add columns 'mod_seq_hash' and 'mod_seq_charge_hash'
-    into precursor_df (inplace). 
+    into precursor_df (inplace).
     The 64-bit hash function is from xxhash (xxhash.xxh64).
 
     Parameters
     ----------
     precursor_df : pd.DataFrame
-        
+
         precursor_df
-        
+
     Seed : int
-    
+
         Seed for xxhash.xxh64.
         Optional, by default 0
 
     Returns
     -------
     pd.DataFrame
 
         DataFrame with columns 'mod_seq_hash' and 'mod_seq_charge_hash'
     """
     hash_mod_seq_df(precursor_df, seed=seed)
 
-    if 'charge' in precursor_df.columns:
+    if "charge" in precursor_df.columns:
         hash_mod_seq_charge_df(precursor_df, seed=seed)
     return precursor_df
 
-def get_mod_seq_formula(seq:str, mods:str)->list:
-    """ 
-    'PEPTIDE','Acetyl@Any N-term' --> [('C',n), ('H',m), ...] 
+
+def get_mod_seq_formula(seq: str, mods: str) -> list:
+    """
+    'PEPTIDE','Acetyl@Any N-term' --> [('C',n), ('H',m), ...]
     """
     formula = {}
     for aa in seq:
-        for chem,n in AA_Composition[aa].items():
+        for chem, n in AA_Composition[aa].items():
             if chem in formula:
-                formula[chem]+=n
+                formula[chem] += n
             else:
-                formula[chem]=n
+                formula[chem] = n
     if len(mods) > 0:
-        for mod in mods.split(';'):
-            for chem,n in MOD_Composition[mod].items():
+        for mod in mods.split(";"):
+            for chem, n in MOD_Composition[mod].items():
                 if chem in formula:
-                    formula[chem]+=n
+                    formula[chem] += n
                 else:
-                    formula[chem]=n
+                    formula[chem] = n
     return list(formula.items())
 
+
 @numba.njit
 def get_right_most_isotope_offset(
-    intensities:np.ndarray, 
-    apex_idx:int,
-    min_right_most_intensity:float,
-)->int:
+    intensities: np.ndarray,
+    apex_idx: int,
+    min_right_most_intensity: float,
+) -> int:
     """Get right-most isotope index
 
     Parameters
     ----------
     intensities : np.ndarray
 
         Isotope intensities
@@ -326,88 +341,88 @@
     -------
     int
 
         Index or position of the right-most peak
     """
 
     apex_inten = intensities[apex_idx]
-    for i in range(len(intensities)-1,-1,-1):
-        if intensities[i] >= apex_inten*min_right_most_intensity:
+    for i in range(len(intensities) - 1, -1, -1):
+        if intensities[i] >= apex_inten * min_right_most_intensity:
             return i
     return apex_idx
 
+
 def get_mod_seq_isotope_distribution(
-    seq_mods:tuple, 
-    isotope_dist:IsotopeDistribution,
-    min_right_most_intensity:float=0.2,
-)->tuple:
+    seq_mods: tuple,
+    isotope_dist: IsotopeDistribution,
+    min_right_most_intensity: float = 0.2,
+) -> tuple:
     """Get isotope abundance distribution by IsotopeDistribution.
     This function is designed for multiprocessing.
 
     Parameters
     ----------
     seq_mods : tuple
         (sequence, mods)
-    
+
     isotope_dist : IsotopeDistribution
         See `IsotopeDistribution` in `alphabase.constants.isotope`
 
     min_right_most_intensity : float
-        The minimal intensity value of the right-most peak relative to apex peak. 
+        The minimal intensity value of the right-most peak relative to apex peak.
         Optional, by default 0.2
 
     Returns
     -------
     tuple
         float - Abundance of mono+1 / mono
         float - Abundance of apex / mono
         int - Apex isotope position relative to mono, i.e. apex index - mono index and 0 refers to the position of mono itself
         float - Abundance of right-most peak which has at least `min_right_most_intensity` intensity relative to the apex peak
         int - Right-most position relative to mono, i.e. right-most index - mono index
     """
-    dist, mono = isotope_dist.calc_formula_distribution(
-        get_mod_seq_formula(*seq_mods)
-    )
+    dist, mono = isotope_dist.calc_formula_distribution(get_mod_seq_formula(*seq_mods))
 
     apex_idx = np.argmax(dist)
 
     # find right-most peak
     right_most_idx = get_right_most_isotope_offset(
         dist, apex_idx, min_right_most_intensity
     )
 
     return (
-        dist[mono+1]/dist[mono], 
-        dist[apex_idx]/dist[mono], 
-        apex_idx-mono,
-        dist[right_most_idx]/dist[mono],
-        right_most_idx-mono,
+        dist[mono + 1] / dist[mono],
+        dist[apex_idx] / dist[mono],
+        apex_idx - mono,
+        dist[right_most_idx] / dist[mono],
+        right_most_idx - mono,
     )
 
+
 def calc_precursor_isotope_info(
-    precursor_df:pd.DataFrame,
-    min_right_most_intensity:float=0.2,
+    precursor_df: pd.DataFrame,
+    min_right_most_intensity: float = 0.2,
 ):
     """Calculate isotope mz values and relative (to M0) intensity values for precursor_df inplace.
 
     Parameters
     ----------
     precursor_df : pd.DataFrame
         precursor_df to calculate
 
     min_right_most_intensity : float
-        The minimal intensity value of the right-most peak relative to apex peak. 
+        The minimal intensity value of the right-most peak relative to apex peak.
         Optional, by default 0.2
 
     Returns
     -------
     pd.DataFrame
         precursor_df with additional columns:
 
-        - isotope_m1_intensity: relative intensity of M1 to mono peak 
+        - isotope_m1_intensity: relative intensity of M1 to mono peak
         - isotope_m1_mz: mz of M1
         - isotope_apex_intensity: relative intensity of the apex peak
         - isotope_apex_mz: mz of the apex peak
         - isotope_apex_offset: position offset of the apex peak to mono peak
         - isotope_right_most_intensity: relative intensity of the right-most peak
         - isotope_right_most_mz: mz of the right-most peak
         - isotope_right_most_offset: position offset of the right-most peak
@@ -415,149 +430,142 @@
 
     if "precursor_mz" not in precursor_df.columns:
         update_precursor_mz(precursor_df)
 
     isotope_dist = IsotopeDistribution()
 
     (
-        precursor_df['isotope_m1_intensity'], 
-        precursor_df['isotope_apex_intensity'],
-        precursor_df['isotope_apex_offset'],
-        precursor_df['isotope_right_most_intensity'],
-        precursor_df['isotope_right_most_offset'],
+        precursor_df["isotope_m1_intensity"],
+        precursor_df["isotope_apex_intensity"],
+        precursor_df["isotope_apex_offset"],
+        precursor_df["isotope_right_most_intensity"],
+        precursor_df["isotope_right_most_offset"],
     ) = zip(
-        *precursor_df[['sequence','mods']].apply(
-            get_mod_seq_isotope_distribution, 
-            axis=1, isotope_dist=isotope_dist,
+        *precursor_df[["sequence", "mods"]].apply(
+            get_mod_seq_isotope_distribution,
+            axis=1,
+            isotope_dist=isotope_dist,
             min_right_most_intensity=min_right_most_intensity,
         )
     )
-    precursor_df['isotope_m1_intensity'] = precursor_df[
-        'isotope_m1_intensity'
-    ].astype(np.float32)
-    precursor_df['isotope_apex_intensity'] = precursor_df[
-        'isotope_apex_intensity'
+    precursor_df["isotope_m1_intensity"] = precursor_df["isotope_m1_intensity"].astype(
+        np.float32
+    )
+    precursor_df["isotope_apex_intensity"] = precursor_df[
+        "isotope_apex_intensity"
     ].astype(np.float32)
-    precursor_df['isotope_apex_offset'] = precursor_df[
-        'isotope_apex_offset'
-    ].astype(np.int8)
-    precursor_df['isotope_right_most_intensity'] = precursor_df[
-        'isotope_right_most_intensity'
+    precursor_df["isotope_apex_offset"] = precursor_df["isotope_apex_offset"].astype(
+        np.int8
+    )
+    precursor_df["isotope_right_most_intensity"] = precursor_df[
+        "isotope_right_most_intensity"
     ].astype(np.float32)
-    precursor_df['isotope_right_most_offset'] = precursor_df[
-        'isotope_right_most_offset'
+    precursor_df["isotope_right_most_offset"] = precursor_df[
+        "isotope_right_most_offset"
     ].astype(np.int8)
 
-    precursor_df['isotope_m1_mz'] = (
-        precursor_df.precursor_mz + 
-        MASS_ISOTOPE/precursor_df.charge
+    precursor_df["isotope_m1_mz"] = (
+        precursor_df.precursor_mz + MASS_ISOTOPE / precursor_df.charge
     )
 
-    precursor_df['isotope_apex_mz'] = (
-        precursor_df.precursor_mz + 
-        (
-            MASS_ISOTOPE
-            *precursor_df.isotope_apex_offset
-            /precursor_df.charge
-        )
+    precursor_df["isotope_apex_mz"] = precursor_df.precursor_mz + (
+        MASS_ISOTOPE * precursor_df.isotope_apex_offset / precursor_df.charge
     )
-    precursor_df['isotope_right_most_mz'] = (
-        precursor_df.precursor_mz + 
-        (
-            MASS_ISOTOPE
-            *precursor_df.isotope_right_most_offset
-            /precursor_df.charge
-        )
+    precursor_df["isotope_right_most_mz"] = precursor_df.precursor_mz + (
+        MASS_ISOTOPE * precursor_df.isotope_right_most_offset / precursor_df.charge
     )
 
     return precursor_df
 
+
 def _batchify_df(df_group, mp_batch_size):
     """Internal funciton for multiprocessing"""
     for _, df in df_group:
         for i in range(0, len(df), mp_batch_size):
-            yield df.iloc[i:i+mp_batch_size,:]
+            yield df.iloc[i : i + mp_batch_size, :]
+
 
 def _count_batchify_df(df_group, mp_batch_size):
     """Internal funciton for multiprocessing"""
     count = 0
     for _, df in df_group:
         for _ in range(0, len(df), mp_batch_size):
             count += 1
     return count
 
+
 # `progress_bar` should be replaced by more advanced tqdm wrappers created by Sander
 # I will leave it to alphabase.utils
 def calc_precursor_isotope_info_mp(
-    precursor_df:pd.DataFrame, 
-    processes:int=8,
-    mp_batch_size:int=10000,
+    precursor_df: pd.DataFrame,
+    processes: int = 8,
+    mp_batch_size: int = 10000,
     progress_bar=None,
-    min_right_most_intensity:float=0.2,
-    min_precursor_num_to_run_mp:int=10000,
-)->pd.DataFrame:
-    """`calc_precursor_isotope` is not that fast for large dataframes, 
-    so here we use multiprocessing for faster isotope pattern calculation. 
+    min_right_most_intensity: float = 0.2,
+    min_precursor_num_to_run_mp: int = 10000,
+) -> pd.DataFrame:
+    """`calc_precursor_isotope` is not that fast for large dataframes,
+    so here we use multiprocessing for faster isotope pattern calculation.
     The speed is acceptable with multiprocessing (3.8 min for 21M precursors, 8 processes).
 
     Parameters
     ----------
     precursor_df : pd.DataFrame
         Precursor_df to calculate
-        
+
     processes : int
         Process number. Optional, by default 8
-    
+
     mp_batch_size : int
         Multiprocessing batch size. Optional, by default 100000.
-        
+
     progress_bar : Callable
-        The tqdm-based callback function 
+        The tqdm-based callback function
         to check multiprocessing. Defaults to None.
 
     min_right_most_intensity : float
-        The minimal intensity value of the right-most peak relative to apex peak. 
+        The minimal intensity value of the right-most peak relative to apex peak.
         Optional, by default 0.2
 
     Returns
     -------
     pd.DataFrame
-        DataFrame with `isotope_*` columns, 
+        DataFrame with `isotope_*` columns,
         see :meth:'calc_precursor_isotope()'.
     """
-    if len(precursor_df) < min_precursor_num_to_run_mp or processes<=1:
+    if len(precursor_df) < min_precursor_num_to_run_mp or processes <= 1:
         return calc_precursor_isotope_info(
             precursor_df=precursor_df,
             min_right_most_intensity=min_right_most_intensity,
         )
     df_list = []
-    df_group = precursor_df.groupby('nAA')
+    df_group = precursor_df.groupby("nAA")
     with mp.get_context("spawn").Pool(processes) as p:
         processing = p.imap(
             partial(
                 calc_precursor_isotope_info,
-                min_right_most_intensity=min_right_most_intensity
-            ), _batchify_df(df_group, mp_batch_size)
+                min_right_most_intensity=min_right_most_intensity,
+            ),
+            _batchify_df(df_group, mp_batch_size),
         )
         if progress_bar:
             processing = progress_bar(
-                processing, _count_batchify_df(
-                    df_group, mp_batch_size
-                )
+                processing, _count_batchify_df(df_group, mp_batch_size)
             )
         for df in processing:
             df_list.append(df)
     return pd.concat(df_list)
 
+
 def calc_precursor_isotope_intensity(
     precursor_df,
-    max_isotope = 6, 
-    min_right_most_intensity = 0.001,
-    normalize:typing.Literal['mono','sum'] = "sum",
-)->pd.DataFrame:
+    max_isotope=6,
+    min_right_most_intensity=0.001,
+    normalize: typing.Literal["mono", "sum"] = "sum",
+) -> pd.DataFrame:
     """Calculate isotope intensity values for precursor_df inplace.
 
     Parameters
     ----------
 
     precursor_df : pd.DataFrame
         Precursor_df to calculate isotope intensity
@@ -569,75 +577,74 @@
         The minimal intensity value of the right-most peak relative to apex peak.
 
     Returns
     -------
 
     pd.DataFrame
         precursor_df with additional columns:
-    
+
     """
 
     isotope_dist = IsotopeDistribution()
 
-    col_names = ['i_{}'.format(i) for i in range(max_isotope)]
+    col_names = ["i_{}".format(i) for i in range(max_isotope)]
 
     precursor_dist = np.zeros((len(precursor_df), max_isotope), dtype=np.float32)
 
-    mono_idxes = np.zeros(len(precursor_df),dtype=np.int32)
+    mono_idxes = np.zeros(len(precursor_df), dtype=np.int32)
 
     for i in range(len(precursor_df)):
-
         row = precursor_df.iloc[i]
         dist, mono = isotope_dist.calc_formula_distribution(
-            get_mod_seq_formula(row['sequence'], row['mods'])
+            get_mod_seq_formula(row["sequence"], row["mods"])
         )
-        dist[dist <= min_right_most_intensity] = 0.
+        dist[dist <= min_right_most_intensity] = 0.0
 
         # mono should be always included in the i_x list
         # after clipping max_isotope isotopes
-        mono_left_half_isotope = max_isotope//2
+        mono_left_half_isotope = max_isotope // 2
         mono_right_half_isotope = (
-            mono_left_half_isotope if max_isotope%2==0 
-            else (mono_left_half_isotope+1)
+            mono_left_half_isotope
+            if max_isotope % 2 == 0
+            else (mono_left_half_isotope + 1)
         )
         if mono < mono_left_half_isotope:
             precursor_dist[i] = dist[:max_isotope]
             mono_idxes[i] = mono
         elif mono + mono_right_half_isotope >= len(dist):
             precursor_dist[i] = dist[-max_isotope:]
-            mono_idxes[i] = max_isotope+mono-len(dist)+1
+            mono_idxes[i] = max_isotope + mono - len(dist) + 1
         else:
             precursor_dist[i] = dist[
-                mono-mono_left_half_isotope:
-                mono+mono_right_half_isotope
+                mono - mono_left_half_isotope : mono + mono_right_half_isotope
             ]
-            mono_idxes[i] = mono-mono_left_half_isotope
+            mono_idxes[i] = mono - mono_left_half_isotope
 
     if normalize == "sum":
         precursor_dist /= np.sum(precursor_dist, axis=1, keepdims=True)
     else:
         precursor_dist /= precursor_dist[
             np.arange(len(precursor_dist)), mono_idxes
-        ].reshape(-1,1)
+        ].reshape(-1, 1)
 
     precursor_df[col_names] = precursor_dist
     precursor_df["mono_isotope_idx"] = mono_idxes
 
     return precursor_df
 
+
 def calc_precursor_isotope_intensity_mp(
     precursor_df,
-    max_isotope = 6,
-    min_right_most_intensity = 0.001,
-    normalize:typing.Literal['mono','sum'] = "sum",
-    mp_batch_size = 1000,
-    mp_process_num = 8,
-    progress_bar = True,
-)->pd.DataFrame:
-
+    max_isotope=6,
+    min_right_most_intensity=0.001,
+    normalize: typing.Literal["mono", "sum"] = "sum",
+    mp_batch_size=1000,
+    mp_process_num=8,
+    progress_bar=True,
+) -> pd.DataFrame:
     """Calculate isotope intensity values for precursor_df using multiprocessing.
 
     Parameters
     ----------
 
     precursor_df : pd.DataFrame
         Precursor_df to calculate isotope intensity
@@ -658,40 +665,44 @@
         Whether to show progress bar. Optional, by default True
 
     Returns
     -------
 
     pd.DataFrame
         precursor_df with additional columns i_0, i_1, i_2, ... i_{max_isotope-1}
-    
+
     """
 
     if mp_process_num <= 1:
         return calc_precursor_isotope_intensity(
             precursor_df=precursor_df,
             max_isotope=max_isotope,
             min_right_most_intensity=min_right_most_intensity,
-            normalize=normalize
+            normalize=normalize,
         )
 
     df_list = []
-    df_group = precursor_df.groupby('nAA')
+    df_group = precursor_df.groupby("nAA")
 
     with mp.get_context("spawn").Pool(mp_process_num) as p:
         processing = p.imap(
             partial(
                 calc_precursor_isotope_intensity,
                 max_isotope=max_isotope,
                 min_right_most_intensity=min_right_most_intensity,
                 normalize=normalize,
-            ), _batchify_df(df_group, mp_batch_size)
+            ),
+            _batchify_df(df_group, mp_batch_size),
         )
 
         if progress_bar:
-            df_list = list(tqdm(processing, total=_count_batchify_df(df_group, mp_batch_size)))
+            df_list = list(
+                tqdm(processing, total=_count_batchify_df(df_group, mp_batch_size))
+            )
         else:
             df_list = list(processing)
 
     return pd.concat(df_list, ignore_index=True)
 
+
 calc_precursor_isotope = calc_precursor_isotope_intensity
-calc_precursor_isotope_mp = calc_precursor_isotope_intensity_mp
+calc_precursor_isotope_mp = calc_precursor_isotope_intensity_mp
```

### Comparing `alphabase-1.2.3/alphabase/protein/fasta.py` & `alphabase-1.2.4/alphabase/protein/fasta.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,33 +17,37 @@
 from alphabase.io.hdf import HDF_File
 from alphabase.utils import explode_multiple_columns
 
 from alphabase.constants._const import CONST_FILE_FOLDER
 
 from alphabase.spectral_library.base import SpecLibBase
 
-def get_uniprot_gene_name(description:str):
-    idx = description.find(' GN=')
-    if idx == -1: return ''
-    else: idx += 4
-    return description[idx:description.find(' ', idx)]
 
-def read_fasta_file(fasta_filename:str=""):
+def get_uniprot_gene_name(description: str):
+    idx = description.find(" GN=")
+    if idx == -1:
+        return ""
+    else:
+        idx += 4
+    return description[idx : description.find(" ", idx)]
+
+
+def read_fasta_file(fasta_filename: str = ""):
     """
     Read a FASTA file line by line
 
     Parameters
     ----------
     fasta_filename : str
         fasta.
-        
+
     Yields
     ------
-    dict 
-        protein information, 
+    dict
+        protein information,
         {protein_id:str, full_name:str, gene_name:str, description:str, sequence:str}
     """
     with open(fasta_filename, "rt") as handle:
         iterator = SeqIO.parse(handle, "fasta")
         while iterator:
             try:
                 record = next(iterator)
@@ -64,70 +68,68 @@
                     "sequence": sequence,
                 }
 
                 yield entry
             except StopIteration:
                 break
 
-def load_all_proteins(fasta_file_list:list):
+
+def load_all_proteins(fasta_file_list: list):
     protein_dict = {}
     for fasta in fasta_file_list:
         for protein in read_fasta_file(fasta):
-            protein_dict[protein['full_name']] = protein
+            protein_dict[protein["full_name"]] = protein
     return protein_dict
 
-def load_fasta_list_as_protein_df(fasta_list:list):
+
+def load_fasta_list_as_protein_df(fasta_list: list):
     protein_dict = load_all_proteins(fasta_list)
-    return pd.DataFrame().from_dict(
-        protein_dict, orient="index"
-    ).reset_index(drop=True)
+    return pd.DataFrame().from_dict(protein_dict, orient="index").reset_index(drop=True)
+
 
-def concat_proteins(protein_dict:dict, sep='$')->str:
-    """Concatenate all protein sequences into a single sequence, 
+def concat_proteins(protein_dict: dict, sep="$") -> str:
+    """Concatenate all protein sequences into a single sequence,
     seperated by `sep ($ by default)`.
 
     Parameters
     ----------
     protein_dict : dict
         protein_dict by read_fasta_file()
 
     Returns
     -------
     str
         concatenated sequence seperated by `sep`.
     """
-    seq_list = ['']
+    seq_list = [""]
     seq_count = 1
     for key in protein_dict:
-        protein_dict[key]['offset'] = seq_count
-        seq_list.append(protein_dict[key]['sequence'])
-        seq_count += protein_dict[key]['sequence']+1
-    seq_list.append('')
-    return '$'.join(seq_list)
-
-protease_dict = load_yaml(
-    os.path.join(
-        CONST_FILE_FOLDER, 
-        'protease.yaml'
-    )
-)
+        protein_dict[key]["offset"] = seq_count
+        seq_list.append(protein_dict[key]["sequence"])
+        seq_count += protein_dict[key]["sequence"] + 1
+    seq_list.append("")
+    return "$".join(seq_list)
+
+
+protease_dict = load_yaml(os.path.join(CONST_FILE_FOLDER, "protease.yaml"))
 """
 Pre-built protease dict with regular expression.
 """
 
+
 @numba.njit
 def cleave_sequence_with_cut_pos(
-    sequence:str,
-    cut_pos:np.ndarray,
-    n_missed_cleavages:int=2,
-    pep_length_min:int=6,
-    pep_length_max:int=45,
-)->tuple:
+    sequence: str,
+    cut_pos: np.ndarray,
+    n_missed_cleavages: int = 2,
+    pep_length_min: int = 6,
+    pep_length_max: int = 45,
+) -> tuple:
     """
-    Cleave a sequence with cut postions (cut_pos). 
+    Cleave a sequence with cut postions (cut_pos).
     Filters to have a minimum and maximum length.
 
     Parameters
     ----------
     sequence : str
         protein sequence
 
@@ -154,18 +156,16 @@
 
         List[bool]. If C-term pepetide
     """
     seq_list = []
     miss_list = []
     nterm_list = []
     cterm_list = []
-    for i,start_pos in enumerate(cut_pos):
-        for n_miss,end_pos in enumerate(
-            cut_pos[i+1:i+2+n_missed_cleavages]
-        ):
+    for i, start_pos in enumerate(cut_pos):
+        for n_miss, end_pos in enumerate(cut_pos[i + 1 : i + 2 + n_missed_cleavages]):
             if end_pos > start_pos + pep_length_max:
                 break
             elif end_pos < start_pos + pep_length_min:
                 continue
             else:
                 seq_list.append(sequence[start_pos:end_pos])
                 miss_list.append(n_miss)
@@ -175,20 +175,22 @@
                     nterm_list.append(False)
                 if end_pos == len(sequence):
                     cterm_list.append(True)
                 else:
                     cterm_list.append(False)
     return seq_list, miss_list, nterm_list, cterm_list
 
+
 class Digest(object):
-    def __init__(self,
-        protease:str='trypsin',
-        max_missed_cleavages:int=2,
-        peptide_length_min:int=6,
-        peptide_length_max:int=45,
+    def __init__(
+        self,
+        protease: str = "trypsin",
+        max_missed_cleavages: int = 2,
+        peptide_length_min: int = 6,
+        peptide_length_max: int = 45,
     ):
         """Digest a protein sequence
 
         Parameters
         ----------
         protease : str, optional
             protease name, could be pre-defined name defined in `protease_dict`
@@ -196,43 +198,37 @@
 
         max_missed_cleavages : int, optional
             Max number of misses cleavage sites.
             By default 2
 
         peptide_length_min : int, optional
             Minimal cleaved peptide length, by default 6
-            
+
         peptide_length_max : int, optional
             Maximal cleaved peptide length, by default 45
         """
 
         self.n_miss_cleave = max_missed_cleavages
         self.peptide_length_min = peptide_length_min
         self.peptide_length_max = peptide_length_max
         if protease.lower() in protease_dict:
-            self.regex_pattern = re.compile(
-                protease_dict[protease.lower()]
-            )
+            self.regex_pattern = re.compile(protease_dict[protease.lower()])
         else:
-            self.regex_pattern = re.compile(
-                protease
-            )
+            self.regex_pattern = re.compile(protease)
 
     def get_cut_positions(self, sequence):
         cut_pos = [0]
-        cut_pos.extend([
-            m.start()+1 for m in 
-            self.regex_pattern.finditer(sequence)
-        ])
+        cut_pos.extend([m.start() + 1 for m in self.regex_pattern.finditer(sequence)])
         cut_pos.append(len(sequence))
         return np.array(cut_pos, dtype=np.int64)
 
-    def cleave_sequence(self,
-        sequence:str,
-    )->tuple:
+    def cleave_sequence(
+        self,
+        sequence: str,
+    ) -> tuple:
         """
         Cleave a sequence.
 
         Parameters
         ----------
         sequence : str
             the given (protein) sequence.
@@ -244,56 +240,46 @@
             list[int]: miss cleavage list
             list[bool]: is protein N-term
             list[bool]: is protein C-term
         """
 
         cut_pos = self.get_cut_positions(sequence)
 
-        (
-            seq_list, miss_list, nterm_list, cterm_list
-        ) = cleave_sequence_with_cut_pos(
-            sequence, cut_pos, 
+        (seq_list, miss_list, nterm_list, cterm_list) = cleave_sequence_with_cut_pos(
+            sequence,
+            cut_pos,
             self.n_miss_cleave,
             self.peptide_length_min,
             self.peptide_length_max,
         )
         # Consider M loss at protein N-term
-        if sequence.startswith('M'):
-            for seq,miss,cterm in zip(
-                seq_list,miss_list,cterm_list
-            ):
-                if (
-                    sequence.startswith(seq) 
-                    and len(seq)>self.peptide_length_min
-                ):
+        if sequence.startswith("M"):
+            for seq, miss, cterm in zip(seq_list, miss_list, cterm_list):
+                if sequence.startswith(seq) and len(seq) > self.peptide_length_min:
                     seq_list.append(seq[1:])
                     miss_list.append(miss)
                     nterm_list.append(True)
                     cterm_list.append(cterm)
         return seq_list, miss_list, nterm_list, cterm_list
 
-def get_fix_mods(
-    sequence:str,
-    fix_mod_aas:str,
-    fix_mod_dict:dict
-)->tuple:
+
+def get_fix_mods(sequence: str, fix_mod_aas: str, fix_mod_dict: dict) -> tuple:
     """
     Generate fix modifications for the sequence
     """
     mods = []
     mod_sites = []
-    for i,aa in enumerate(sequence):
+    for i, aa in enumerate(sequence):
         if aa in fix_mod_aas:
-            mod_sites.append(i+1)
+            mod_sites.append(i + 1)
             mods.append(fix_mod_dict[aa])
-    return ';'.join(mods), ';'.join(str(i) for i in mod_sites)
+    return ";".join(mods), ";".join(str(i) for i in mod_sites)
 
-def get_candidate_sites(
-    sequence:str, target_mod_aas:str
-)->list:
+
+def get_candidate_sites(sequence: str, target_mod_aas: str) -> list:
     """get candidate modification sites
 
     Parameters
     ----------
     sequence : str
         peptide sequence
 
@@ -302,26 +288,27 @@
 
     Returns
     -------
     list
         candiadte mod sites in alphabase format (0: N-term, -1: C-term, 1-n:others)
     """
     candidate_sites = []
-    for i,aa in enumerate(sequence):
+    for i, aa in enumerate(sequence):
         if aa in target_mod_aas:
-            candidate_sites.append(i+1) #alphabase mod sites
+            candidate_sites.append(i + 1)  # alphabase mod sites
     return candidate_sites
 
+
 def get_var_mod_sites(
-    sequence:str,
-    target_mod_aas:str,
+    sequence: str,
+    target_mod_aas: str,
     min_var_mod: int,
     max_var_mod: int,
     max_combs: int,
-)->list:
+) -> list:
     """get all combinations of variable modification sites
 
     Parameters
     ----------
     sequence : str
         peptide sequence
 
@@ -336,363 +323,373 @@
 
     max_combs : int
         max number of combinations for a sequence
 
     Returns
     -------
     list
-        list of combinations (tuple) of modification sites 
+        list of combinations (tuple) of modification sites
     """
-    candidate_sites = get_candidate_sites(
-        sequence, target_mod_aas
-    )
+    candidate_sites = get_candidate_sites(sequence, target_mod_aas)
     if min_var_mod <= 1 and max_var_mod >= 1:
         mod_sites = [(s,) for s in candidate_sites]
     else:
         mod_sites = []
-    for n_var_mod in range(max(2,min_var_mod), max_var_mod+1):
-        if len(mod_sites)>=max_combs: break
+    for n_var_mod in range(max(2, min_var_mod), max_var_mod + 1):
+        if len(mod_sites) >= max_combs:
+            break
         mod_sites.extend(
             itertools.islice(
-                itertools.combinations(
-                    candidate_sites, n_var_mod
-                ),
-                max_combs-len(mod_sites)
+                itertools.combinations(candidate_sites, n_var_mod),
+                max_combs - len(mod_sites),
             )
         )
     return mod_sites
 
+
 def get_var_mods_per_sites_multi_mods_on_aa(
-    sequence:str,
-    mod_sites:tuple,
-    var_mod_dict:dict
-)->list:
+    sequence: str, mod_sites: tuple, var_mod_dict: dict
+) -> list:
     """
-    Used only when the var mod list contains 
+    Used only when the var mod list contains
     more than one mods on the same AA, for example:
     Mod1@A, Mod2@A ...
     """
-    mods_str_list = ['']
-    for i,site in enumerate(mod_sites):
-        if len(var_mod_dict[sequence[site-1]]) == 1:
+    mods_str_list = [""]
+    for i, site in enumerate(mod_sites):
+        if len(var_mod_dict[sequence[site - 1]]) == 1:
             for i in range(len(mods_str_list)):
-                mods_str_list[i] += var_mod_dict[sequence[site-1]][0]+';'
+                mods_str_list[i] += var_mod_dict[sequence[site - 1]][0] + ";"
         else:
             _new_list = []
-            for mod in var_mod_dict[sequence[site-1]]:
+            for mod in var_mod_dict[sequence[site - 1]]:
                 _lst = copy.deepcopy(mods_str_list)
                 for i in range(len(_lst)):
-                    _lst[i] += mod+';'
+                    _lst[i] += mod + ";"
                 _new_list.extend(_lst)
             mods_str_list = _new_list
     return [mod[:-1] for mod in mods_str_list]
 
+
 def get_var_mods_per_sites_single_mod_on_aa(
-    sequence:str,
-    mod_sites:tuple,
-    var_mod_dict:dict
-)->list:
+    sequence: str, mod_sites: tuple, var_mod_dict: dict
+) -> list:
     """
-    Used when the var mod list contains 
+    Used when the var mod list contains
     only one mods on the each AA, for example:
     Mod1@A, Mod2@D ...
     """
-    mod_str = ''
+    mod_str = ""
     for site in mod_sites:
-            mod_str += var_mod_dict[sequence[site-1]]+';'
+        mod_str += var_mod_dict[sequence[site - 1]] + ";"
     return [mod_str[:-1]]
 
+
 get_var_mods_per_sites = get_var_mods_per_sites_single_mod_on_aa
 
+
 def get_var_mods(
-    sequence:str,
-    var_mod_aas:str,
-    mod_dict:dict,
-    min_var_mod:int,
-    max_var_mod:int,
-    max_combs:int,
-)->tuple:
+    sequence: str,
+    var_mod_aas: str,
+    mod_dict: dict,
+    min_var_mod: int,
+    max_var_mod: int,
+    max_combs: int,
+) -> tuple:
     """
     Generate all modification combinations and associated sites
     for the sequence.
     """
     mod_sites_list = get_var_mod_sites(
-        sequence, var_mod_aas, 
-        min_var_mod, max_var_mod, max_combs
+        sequence, var_mod_aas, min_var_mod, max_var_mod, max_combs
     )
     ret_mods = []
     ret_sites_list = []
     for mod_sites in mod_sites_list:
-        _mods = get_var_mods_per_sites(
-            sequence,mod_sites,mod_dict
-        )
-        mod_sites_str = ';'.join([str(i) for i in mod_sites])
+        _mods = get_var_mods_per_sites(sequence, mod_sites, mod_dict)
+        mod_sites_str = ";".join([str(i) for i in mod_sites])
         ret_mods.extend(_mods)
-        ret_sites_list.extend([mod_sites_str]*len(_mods))
+        ret_sites_list.extend([mod_sites_str] * len(_mods))
     if min_var_mod == 0:
-        ret_mods.append('')
-        ret_sites_list.append('')
+        ret_mods.append("")
+        ret_sites_list.append("")
     return ret_mods, ret_sites_list
 
-def parse_term_mod(term_mod_name:str):
-    _mod, term = term_mod_name.split('@')
-    if '^' in term:
-        return tuple(term.split('^'))
+
+def parse_term_mod(term_mod_name: str):
+    _mod, term = term_mod_name.split("@")
+    if "^" in term:
+        return tuple(term.split("^"))
     else:
-        return '', term
+        return "", term
+
 
 def add_single_peptide_labeling(
-    seq:str,
-    mods:str,
-    mod_sites:str, 
-    label_aas:str, 
-    label_mod_dict:dict, 
-    nterm_label_mod:str, 
-    cterm_label_mod:str
+    seq: str,
+    mods: str,
+    mod_sites: str,
+    label_aas: str,
+    label_mod_dict: dict,
+    nterm_label_mod: str,
+    cterm_label_mod: str,
 ):
     add_nterm_label = True if nterm_label_mod else False
     add_cterm_label = True if cterm_label_mod else False
     if mod_sites:
-        _sites = mod_sites.split(';')
-        if '0' in _sites: add_nterm_label = False
-        if '-1' in _sites: add_cterm_label = False
+        _sites = mod_sites.split(";")
+        if "0" in _sites:
+            add_nterm_label = False
+        if "-1" in _sites:
+            add_cterm_label = False
         mod_list = [mods]
         mod_site_list = [mod_sites]
     else:
         mod_list = []
         mod_site_list = []
     if add_nterm_label:
         mod_list.append(nterm_label_mod)
-        mod_site_list.append('0')
+        mod_site_list.append("0")
     if add_cterm_label:
         mod_list.append(cterm_label_mod)
-        mod_site_list.append('-1')
+        mod_site_list.append("-1")
     aa_labels, aa_label_sites = get_fix_mods(seq, label_aas, label_mod_dict)
     if aa_labels:
         mod_list.append(aa_labels)
         mod_site_list.append(aa_label_sites)
-    return ';'.join(mod_list), ';'.join(mod_site_list)
+    return ";".join(mod_list), ";".join(mod_site_list)
+
 
-def parse_labels(labels:list):
-    label_aas = ''
+def parse_labels(labels: list):
+    label_aas = ""
     label_mod_dict = {}
-    nterm_label_mod = ''
-    cterm_label_mod = ''
+    nterm_label_mod = ""
+    cterm_label_mod = ""
     for label in labels:
-        _, aa = label.split('@')
+        _, aa = label.split("@")
         if len(aa) == 1:
             label_aas += aa
             label_mod_dict[aa] = label
-        elif aa == 'Any N-term' or aa == "Any_N-term":
+        elif aa == "Any N-term" or aa == "Any_N-term":
             nterm_label_mod = label
-        elif aa == 'Any C-term' or aa == "Any_C-term":
+        elif aa == "Any C-term" or aa == "Any_C-term":
             cterm_label_mod = label
     return label_aas, label_mod_dict, nterm_label_mod, cterm_label_mod
-        
+
+
 def create_labeling_peptide_df(
-        peptide_df:pd.DataFrame, labels:list,
-        inplace:bool=False
-    ):
-    if len(peptide_df) == 0: return peptide_df
+    peptide_df: pd.DataFrame, labels: list, inplace: bool = False
+):
+    if len(peptide_df) == 0:
+        return peptide_df
 
     if inplace:
         df = peptide_df
     else:
         df = peptide_df.copy()
 
-    (
-        label_aas, label_mod_dict, 
-        nterm_label_mod, cterm_label_mod
-    ) = parse_labels(labels)
-
-    (
-        df['mods'],
-        df['mod_sites']
-    ) = zip(*df[
-        ['sequence','mods','mod_sites']
-    ].apply(lambda x:
-        add_single_peptide_labeling(
-            *x, label_aas, label_mod_dict, 
-            nterm_label_mod, cterm_label_mod
-        ), axis=1,
-    ))
+    (label_aas, label_mod_dict, nterm_label_mod, cterm_label_mod) = parse_labels(labels)
+
+    (df["mods"], df["mod_sites"]) = zip(
+        *df[["sequence", "mods", "mod_sites"]].apply(
+            lambda x: add_single_peptide_labeling(
+                *x, label_aas, label_mod_dict, nterm_label_mod, cterm_label_mod
+            ),
+            axis=1,
+        )
+    )
 
     return df
 
-def protein_idxes_to_names(protein_idxes:str, protein_names:list):
-    if len(protein_idxes) == 0: return ''
-    proteins = [protein_names[int(i)] for i in protein_idxes.split(';')]
+
+def protein_idxes_to_names(protein_idxes: str, protein_names: list):
+    if len(protein_idxes) == 0:
+        return ""
+    proteins = [protein_names[int(i)] for i in protein_idxes.split(";")]
     proteins = [protein for protein in proteins if protein]
-    return ';'.join(proteins)
+    return ";".join(proteins)
+
 
 def append_special_modifications(
-    df:pd.DataFrame, 
-    var_mods:list = ['Phospho@S','Phospho@T','Phospho@Y'], 
-    min_mod_num:int=0, max_mod_num:int=1, 
-    max_peptidoform_num:int=100,
-    cannot_modify_pep_nterm_aa:bool=False,
-    cannot_modify_pep_cterm_aa:bool=False,
-)->pd.DataFrame:
+    df: pd.DataFrame,
+    var_mods: list = ["Phospho@S", "Phospho@T", "Phospho@Y"],
+    min_mod_num: int = 0,
+    max_mod_num: int = 1,
+    max_peptidoform_num: int = 100,
+    cannot_modify_pep_nterm_aa: bool = False,
+    cannot_modify_pep_cterm_aa: bool = False,
+) -> pd.DataFrame:
     """
-    Append special (not N/C-term) variable modifications to the 
+    Append special (not N/C-term) variable modifications to the
     exsiting modifications of each sequence in `df`.
 
     Parameters
     ----------
     df : pd.DataFrame
         Precursor dataframe
-    
+
     var_mods : list, optional
-        Considered varialbe modification list. 
+        Considered varialbe modification list.
         Defaults to ['Phospho@S','Phospho@T','Phospho@Y'].
 
     min_mod_num : int, optional
-        Minimal modification number for 
+        Minimal modification number for
         each sequence of the `var_mods`. Defaults to 0.
 
     max_mod_num : int, optional
-        Maximal modification number for 
+        Maximal modification number for
         each sequence of the `var_mods`. Defaults to 1.
 
     max_peptidoform_num : int, optional
-        One sequence is only allowed to explode 
+        One sequence is only allowed to explode
         to `max_peptidoform_num` number of modified peptides. Defaults to 100.
 
     cannot_modify_pep_nterm_aa : bool, optional
         Similar to `cannot_modify_pep_cterm_aa`, by default False
 
     cannot_modify_pep_cterm_aa : bool, optional
         If the modified AA is at C-term, then the modification cannot modified it.
-        For example GlyGly@K, for a peptide `ACDKEFGK`, if GlyGly is at the C-term, 
+        For example GlyGly@K, for a peptide `ACDKEFGK`, if GlyGly is at the C-term,
         trypsin cannot cleave the C-term K, hence there will be no such a modified peptide ACDKEFGK(GlyGly).
         by default False
 
     Returns
     -------
     pd.DataFrame
         The precursor_df with new modification added.
     """
-    if len(var_mods) == 0 or len(df) == 0: 
+    if len(var_mods) == 0 or len(df) == 0:
         return df
 
     if cannot_modify_pep_nterm_aa:
-        df['sequence'] = df['sequence'].apply(
-            lambda seq: seq[0].lower()+seq[1:]
-        )
-    
+        df["sequence"] = df["sequence"].apply(lambda seq: seq[0].lower() + seq[1:])
+
     if cannot_modify_pep_cterm_aa:
-        df['sequence'] = df['sequence'].apply(
-            lambda seq: seq[:-1]+seq[-1].lower()
-        )
+        df["sequence"] = df["sequence"].apply(lambda seq: seq[:-1] + seq[-1].lower())
 
-    mod_dict = dict([(mod[-1],mod) for mod in var_mods])
-    var_mod_aas = ''.join(mod_dict.keys())
-    
-    (
-        df['mods_app'],
-        df['mod_sites_app']
-    ) = zip(*df.sequence.apply(get_var_mods,
-            var_mod_aas=var_mod_aas, mod_dict=mod_dict, 
-            min_var_mod=min_mod_num, max_var_mod=max_mod_num, 
+    global get_var_mods_per_sites
+    var_mod_aas = ""
+    mod_dict = {}
+    if _check_if_multi_mods_on_aa(var_mods):
+        for mod in var_mods:
+            if mod.find("@") + 2 == len(mod):
+                # if mod[-1] in self.fix_mod_dict: continue
+                if mod[-1] in mod_dict:
+                    mod_dict[mod[-1]].append(mod)
+                else:
+                    var_mod_aas += mod[-1]
+                    mod_dict[mod[-1]] = [mod]
+        get_var_mods_per_sites = get_var_mods_per_sites_multi_mods_on_aa
+    else:
+        for mod in var_mods:
+            if mod.find("@") + 2 == len(mod):
+                # if mod[-1] in self.fix_mod_dict: continue
+                var_mod_aas += mod[-1]
+                mod_dict[mod[-1]] = mod
+        get_var_mods_per_sites = get_var_mods_per_sites_single_mod_on_aa
+
+    (df["mods_app"], df["mod_sites_app"]) = zip(
+        *df.sequence.apply(
+            get_var_mods,
+            var_mod_aas=var_mod_aas,
+            mod_dict=mod_dict,
+            min_var_mod=min_mod_num,
+            max_var_mod=max_mod_num,
             max_combs=max_peptidoform_num,
         )
     )
 
     if cannot_modify_pep_nterm_aa:
-        df['sequence'] = df['sequence'].apply(
-            lambda seq: seq[0].upper()+seq[1:]
-        )
-    
+        df["sequence"] = df["sequence"].apply(lambda seq: seq[0].upper() + seq[1:])
+
     if cannot_modify_pep_cterm_aa:
-        df['sequence'] = df['sequence'].apply(
-            lambda seq: seq[:-1]+seq[-1].upper()
-        )
-    
-    if min_mod_num==0:
-        df = explode_multiple_columns(df, ['mods_app','mod_sites_app'])
-        df.fillna('', inplace=True)
+        df["sequence"] = df["sequence"].apply(lambda seq: seq[:-1] + seq[-1].upper())
+
+    if min_mod_num == 0:
+        df = explode_multiple_columns(df, ["mods_app", "mod_sites_app"])
+        df.fillna("", inplace=True)
     else:
-        df.drop(df[df.mods_app.apply(lambda x: len(x)==0)].index, inplace=True)
-        df = explode_multiple_columns(df, ['mods_app','mod_sites_app'])
-    df['mods'] = df[['mods','mods_app']].apply(
-        lambda x: ';'.join(i for i in x if i), axis=1
+        df.drop(df[df.mods_app.apply(lambda x: len(x) == 0)].index, inplace=True)
+        df = explode_multiple_columns(df, ["mods_app", "mod_sites_app"])
+    df["mods"] = df[["mods", "mods_app"]].apply(
+        lambda x: ";".join(i for i in x if i), axis=1
     )
-    df['mod_sites'] = df[['mod_sites','mod_sites_app']].apply(
-        lambda x: ';'.join(i for i in x if i), axis=1
+    df["mod_sites"] = df[["mod_sites", "mod_sites_app"]].apply(
+        lambda x: ";".join(i for i in x if i), axis=1
     )
-    df.drop(columns=['mods_app', 'mod_sites_app'], inplace=True)
+    df.drop(columns=["mods_app", "mod_sites_app"], inplace=True)
     df.reset_index(drop=True, inplace=True)
     return df
 
+
 class SpecLibFasta(SpecLibBase):
     """
     This is the main entry of AlphaBase when generating spectral libraries from fasta files
     It includes functionalities to:
-    
+
     - Load protein sequences
     - Digest protein sequences
     - Append decoy peptides
     - Add fixed, variable or labeling modifications to the peptide sequences
     - Add charge states
     - Save libraries into hdf file
 
     Attributes
     ----------
     max_peptidoform_num : int, 100 by default
-        For some modifications such as Phospho, there may be 
-        thousands of peptidoforms generated for some peptides, 
-        so we use this attribute to control the overall number of 
+        For some modifications such as Phospho, there may be
+        thousands of peptidoforms generated for some peptides,
+        so we use this attribute to control the overall number of
         peptidoforms of a peptide.
-    
+
     protein_df : pd.DataFrame
-        Protein dataframe with columns 'protein_id', 
+        Protein dataframe with columns 'protein_id',
         'sequence', 'description', 'gene_name', etc.
     """
-    def __init__(self,
-        charged_frag_types:list = [
-            'b_z1','b_z2','y_z1', 'y_z2'
-        ],
+
+    def __init__(
+        self,
+        charged_frag_types: list = ["b_z1", "b_z2", "y_z1", "y_z2"],
         *,
-        protease:str = 'trypsin',
-        max_missed_cleavages:int = 2,
-        peptide_length_min:int = 7,
-        peptide_length_max:int = 35,
-        precursor_charge_min:int = 2,
-        precursor_charge_max:int = 4,
-        precursor_mz_min:float = 400.0, 
-        precursor_mz_max:float = 2000.0,
-        var_mods:list = ['Acetyl@Protein_N-term','Oxidation@M'],
-        min_var_mod_num:int = 0,
-        max_var_mod_num:int = 2,
-        fix_mods:list = ['Carbamidomethyl@C'],
-        labeling_channels:dict = None,
-        special_mods:list = [],
-        min_special_mod_num:int = 0,
-        max_special_mod_num:int = 1,
-        special_mods_cannot_modify_pep_n_term:bool=False,
-        special_mods_cannot_modify_pep_c_term:bool=False,
+        protease: str = "trypsin",
+        max_missed_cleavages: int = 2,
+        peptide_length_min: int = 7,
+        peptide_length_max: int = 35,
+        precursor_charge_min: int = 2,
+        precursor_charge_max: int = 4,
+        precursor_mz_min: float = 400.0,
+        precursor_mz_max: float = 2000.0,
+        var_mods: list = ["Acetyl@Protein_N-term", "Oxidation@M"],
+        min_var_mod_num: int = 0,
+        max_var_mod_num: int = 2,
+        fix_mods: list = ["Carbamidomethyl@C"],
+        labeling_channels: dict = None,
+        special_mods: list = [],
+        min_special_mod_num: int = 0,
+        max_special_mod_num: int = 1,
+        special_mods_cannot_modify_pep_n_term: bool = False,
+        special_mods_cannot_modify_pep_c_term: bool = False,
         decoy: str = None,
-        include_contaminants:bool=False,
-        I_to_L:bool=False,
+        include_contaminants: bool = False,
+        I_to_L: bool = False,
     ):
         """
         Parameters
         ----------
         charged_frag_types : list, optional
-            Fragment types with charge, 
+            Fragment types with charge,
             by default [ 'b_z1','b_z2','y_z1', 'y_z2' ]
 
         protease : str, optional
             Could be pre-defined protease name defined in :data:`protease_dict`,
-            or a regular expression. 
+            or a regular expression.
             By default 'trypsin'
 
         max_missed_cleavages : int, optional
             Maximal missed cleavages, by default 2
-            
+
         peptide_length_min : int, optional
             Minimal cleaved peptide length, by default 7
 
         peptide_length_max : int, optional
             Maximal cleaved peptide length, by default 35
 
         precursor_charge_min : int, optional
@@ -704,51 +701,51 @@
         precursor_mz_min : float, optional
             Minimal precursor mz, by default 200.0
 
         precursor_mz_max : float, optional
             Maximal precursor mz, by default 2000.0
 
         var_mods : list, optional
-            list of variable modifications, 
+            list of variable modifications,
             by default ['Acetyl@Protein_N-term','Oxidation@M']
 
         max_var_mod_num : int, optional
-            Minimal number of variable modifications on a peptide sequence, 
+            Minimal number of variable modifications on a peptide sequence,
             by default 0
 
         max_var_mod_num : int, optional
-            Maximal number of variable modifications on a peptide sequence, 
+            Maximal number of variable modifications on a peptide sequence,
             by default 2
 
         fix_mods : list, optional
             list of fixed modifications, by default ['Carbamidomethyl@C']
 
         labeling_channels : dict, optional
-            Add isotope labeling with different channels, 
-            see :meth:`add_peptide_labeling()`. 
+            Add isotope labeling with different channels,
+            see :meth:`add_peptide_labeling()`.
             Defaults to None
 
         special_mods : list, optional
             Modifications with special occurance per peptide.
-            It is useful for modificaitons like Phospho which may largely 
+            It is useful for modificaitons like Phospho which may largely
             explode the number of candidate modified peptides.
-            The number of special_mods per peptide 
+            The number of special_mods per peptide
             is controlled by `max_append_mod_num`.
             Defaults to [].
 
         min_special_mod_num : int, optional
             Control the min number of special_mods per peptide, by default 0.
 
         max_special_mod_num : int, optional
             Control the max number of special_mods per peptide, by default 1.
 
         special_mods_cannot_modify_pep_c_term : bool, optional
-            Some modifications cannot modify the peptide C-term, 
-            this will be useful for GlyGly@K as if C-term is di-Glyed, 
-            it cannot be cleaved/digested. 
+            Some modifications cannot modify the peptide C-term,
+            this will be useful for GlyGly@K as if C-term is di-Glyed,
+            it cannot be cleaved/digested.
             Defaults to False.
 
         special_mods_cannot_modify_pep_n_term : bool, optional
             Similar to `special_mods_cannot_modify_pep_c_term`, but at N-term.
             Defaults to False.
 
         decoy : str, optional
@@ -764,164 +761,148 @@
         include_contaminants : bool, optional
             If include contaminants.fasta, by default False
         """
         super().__init__(
             charged_frag_types=charged_frag_types,
             precursor_mz_min=precursor_mz_min,
             precursor_mz_max=precursor_mz_max,
-            decoy=decoy
+            decoy=decoy,
         )
-        self.protein_df:pd.DataFrame = pd.DataFrame()
+        self.protein_df: pd.DataFrame = pd.DataFrame()
         self.I_to_L = I_to_L
         self.include_contaminants = include_contaminants
         self.max_peptidoform_num = 100
         self._digest = Digest(
-            protease, max_missed_cleavages,
-            peptide_length_min, peptide_length_max
+            protease, max_missed_cleavages, peptide_length_min, peptide_length_max
         )
         self.min_precursor_charge = precursor_charge_min
         self.max_precursor_charge = precursor_charge_max
 
         self.var_mods = var_mods
         self.fix_mods = fix_mods
         self.min_var_mod_num = min_var_mod_num
         self.max_var_mod_num = max_var_mod_num
         self.labeling_channels = labeling_channels
         self.special_mods = special_mods
         self.min_special_mod_num = min_special_mod_num
         self.max_special_mod_num = max_special_mod_num
-        self.special_mods_cannot_modify_pep_n_term = special_mods_cannot_modify_pep_n_term
-        self.special_mods_cannot_modify_pep_c_term = special_mods_cannot_modify_pep_c_term
+        self.special_mods_cannot_modify_pep_n_term = (
+            special_mods_cannot_modify_pep_n_term
+        )
+        self.special_mods_cannot_modify_pep_c_term = (
+            special_mods_cannot_modify_pep_c_term
+        )
 
         self._parse_fix_and_var_mods()
-    
+
     def _parse_fix_and_var_mods(self):
         # self.fix_mod_aas = ''
         # self.fix_mod_prot_nterm_dict = {}
         # self.fix_mod_prot_cterm_dict = {}
         # self.fix_mod_pep_nterm_dict = {}
         # self.fix_mod_pep_cterm_dict = {}
         # self.fix_mod_dict = {}
 
-        def _set_term_mod(term_mod,
-            prot_nterm, prot_cterm, pep_nterm, pep_cterm,
-            allow_conflicts
+        def _set_term_mod(
+            term_mod, prot_nterm, prot_cterm, pep_nterm, pep_cterm, allow_conflicts
         ):
-            def _set_dict(term_dict,site,mod,
-                allow_conflicts
-            ):
+            def _set_dict(term_dict, site, mod, allow_conflicts):
                 if allow_conflicts:
                     if site in term_dict:
                         term_dict[site].append(term_mod)
                     else:
                         term_dict[site] = [term_mod]
                 else:
                     term_dict[site] = term_mod
+
             site, term = parse_term_mod(term_mod)
             if term == "Any N-term" or term == "Any_N-term":
-                _set_dict(pep_nterm, site, term_mod, 
-                    allow_conflicts
-                )
-            elif term == 'Protein N-term' or term == "Protein_N-term":
-                _set_dict(prot_nterm, site, term_mod, 
-                    allow_conflicts
-                )
-            elif term == 'Any C-term' or term == "Any_C-term":
-                _set_dict(pep_cterm, site, term_mod, 
-                    allow_conflicts
-                )
-            elif term == 'Protein C-term' or term == "Protein_C-term":
-                _set_dict(prot_cterm, site, term_mod, 
-                    allow_conflicts
-                )
-        
+                _set_dict(pep_nterm, site, term_mod, allow_conflicts)
+            elif term == "Protein N-term" or term == "Protein_N-term":
+                _set_dict(prot_nterm, site, term_mod, allow_conflicts)
+            elif term == "Any C-term" or term == "Any_C-term":
+                _set_dict(pep_cterm, site, term_mod, allow_conflicts)
+            elif term == "Protein C-term" or term == "Protein_C-term":
+                _set_dict(prot_cterm, site, term_mod, allow_conflicts)
+
         # for mod in self.fix_mods:
         #     if mod.find('@')+2 == len(mod):
         #         self.fix_mod_aas += mod[-1]
         #         self.fix_mod_dict[mod[-1]] = mod
         #     else:
         #         _set_term_mod(
-        #             mod, 
+        #             mod,
         #             self.fix_mod_prot_nterm_dict,
         #             self.fix_mod_prot_cterm_dict,
         #             self.fix_mod_pep_nterm_dict,
         #             self.fix_mod_pep_cterm_dict,
         #             allow_conflicts=False
         #         )
 
-        self.var_mod_aas = ''
+        self.var_mod_aas = ""
         self.var_mod_prot_nterm_dict = {}
         self.var_mod_prot_cterm_dict = {}
         self.var_mod_pep_nterm_dict = {}
         self.var_mod_pep_cterm_dict = {}
         self.var_mod_dict = {}
 
         global get_var_mods_per_sites
-        if self._check_if_multi_mods_on_aa(self.var_mods):
+        if _check_if_multi_mods_on_aa(self.var_mods):
             for mod in self.var_mods:
-                if mod.find('@')+2 == len(mod):
+                if mod.find("@") + 2 == len(mod):
                     # if mod[-1] in self.fix_mod_dict: continue
-                    self.var_mod_aas += mod[-1]
                     if mod[-1] in self.var_mod_dict:
                         self.var_mod_dict[mod[-1]].append(mod)
                     else:
+                        self.var_mod_aas += mod[-1]
                         self.var_mod_dict[mod[-1]] = [mod]
             get_var_mods_per_sites = get_var_mods_per_sites_multi_mods_on_aa
         else:
             for mod in self.var_mods:
-                if mod.find('@')+2 == len(mod):
+                if mod.find("@") + 2 == len(mod):
                     # if mod[-1] in self.fix_mod_dict: continue
                     self.var_mod_aas += mod[-1]
                     self.var_mod_dict[mod[-1]] = mod
             get_var_mods_per_sites = get_var_mods_per_sites_single_mod_on_aa
-        
+
         for mod in self.var_mods:
-            if mod.find('@')+2 < len(mod):
+            if mod.find("@") + 2 < len(mod):
                 _set_term_mod(
-                    mod, 
+                    mod,
                     self.var_mod_prot_nterm_dict,
                     self.var_mod_prot_cterm_dict,
                     self.var_mod_pep_nterm_dict,
                     self.var_mod_pep_cterm_dict,
-                    allow_conflicts=True
+                    allow_conflicts=True,
                 )
 
-    def _check_if_multi_mods_on_aa(self, var_mods):
-        mod_set = set()
-        for mod in var_mods:
-            if mod.find('@')+2 == len(mod):
-                if mod[-1] in mod_set: return True
-                mod_set.add(mod[-1])
-        return False
-
-    def import_and_process_fasta(self, 
-        fasta_files:list,
+    def import_and_process_fasta(
+        self,
+        fasta_files: list,
     ):
         """
         Import and process a fasta file or a list of fasta files.
         It includes 3 steps:
 
         1. Digest and get peptide sequences, it uses `self.get_peptides_from_...()`
-        2. Process the peptides including add modifications, 
+        2. Process the peptides including add modifications,
         it uses :meth:`process_from_naked_peptide_seqs()`.
 
         Parameters
         ----------
         fasta_files : list
             A fasta file or a list of fasta files
         """
         if self.include_contaminants:
-            fasta_files.append(os.path.join(
-                CONST_FILE_FOLDER, 'contaminants.fasta'
-            ))
+            fasta_files.append(os.path.join(CONST_FILE_FOLDER, "contaminants.fasta"))
         protein_dict = load_all_proteins(fasta_files)
         self.import_and_process_protein_dict(protein_dict)
 
-    def import_and_process_protein_dict(self, protein_dict:dict):
-        """ 
+    def import_and_process_protein_dict(self, protein_dict: dict):
+        """
         Import and process the protein_dict.
         The processing step is in :meth:`process_from_naked_peptide_seqs()`.
         ```
         protein_dict = load_all_proteins(fasta_files)
         ```
 
         Parameters
@@ -933,206 +914,198 @@
             'prot_id2': {...}
             ...
             }
         """
         self.get_peptides_from_protein_dict(protein_dict)
         self.process_from_naked_peptide_seqs()
 
-    def import_and_process_protein_df(self, protein_df:pd.DataFrame):
-        """ 
+    def import_and_process_protein_df(self, protein_df: pd.DataFrame):
+        """
         Import and process the protein_dict.
         The processing step is in :meth:`process_from_naked_peptide_seqs()`.
         ```
         protein_dict = load_all_proteins(fasta_files)
         ```
 
         Parameters
         ----------
         protein_df : pd.DataFrame
             DataFrame with columns 'protein_id', 'sequence', 'gene_name', 'description'
         """
         self.get_peptides_from_protein_df(protein_df)
         self.process_from_naked_peptide_seqs()
 
-    def import_and_process_peptide_sequences(self, 
-        pep_seq_list:list, protein_list:list=None,
+    def import_and_process_peptide_sequences(
+        self,
+        pep_seq_list: list,
+        protein_list: list = None,
     ):
-        """ 
+        """
         Importing and process peptide sequences instead of proteins.
         The processing step is in :meth:`process_from_naked_peptide_seqs()`.
 
         Parameters
         ----------
         pep_seq_list : list
             Peptide sequence list
 
         protein_list : list, optional
-            Protein id list which maps to pep_seq_list one-by-one, 
+            Protein id list which maps to pep_seq_list one-by-one,
             by default None
         """
-        self.get_peptides_from_peptide_sequence_list(
-            pep_seq_list, protein_list
-        )
+        self.get_peptides_from_peptide_sequence_list(pep_seq_list, protein_list)
         self.process_from_naked_peptide_seqs()
 
     def process_from_naked_peptide_seqs(self):
         """
-        The peptide processing step which is 
+        The peptide processing step which is
         called by `import_and_process_...` methods.
         """
         self.append_decoy_sequence()
         self.add_modifications()
         self.add_special_modifications()
         self.add_peptide_labeling()
         self.add_charge()
         self.calc_and_clip_precursor_mz()
 
-    def get_peptides_from_fasta(self, fasta_file:Union[str,list]):
+    def get_peptides_from_fasta(self, fasta_file: Union[str, list]):
         """Load peptide sequences from fasta files.
 
         Parameters
         ----------
         fasta_file : Union[str,list]
             Could be a fasta file (str) or a list of fasta files (list[str])
         """
         if isinstance(fasta_file, str):
             self.get_peptides_from_fasta_list([fasta_file])
         else:
             self.get_peptides_from_fasta_list(fasta_file)
 
-    def get_peptides_from_fasta_list(self, fasta_files:list):
+    def get_peptides_from_fasta_list(self, fasta_files: list):
         """Load peptide sequences from fasta file list
 
         Parameters
         ----------
         fasta_files : list
             fasta file list
         """
         if self.include_contaminants:
-            fasta_files.append(os.path.join(
-                CONST_FILE_FOLDER, 'contaminants.fasta'
-            ))
+            fasta_files.append(os.path.join(CONST_FILE_FOLDER, "contaminants.fasta"))
         protein_dict = load_all_proteins(fasta_files)
         self.get_peptides_from_protein_dict(protein_dict)
 
-    def get_peptides_from_protein_df(self, protein_df:pd.DataFrame):
+    def get_peptides_from_protein_df(self, protein_df: pd.DataFrame):
         self.protein_df = protein_df
         if self.I_to_L:
-            self.protein_df[
-                'sequence_I2L'
-            ] = self.protein_df.sequence.str.replace('I','L')
-            digest_seq = 'sequence_I2L'
+            self.protein_df["sequence_I2L"] = self.protein_df.sequence.str.replace(
+                "I", "L"
+            )
+            digest_seq = "sequence_I2L"
         else:
-            digest_seq = 'sequence'
-        self._cleave_to_peptides(
-            self.protein_df,
-            protein_seq_column=digest_seq
-        )
+            digest_seq = "sequence"
+        self._cleave_to_peptides(self.protein_df, protein_seq_column=digest_seq)
 
-    def get_peptides_from_protein_dict(self, protein_dict:dict):
+    def get_peptides_from_protein_dict(self, protein_dict: dict):
         """Cleave the protein sequences in protein_dict.
 
         Parameters
         ----------
         protein_dict : dict
             Format:
             ```
             {
             'prot_id1': {'protein_id': 'prot_id1', 'sequence': string, 'gene_name': string, 'description': string
             'prot_id2': {...}
             ...
             }
             ```
         """
-        protein_df = pd.DataFrame.from_dict(
-            protein_dict, orient='index'
-        ).reset_index(drop=True)
+        protein_df = pd.DataFrame.from_dict(protein_dict, orient="index").reset_index(
+            drop=True
+        )
         self.get_peptides_from_protein_df(protein_df)
 
-    def _cleave_to_peptides(self, 
-        protein_df:pd.DataFrame,
-        protein_seq_column:str='sequence'
+    def _cleave_to_peptides(
+        self, protein_df: pd.DataFrame, protein_seq_column: str = "sequence"
     ):
         """Cleave protein sequences in protein_df
 
         Parameters
         ----------
         protein_df : pd.DataFrame
             Protein DataFrame containing `protein_seq_column`
         protein_seq_column : str, optional
             Target column containing protein sequences, by default 'sequence'
         """
         pep_dict = {}
 
-        for i,prot_seq in enumerate(
-            protein_df[protein_seq_column].values
-        ):
-            (
+        for i, prot_seq in enumerate(protein_df[protein_seq_column].values):
+            (seq_list, miss_list, nterm_list, cterm_list) = (
+                self._digest.cleave_sequence(prot_seq)
+            )
+            for seq, miss, nterm, cterm in zip(
                 seq_list, miss_list, nterm_list, cterm_list
-            ) = self._digest.cleave_sequence(prot_seq)
-            for seq,miss,nterm,cterm in zip(
-                seq_list,miss_list,nterm_list, cterm_list
             ):
                 prot_id = str(i)
                 if seq in pep_dict:
                     if not pep_dict[seq][0].endswith(prot_id):
-                        pep_dict[seq][0] += ';'+prot_id
+                        pep_dict[seq][0] += ";" + prot_id
                     if nterm:
                         pep_dict[seq][2] = nterm
                     if cterm:
                         pep_dict[seq][3] = cterm
                 else:
-                    pep_dict[seq] = [prot_id,miss,nterm,cterm]
+                    pep_dict[seq] = [prot_id, miss, nterm, cterm]
         self._precursor_df = pd.DataFrame().from_dict(
-            pep_dict, orient='index', columns = [
-                'protein_idxes','miss_cleavage',
-                'is_prot_nterm','is_prot_cterm'
-            ]
+            pep_dict,
+            orient="index",
+            columns=[
+                "protein_idxes",
+                "miss_cleavage",
+                "is_prot_nterm",
+                "is_prot_cterm",
+            ],
         )
         self._precursor_df.reset_index(drop=False, inplace=True)
-        self._precursor_df.rename(
-            columns={'index':'sequence'}, inplace=True
-        )
-        self._precursor_df['mods'] = ''
-        self._precursor_df['mod_sites'] = ''
+        self._precursor_df.rename(columns={"index": "sequence"}, inplace=True)
+        self._precursor_df["mods"] = ""
+        self._precursor_df["mod_sites"] = ""
         self.refine_df()
 
     def append_protein_name(self):
         if (
-            'protein_id' not in self.protein_df or 
-            'protein_idxes' not in self._precursor_df
-        ): 
+            "protein_id" not in self.protein_df
+            or "protein_idxes" not in self._precursor_df
+        ):
             return
 
-        self._precursor_df['proteins'] = self._precursor_df['protein_idxes'].apply(
-            protein_idxes_to_names,
-            protein_names=self.protein_df['protein_id'].values
+        self._precursor_df["proteins"] = self._precursor_df["protein_idxes"].apply(
+            protein_idxes_to_names, protein_names=self.protein_df["protein_id"].values
         )
 
-        if 'gene_name' in self.protein_df.columns:
-            self._precursor_df['genes'] = self._precursor_df['protein_idxes'].apply(
+        if "gene_name" in self.protein_df.columns:
+            self._precursor_df["genes"] = self._precursor_df["protein_idxes"].apply(
                 protein_idxes_to_names,
-                protein_names=self.protein_df['gene_name'].values
+                protein_names=self.protein_df["gene_name"].values,
             )
 
-    def get_peptides_from_peptide_sequence_list(self, 
-        pep_seq_list:list,
-        protein_list:list = None
+    def get_peptides_from_peptide_sequence_list(
+        self, pep_seq_list: list, protein_list: list = None
     ):
         self._precursor_df = pd.DataFrame()
-        self._precursor_df['sequence'] = pep_seq_list
+        self._precursor_df["sequence"] = pep_seq_list
         if protein_list is not None:
-            self._precursor_df['protein_name'] = protein_list
-        self._precursor_df['is_prot_nterm'] = False
-        self._precursor_df['is_prot_cterm'] = False
+            self._precursor_df["protein_name"] = protein_list
+        self._precursor_df["is_prot_nterm"] = False
+        self._precursor_df["is_prot_cterm"] = False
         self.refine_df()
 
-    def add_mods_for_one_seq(self, sequence:str, 
-        is_prot_nterm, is_prot_cterm
-    )->tuple:
+    def add_mods_for_one_seq(
+        self, sequence: str, is_prot_nterm, is_prot_cterm
+    ) -> tuple:
         """Add fixed and variable modifications to a sequence
 
         Parameters
         ----------
         sequence : str
             Peptide sequence
         is_prot_nterm : bool
@@ -1156,207 +1129,196 @@
         #     fix_mods = ['']
         #     fix_mod_sites = ['']
         # else:
         #     fix_mods = [fix_mods]
         #     fix_mod_sites = [fix_mod_sites]
 
         var_mods_list, var_mod_sites_list = get_var_mods(
-            sequence, self.var_mod_aas, self.var_mod_dict, 
-            self.min_var_mod_num, self.max_var_mod_num, 
-            self.max_peptidoform_num-1, # 1 for unmodified
+            sequence,
+            self.var_mod_aas,
+            self.var_mod_dict,
+            self.min_var_mod_num,
+            self.max_var_mod_num,
+            self.max_peptidoform_num - 1,  # 1 for unmodified
         )
 
-        nterm_var_mods = ['']
-        nterm_var_mod_sites = ['']
-        if is_prot_nterm and len(self.var_mod_prot_nterm_dict)>0:
-            if '' in self.var_mod_prot_nterm_dict:
-                nterm_var_mods.extend(self.var_mod_prot_nterm_dict[''])
+        nterm_var_mods = [""]
+        nterm_var_mod_sites = [""]
+        if is_prot_nterm and len(self.var_mod_prot_nterm_dict) > 0:
+            if "" in self.var_mod_prot_nterm_dict:
+                nterm_var_mods.extend(self.var_mod_prot_nterm_dict[""])
             if sequence[0] in self.var_mod_prot_nterm_dict:
                 nterm_var_mods.extend(self.var_mod_prot_nterm_dict[sequence[0]])
-        if len(self.var_mod_pep_nterm_dict)>0:
-            if '' in self.var_mod_pep_nterm_dict:
-                nterm_var_mods.extend(self.var_mod_pep_nterm_dict[''])
+        if len(self.var_mod_pep_nterm_dict) > 0:
+            if "" in self.var_mod_pep_nterm_dict:
+                nterm_var_mods.extend(self.var_mod_pep_nterm_dict[""])
             if sequence[0] in self.var_mod_pep_nterm_dict:
                 nterm_var_mods.extend(self.var_mod_pep_nterm_dict[sequence[0]])
-        nterm_var_mod_sites.extend(['0']*(len(nterm_var_mods)-1))
+        nterm_var_mod_sites.extend(["0"] * (len(nterm_var_mods) - 1))
 
-        #TODO add prot and pep C-term var mods
+        # TODO add prot and pep C-term var mods
 
         return (
             list(
-                ';'.join([i for i in items if i]) for items in itertools.product(
-                    nterm_var_mods, var_mods_list
-                )
+                ";".join([i for i in items if i])
+                for items in itertools.product(nterm_var_mods, var_mods_list)
             ),
             list(
-                ';'.join([i for i in items if i]) for items in itertools.product(
-                    nterm_var_mod_sites, var_mod_sites_list
-                )
+                ";".join([i for i in items if i])
+                for items in itertools.product(nterm_var_mod_sites, var_mod_sites_list)
             ),
         )
 
     def add_modifications(self):
-        """Add fixed and variable modifications to all peptide sequences in `self.precursor_df`
-        """
-        if 'is_prot_nterm' not in self._precursor_df.columns:
-            self._precursor_df['is_prot_nterm'] = False
-        if 'is_prot_cterm' not in self._precursor_df.columns:
-            self._precursor_df['is_prot_cterm'] = False
-        
+        """Add fixed and variable modifications to all peptide sequences in `self.precursor_df`"""
+        if "is_prot_nterm" not in self._precursor_df.columns:
+            self._precursor_df["is_prot_nterm"] = False
+        if "is_prot_cterm" not in self._precursor_df.columns:
+            self._precursor_df["is_prot_cterm"] = False
+
         if len(self._precursor_df) == 0:
-            self._precursor_df['mods'] = ""
-            self._precursor_df['mod_sites'] = ""
+            self._precursor_df["mods"] = ""
+            self._precursor_df["mod_sites"] = ""
             return
-            
-        (
-            self._precursor_df['mods'],
-            self._precursor_df['mod_sites']
-        ) = zip(*self._precursor_df[
-            ['sequence','is_prot_nterm','is_prot_cterm']
-        ].apply(lambda x:
-            self.add_mods_for_one_seq(*x), axis=1
-        ))
+
+        (self._precursor_df["mods"], self._precursor_df["mod_sites"]) = zip(
+            *self._precursor_df[["sequence", "is_prot_nterm", "is_prot_cterm"]].apply(
+                lambda x: self.add_mods_for_one_seq(*x), axis=1
+            )
+        )
         self._precursor_df = explode_multiple_columns(
-            self._precursor_df,
-            ['mods','mod_sites']
+            self._precursor_df, ["mods", "mod_sites"]
         )
-        self._precursor_df.dropna(subset=['mods'], inplace=True)
+        self._precursor_df.dropna(subset=["mods"], inplace=True)
         self._precursor_df = create_labeling_peptide_df(
-            self._precursor_df, self.fix_mods,
-            inplace=True
+            self._precursor_df, self.fix_mods, inplace=True
         )
         self._precursor_df.reset_index(drop=True, inplace=True)
 
     def add_special_modifications(self):
         """
-        Add external defined variable modifications to 
+        Add external defined variable modifications to
         all peptide sequences in `self._precursor_df`.
         See :meth:`append_special_modifications()` for details.
         """
-        if len(self.special_mods) == 0: return
+        if len(self.special_mods) == 0:
+            return
         self._precursor_df = append_special_modifications(
-            self._precursor_df, self.special_mods,
-            self.min_special_mod_num, self.max_special_mod_num, 
+            self._precursor_df,
+            self.special_mods,
+            self.min_special_mod_num,
+            self.max_special_mod_num,
             self.max_peptidoform_num,
             cannot_modify_pep_nterm_aa=self.special_mods_cannot_modify_pep_n_term,
             cannot_modify_pep_cterm_aa=self.special_mods_cannot_modify_pep_c_term,
         )
 
-    def add_peptide_labeling(self, labeling_channel_dict:dict=None):
-        """ 
+    def add_peptide_labeling(self, labeling_channel_dict: dict = None):
+        """
         Add labeling onto peptides inplace of self._precursor_df
 
         Parameters
         ----------
         labeling_channel_dict : dict, optional
             For example:
             ```
             {
             -1: [], # not labeled
             0: ['Dimethyl@Any_N-term','Dimethyl@K'],
             4: ['Dimethyl:2H(4)@Any_N-term','Dimethyl:2H(4)@K'],
             8: ['Dimethyl:2H(6)13C(2)@Any_N-term','Dimethyl:2H(6)13C(2)@K'],
             }
             ```.
-            The key name could be int (highly recommended or 
-            must be in the future) or str, and the value must be 
+            The key name could be int (highly recommended or
+            must be in the future) or str, and the value must be
             a list of modification names (str) in alphabase format.
             It is set to `self.labeling_channels` if None.
             Defaults to None
-    
+
         """
         if labeling_channel_dict is None:
             labeling_channel_dict = self.labeling_channels
         if labeling_channel_dict is None or len(labeling_channel_dict) == 0:
             return
         df_list = []
         for channel, labels in labeling_channel_dict.items():
             df = create_labeling_peptide_df(self._precursor_df, labels)
-            df['labeling_channel'] = channel
+            df["labeling_channel"] = channel
             df_list.append(df)
         self._precursor_df = pd.concat(df_list, ignore_index=True)
         try:
-            self._precursor_df[
-                'labeling_channel'
-            ] = self._precursor_df.labeling_channel.astype(np.int32)
-            if 'labeling_channel' not in self.key_numeric_columns:
-                self.key_numeric_columns.append('labeling_channel')
-        except:
-            if 'labeling_channel' in self.key_numeric_columns:
-                self.key_numeric_columns.remove('labeling_channel')
-
+            self._precursor_df["labeling_channel"] = (
+                self._precursor_df.labeling_channel.astype(np.int32)
+            )
+            if "labeling_channel" not in self.key_numeric_columns:
+                self.key_numeric_columns.append("labeling_channel")
+        except Exception:
+            if "labeling_channel" in self.key_numeric_columns:
+                self.key_numeric_columns.remove("labeling_channel")
 
     def add_charge(self):
-        """Add charge states
-        """
+        """Add charge states"""
         if "charge" in self._precursor_df.columns:
             return
-        self._precursor_df['charge'] = [
-            np.arange(
-                self.min_precursor_charge, 
-                self.max_precursor_charge+1
-            )
-        ]*len(self._precursor_df)
-        self._precursor_df = self._precursor_df.explode('charge')
-        self._precursor_df['charge'] = self._precursor_df.charge.astype(np.int8)
+        self._precursor_df["charge"] = [
+            np.arange(self.min_precursor_charge, self.max_precursor_charge + 1)
+        ] * len(self._precursor_df)
+        self._precursor_df = self._precursor_df.explode("charge")
+        self._precursor_df["charge"] = self._precursor_df.charge.astype(np.int8)
         self._precursor_df.reset_index(drop=True, inplace=True)
 
-    def save_hdf(self, hdf_file:str):
+    def save_hdf(self, hdf_file: str):
         """Save the contents into hdf file (attribute -> hdf_file):
         - self.precursor_df -> library/precursor_df
         - self.protein_df -> library/protein_df
         - self.fragment_mz_df -> library/fragment_mz_df
         - self.fragment_intensity_df -> library/fragment_intensity_df
 
         Parameters
         ----------
         hdf_file : str
             The hdf file path
         """
         super().save_hdf(hdf_file)
-        _hdf = HDF_File(
-            hdf_file,
-            read_only=False,
-            truncate=True,
-            delete_existing=False
-        )
+        _hdf = HDF_File(hdf_file, read_only=False, truncate=True, delete_existing=False)
         _hdf.library.protein_df = self.protein_df
 
-    def load_hdf(self, hdf_file:str, load_mod_seq:bool=False):
+    def load_hdf(self, hdf_file: str, load_mod_seq: bool = False):
         """Load contents from hdf file:
         - self.precursor_df <- library/precursor_df
         - self.precursor_df <- library/mod_seq_df if load_mod_seq is True
         - self.protein_df <- library/protein_df
         - self.fragment_mz_df <- library/fragment_mz_df
         - self.fragment_intensity_df <- library/fragment_intensity_df
 
         Parameters
         ----------
         hdf_file : str
             hdf file path
 
         load_mod_seq : bool, optional
             After library is generated with hash values (int64) for sequences (str) and modifications (str),
-            we don't need sequence information for searching. 
+            we don't need sequence information for searching.
             So we can skip loading sequences to make the loading much faster.
             By default False
         """
         super().load_hdf(hdf_file, load_mod_seq=load_mod_seq)
         try:
             _hdf = HDF_File(
                 hdf_file,
             )
             self.protein_df = _hdf.library.protein_df.values
         except (AttributeError, KeyError, ValueError, TypeError):
             print(f"No protein_df in {hdf_file}")
 
+
 def annotate_precursor_df(
-        precursor_df : pd.DataFrame,
-        protein_df : pd.DataFrame,
-    ):
+    precursor_df: pd.DataFrame,
+    protein_df: pd.DataFrame,
+):
     """Annotate a list of peptides with genes and proteins by using an ahocorasick automaton.
 
     Parameters
     ----------
 
     precursor_df : pd.DataFrame
         A dataframe containing a sequence column.
@@ -1365,61 +1327,69 @@
         protein dataframe containing `sequence` column.
 
     Returns
     -------
 
     pd.DataFrame
         updated precursor_df with `genes`, `proteins` and `cardinality` columns.
-    
+
     """
     if len(precursor_df) == 0:
         return precursor_df
-    
+
     if len(protein_df) == 0:
         return precursor_df
 
-    if 'sequence' not in precursor_df.columns:
-        raise SystemError('precursor_df must contain a sequence column')
-        
-    peptide_df = pd.DataFrame({
-        'sequence': precursor_df['sequence'].unique()
-    })
+    if "sequence" not in precursor_df.columns:
+        raise SystemError("precursor_df must contain a sequence column")
+
+    peptide_df = pd.DataFrame({"sequence": precursor_df["sequence"].unique()})
 
     # ahocorasick automaton will be used to index the protein_df
     automaton = ahocorasick.Automaton()
-    for i, peptide_sequence in enumerate(peptide_df['sequence']):
+    for i, peptide_sequence in enumerate(peptide_df["sequence"]):
         automaton.add_word(peptide_sequence, i)
     automaton.make_automaton()
 
     genes = [[] for _ in range(len(peptide_df))]
     proteins = [[] for _ in range(len(peptide_df))]
 
     # iter as dictionary
-    for protein_entry in tqdm(protein_df.to_dict('records')):
-        idx = [idx for _, idx in automaton.iter(protein_entry['sequence'])]
+    for protein_entry in tqdm(protein_df.to_dict("records")):
+        idx = [idx for _, idx in automaton.iter(protein_entry["sequence"])]
         idx = np.unique(idx)
         if len(idx) > 0:
             for i in idx:
-                genes[i].append(protein_entry['gene_org'])
-                proteins[i].append(protein_entry['protein_id'])
+                genes[i].append(protein_entry["gene_org"])
+                proteins[i].append(protein_entry["protein_id"])
 
-    peptide_df['genes'] = [';'.join(g) for g in genes]
-    peptide_df['proteins'] = [';'.join(g) for g in proteins]
-    peptide_df['cardinality'] = [len(g) for g in genes]
+    peptide_df["genes"] = [";".join(g) for g in genes]
+    peptide_df["proteins"] = [";".join(g) for g in proteins]
+    peptide_df["cardinality"] = [len(g) for g in genes]
 
-    if 'genes' in precursor_df.columns:
-        precursor_df.drop(columns=['genes'], inplace=True)
+    if "genes" in precursor_df.columns:
+        precursor_df.drop(columns=["genes"], inplace=True)
 
-    if 'proteins' in precursor_df.columns:
-        precursor_df.drop(columns=['proteins'], inplace=True)
+    if "proteins" in precursor_df.columns:
+        precursor_df.drop(columns=["proteins"], inplace=True)
 
-    if 'proteotypic' in precursor_df.columns:
-        precursor_df.drop(columns=['proteotypic'], inplace=True)
+    if "proteotypic" in precursor_df.columns:
+        precursor_df.drop(columns=["proteotypic"], inplace=True)
 
-    if 'cardinality' in precursor_df.columns:
-        precursor_df.drop(columns=['cardinality'], inplace=True)
+    if "cardinality" in precursor_df.columns:
+        precursor_df.drop(columns=["cardinality"], inplace=True)
 
-    failed_annotation = np.sum(peptide_df['genes'] == '')
+    failed_annotation = np.sum(peptide_df["genes"] == "")
     if failed_annotation > 0:
-        warnings.warn(f'{failed_annotation} peptides could not be annotated')
+        warnings.warn(f"{failed_annotation} peptides could not be annotated")
+
+    return precursor_df.merge(peptide_df, on="sequence", how="left")
+
 
-    return precursor_df.merge(peptide_df, on='sequence', how='left')
+def _check_if_multi_mods_on_aa(var_mods):
+    mod_set = set()
+    for mod in var_mods:
+        if mod.find("@") + 2 == len(mod):
+            if mod[-1] in mod_set:
+                return True
+            mod_set.add(mod[-1])
+    return False
```

### Comparing `alphabase-1.2.3/alphabase/protein/lcp_digest.py` & `alphabase-1.2.4/alphabase/protein/lcp_digest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 import numba
 import numpy as np
 from pydivsufsort import divsufsort, kasai
 
-def get_lcp_array(cat_prot:str):
-    data = np.array(cat_prot,'c').view(np.int8)
+
+def get_lcp_array(cat_prot: str):
+    data = np.array(cat_prot, "c").view(np.int8)
     suffix_array = divsufsort(data)
     lcp_array = kasai(data, suffix_array)
     return lcp_array[np.argsort(suffix_array)]
 
+
 @numba.njit
-def get_next_stop_char(seq, stop_char='$'):
+def get_next_stop_char(seq, stop_char="$"):
     next_stop_indices = np.zeros(len(seq), dtype=np.uint32)
-    curr_next_stop = len(seq)-1
-    for i in range(len(seq)-1, -1, -1):
-        if seq[i]==stop_char:
+    curr_next_stop = len(seq) - 1
+    for i in range(len(seq) - 1, -1, -1):
+        if seq[i] == stop_char:
             curr_next_stop = i
         else:
             next_stop_indices[i] = curr_next_stop
     return next_stop_indices
 
+
 @numba.njit
-def get_all_substring_indices_from_lcp(cat_prot, lcp_array, min_len, max_len, stop_char='$'):
+def get_all_substring_indices_from_lcp(
+    cat_prot, lcp_array, min_len, max_len, stop_char="$"
+):
     pos_starts = []
     pos_ends = []
     next_stops = get_next_stop_char(cat_prot, stop_char)
     for i in range(len(cat_prot)):
-        if cat_prot[i] == stop_char: continue
+        if cat_prot[i] == stop_char:
+            continue
         for seq_len in range(
-            max(lcp_array[i]+1,min_len),
-            min(len(cat_prot)-i,max_len+1)
+            max(lcp_array[i] + 1, min_len), min(len(cat_prot) - i, max_len + 1)
         ):
-            end_pos = i+seq_len
-            if end_pos>next_stops[i]: break
+            end_pos = i + seq_len
+            if end_pos > next_stops[i]:
+                break
             pos_starts.append(i)
             pos_ends.append(end_pos)
-    return np.array(pos_starts,dtype=np.uint32), np.array(pos_ends,dtype=np.uint32)
+    return np.array(pos_starts, dtype=np.uint32), np.array(pos_ends, dtype=np.uint32)
 
-def get_substring_indices(cat_prot:str, min_len=7, max_len=25, stop_char='$'):
+
+def get_substring_indices(cat_prot: str, min_len=7, max_len=25, stop_char="$"):
     lcp_array = get_lcp_array(cat_prot)
-    return get_all_substring_indices_from_lcp(cat_prot, lcp_array, min_len, max_len, stop_char=stop_char)
+    return get_all_substring_indices_from_lcp(
+        cat_prot, lcp_array, min_len, max_len, stop_char=stop_char
+    )
+
 
-#compile
+# compile
 get_substring_indices("$ABCABCD$ABCDE$ABCE$BCDEF$", 2, 100)
 
-'''
+"""
 cat_prots = "$ABCABCD$ABCDE$ABCE$BCDEF$"
 pos_starts, pos_ends = get_substring_indices(cat_prots, 2, 100)
 substr_set = set()
 for start,end in zip(pos_starts, pos_ends):
     substr_set.add(cat_prots[start:end])
 assert len(substr_set)==len(pos_starts) #not redundant
 for i in range(len(cat_prots)):
     for j in range(i+2,len(cat_prots)):
         if '$' in cat_prots[i:j]: break
         assert cat_prots[i:j] in substr_set, f"{cat_prots[i:j]} not found" #not missing
-'''
+"""
```

### Comparing `alphabase-1.2.3/alphabase/protein/protein_level_decoy.py` & `alphabase-1.2.4/alphabase/protein/protein_level_decoy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,75 @@
 import pandas as pd
 
 from alphabase.protein.fasta import SpecLibFasta
-from alphabase.spectral_library.decoy import (
-    decoy_lib_provider, SpecLibDecoy
-)
+from alphabase.spectral_library.decoy import decoy_lib_provider, SpecLibDecoy
+
 
 class ProteinReverseDecoy(SpecLibDecoy):
-    def __init__(self, target_lib:SpecLibFasta):
+    def __init__(self, target_lib: SpecLibFasta):
         self.target_lib = target_lib
-        self._precursor_df:pd.DataFrame = pd.DataFrame()
+        self._precursor_df: pd.DataFrame = pd.DataFrame()
         self.protein_df = pd.DataFrame()
         self.decoy_tag = "REV_"
 
-    def _add_tag_to_a_column_in_protein_df(self, column:str):
+    def _add_tag_to_a_column_in_protein_df(self, column: str):
         if column in self.protein_df.columns:
-            self.protein_df[column] = self.decoy_tag+self.protein_df[column]
+            self.protein_df[column] = self.decoy_tag + self.protein_df[column]
 
-    
     def _make_empty_loc_for_target_protein_df(self):
         self.protein_df = pd.concat(
             [
-                pd.DataFrame({'sequence':[""]*len(self.target_lib.protein_df)}),
-                self.protein_df
-            ], ignore_index=True
-        ).fillna('')
+                pd.DataFrame({"sequence": [""] * len(self.target_lib.protein_df)}),
+                self.protein_df,
+            ],
+            ignore_index=True,
+        ).fillna("")
 
     def _decoy_protein_df(self):
         self.protein_df = self.target_lib.protein_df.copy()
-        self.protein_df['sequence'] = self.protein_df.sequence.str[::-1]
-        self._add_tag_to_a_column_in_protein_df(
-            'protein_id'
-        )
-        self._add_tag_to_a_column_in_protein_df(
-            'full_name'
-        )
-        self._add_tag_to_a_column_in_protein_df(
-            'gene_name'
-        )
+        self.protein_df["sequence"] = self.protein_df.sequence.str[::-1]
+        self._add_tag_to_a_column_in_protein_df("protein_id")
+        self._add_tag_to_a_column_in_protein_df("full_name")
+        self._add_tag_to_a_column_in_protein_df("gene_name")
         self._make_empty_loc_for_target_protein_df()
 
     def _generate_decoy_sequences(self):
         _target_prot_df = self.target_lib.protein_df
         _target_pep_df = self.target_lib.precursor_df
         self.target_lib.get_peptides_from_protein_df(self.protein_df)
         self._precursor_df = self.target_lib.precursor_df
         self.target_lib.protein_df = _target_prot_df
         self.target_lib._precursor_df = _target_pep_df
 
     def decoy_sequence(self):
         if (
-            not hasattr(self.target_lib, 'protein_df')
+            not hasattr(self.target_lib, "protein_df")
             or len(self.target_lib.protein_df) == 0
-        ): return
-        
+        ):
+            return
+
         self._decoy_protein_df()
         self._generate_decoy_sequences()
         self._remove_target_seqs()
 
     def append_to_target_lib(self):
         if (
-            not hasattr(self.target_lib, 'protein_df')
+            not hasattr(self.target_lib, "protein_df")
             or len(self.target_lib.protein_df) == 0
-        ): return
+        ):
+            return
         super().append_to_target_lib()
         self._append_protein_df_to_target_lib()
 
     def _append_protein_df_to_target_lib(self):
-        self.protein_df['decoy'] = 1
-        self.target_lib.protein_df['decoy'] = 0
-        self.target_lib.protein_df = pd.concat([
-            self.target_lib.protein_df,
-            self.protein_df.loc[len(self.target_lib.protein_df):]
-        ])
-
-
-decoy_lib_provider.register('protein_reverse', ProteinReverseDecoy)
-
-        
+        self.protein_df["decoy"] = 1
+        self.target_lib.protein_df["decoy"] = 0
+        self.target_lib.protein_df = pd.concat(
+            [
+                self.target_lib.protein_df,
+                self.protein_df.loc[len(self.target_lib.protein_df) :],
+            ]
+        )
 
 
+def register_decoy():
+    decoy_lib_provider.register("protein_reverse", ProteinReverseDecoy)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/alphapept_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/alphapept_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import numba
 import os
 import pandas as pd
 import numpy as np
 import h5py
 
 from alphabase.psm_reader.psm_reader import (
-    PSMReaderBase, psm_reader_provider,
-    psm_reader_yaml
+    PSMReaderBase,
+    psm_reader_provider,
+    psm_reader_yaml,
 )
 
+
 @numba.njit
 def parse_ap(precursor):
     """
     Parser to parse peptide strings
     """
-    items = precursor.split('_')
+    items = precursor.split("_")
     if len(items) == 3:
         decoy = 1
     else:
         decoy = 0
     modseq = items[0]
     charge = items[-1]
 
@@ -27,82 +29,84 @@
     sites = []
     string = ""
 
     for i in range(len(modseq)):
         if modseq[i].isupper():
             break
     if i > 0:
-        sites.append('0')
+        sites.append("0")
         mods.append(modseq[:i])
         modseq = modseq[i:]
 
     for i in modseq:
         string += i
         if i.isupper():
             parsed.append(i)
             if len(string) > 1:
                 sites.append(str(len(parsed)))
                 mods.append(string)
             string = ""
 
-    return ''.join(parsed), ';'.join(mods), ';'.join(sites), charge, decoy
+    return "".join(parsed), ";".join(mods), ";".join(sites), charge, decoy
+
 
 class AlphaPeptReader(PSMReaderBase):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
         **kwargs,
     ):
         """
         Reading PSMs from alphapept's *.ms_data.hdf
         """
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr = fdr,
-            keep_decoy = keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             **kwargs,
         )
-        self.hdf_dataset = 'identifications'
+        self.hdf_dataset = "identifications"
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'alphapept'
-        ]['column_mapping']
+        self.column_mapping = psm_reader_yaml["alphapept"]["column_mapping"]
 
     def _init_modification_mapping(self):
-        self.modification_mapping = psm_reader_yaml[
-            'alphapept'
-        ]['modification_mapping']
+        self.modification_mapping = psm_reader_yaml["alphapept"]["modification_mapping"]
 
     def _load_file(self, filename):
-        with h5py.File(filename, 'r') as _hdf:
+        with h5py.File(filename, "r") as _hdf:
             dataset = _hdf[self.hdf_dataset]
-            df = pd.DataFrame({col:dataset[col] for col in dataset.keys()})
-            df['raw_name'] = os.path.basename(filename)[:-len('.ms_data.hdf')]
-            df['precursor'] = df['precursor'].str.decode('utf-8')
-            #df['naked_sequence'] = df['naked_sequence'].str.decode('utf-8')
-            if 'scan_no' in df.columns:
-                df['scan_no'] = df['scan_no'].astype('int')
-                df['raw_idx'] = df['scan_no']-1 # if thermo, use scan-1 as spec_idx
-            df['charge'] = df['charge'].astype(int)
+            df = pd.DataFrame({col: dataset[col] for col in dataset.keys()})
+            df["raw_name"] = os.path.basename(filename)[: -len(".ms_data.hdf")]
+            df["precursor"] = df["precursor"].str.decode("utf-8")
+            # df['naked_sequence'] = df['naked_sequence'].str.decode('utf-8')
+            if "scan_no" in df.columns:
+                df["scan_no"] = df["scan_no"].astype("int")
+                df["raw_idx"] = df["scan_no"] - 1  # if thermo, use scan-1 as spec_idx
+            df["charge"] = df["charge"].astype(int)
         return df
-    
+
     def _load_modifications(self, df: pd.DataFrame):
-        if len(df) == 0: 
-            self._psm_df['sequence'] = '' 
-            self._psm_df['mods'] = ''
-            self._psm_df['mod_sites'] = ''
-            self._psm_df['decoy'] = 0
+        if len(df) == 0:
+            self._psm_df["sequence"] = ""
+            self._psm_df["mods"] = ""
+            self._psm_df["mod_sites"] = ""
+            self._psm_df["decoy"] = 0
             return
-            
+
         (
-            self._psm_df['sequence'], self._psm_df['mods'],
-            self._psm_df['mod_sites'], _charges,
-            self._psm_df['decoy']
-        ) = zip(*df['precursor'].apply(parse_ap))
+            self._psm_df["sequence"],
+            self._psm_df["mods"],
+            self._psm_df["mod_sites"],
+            _charges,
+            self._psm_df["decoy"],
+        ) = zip(*df["precursor"].apply(parse_ap))
         self._psm_df.decoy = self._psm_df.decoy.astype(np.int8)
-    
-psm_reader_provider.register_reader('alphapept', AlphaPeptReader)
+
+
+def register_readers():
+    psm_reader_provider.register_reader("alphapept", AlphaPeptReader)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/dia_psm_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/dia_psm_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,208 +1,191 @@
 import pandas as pd
 import numpy as np
 
-from alphabase.psm_reader.psm_reader import (
-    psm_reader_provider, psm_reader_yaml
-)
-
-from alphabase.psm_reader.maxquant_reader import (
-    MaxQuantReader
-)
+from alphabase.psm_reader.psm_reader import psm_reader_provider, psm_reader_yaml
+
+from alphabase.psm_reader.maxquant_reader import MaxQuantReader
+
 
 class SpectronautReader(MaxQuantReader):
     """Reader for Spectronaut's output library TSV/CSV.
 
-    Other parameters, please see `MaxQuantReader` 
+    Other parameters, please see `MaxQuantReader`
     in `alphabase.psm_reader.maxquant_reader`
 
     Parameters
     ----------
     csv_sep : str, optional
         Delimiter for TSV/CSV, by default '\t'
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        fixed_C57 = False,
-        mod_seq_columns=psm_reader_yaml[
-            'spectronaut'
-        ]['mod_seq_columns'],
-        rt_unit = 'minute',
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        fixed_C57=False,
+        mod_seq_columns=psm_reader_yaml["spectronaut"]["mod_seq_columns"],
+        rt_unit="minute",
         **kwargs,
     ):
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr=fdr, keep_decoy=keep_decoy,
-            mod_seq_columns = mod_seq_columns,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
+            mod_seq_columns=mod_seq_columns,
             fixed_C57=fixed_C57,
             rt_unit=rt_unit,
             **kwargs,
         )
 
-        self.mod_seq_column = 'ModifiedPeptide'
+        self.mod_seq_column = "ModifiedPeptide"
         self._min_max_rt_norm = True
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'spectronaut'
-        ]['column_mapping']
-    
+        self.column_mapping = psm_reader_yaml["spectronaut"]["column_mapping"]
+
     def _load_file(self, filename):
         self.csv_sep = self._get_table_delimiter(filename)
-        df = pd.read_csv(filename, sep=self.csv_sep,keep_default_na=False)
+        df = pd.read_csv(filename, sep=self.csv_sep, keep_default_na=False)
         self._find_mod_seq_column(df)
-        if 'ReferenceRun' in df.columns:
-            df.drop_duplicates([
-                'ReferenceRun',self.mod_seq_column, 'PrecursorCharge'
-            ], inplace=True)
+        if "ReferenceRun" in df.columns:
+            df.drop_duplicates(
+                ["ReferenceRun", self.mod_seq_column, "PrecursorCharge"], inplace=True
+            )
         else:
-            df.drop_duplicates([
-                self.mod_seq_column, 'PrecursorCharge'
-            ], inplace=True)
+            df.drop_duplicates([self.mod_seq_column, "PrecursorCharge"], inplace=True)
         df.reset_index(drop=True, inplace=True)
-        
+
         return df
 
+
 class SwathReader(SpectronautReader):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        fixed_C57 = False,
-        mod_seq_columns=psm_reader_yaml[
-            'spectronaut'
-        ]['mod_seq_columns'],
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        fixed_C57=False,
+        mod_seq_columns=psm_reader_yaml["spectronaut"]["mod_seq_columns"],
         **kwargs,
     ):
-        """ 
+        """
         SWATH or OpenSWATH library, similar to `SpectronautReader`
         """
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr=fdr, keep_decoy=keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             fixed_C57=fixed_C57,
             mod_seq_columns=mod_seq_columns,
             **kwargs,
         )
 
+
 class DiannReader(SpectronautReader):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        fixed_C57 = False,
-        rt_unit = 'minute',
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        fixed_C57=False,
+        rt_unit="minute",
         **kwargs,
     ):
         """
-        Also similar to `MaxQuantReader`, 
+        Also similar to `MaxQuantReader`,
         but different in column_mapping and modificatin_mapping
         """
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr=fdr, keep_decoy=keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             fixed_C57=fixed_C57,
             rt_unit=rt_unit,
             **kwargs,
         )
 
-        self.mod_seq_column = 'Modified.Sequence'
+        self.mod_seq_column = "Modified.Sequence"
         self._min_max_rt_norm = False
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'diann'
-        ]['column_mapping']
-    
+        self.column_mapping = psm_reader_yaml["diann"]["column_mapping"]
+
     def _load_file(self, filename):
         self.csv_sep = self._get_table_delimiter(filename)
-        df = pd.read_csv(filename, sep=self.csv_sep,keep_default_na=False)
+        df = pd.read_csv(filename, sep=self.csv_sep, keep_default_na=False)
 
         return df
-    
+
     def _post_process(self, origin_df: pd.DataFrame):
         super()._post_process(origin_df)
-        self._psm_df.rename(
-            columns={"spec_idx":"diann_spec_idx"}, inplace=True
-        )
+        self._psm_df.rename(columns={"spec_idx": "diann_spec_idx"}, inplace=True)
 
-psm_reader_provider.register_reader(
-    'spectronaut', SpectronautReader
-)
-psm_reader_provider.register_reader(
-    "speclib_tsv", SpectronautReader
-)
-psm_reader_provider.register_reader(
-    'openswath', SwathReader
-)
-psm_reader_provider.register_reader(
-    'swath', SwathReader
-)
-psm_reader_provider.register_reader(
-    'diann', DiannReader
-)
 
 class SpectronautReportReader(MaxQuantReader):
     """Reader for Spectronaut's report TSV/CSV.
 
-    Other parameters, please see `MaxQuantReader` 
+    Other parameters, please see `MaxQuantReader`
     in `alphabase.psm_reader.maxquant_reader`
 
     Parameters
     ----------
     csv_sep : str, optional
         Delimiter for TSV/CSV, by default ','
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        fixed_C57 = False,
-        rt_unit = 'minute',
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        fixed_C57=False,
+        rt_unit="minute",
         **kwargs,
     ):
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr=fdr, keep_decoy=keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             fixed_C57=fixed_C57,
             rt_unit=rt_unit,
             **kwargs,
         )
 
-        self.precursor_column = 'EG.PrecursorId'
+        self.precursor_column = "EG.PrecursorId"
 
         self._min_max_rt_norm = False
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'spectronaut_report'
-        ]['column_mapping']
-    
+        self.column_mapping = psm_reader_yaml["spectronaut_report"]["column_mapping"]
+
     def _load_file(self, filename):
-        self.mod_seq_column = 'ModifiedSequence'
+        self.mod_seq_column = "ModifiedSequence"
         self.csv_sep = self._get_table_delimiter(filename)
-        df = pd.read_csv(filename, sep=self.csv_sep,keep_default_na=False)
-        df[[self.mod_seq_column,'charge']] = df[
-            self.precursor_column
-        ].str.split('.', expand=True, n=2)
-        df['charge'] = df.charge.astype(np.int8)
+        df = pd.read_csv(filename, sep=self.csv_sep, keep_default_na=False)
+        df[[self.mod_seq_column, "charge"]] = df[self.precursor_column].str.split(
+            ".", expand=True, n=2
+        )
+        df["charge"] = df.charge.astype(np.int8)
         return df
 
 
-psm_reader_provider.register_reader(
-    'spectronaut_report', SpectronautReportReader
-)
-
+def register_readers():
+    psm_reader_provider.register_reader("spectronaut", SpectronautReader)
+    psm_reader_provider.register_reader("speclib_tsv", SpectronautReader)
+    psm_reader_provider.register_reader("openswath", SwathReader)
+    psm_reader_provider.register_reader("swath", SwathReader)
+    psm_reader_provider.register_reader("diann", DiannReader)
+    psm_reader_provider.register_reader("spectronaut_report", SpectronautReportReader)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/maxquant_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/maxquant_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,187 +1,200 @@
 import pandas as pd
 import numpy as np
 import numba
 import copy
 
 from alphabase.psm_reader.psm_reader import (
-    PSMReaderBase, psm_reader_provider,
-    psm_reader_yaml
+    PSMReaderBase,
+    psm_reader_provider,
+    psm_reader_yaml,
 )
 
 from alphabase.constants.modification import MOD_DF
 
 mod_to_unimod_dict = {}
-for mod_name,unimod_id in MOD_DF[['mod_name','unimod_id']].values:
+for mod_name, unimod_id in MOD_DF[["mod_name", "unimod_id"]].values:
     unimod_id = int(unimod_id)
-    if unimod_id==-1 or unimod_id=='-1': continue
-    if mod_name[-2]=='@':
+    if unimod_id == -1 or unimod_id == "-1":
+        continue
+    if mod_name[-2] == "@":
         mod_to_unimod_dict[mod_name] = f"{mod_name[-1]}(UniMod:{unimod_id})"
     else:
         mod_to_unimod_dict[mod_name] = f"_(UniMod:{unimod_id})"
 
+
 @numba.njit
 def replace_parentheses_with_brackets(
-    modseq:str,
+    modseq: str,
 ):
     mod_depth = 0
-    for i,aa in enumerate(modseq):
-        if aa == '(':
+    for i, aa in enumerate(modseq):
+        if aa == "(":
             if mod_depth <= 0:
-                modseq = modseq[:i] + '[' + modseq[i+1:]
+                modseq = modseq[:i] + "[" + modseq[i + 1 :]
             mod_depth += 1
-        elif aa == '[':
+        elif aa == "[":
             mod_depth += 1
-        elif aa == ')':
+        elif aa == ")":
             mod_depth -= 1
             if mod_depth <= 0:
-                modseq = modseq[:i] + ']' + modseq[i+1:]
-        elif aa == ']':
+                modseq = modseq[:i] + "]" + modseq[i + 1 :]
+        elif aa == "]":
             mod_depth -= 1
     return modseq
-        
+
 
 @numba.njit
 def parse_mod_seq(
-    modseq:str,
-    mod_sep:str='()',
-    fixed_C57:bool=True,
-)->tuple:
+    modseq: str,
+    mod_sep: str = "()",
+    fixed_C57: bool = True,
+) -> tuple:
     """Extract modifications and sites from the modified sequence (modseq)
 
     Parameters
     ----------
     modseq : str
         modified sequence to extract modifications.
 
     mod_sep : str, optional
-        separator to indicate the modification section. 
+        separator to indicate the modification section.
         Defaults to '()'
 
     fixed_C : bool
-        If Carbamidomethyl@C is a fixed modification 
+        If Carbamidomethyl@C is a fixed modification
         and not displayed in the sequence. Defaults to True for MaxQuant.
 
     Returns
     -------
     tuple
         str: naked peptide sequence
 
         str: modification names, separated by ';'
-        
-        str: modification sites, separated by ';'. 
+
+        str: modification sites, separated by ';'.
         0 for N-term; -1 for C-term; 1 to N for normal modifications.
     """
     PeptideModSeq = modseq
-    if modseq[0] == '_':
+    if modseq[0] == "_":
         underscore_for_ncterm = True
     else:
         underscore_for_ncterm = False
     mod_list = []
     site_list = []
     site = PeptideModSeq.find(mod_sep[0])
     while site != -1:
-        site_end = PeptideModSeq.find(mod_sep[1],site+1)+1
-        if site_end < len(PeptideModSeq) and PeptideModSeq[site_end] == mod_sep[1]: 
+        site_end = PeptideModSeq.find(mod_sep[1], site + 1) + 1
+        if site_end < len(PeptideModSeq) and PeptideModSeq[site_end] == mod_sep[1]:
             site_end += 1
-        if underscore_for_ncterm: site_list.append(site-1)
-        else: site_list.append(site)
+        if underscore_for_ncterm:
+            site_list.append(site - 1)
+        else:
+            site_list.append(site)
         start_mod = site
-        if start_mod > 0: start_mod -= 1
+        if start_mod > 0:
+            start_mod -= 1
         mod_list.append(PeptideModSeq[start_mod:site_end])
         PeptideModSeq = PeptideModSeq[:site] + PeptideModSeq[site_end:]
         site = PeptideModSeq.find(mod_sep[0], site)
 
     # patch for phos. How many other modification formats does MQ have?
-    site = PeptideModSeq.find('p') 
+    site = PeptideModSeq.find("p")
     while site != -1:
-        mod_list.append(PeptideModSeq[site:site+2])
-        site_list = [i-1 if i > site else i for i in site_list]
-        if underscore_for_ncterm: site_list.append(site)
-        else: site_list.append(site+1)
-        PeptideModSeq = PeptideModSeq[:site] + PeptideModSeq[site+1:]
-        site = PeptideModSeq.find('p', site)
-        
+        mod_list.append(PeptideModSeq[site : site + 2])
+        site_list = [i - 1 if i > site else i for i in site_list]
+        if underscore_for_ncterm:
+            site_list.append(site)
+        else:
+            site_list.append(site + 1)
+        PeptideModSeq = PeptideModSeq[:site] + PeptideModSeq[site + 1 :]
+        site = PeptideModSeq.find("p", site)
+
     if fixed_C57:
-        site = PeptideModSeq.find('C')
+        site = PeptideModSeq.find("C")
         while site != -1:
-            if underscore_for_ncterm: site_list.append(site)
-            else: site_list.append(site+1)
-            mod_list.append('C'+"Carbamidomethyl (C)".join(mod_sep))
-            site = PeptideModSeq.find('C',site+1)
-    sequence = PeptideModSeq.strip('_')
+            if underscore_for_ncterm:
+                site_list.append(site)
+            else:
+                site_list.append(site + 1)
+            mod_list.append("C" + "Carbamidomethyl (C)".join(mod_sep))
+            site = PeptideModSeq.find("C", site + 1)
+    sequence = PeptideModSeq.strip("_")
     nAA = len(sequence)
-    return sequence, ';'.join(mod_list), ';'.join([str(i) if i <= nAA else '-1' for i in site_list])
+    return (
+        sequence,
+        ";".join(mod_list),
+        ";".join([str(i) if i <= nAA else "-1" for i in site_list]),
+    )
 
 
 class MaxQuantReader(PSMReaderBase):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        fixed_C57 = True,
-        mod_seq_columns = ['Modified sequence'],
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        fixed_C57=True,
+        mod_seq_columns=["Modified sequence"],
         **kwargs,
     ):
         """Reader for MaxQuant msms.txt and evidence.txt
 
         Parameters
         ----------
         column_mapping : dict, optional
-            By default None. If None, use 
-            `psm_reader_yaml['maxquant']['column_mapping']` 
+            By default None. If None, use
+            `psm_reader_yaml['maxquant']['column_mapping']`
             (alphabase.psm_reader.psm_reader_yaml).
 
         modification_mapping : dict, optional
-            By default None. If None, use 
-            `psm_reader_yaml['maxquant']['modification_mapping']` 
+            By default None. If None, use
+            `psm_reader_yaml['maxquant']['modification_mapping']`
             (alphabase.psm_reader.psm_reader_yaml).
 
         fdr : float, optional
             Load PSMs with FDR < this fdr, by default 0.01
 
         keep_decoy : bool, optional
             If keep decoy PSMs, by default False
 
         fixed_C57 : bool, optional
             If true, the search engine will not show `Carbamidomethyl`
-            in the modified sequences. 
+            in the modified sequences.
             by default True
 
         mod_seq_columns : list, optional
-            The columns to find modified sequences, 
+            The columns to find modified sequences,
             by default ['Modified sequence']
         """
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr = fdr,
-            keep_decoy = keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             **kwargs,
         )
 
         self.fixed_C57 = fixed_C57
         self._mod_seq_columns = mod_seq_columns
-        self.mod_seq_column = 'Modified sequence'
+        self.mod_seq_column = "Modified sequence"
 
     def _find_mod_seq_column(self, df):
         for mod_seq_col in self._mod_seq_columns:
             if mod_seq_col in df.columns:
                 self.mod_seq_column = mod_seq_col
                 break
-        
+
     def _init_modification_mapping(self):
         self.modification_mapping = copy.deepcopy(
             # otherwise maxquant reader will modify the dict inplace
-            psm_reader_yaml['maxquant'][
-                'modification_mapping'
-            ]
-        ) 
+            psm_reader_yaml["maxquant"]["modification_mapping"]
+        )
 
     def set_modification_mapping(self, modification_mapping: dict):
         super().set_modification_mapping(modification_mapping)
         self._add_all_unimod()
         self._extend_mod_brackets()
         self._reverse_mod_mapping()
 
@@ -189,85 +202,75 @@
         for mod_name, unimod in mod_to_unimod_dict.items():
             if mod_name in self.modification_mapping:
                 self.modification_mapping[mod_name].append(unimod)
             else:
                 self.modification_mapping[mod_name] = [unimod]
 
     def _extend_mod_brackets(self):
-        """update modification_mapping to include different bracket types.
-                
-        """
+        """update modification_mapping to include different bracket types."""
 
         for key, mod_list in list(self.modification_mapping.items()):
-
             mod_set = set(mod_list)
             # extend bracket types of modifications
             # K(Acetyl) -> K[Acetyl]
             # (Phospho) -> _(Phospho)
             # _[Phospho] -> _(Phospho)
             for mod in mod_list:
-
-                if mod[1] == '(':
-                    mod_set.add(f'{mod[0]}[{mod[2:-1]}]')
-                elif mod[1] == '[':
-                    mod_set.add(f'{mod[0]}({mod[2:-1]})')
-                    
-                if mod.startswith('_'):
-                    mod_set.add(f'{mod[1:]}')
-                elif mod.startswith('('):
-                    mod_set.add(f'_{mod}')
-                    mod_set.add(f'[{mod[1:-1]}]')
-                    mod_set.add(f'_[{mod[1:-1]}]')
-                elif mod.startswith('['):
-                    mod_set.add(f'_{mod}')
-                    mod_set.add(f'({mod[1:-1]})')
-                    mod_set.add(f'_({mod[1:-1]})')
+                if mod[1] == "(":
+                    mod_set.add(f"{mod[0]}[{mod[2:-1]}]")
+                elif mod[1] == "[":
+                    mod_set.add(f"{mod[0]}({mod[2:-1]})")
+
+                if mod.startswith("_"):
+                    mod_set.add(f"{mod[1:]}")
+                elif mod.startswith("("):
+                    mod_set.add(f"_{mod}")
+                    mod_set.add(f"[{mod[1:-1]}]")
+                    mod_set.add(f"_[{mod[1:-1]}]")
+                elif mod.startswith("["):
+                    mod_set.add(f"_{mod}")
+                    mod_set.add(f"({mod[1:-1]})")
+                    mod_set.add(f"_({mod[1:-1]})")
 
             self.modification_mapping[key] = list(mod_set)
 
-    
     def _translate_decoy(self, origin_df=None):
-        if 'decoy' in self._psm_df.columns:
-            self._psm_df.decoy = (
-                self._psm_df.decoy == '-'
-            ).astype(np.int8)
+        if "decoy" in self._psm_df.columns:
+            self._psm_df.decoy = (self._psm_df.decoy == "-").astype(np.int8)
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'maxquant'
-        ]['column_mapping']
+        self.column_mapping = psm_reader_yaml["maxquant"]["column_mapping"]
 
     def _load_file(self, filename):
         csv_sep = self._get_table_delimiter(filename)
-        df = pd.read_csv(filename, sep=csv_sep,keep_default_na=False)
+        df = pd.read_csv(filename, sep=csv_sep, keep_default_na=False)
         self._find_mod_seq_column(df)
-        df = df[~pd.isna(df['Retention time'])]
-        df.fillna('', inplace=True)
+        df = df[~pd.isna(df["Retention time"])]
+        df.fillna("", inplace=True)
         # if 'K0' in df.columns:
         #     df['Mobility'] = df['K0'] # Bug in MaxQuant? It should be 1/K0
         # min_rt = df['Retention time'].min()
         return df
 
     def _load_modifications(self, origin_df: pd.DataFrame):
-        if origin_df[self.mod_seq_column].str.contains('[', regex=False).any():
-            if origin_df[self.mod_seq_column].str.contains('(', regex=False).any():
+        if origin_df[self.mod_seq_column].str.contains("[", regex=False).any():
+            if origin_df[self.mod_seq_column].str.contains("(", regex=False).any():
                 origin_df[self.mod_seq_column] = origin_df[self.mod_seq_column].apply(
                     replace_parentheses_with_brackets
                 )
             mod_sep = "[]"
         else:
             mod_sep = "()"
-        
-        (
-            seqs,
-            self._psm_df['mods'], 
-            self._psm_df['mod_sites']
-        ) = zip(
+
+        (seqs, self._psm_df["mods"], self._psm_df["mod_sites"]) = zip(
             *origin_df[self.mod_seq_column].apply(
-                parse_mod_seq, mod_sep=mod_sep,
+                parse_mod_seq,
+                mod_sep=mod_sep,
                 fixed_C57=self.fixed_C57,
             )
         )
-        if 'sequence' not in self._psm_df.columns:
-            self._psm_df['sequence'] = seqs
+        if "sequence" not in self._psm_df.columns:
+            self._psm_df["sequence"] = seqs
+
 
-psm_reader_provider.register_reader('maxquant', MaxQuantReader)
+def register_readers():
+    psm_reader_provider.register_reader("maxquant", MaxQuantReader)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/msfragger_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/msfragger_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,183 +1,188 @@
 import numpy as np
 import pandas as pd
 
 from alphabase.psm_reader.psm_reader import (
-    PSMReaderBase, psm_reader_yaml,
-    psm_reader_provider
+    PSMReaderBase,
+    psm_reader_yaml,
+    psm_reader_provider,
 )
 from alphabase.constants.aa import AA_ASCII_MASS
-from alphabase.constants.atom import MASS_H, MASS_O, MASS_PROTON
+from alphabase.constants.atom import MASS_H, MASS_O
 from alphabase.constants.modification import MOD_MASS
 
-try:
-    import pyteomics.pepxml as pepxml
-except:
-    pepxml = None
+import pyteomics.pepxml as pepxml
+
 
 def _is_fragger_decoy(proteins):
     for prot in proteins:
-        if not prot.lower().startswith('rev_'):
+        if not prot.lower().startswith("rev_"):
             return False
     return True
 
-mass_mapped_mods = psm_reader_yaml['msfragger_pepxml']['mass_mapped_mods']
-mod_mass_tol = psm_reader_yaml['msfragger_pepxml']['mod_mass_tol']
+
+mass_mapped_mods = psm_reader_yaml["msfragger_pepxml"]["mass_mapped_mods"]
+mod_mass_tol = psm_reader_yaml["msfragger_pepxml"]["mod_mass_tol"]
+
 
 def _get_mods_from_masses(sequence, msf_aa_mods):
     mods = []
     mod_sites = []
     aa_mass_diffs = []
     aa_mass_diff_sites = []
     for mod in msf_aa_mods:
-        _mass_str, site_str = mod.split('@')
+        _mass_str, site_str = mod.split("@")
         mod_mass = float(_mass_str)
         site = int(site_str)
         cterm_position = len(sequence) + 1
         if site > 0:
             if site < cterm_position:
-                mod_mass = mod_mass - AA_ASCII_MASS[ord(sequence[site-1])]
+                mod_mass = mod_mass - AA_ASCII_MASS[ord(sequence[site - 1])]
             else:
-                mod_mass -= (2* MASS_H + MASS_O)
+                mod_mass -= 2 * MASS_H + MASS_O
         else:
             mod_mass -= MASS_H
 
         mod_translated = False
         for mod_name in mass_mapped_mods:
-            if abs(mod_mass-MOD_MASS[mod_name])<mod_mass_tol:
-                if site==0:
-                    _mod = mod_name.split('@')[0]+'@Any N-term'
-                elif site==1:
-                    if mod_name.endswith('^Any N-term'):
+            if abs(mod_mass - MOD_MASS[mod_name]) < mod_mass_tol:
+                if site == 0:
+                    _mod = mod_name.split("@")[0] + "@Any N-term"
+                elif site == 1:
+                    if mod_name.endswith("^Any N-term"):
                         _mod = mod_name
-                        site_str = '0'
+                        site_str = "0"
                     else:
-                        _mod = mod_name.split('@')[0]+'@'+sequence[0]
-                elif site==cterm_position:
-                    if mod_name.endswith('C-term'):
+                        _mod = mod_name.split("@")[0] + "@" + sequence[0]
+                elif site == cterm_position:
+                    if mod_name.endswith("C-term"):
                         _mod = mod_name
                     else:
-                        _mod = mod_name.split('@')[0]+'@Any C-term' #what if only Protein C-term is listed?
-                    site_str = '-1'
+                        _mod = (
+                            mod_name.split("@")[0] + "@Any C-term"
+                        )  # what if only Protein C-term is listed?
+                    site_str = "-1"
                 else:
-                    _mod = mod_name.split('@')[0]+'@'+sequence[site-1]
+                    _mod = mod_name.split("@")[0] + "@" + sequence[site - 1]
                 if _mod in MOD_MASS:
                     mods.append(_mod)
                     mod_sites.append(site_str)
                     mod_translated = True
                     break
         if not mod_translated:
-            aa_mass_diffs.append(f'{mod_mass:.5f}')
+            aa_mass_diffs.append(f"{mod_mass:.5f}")
             aa_mass_diff_sites.append(site_str)
-    return ';'.join(mods), ';'.join(mod_sites), ';'.join(aa_mass_diffs), ';'.join(aa_mass_diff_sites)
+    return (
+        ";".join(mods),
+        ";".join(mod_sites),
+        ";".join(aa_mass_diffs),
+        ";".join(aa_mass_diff_sites),
+    )
 
 
 class MSFragger_PSM_TSV_Reader(PSMReaderBase):
-    def __init__(self, *, 
-        column_mapping: dict = None, 
-        modification_mapping: dict = None, 
-        fdr=0.01, 
-        keep_decoy=False, 
-        rt_unit = 'second',
-        **kwargs
+    def __init__(
+        self,
+        *,
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        rt_unit="second",
+        **kwargs,
     ):
         raise NotImplementedError("MSFragger_PSM_TSV_Reader for psm.tsv")
 
-psm_reader_provider.register_reader('msfragger_psm_tsv', MSFragger_PSM_TSV_Reader)
-psm_reader_provider.register_reader('msfragger', MSFragger_PSM_TSV_Reader)
 
-if pepxml is None:
-    class MSFraggerPepXML:
-        def __init__(self): raise NotImplementedError("")
-else:
-    class MSFraggerPepXML(PSMReaderBase):
-        def __init__(self, *, 
-            column_mapping: dict = None, 
-            modification_mapping: dict = None,
-            fdr = 0.001, # refers to E-value in the PepXML
-            keep_decoy=False, 
-            rt_unit = 'second',
-            keep_unknown_aa_mass_diffs=False,
-            **kwargs
-        ):
-            """MSFragger is not fully supported as we can only access the pepxml file.
-            """
-            super().__init__(
-                column_mapping=column_mapping, 
-                modification_mapping=modification_mapping,
-                fdr = fdr,
-                keep_decoy=keep_decoy, 
-                rt_unit = rt_unit,
-                **kwargs
+class MSFraggerPepXML(PSMReaderBase):
+    def __init__(
+        self,
+        *,
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.001,  # refers to E-value in the PepXML
+        keep_decoy=False,
+        rt_unit="second",
+        keep_unknown_aa_mass_diffs=False,
+        **kwargs,
+    ):
+        """MSFragger is not fully supported as we can only access the pepxml file."""
+        super().__init__(
+            column_mapping=column_mapping,
+            modification_mapping=modification_mapping,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
+            rt_unit=rt_unit,
+            **kwargs,
+        )
+        self.keep_unknown_aa_mass_diffs = keep_unknown_aa_mass_diffs
+
+    def _init_column_mapping(self):
+        self.column_mapping = psm_reader_yaml["msfragger_pepxml"]["column_mapping"]
+
+    def _init_modification_mapping(self):
+        self.modification_mapping = {}
+
+    def _translate_modifications(self):
+        pass
+
+    def _load_file(self, filename):
+        msf_df = pepxml.DataFrame(filename)
+        msf_df.fillna("", inplace=True)
+        if "ion_mobility" in msf_df.columns:
+            msf_df["ion_mobility"] = msf_df.ion_mobility.astype(float)
+        msf_df["raw_name"] = msf_df["spectrum"].str.split(".").apply(lambda x: x[0])
+        msf_df["to_remove"] = 0
+        self.column_mapping["to_remove"] = "to_remove"
+        return msf_df
+
+    def _translate_decoy(self, origin_df=None):
+        self._psm_df["decoy"] = self._psm_df.proteins.apply(_is_fragger_decoy).astype(
+            np.int8
+        )
+
+        self._psm_df.proteins = self._psm_df.proteins.apply(lambda x: ";".join(x))
+        if not self.keep_decoy:
+            self._psm_df["to_remove"] += self._psm_df.decoy > 0
+
+    def _translate_score(self, origin_df=None):
+        # evalue score
+        self._psm_df["score"] = -np.log(self._psm_df["score"] + 1e-100)
+
+    def _load_modifications(self, msf_df):
+        if len(msf_df) == 0:
+            self._psm_df["mods"] = ""
+            self._psm_df["mod_sites"] = ""
+            self._psm_df["aa_mass_diffs"] = ""
+            self._psm_df["aa_mass_diff_sites"] = ""
+            return
+
+        (
+            self._psm_df["mods"],
+            self._psm_df["mod_sites"],
+            self._psm_df["aa_mass_diffs"],
+            self._psm_df["aa_mass_diff_sites"],
+        ) = zip(
+            *msf_df[["peptide", "modifications"]].apply(
+                lambda x: _get_mods_from_masses(*x), axis=1
             )
-            self.keep_unknown_aa_mass_diffs = keep_unknown_aa_mass_diffs
+        )
 
-        def _init_column_mapping(self):
-            self.column_mapping = psm_reader_yaml[
-                'msfragger_pepxml'
-            ]['column_mapping']
-            
-        def _init_modification_mapping(self):
-            self.modification_mapping = {}
-
-        def _translate_modifications(self):
-            pass
-
-        def _load_file(self, filename):
-            msf_df = pepxml.DataFrame(filename)
-            msf_df.fillna('', inplace=True)
-            if 'ion_mobility' in msf_df.columns:
-                msf_df['ion_mobility'] = msf_df.ion_mobility.astype(float)
-            msf_df['raw_name'] = msf_df[
-                'spectrum'
-            ].str.split('.').apply(lambda x: x[0])
-            msf_df['to_remove'] = 0
-            self.column_mapping['to_remove'] = 'to_remove'
-            return msf_df
-
-        def _translate_decoy(self, origin_df=None):
-            self._psm_df['decoy'] = self._psm_df.proteins.apply(
-                _is_fragger_decoy
-            ).astype(np.int8)
-
-            self._psm_df.proteins = self._psm_df.proteins.apply(
-                lambda x: ';'.join(x)
-            )
-            if not self.keep_decoy:
-                self._psm_df['to_remove'] += (self._psm_df.decoy > 0)
-        
-        def _translate_score(self, origin_df=None):
-            # evalue score
-            self._psm_df['score'] = -np.log(
-                self._psm_df['score']+1e-100
+        if not self.keep_unknown_aa_mass_diffs:
+            self._psm_df["to_remove"] += self._psm_df.aa_mass_diffs != ""
+            self._psm_df.drop(
+                columns=["aa_mass_diffs", "aa_mass_diff_sites"], inplace=True
             )
 
-        def _load_modifications(self, msf_df):
-            if len(msf_df) == 0:
-                self._psm_df['mods'] = ''
-                self._psm_df['mod_sites'] = ''
-                self._psm_df['aa_mass_diffs'] = ''
-                self._psm_df['aa_mass_diff_sites'] = ''
-                return
-
-            (
-                self._psm_df['mods'], self._psm_df['mod_sites'],
-                self._psm_df['aa_mass_diffs'], self._psm_df['aa_mass_diff_sites'],
-            ) = zip(*msf_df[['peptide','modifications']].apply(
-                lambda x: _get_mods_from_masses(*x), axis=1)
-            )
-                
-            if not self.keep_unknown_aa_mass_diffs:
-                self._psm_df['to_remove'] += (self._psm_df.aa_mass_diffs != '')
-                self._psm_df.drop(
-                    columns=['aa_mass_diffs','aa_mass_diff_sites'], 
-                    inplace=True
-                )
-
-        def _post_process(self, origin_df: pd.DataFrame):
-            super()._post_process(origin_df)
-            self._psm_df = self._psm_df.query(
-                'to_remove==0'
-            ).drop(columns='to_remove').reset_index(drop=True)
+    def _post_process(self, origin_df: pd.DataFrame):
+        super()._post_process(origin_df)
+        self._psm_df = (
+            self._psm_df.query("to_remove==0")
+            .drop(columns="to_remove")
+            .reset_index(drop=True)
+        )
 
-    psm_reader_provider.register_reader('msfragger_pepxml', MSFraggerPepXML)
 
+def register_readers():
+    psm_reader_provider.register_reader("msfragger_psm_tsv", MSFragger_PSM_TSV_Reader)
+    psm_reader_provider.register_reader("msfragger", MSFragger_PSM_TSV_Reader)
+    psm_reader_provider.register_reader("msfragger_pepxml", MSFraggerPepXML)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/pfind_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/pfind_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,148 +1,149 @@
 import pandas as pd
 import numpy as np
 
 import alphabase.constants.modification as ap_mod
 
 from alphabase.psm_reader.psm_reader import (
-    PSMReaderBase, psm_reader_provider,
-    psm_reader_yaml
+    PSMReaderBase,
+    psm_reader_provider,
+    psm_reader_yaml,
 )
 
+
 def convert_one_pFind_mod(mod):
-    if mod[-1] == ')':
-        mod = mod[:(mod.find('(')-1)]
-        idx = mod.rfind('[')
+    if mod[-1] == ")":
+        mod = mod[: (mod.find("(") - 1)]
+        idx = mod.rfind("[")
         name = mod[:idx]
-        site = mod[(idx+1):]
+        site = mod[(idx + 1) :]
     else:
-        idx = mod.rfind('[')
+        idx = mod.rfind("[")
         name = mod[:idx]
-        site = mod[(idx+1):-1]
+        site = mod[(idx + 1) : -1]
     if len(site) == 1:
-        return name + '@' + site
-    elif site == 'AnyN-term':
-        return name + '@' + 'Any N-term'
-    elif site == 'ProteinN-term':
-        return name + '@' + 'Protein N-term'
-    elif site.startswith('AnyN-term'):
-        return name + '@' + site[-1] + '^Any N-term'
-    elif site.startswith('ProteinN-term'):
-        return name + '@' + site[-1] + '^Protein N-term'
-    elif site == 'AnyC-term':
-        return name + '@' + 'Any C-term'
-    elif site == 'ProteinC-term':
-        return name + '@' + 'Protein C-term'
-    elif site.startswith('AnyC-term'):
-        return name + '@' + site[-1] + '^Any C-term'
-    elif site.startswith('ProteinC-term'):
-        return name + '@' + site[-1] + '^Protein C-term'
+        return name + "@" + site
+    elif site == "AnyN-term":
+        return name + "@" + "Any N-term"
+    elif site == "ProteinN-term":
+        return name + "@" + "Protein N-term"
+    elif site.startswith("AnyN-term"):
+        return name + "@" + site[-1] + "^Any N-term"
+    elif site.startswith("ProteinN-term"):
+        return name + "@" + site[-1] + "^Protein N-term"
+    elif site == "AnyC-term":
+        return name + "@" + "Any C-term"
+    elif site == "ProteinC-term":
+        return name + "@" + "Protein C-term"
+    elif site.startswith("AnyC-term"):
+        return name + "@" + site[-1] + "^Any C-term"
+    elif site.startswith("ProteinC-term"):
+        return name + "@" + site[-1] + "^Protein C-term"
     else:
         return None
 
+
 def translate_pFind_mod(mod_str):
-    if not mod_str: return ""
+    if not mod_str:
+        return ""
     ret_mods = []
-    for mod in mod_str.split(';'):
+    for mod in mod_str.split(";"):
         mod = convert_one_pFind_mod(mod)
-        if not mod: return pd.NA
-        elif mod not in ap_mod.MOD_INFO_DICT: return pd.NA
-        else: ret_mods.append(mod)
-    return ';'.join(ret_mods)
+        if not mod:
+            return pd.NA
+        elif mod not in ap_mod.MOD_INFO_DICT:
+            return pd.NA
+        else:
+            ret_mods.append(mod)
+    return ";".join(ret_mods)
+
 
 def get_pFind_mods(pfind_mod_str):
-    pfind_mod_str = pfind_mod_str.strip(';')
-    if not pfind_mod_str: return "", ""
+    pfind_mod_str = pfind_mod_str.strip(";")
+    if not pfind_mod_str:
+        return "", ""
+
+    items = [item.split(",", 3) for item in pfind_mod_str.split(";")]
 
     items = [
-        item.split(',',3) 
-        for item in pfind_mod_str.split(';')
-    ]
-    
-    items = [
-        ('-1',mod) if (mod.endswith('C-term]') 
-        or mod[:-2].endswith('C-term'))
-        #else ('0', mod) if mod.endswith('N-term]')
-        else (site, mod) for site, mod in items
+        ("-1", mod)
+        if (mod.endswith("C-term]") or mod[:-2].endswith("C-term"))
+        # else ('0', mod) if mod.endswith('N-term]')
+        else (site, mod)
+        for site, mod in items
     ]
     items = list(zip(*items))
-    return ';'.join(items[1]), ';'.join(items[0])
+    return ";".join(items[1]), ";".join(items[0])
+
 
 def parse_pfind_protein(protein, keep_reverse=True):
-    proteins = protein.strip('/').split('/')
-    return ';'.join(
+    proteins = protein.strip("/").split("/")
+    return ";".join(
         [
-            protein for protein in proteins 
-            if (
-                not protein.startswith('REV_') 
-                or keep_reverse
-            )
+            protein
+            for protein in proteins
+            if (not protein.startswith("REV_") or keep_reverse)
         ]
     )
 
 
 class pFindReader(PSMReaderBase):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
         **kwargs,
     ):
         super().__init__(
             column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr = fdr,
-            keep_decoy = keep_decoy,
+            fdr=fdr,
+            keep_decoy=keep_decoy,
             **kwargs,
         )
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'pfind'
-        ]['column_mapping']
-        
+        self.column_mapping = psm_reader_yaml["pfind"]["column_mapping"]
+
     def _init_modification_mapping(self):
         self.modification_mapping = {}
 
     def _translate_modifications(self):
         pass
 
     def _load_file(self, filename):
-        pfind_df = pd.read_csv(filename, index_col=False, sep='\t',keep_default_na=False)
-        pfind_df.fillna('', inplace=True)
-        pfind_df = pfind_df[pfind_df.Sequence != '']
-        pfind_df['raw_name'] = pfind_df[
-            'File_Name'
-        ].str.split('.').apply(lambda x: x[0])
-        pfind_df['Proteins'] = pfind_df[
-            'Proteins'
-        ].apply(parse_pfind_protein)
+        pfind_df = pd.read_csv(
+            filename, index_col=False, sep="\t", keep_default_na=False
+        )
+        pfind_df.fillna("", inplace=True)
+        pfind_df = pfind_df[pfind_df.Sequence != ""]
+        pfind_df["raw_name"] = (
+            pfind_df["File_Name"].str.split(".").apply(lambda x: x[0])
+        )
+        pfind_df["Proteins"] = pfind_df["Proteins"].apply(parse_pfind_protein)
         return pfind_df
 
     def _translate_decoy(self, origin_df=None):
-        self._psm_df.decoy = (
-            self._psm_df.decoy == 'decoy'
-        ).astype(np.int8)
-        
+        self._psm_df.decoy = (self._psm_df.decoy == "decoy").astype(np.int8)
+
     def _translate_score(self, origin_df=None):
-        self._psm_df.score = -np.log(
-            self._psm_df.score.astype(float)+1e-100
-        )
+        self._psm_df.score = -np.log(self._psm_df.score.astype(float) + 1e-100)
 
     def _load_modifications(self, pfind_df):
         if len(pfind_df) == 0:
-            self._psm_df['mods'] = ''
-            self._psm_df['mod_sites'] = ''
+            self._psm_df["mods"] = ""
+            self._psm_df["mod_sites"] = ""
             return
-            
-        (
-            self._psm_df['mods'], self._psm_df['mod_sites']
-        ) = zip(*pfind_df['Modification'].apply(get_pFind_mods))
 
-        self._psm_df['mods'] = self._psm_df['mods'].apply(
-            translate_pFind_mod
+        (self._psm_df["mods"], self._psm_df["mod_sites"]) = zip(
+            *pfind_df["Modification"].apply(get_pFind_mods)
         )
-        
-psm_reader_provider.register_reader('pfind', pFindReader)
-psm_reader_provider.register_reader('pfind3', pFindReader)
+
+        self._psm_df["mods"] = self._psm_df["mods"].apply(translate_pFind_mod)
+
+
+def register_readers():
+    psm_reader_provider.register_reader("pfind", pFindReader)
+    psm_reader_provider.register_reader("pfind3", pFindReader)
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/psm_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/psm_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,213 +1,202 @@
 import os
 import copy
-import io
 import pandas as pd
 import numpy as np
 import warnings
 
 import alphabase.peptide.mobility as mobility
-from alphabase.peptide.precursor import (
-    update_precursor_mz, reset_precursor_df
-)
+from alphabase.peptide.precursor import update_precursor_mz, reset_precursor_df
 from alphabase.constants._const import CONST_FILE_FOLDER
 
 from alphabase.utils import get_delimiter
 from alphabase.yaml_utils import load_yaml
 
 
-
-def translate_other_modification(
-    mod_str: str, 
-    mod_dict: dict
-)->str:
-    '''
-    Translate modifications of `mod_str` to the AlphaBase 
+def translate_other_modification(mod_str: str, mod_dict: dict) -> str:
+    """
+    Translate modifications of `mod_str` to the AlphaBase
     format mapped by mod_dict.
-    
+
     Parameters
     ----------
         mod_str : str
-            mod list in str format, seperated by ';', 
+            mod list in str format, seperated by ';',
             e.g. ModA;ModB
         mod_dict : dict
-            translate mod dict from others to AlphaBase, 
-            e.g. for pFind, key=['Phospho[S]','Oxidation[M]'], 
+            translate mod dict from others to AlphaBase,
+            e.g. for pFind, key=['Phospho[S]','Oxidation[M]'],
             value=['Phospho@S','Oxidation@M']
     Returns
     -------
     str
         new mods in AlphaBase format seperated by ';'. if any
         modification is not in `mod_dict`, return pd.NA.
-    '''
+    """
 
-    if mod_str == "" : return "", []
+    if mod_str == "":
+        return "", []
     ret_mods = []
     unknown_mods = []
-    for mod in mod_str.split(';'):
+    for mod in mod_str.split(";"):
         if mod in mod_dict:
             ret_mods.append(mod_dict[mod])
         else:
             unknown_mods.append(mod)
 
     if len(unknown_mods) > 0:
         return pd.NA, unknown_mods
     else:
         return ";".join(ret_mods), []
 
-def keep_modifications(
-    mod_str: str, 
-    mod_set: set
-)->str:
-    '''
+
+def keep_modifications(mod_str: str, mod_set: set) -> str:
+    """
     Check if modifications of `mod_str` are in `mod_set`.
 
     Parameters
     ----------
     mod_str : str
-        mod list in str format, seperated by ';', 
+        mod list in str format, seperated by ';',
         e.g. Oxidation@M;Phospho@S.
     mod_set : set
         mod set to check
     Returns
     -------
     str
-        original `mod_str` if all modifications are in mod_set 
+        original `mod_str` if all modifications are in mod_set
         else pd.NA.
-    '''
-    if not mod_str: return ""
-    for mod in mod_str.split(';'):
-        if not mod in mod_set:
+    """
+    if not mod_str:
+        return ""
+    for mod in mod_str.split(";"):
+        if mod not in mod_set:
             return pd.NA
     return mod_str
 
+
 #: See `psm_reader.yaml <https://github.com/MannLabs/alphabase/blob/main/alphabase/constants/const_files/psm_reader.yaml>`_
-psm_reader_yaml = load_yaml(
-    os.path.join(
-        CONST_FILE_FOLDER,
-        'psm_reader.yaml'
-    )
-)
+psm_reader_yaml = load_yaml(os.path.join(CONST_FILE_FOLDER, "psm_reader.yaml"))
+
 
 class PSMReaderBase(object):
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        keep_decoy = False,
-        rt_unit:str = 'minute',
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        rt_unit: str = "minute",
         **kwargs,
     ):
-        """The Base class for all PSMReaders. The key of the sub-classes for different 
+        """The Base class for all PSMReaders. The key of the sub-classes for different
         search engine format is to re-define `column_mapping` and `modification_mapping`.
-        
+
         Parameters
         ----------
         column_mapping : dict, optional
             A dict that maps alphabase's columns to other search engine's.
-            The key of the column_mapping is alphabase's column name, and 
+            The key of the column_mapping is alphabase's column name, and
             the value could be the column name or a list of column names
             in other engine's result.
-            If it is None, this dict will be init by 
-            `self._init_column_mapping`. The dict values could be 
+            If it is None, this dict will be init by
+            `self._init_column_mapping`. The dict values could be
             either str or list, for exaplme:
             ```
             columns_mapping = {
             'sequence': 'NakedSequence', #str
             'charge': 'Charge', #str
             'proteins':['Proteins','UniprotIDs'], # list, this reader will automatically detect all of them.
             }
             ```
             Defaults to None.
         modification_mapping : dict, optional
             A dict that maps alphabase's modifications to other engine's.
-            If it is None, this dict will be init by 
-            default modification mapping for each search engine 
-            (see :data:`psm_reader_yaml`). 
-            The dict values can be 
+            If it is None, this dict will be init by
+            default modification mapping for each search engine
+            (see :data:`psm_reader_yaml`).
+            The dict values can be
             either str or list, for exaplme:
             ```
             modification_mapping = {
             'Oxidation@M': 'Oxidation (M)', # str
             'Phospho@S': ['S(Phospho (STY))','S(ph)','pS'], # list, this reader will automatically detect all of them.
             }
             ```
             Defaults to None.
         fdr : float, optional
             FDR level to keep PSMs.
             Defaults to 0.01.
         keep_decoy : bool, optional
             If keep decoy PSMs in self.psm_df.
             Defautls to False.
-        
+
         Attributes
         ----------
         column_mapping : dict
             Dict structure same as column_mapping in Args.
         modification_mapping : dict
             Dict structure same as modification_mapping in Args.
             We must use self.set_modification_mapping(new_mapping) to update it.
         _psm_df : pd.DataFrame
             the PSM DataFrame after loading from search engines.
         psm_df : pd.DataFrame
             the getter of self._psm_df
         keep_fdr : float
-            The only PSMs with FDR<=keep_fdr were returned in self._psm_df. 
+            The only PSMs with FDR<=keep_fdr were returned in self._psm_df.
         keep_decoy : bool
             If keep decoy PSMs in self.psm_df.
         _min_max_rt_norm : bool
-            if True, the 'rt_norm' values in self._psm_df 
+            if True, the 'rt_norm' values in self._psm_df
             will be normalized by rt_norm = (self.psm_df.rt-rt_min)/(rt_max-rt_min).
             It is useful to normalize iRT values as they contain negative values.
             Defaults to False.
         """
 
         self.set_modification_mapping(None)
-        self.add_modification_mapping(
-            modification_mapping
-        )
-        
+        self.add_modification_mapping(modification_mapping)
+
         if column_mapping is not None:
             self.column_mapping = column_mapping
         else:
             self._init_column_mapping()
 
         self._psm_df = pd.DataFrame()
         self.keep_fdr = fdr
         self.keep_decoy = keep_decoy
         self._min_max_rt_norm = False
         self._engine_rt_unit = rt_unit
         self._min_irt_value = -100
         self._max_irt_value = 200
 
     @property
-    def psm_df(self)->pd.DataFrame:
+    def psm_df(self) -> pd.DataFrame:
         return self._psm_df
 
-    def add_modification_mapping(self, modification_mapping:dict):
+    def add_modification_mapping(self, modification_mapping: dict):
         """
         Append additional modification mappings for the search engine.
 
         Parameters
         ----------
         modification_mapping : dict
-            The key of dict is a modification name in AlphaBase format; 
+            The key of dict is a modification name in AlphaBase format;
             the value could be a str or a list, see below
             ```
             add_modification_mapping({
             'Dimethyl@K': ['K(Dimethyl)'], # list
             'Dimethyl@Any N-term': '_(Dimethyl)', # str
             })
             ```
         """
         if (
-            modification_mapping is None or
-            len(modification_mapping) == 0 or
-            not isinstance(modification_mapping,dict)
+            modification_mapping is None
+            or len(modification_mapping) == 0
+            or not isinstance(modification_mapping, dict)
         ):
             return
 
         for key, val in list(modification_mapping.items()):
             if key in self.modification_mapping:
                 if isinstance(val, str):
                     self.modification_mapping[key].append(val)
@@ -217,90 +206,84 @@
                 if isinstance(val, str):
                     self.modification_mapping[key] = [val]
                 else:
                     self.modification_mapping[key] = val
 
         self.set_modification_mapping(self.modification_mapping)
 
-    def set_modification_mapping(self, modification_mapping:dict):
+    def set_modification_mapping(self, modification_mapping: dict):
         if modification_mapping is None:
             self._init_modification_mapping()
         elif isinstance(modification_mapping, str):
             if modification_mapping in psm_reader_yaml:
                 self.modification_mapping = copy.deepcopy(
-                    psm_reader_yaml[
-                        modification_mapping
-                    ]['modification_mapping']
+                    psm_reader_yaml[modification_mapping]["modification_mapping"]
                 )
             else:
                 raise ValueError(
-                    f'Unknown modification mapping: {modification_mapping}'
+                    f"Unknown modification mapping: {modification_mapping}"
                 )
         else:
-            self.modification_mapping = copy.deepcopy(
-                modification_mapping
-            )
+            self.modification_mapping = copy.deepcopy(modification_mapping)
         self._mods_as_lists()
         self._reverse_mod_mapping()
 
     def _init_modification_mapping(self):
         self.modification_mapping = {}
-    
+
     def _mods_as_lists(self):
-        for mod,val in list(self.modification_mapping.items()):
+        for mod, val in list(self.modification_mapping.items()):
             if isinstance(val, str):
                 self.modification_mapping[mod] = [val]
-        
+
     def _reverse_mod_mapping(self):
         self.rev_mod_mapping = {}
-        for (
-            this_mod, other_mod
-        ) in self.modification_mapping.items():
+        for this_mod, other_mod in self.modification_mapping.items():
             if isinstance(other_mod, (list, tuple)):
                 for _mod in other_mod:
                     if _mod in self.rev_mod_mapping:
-                        if this_mod.endswith('Protein N-term'):
+                        if this_mod.endswith("Protein N-term"):
                             continue
                     self.rev_mod_mapping[_mod] = this_mod
             else:
                 self.rev_mod_mapping[other_mod] = this_mod
-                
+
     def _init_column_mapping(self):
         raise NotImplementedError(
             f'"{self.__class__}" must implement "_init_column_mapping()"'
         )
-    
-    def load(self, _file)->pd.DataFrame:
-        """ Wrapper for import_file() """
-        if isinstance(_file, list): 
+
+    def load(self, _file) -> pd.DataFrame:
+        """Wrapper for import_file()"""
+        if isinstance(_file, list):
             return self.import_files(_file)
-        else: 
+        else:
             return self.import_file(_file)
 
-    def import_files(self, file_list:list):
+    def import_files(self, file_list: list):
         df_list = []
         for _file in file_list:
             df_list.append(self.import_file(_file))
         self._psm_df = pd.concat(df_list, ignore_index=True)
         return self._psm_df
 
-    def import_file(self, _file:str)->pd.DataFrame:
+    def import_file(self, _file: str) -> pd.DataFrame:
         """
-        This is the main entry function of PSM readers, 
+        This is the main entry function of PSM readers,
         it imports the file with following steps:
         ```
         origin_df = self._load_file(_file)
         self._translate_columns(origin_df)
         self._translate_decoy(origin_df)
         self._translate_score(origin_df)
         self._load_modifications(origin_df)
         self._translate_modifications()
         self._post_process(origin_df)
         ```
-        
+
         Parameters
         ----------
         _file: str
             file path or file stream (io).
         """
         origin_df = self._load_file(_file)
         if len(origin_df) == 0:
@@ -311,74 +294,68 @@
             self._translate_decoy(origin_df)
             self._translate_score(origin_df)
             self._load_modifications(origin_df)
             self._translate_modifications()
             self._post_process(origin_df)
         return self._psm_df
 
-    def _translate_decoy(
-        self, 
-        origin_df:pd.DataFrame=None
-    ):
+    def _translate_decoy(self, origin_df: pd.DataFrame = None):
         pass
 
-    def _translate_score(
-        self, 
-        origin_df:pd.DataFrame=None
-    ):
+    def _translate_score(self, origin_df: pd.DataFrame = None):
         # some scores are evalue/pvalue, it should be translated
         # to -log(evalue), as score is the larger the better
         pass
 
     def _get_table_delimiter(self, _filename):
         return get_delimiter(_filename)
 
     def normalize_rt(self):
-        if 'rt' in self.psm_df.columns:
-            if self._engine_rt_unit == 'second':
+        if "rt" in self.psm_df.columns:
+            if self._engine_rt_unit == "second":
                 # self.psm_df['rt_sec'] = self.psm_df.rt
-                self.psm_df['rt'] = self.psm_df.rt/60
+                self.psm_df["rt"] = self.psm_df.rt / 60
                 if "rt_start" in self.psm_df.columns:
-                    self.psm_df["rt_start"] = self.psm_df.rt_start/60
-                    self.psm_df["rt_stop"] = self.psm_df.rt_stop/60
+                    self.psm_df["rt_start"] = self.psm_df.rt_start / 60
+                    self.psm_df["rt_stop"] = self.psm_df.rt_stop / 60
             # elif self._engine_rt_unit == 'minute':
-                # self.psm_df['rt_sec'] = self.psm_df.rt*60
+            # self.psm_df['rt_sec'] = self.psm_df.rt*60
             min_rt = self.psm_df.rt.min()
             max_rt = self.psm_df.rt.max()
-            if min_rt < 0: # iRT
+            if min_rt < 0:  # iRT
                 if min_rt < self._min_irt_value:
                     min_rt = self._min_irt_value
                 if max_rt > self._max_irt_value:
                     max_rt = self._max_irt_value
 
-            elif not self._min_max_rt_norm :
+            elif not self._min_max_rt_norm:
                 min_rt = 0
-            
-            self.psm_df['rt_norm'] = ((
-                self.psm_df.rt - min_rt
-            ) / (max_rt-min_rt)).clip(0, 1)
+
+            self.psm_df["rt_norm"] = (
+                (self.psm_df.rt - min_rt) / (max_rt - min_rt)
+            ).clip(0, 1)
 
     def norm_rt(self):
         self.normalize_rt()
 
     def normalize_rt_by_raw_name(self):
-        if not 'rt' in self.psm_df.columns:
+        if "rt" not in self.psm_df.columns:
             return
-        if not 'rt_norm' in self.psm_df.columns:
+        if "rt_norm" not in self.psm_df.columns:
             self.norm_rt()
-        if not 'raw_name' in self.psm_df.columns:
+        if "raw_name" not in self.psm_df.columns:
             return
-        for raw_name, df_group in self.psm_df.groupby('raw_name'):
-            self.psm_df.loc[
-                df_group.index,'rt_norm'
-            ] = df_group.rt_norm / df_group.rt_norm.max()
+        for raw_name, df_group in self.psm_df.groupby("raw_name"):
+            self.psm_df.loc[df_group.index, "rt_norm"] = (
+                df_group.rt_norm / df_group.rt_norm.max()
+            )
 
-    def _load_file(self, filename:str)->pd.DataFrame:
+    def _load_file(self, filename: str) -> pd.DataFrame:
         """
-        Load original dataframe from PSM filename. 
+        Load original dataframe from PSM filename.
         Different search engines may store PSMs in different ways:
         tsv, csv, HDF, XML, ...
 
         Parameters
         ----------
         filename : str
             psm filename
@@ -388,34 +365,32 @@
         NotImplementedError
             Subclasses must re-implement this method
 
         Returns:
         pd.DataFrame
             loaded dataframe
         """
-        raise NotImplementedError(
-            f'"{self.__class__}" must implement "_load_file()"'
-        )
+        raise NotImplementedError(f'"{self.__class__}" must implement "_load_file()"')
 
-    def _find_mapped_columns(self, origin_df:pd.DataFrame):
+    def _find_mapped_columns(self, origin_df: pd.DataFrame):
         mapped_columns = {}
         for col, map_col in self.column_mapping.items():
             if isinstance(map_col, str):
                 if map_col in origin_df.columns:
                     mapped_columns[col] = map_col
-            elif isinstance(map_col, (list,tuple)):
+            elif isinstance(map_col, (list, tuple)):
                 for other_col in map_col:
                     if other_col in origin_df.columns:
                         mapped_columns[col] = other_col
                         break
         return mapped_columns
 
-    def _translate_columns(self, origin_df:pd.DataFrame):
+    def _translate_columns(self, origin_df: pd.DataFrame):
         """
-        Translate the dataframe from other search engines 
+        Translate the dataframe from other search engines
         to AlphaBase format
 
         Parameters
         ----------
         origin_df : pd.DataFrame
             df of other search engines
 
@@ -424,22 +399,22 @@
         None
             Add information inplace into self._psm_df
         """
         mapped_columns = self._find_mapped_columns(origin_df)
         self._psm_df = pd.DataFrame()
         for col, map_col in mapped_columns.items():
             self._psm_df[col] = origin_df[map_col]
-               
+
         if (
-            'scan_num' in self._psm_df.columns and 
-            not 'spec_idx' in self._psm_df.columns
+            "scan_num" in self._psm_df.columns
+            and "spec_idx" not in self._psm_df.columns
         ):
-            self._psm_df['spec_idx'] = self._psm_df.scan_num - 1
-    
-    def _transform_table(self, origin_df:pd.DataFrame):
+            self._psm_df["spec_idx"] = self._psm_df.scan_num - 1
+
+    def _transform_table(self, origin_df: pd.DataFrame):
         """
         Transform the dataframe format if needed.
         Usually only needed in combination with spectral libraries.
 
         Parameters
         ----------
         origin_df : pd.DataFrame
@@ -448,158 +423,147 @@
         Returns
         -------
         None
             Add information inplace into self._psm_df
         """
         pass
 
-    def _load_modifications(self, origin_df:pd.DataFrame):
-        """Read modification information from 'origin_df'. 
+    def _load_modifications(self, origin_df: pd.DataFrame):
+        """Read modification information from 'origin_df'.
         Some of search engines use modified_sequence, some of them
         use additional columns to store modifications and the sites.
 
         Parameters
         ----------
         origin_df : pd.DataFrame
             dataframe of original search engine.
         """
         raise NotImplementedError(
             f'"{self.__class__}" must implement "_load_modifications()"'
         )
 
     def _translate_modifications(self):
-        '''
+        """
         Translate modifications to AlphaBase format.
 
         Raises
         ------
         KeyError
-            if `mod` in `mod_names` is 
+            if `mod` in `mod_names` is
             not in `self.modification_mapping`
-        '''
+        """
 
-        self._psm_df.mods, unknown_mods = zip(*self._psm_df.mods.apply(
-            translate_other_modification, 
-            mod_dict=self.rev_mod_mapping
-        ))
+        self._psm_df.mods, unknown_mods = zip(
+            *self._psm_df.mods.apply(
+                translate_other_modification, mod_dict=self.rev_mod_mapping
+            )
+        )
 
         # accumulate unknown mods
         unknwon_mod_set = set()
         for mod_list in unknown_mods:
             if len(mod_list) > 0:
                 unknwon_mod_set.update(mod_list)
 
         if len(unknwon_mod_set) > 0:
             warnings.warn(
-                f'Unknown modifications: {unknwon_mod_set}. Precursors with unknown modifications will be removed.'
+                f"Unknown modifications: {unknwon_mod_set}. Precursors with unknown modifications will be removed."
             )
 
-
-    def _post_process(self, 
-        origin_df:pd.DataFrame
-    ):
+    def _post_process(self, origin_df: pd.DataFrame):
         """
-        Set 'nAA' columns, remove unknown modifications 
-        and perform other post processings, 
+        Set 'nAA' columns, remove unknown modifications
+        and perform other post processings,
         e.g. get 'rt_norm', remove decoys, filter FDR...
 
         Parameters
         ----------
         origin_df : pd.DataFrame
             the loaded original df
         """
-        self._psm_df['nAA'] = self._psm_df.sequence.str.len()
+        self._psm_df["nAA"] = self._psm_df.sequence.str.len()
 
         self.normalize_rt_by_raw_name()
 
-        self._psm_df = self._psm_df[
-            ~self._psm_df['mods'].isna()
-        ]
+        self._psm_df = self._psm_df[~self._psm_df["mods"].isna()]
 
-        keep_rows = np.ones(
-            len(self._psm_df), dtype=bool
-        )
-        if 'fdr' in self._psm_df.columns:
-            keep_rows &= (self._psm_df.fdr <= self.keep_fdr)
-        if (
-            'decoy' in self._psm_df.columns 
-            and not self.keep_decoy
-        ):
-            keep_rows &= (self._psm_df.decoy == 0)
+        keep_rows = np.ones(len(self._psm_df), dtype=bool)
+        if "fdr" in self._psm_df.columns:
+            keep_rows &= self._psm_df.fdr <= self.keep_fdr
+        if "decoy" in self._psm_df.columns and not self.keep_decoy:
+            keep_rows &= self._psm_df.decoy == 0
 
         self._psm_df = self._psm_df[keep_rows]
-        
+
         reset_precursor_df(self._psm_df)
-        
-        if 'precursor_mz' not in self._psm_df:
+
+        if "precursor_mz" not in self._psm_df:
             self._psm_df = update_precursor_mz(self._psm_df)
 
-        if (
-            'ccs' in self._psm_df.columns and 
-            'mobility' not in self._psm_df.columns
-        ):
-            self._psm_df['mobility'] = (
-                mobility.ccs_to_mobility_for_df(
-                    self._psm_df,
-                    'ccs'
-                )
+        if "ccs" in self._psm_df.columns and "mobility" not in self._psm_df.columns:
+            self._psm_df["mobility"] = mobility.ccs_to_mobility_for_df(
+                self._psm_df, "ccs"
             )
-        elif (
-            'mobility' in self._psm_df.columns and
-            'ccs' not in self._psm_df.columns
-        ):
-            self._psm_df['ccs'] = (
-                mobility.mobility_to_ccs_for_df(
-                    self._psm_df,
-                    'mobility'
-                )
+        elif "mobility" in self._psm_df.columns and "ccs" not in self._psm_df.columns:
+            self._psm_df["ccs"] = mobility.mobility_to_ccs_for_df(
+                self._psm_df, "mobility"
             )
 
-    def filter_psm_by_modifications(self, include_mod_set = set([
-        'Oxidation@M','Phospho@S','Phospho@T',
-        'Phospho@Y','Acetyl@Protein N-term'
-    ])):
-        '''
-            Only keeps peptides with modifications in `include_mod_list`.
-        '''
+    def filter_psm_by_modifications(
+        self,
+        include_mod_set=set(
+            [
+                "Oxidation@M",
+                "Phospho@S",
+                "Phospho@T",
+                "Phospho@Y",
+                "Acetyl@Protein N-term",
+            ]
+        ),
+    ):
+        """
+        Only keeps peptides with modifications in `include_mod_list`.
+        """
         self._psm_df.mods = self._psm_df.mods.apply(
             keep_modifications, mod_set=include_mod_set
         )
-        
-        self._psm_df.dropna(
-            subset=['mods'], inplace=True
-        )
+
+        self._psm_df.dropna(subset=["mods"], inplace=True)
         self._psm_df.reset_index(drop=True, inplace=True)
 
 
 class PSMReaderProvider:
     def __init__(self):
         self.reader_dict = {}
 
     def register_reader(self, reader_type, reader_class):
         self.reader_dict[reader_type.lower()] = reader_class
 
-    def get_reader(self, 
-        reader_type:str,
+    def get_reader(
+        self,
+        reader_type: str,
         *,
-        column_mapping:dict=None, 
-        modification_mapping:dict=None,
-        fdr=0.01, keep_decoy=False,
-        **kwargs
-    )->PSMReaderBase:
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        keep_decoy=False,
+        **kwargs,
+    ) -> PSMReaderBase:
         return self.reader_dict[reader_type.lower()](
-            column_mapping = column_mapping,
+            column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr=fdr, keep_decoy=keep_decoy, **kwargs
+            fdr=fdr,
+            keep_decoy=keep_decoy,
+            **kwargs,
         )
 
-    def get_reader_by_yaml(self, 
-        yaml_dict:dict,
-    )->PSMReaderBase:
-        return self.get_reader(
-            **copy.deepcopy(yaml_dict)
-        )
+    def get_reader_by_yaml(
+        self,
+        yaml_dict: dict,
+    ) -> PSMReaderBase:
+        return self.get_reader(**copy.deepcopy(yaml_dict))
+
 
 psm_reader_provider = PSMReaderProvider()
 """
 A factory :class:`PSMReaderProvider` object to register and get readers for different PSM types.
 """
```

### Comparing `alphabase-1.2.3/alphabase/psm_reader/sage_reader.py` & `alphabase-1.2.4/alphabase/psm_reader/sage_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import numpy as np
 import pandas as pd
 import typing
 import re
 from functools import partial
 
 from alphabase.psm_reader.psm_reader import (
-    PSMReaderBase, psm_reader_provider,
-    psm_reader_yaml
+    PSMReaderBase,
+    psm_reader_provider,
+    psm_reader_yaml,
 )
 
 from alphabase.constants.modification import MOD_DF
 
+
 def sage_spec_idx_from_scannr(scannr: str) -> int:
     """Extract the spectrum index from the scannr field in Sage output.
 
     Parameters
     ----------
 
     scannr : str
         The scannr field in Sage output.
-    
+
     """
-    return int(scannr.split('=')[-1])
+    return int(scannr.split("=")[-1])
+
 
 def lookup_modification(
-        mass_observed: float, 
-        previous_aa: str, 
-        mod_annotated_df: pd.DataFrame, 
-        ppm_tolerance:int=10,
-    ) -> str:
+    mass_observed: float,
+    previous_aa: str,
+    mod_annotated_df: pd.DataFrame,
+    ppm_tolerance: int = 10,
+) -> str:
     """
     Look up a single modification based on the observed mass and the previous amino acid.
 
     Parameters
     ----------
 
     mass_observed : float
@@ -48,43 +51,41 @@
         The ppm tolerance for matching the observed mass to the annotated modification mass.
 
     Returns
     -------
 
     str
         The name of the matched modification in alphabase format.
-    
+
     """
 
-    mass_distance = mod_annotated_df['mass'].values - mass_observed
+    mass_distance = mod_annotated_df["mass"].values - mass_observed
     ppm_distance = mass_distance / mass_observed * 1e6
     ppm_distance = np.abs(ppm_distance)
 
     ppm_tolerance = min(np.min(ppm_distance), ppm_tolerance)
 
     # get index of matches
     mass_match = ppm_distance <= ppm_tolerance
-    sequence_match = mod_annotated_df['location'] == previous_aa
-
+    sequence_match = mod_annotated_df["location"] == previous_aa
 
     filtered_mod_df = mod_annotated_df[mass_match & sequence_match]
     if len(filtered_mod_df) == 0:
         print(np.min(ppm_distance))
         return None
 
-    matched_mod = filtered_mod_df.sort_values(by='unimod_id').iloc[0]
-    
-    return matched_mod['mod_name']
+    matched_mod = filtered_mod_df.sort_values(by="unimod_id").iloc[0]
+
+    return matched_mod["mod_name"]
+
 
 def capture_modifications(
-        sequence: str,
-        mod_annotated_df: pd.DataFrame,
-        ppm_tolerance: int=10
-    ) -> typing.Tuple[str, str]:
-    """ Capture modifications from a sequence string.
+    sequence: str, mod_annotated_df: pd.DataFrame, ppm_tolerance: int = 10
+) -> typing.Tuple[str, str]:
+    """Capture modifications from a sequence string.
 
     Parameters
     ----------
 
     sequence : str
         The modified sequence string.
 
@@ -99,125 +100,137 @@
 
     typing.Tuple[str, str]
         A tuple of two strings, the first string is the list of modification sites, and the second string is the list of modifications.
 
     """
 
     # get index of matches
-    matches = re.finditer(r'\[(\+|-)(\d+\.\d+)\]', sequence)
+    matches = re.finditer(r"\[(\+|-)(\d+\.\d+)\]", sequence)
 
     site_list = []
     mod_list = []
 
     error = False
 
     match_delta = 0
 
     for match in matches:
         match_start, match_end = match.start(), match.end()
-        previous_aa = sequence[match_start-1] if match_start > 0 else 'Any_N-term'
-        mass_observed = float(match.group(2)) * (1 if match.group(1) == '+' else -1)
+        previous_aa = sequence[match_start - 1] if match_start > 0 else "Any_N-term"
+        mass_observed = float(match.group(2)) * (1 if match.group(1) == "+" else -1)
 
-        mod = lookup_modification(mass_observed, previous_aa, mod_annotated_df, ppm_tolerance=ppm_tolerance)
+        mod = lookup_modification(
+            mass_observed, previous_aa, mod_annotated_df, ppm_tolerance=ppm_tolerance
+        )
         if mod is not None:
-            site_list.append(str(match_start-1-match_delta))
+            site_list.append(str(match_start - 1 - match_delta))
             mod_list.append(mod)
-        
+
         else:
             error = True
-            print(f'No modification found for mass {mass_observed} at position {match_start} with previous aa {previous_aa}')
+            print(
+                f"No modification found for mass {mass_observed} at position {match_start} with previous aa {previous_aa}"
+            )
 
-        match_delta += (match_end - match_start)
+        match_delta += match_end - match_start
 
     if error:
         return np.nan, np.nan
     else:
-        return ';'.join(site_list), ';'.join(mod_list)
-    
+        return ";".join(site_list), ";".join(mod_list)
+
+
 def get_annotated_mod_df():
-    """ Annotates the modification dataframe with the location of the modification."""
+    """Annotates the modification dataframe with the location of the modification."""
     mod_annotated_df = MOD_DF.copy()
-    mod_annotated_df['location'] = mod_annotated_df['mod_name'].str.split('@').str[1].str.split('^').str[0]
-    mod_annotated_df = mod_annotated_df.sort_values(by='mass').reset_index(drop=True)
-    mod_annotated_df['mod_name_stripped'] = mod_annotated_df['mod_name'].str.replace(' ','_')
+    mod_annotated_df["location"] = (
+        mod_annotated_df["mod_name"].str.split("@").str[1].str.split("^").str[0]
+    )
+    mod_annotated_df = mod_annotated_df.sort_values(by="mass").reset_index(drop=True)
+    mod_annotated_df["mod_name_stripped"] = mod_annotated_df["mod_name"].str.replace(
+        " ", "_"
+    )
     return mod_annotated_df
 
+
 class SageReaderBase(PSMReaderBase):
-    def __init__(self, *, 
-        column_mapping: dict = None, 
+    def __init__(
+        self,
+        *,
+        column_mapping: dict = None,
         modification_mapping: dict = None,
-        fdr = 0.01,
-        keep_decoy=False, 
-        rt_unit = 'second',
-        **kwargs
+        fdr=0.01,
+        keep_decoy=False,
+        rt_unit="second",
+        **kwargs,
     ):
         super().__init__(
-            column_mapping=column_mapping, 
+            column_mapping=column_mapping,
             modification_mapping=modification_mapping,
-            fdr = fdr,
-            keep_decoy=keep_decoy, 
-            rt_unit = rt_unit,
-            **kwargs
+            fdr=fdr,
+            keep_decoy=keep_decoy,
+            rt_unit=rt_unit,
+            **kwargs,
         )
 
     def _init_column_mapping(self):
-        self.column_mapping = psm_reader_yaml[
-            'sage'
-        ]['column_mapping']
-        
+        self.column_mapping = psm_reader_yaml["sage"]["column_mapping"]
+
     def _init_modification_mapping(self):
         self.modification_mapping = {}
 
     def _load_file(self, filename):
         raise NotImplementedError
 
     def _transform_table(self, origin_df):
-        self.psm_df['spec_idx'] = self.psm_df['scannr'].apply(
-                sage_spec_idx_from_scannr
-        )
-        self.psm_df.drop(columns=['scannr'], inplace=True)
+        self.psm_df["spec_idx"] = self.psm_df["scannr"].apply(sage_spec_idx_from_scannr)
+        self.psm_df.drop(columns=["scannr"], inplace=True)
 
     def _translate_decoy(self, origin_df):
         if not self.keep_decoy:
-            self._psm_df = self.psm_df[
-                ~self.psm_df['decoy']
-            ]
-
-        self._psm_df = self.psm_df[self.psm_df['fdr'] <= self.keep_fdr]
-        self._psm_df = self.psm_df[self.psm_df['peptide_fdr'] <= self.keep_fdr]
-        self._psm_df = self.psm_df[self.psm_df['protein_fdr'] <= self.keep_fdr]
+            self._psm_df = self.psm_df[~self.psm_df["decoy"]]
+
+        self._psm_df = self.psm_df[self.psm_df["fdr"] <= self.keep_fdr]
+        self._psm_df = self.psm_df[self.psm_df["peptide_fdr"] <= self.keep_fdr]
+        self._psm_df = self.psm_df[self.psm_df["protein_fdr"] <= self.keep_fdr]
 
         # drop peptide_fdr, protein_fdr
-        self._psm_df.drop(columns=['peptide_fdr', 'protein_fdr'], inplace=True)
+        self._psm_df.drop(columns=["peptide_fdr", "protein_fdr"], inplace=True)
 
     def _load_modifications(self, origin_df):
         pass
 
     def _translate_modifications(self):
-
         mod_annotated_df = get_annotated_mod_df()
 
-        self._psm_df['mod_sites'], self._psm_df['mods'] = zip(*self.psm_df['modified_sequence'].apply(
-            partial(
-                capture_modifications, mod_annotated_df=mod_annotated_df, ppm_tolerance=10
+        self._psm_df["mod_sites"], self._psm_df["mods"] = zip(
+            *self.psm_df["modified_sequence"].apply(
+                partial(
+                    capture_modifications,
+                    mod_annotated_df=mod_annotated_df,
+                    ppm_tolerance=10,
                 )
-            ))
+            )
+        )
         # drop modified_sequence
-        self._psm_df.drop(columns=['modified_sequence'], inplace=True)
+        self._psm_df.drop(columns=["modified_sequence"], inplace=True)
+
 
 class SageReaderTSV(SageReaderBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _load_file(self, filename):
-        return pd.read_csv(filename, sep='\t')
-    
+        return pd.read_csv(filename, sep="\t")
+
+
 class SageReaderParquet(SageReaderBase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _load_file(self, filename):
         return pd.read_parquet(filename)
 
 
-psm_reader_provider.register_reader('sage_tsv', SageReaderTSV)
-psm_reader_provider.register_reader('sage_parquet', SageReaderParquet)
+def register_readers():
+    psm_reader_provider.register_reader("sage_tsv", SageReaderTSV)
+    psm_reader_provider.register_reader("sage_parquet", SageReaderParquet)
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/config_dict_loader.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/config_dict_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,107 +2,126 @@
 import yaml
 import pandas as pd
 import os.path
 import pathlib
 import itertools
 import re
 
-INTABLE_CONFIG = os.path.join(pathlib.Path(__file__).parent.absolute(), "../../../alphabase/constants/const_files/quant_reader_config.yaml") #the yaml config is located one directory below the python library files
+INTABLE_CONFIG = os.path.join(
+    pathlib.Path(__file__).parent.absolute(),
+    "../../../alphabase/constants/const_files/quant_reader_config.yaml",
+)  # the yaml config is located one directory below the python library files
 
-def get_input_type_and_config_dict(input_file, input_type_to_use = None):
+
+def get_input_type_and_config_dict(input_file, input_type_to_use=None):
     all_config_dicts = _load_config(INTABLE_CONFIG)
     type2relevant_columns = _get_type2relevant_cols(all_config_dicts)
 
     if "aq_reformat.tsv" in input_file:
         input_file = _get_original_file_from_aq_reformat(input_file)
 
     sep = _get_seperator(input_file)
 
     uploaded_data_columns = set(pd.read_csv(input_file, sep=sep, nrows=1).columns)
 
     for input_type in type2relevant_columns.keys():
-        if (input_type_to_use is not None) and (input_type!=input_type_to_use):
+        if (input_type_to_use is not None) and (input_type != input_type_to_use):
             continue
         relevant_columns = type2relevant_columns.get(input_type)
-        relevant_columns = [x for x in relevant_columns if x] #filter None values
+        relevant_columns = [x for x in relevant_columns if x]  # filter None values
         if set(relevant_columns).issubset(uploaded_data_columns):
-            config_dict =  all_config_dicts.get(input_type)
+            config_dict = all_config_dicts.get(input_type)
             return input_type, config_dict, sep
-    
+
     raise TypeError("format not specified in intable_config.yaml!")
 
+
 def _get_original_file_from_aq_reformat(input_file):
-    matched = re.match("(.*)(\..*\.)(aq_reformat\.tsv)",input_file)
+    matched = re.match("(.*)(\..*\.)(aq_reformat\.tsv)", input_file)
     return matched.group(1)
 
+
 def _get_seperator(input_file):
     filename = str(input_file)
-    if '.csv' in filename:
-        sep=','
-    if '.tsv' in filename:
-        sep='\t'
-    if '.txt' in filename:
-        sep='\t'
-
-    if 'sep' not in locals():
-        raise TypeError(f"neither of the file extensions (.tsv, .csv, .txt) detected for file {input_file}! Your filename has to contain one of these extensions. Please modify your file name accordingly.")
+    if ".csv" in filename:
+        sep = ","
+    if ".tsv" in filename:
+        sep = "\t"
+    if ".txt" in filename:
+        sep = "\t"
+
+    if "sep" not in locals():
+        raise TypeError(
+            f"neither of the file extensions (.tsv, .csv, .txt) detected for file {input_file}! Your filename has to contain one of these extensions. Please modify your file name accordingly."
+        )
     return sep
 
 
-
 def _load_config(config_yaml):
-    with open(config_yaml, 'r') as stream:
+    with open(config_yaml, "r") as stream:
         config_all = yaml.safe_load(stream)
     return config_all
 
+
 def _get_type2relevant_cols(config_all):
     type2relcols = {}
     for type in config_all.keys():
         config_typedict = config_all.get(type)
         relevant_cols = get_relevant_columns_config_dict(config_typedict)
         type2relcols[type] = relevant_cols
     return type2relcols
 
 
 def get_relevant_columns_config_dict(config_typedict):
     filtcols = []
     dict_ioncols = []
-    for filtconf in config_typedict.get('filters', {}).values():
-        filtcols.append(filtconf.get('param'))
+    for filtconf in config_typedict.get("filters", {}).values():
+        filtcols.append(filtconf.get("param"))
 
-    if 'ion_hierarchy' in config_typedict.keys():
-        for headr in config_typedict.get('ion_hierarchy').values():
+    if "ion_hierarchy" in config_typedict.keys():
+        for headr in config_typedict.get("ion_hierarchy").values():
             ioncols = list(itertools.chain.from_iterable(headr.get("mapping").values()))
             dict_ioncols.extend(ioncols)
 
     quant_ids = _get_quant_ids_from_config_dict(config_typedict)
     sample_ids = _get_sample_ids_from_config_dict(config_typedict)
     channel_ids = _get_channel_ids_from_config_dict(config_typedict)
-    relevant_cols = config_typedict.get("protein_cols") + config_typedict.get("ion_cols", []) + sample_ids + quant_ids + filtcols + dict_ioncols + channel_ids
-    relevant_cols = list(set(relevant_cols)) # to remove possible redudancies
+    relevant_cols = (
+        config_typedict.get("protein_cols")
+        + config_typedict.get("ion_cols", [])
+        + sample_ids
+        + quant_ids
+        + filtcols
+        + dict_ioncols
+        + channel_ids
+    )
+    relevant_cols = list(set(relevant_cols))  # to remove possible redudancies
     return relevant_cols
 
+
 def _get_quant_ids_from_config_dict(config_typedict):
     quantID = config_typedict.get("quant_ID")
-    if type(quantID) ==type("string"):
+    if isinstance(quantID, str):
         return [config_typedict.get("quant_ID")]
-    if quantID == None:
-        return[]
+    if quantID is None:
+        return []
     else:
         return list(config_typedict.get("quant_ID").values())
 
+
 def _get_sample_ids_from_config_dict(config_typedict):
     sampleID = config_typedict.get("sample_ID")
-    if type(sampleID) ==type("string"):
+    if isinstance(sampleID, str):
         return [config_typedict.get("sample_ID")]
-    if sampleID == None:
+    if sampleID is None:
         return []
     else:
         return config_typedict.get("sample_ID")
 
+
 def _get_channel_ids_from_config_dict(config_typedict):
     return config_typedict.get("channel_ID", [])
 
 
 def import_config_dict():
     config_dict = _load_config(INTABLE_CONFIG)
     return config_dict
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/longformat_reader.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/longformat_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,171 +1,253 @@
 import pandas as pd
 import os
 import shutil
 import glob
 import dask.dataframe as dd
 import os.path
-import sys
 
 from . import config_dict_loader
 from . import quantreader_utils
 from . import table_reformatter
 from . import plexdia_reformatter
 
 
-
-
-def reformat_and_write_longtable_according_to_config(input_file, outfile_name, config_dict_for_type, sep = "\t",decimal = ".", enforce_largefile_processing = False, 
-                                                     chunksize =1000_000, use_alphaquant_format = False):
+def reformat_and_write_longtable_according_to_config(
+    input_file,
+    outfile_name,
+    config_dict_for_type,
+    sep="\t",
+    decimal=".",
+    enforce_largefile_processing=False,
+    chunksize=1000_000,
+    use_alphaquant_format=False,
+):
     """Reshape a long format proteomics results table (e.g. Spectronaut or DIA-NN) to a wide format table.
     :param file input_file: long format proteomic results table
     :param string input_type: the configuration key stored in the config file (e.g. "diann_precursor")
     """
 
-
     file_is_large = check_if_file_is_large(input_file, enforce_largefile_processing)
 
     if file_is_large:
-        process_out_of_memory(input_file=input_file, outfile_name=outfile_name, config_dict_for_type=config_dict_for_type, sep=sep, decimal=decimal,
-                              chunksize=chunksize, use_alphaquant_format=use_alphaquant_format)
+        process_out_of_memory(
+            input_file=input_file,
+            outfile_name=outfile_name,
+            config_dict_for_type=config_dict_for_type,
+            sep=sep,
+            decimal=decimal,
+            chunksize=chunksize,
+            use_alphaquant_format=use_alphaquant_format,
+        )
     else:
-        process_in_memory(input_file=input_file, outfile_name=outfile_name, config_dict_for_type=config_dict_for_type, sep=sep, decimal=decimal,
-                              chunksize=chunksize, use_alphaquant_format=use_alphaquant_format)
+        process_in_memory(
+            input_file=input_file,
+            outfile_name=outfile_name,
+            config_dict_for_type=config_dict_for_type,
+            sep=sep,
+            decimal=decimal,
+            chunksize=chunksize,
+            use_alphaquant_format=use_alphaquant_format,
+        )
 
 
 def check_if_file_is_large(input_file, enforce_largefile_processing):
-    filesize = os.path.getsize(input_file)/(1024**3) #size in gigabyte
-    file_is_large = (filesize>10 and str(input_file).endswith(".zip")) or filesize>50 or enforce_largefile_processing
+    filesize = os.path.getsize(input_file) / (1024**3)  # size in gigabyte
+    file_is_large = (
+        (filesize > 10 and str(input_file).endswith(".zip"))
+        or filesize > 50
+        or enforce_largefile_processing
+    )
     return file_is_large
 
-        
-
-def process_out_of_memory(input_file, outfile_name, config_dict_for_type, sep = "\t",decimal = ".", 
-                                                     chunksize =1000_000, use_alphaquant_format = False):
 
+def process_out_of_memory(
+    input_file,
+    outfile_name,
+    config_dict_for_type,
+    sep="\t",
+    decimal=".",
+    chunksize=1000_000,
+    use_alphaquant_format=False,
+):
     tmpfile_large = get_tmpfile_location(input_file)
     remove_possible_old_tmpfiles(tmpfile_large=tmpfile_large, outfile_name=outfile_name)
-    
-    relevant_cols = config_dict_loader.get_relevant_columns_config_dict(config_dict_for_type)
-    input_df_it = pd.read_csv(input_file, sep = sep, decimal=decimal, usecols = relevant_cols, encoding ='latin1', chunksize = chunksize)
+
+    relevant_cols = config_dict_loader.get_relevant_columns_config_dict(
+        config_dict_for_type
+    )
+    input_df_it = pd.read_csv(
+        input_file,
+        sep=sep,
+        decimal=decimal,
+        usecols=relevant_cols,
+        encoding="latin1",
+        chunksize=chunksize,
+    )
     header = True
-    
+
     for input_df_subset in input_df_it:
-        input_df_subset = adapt_subtable(input_df_subset, config_dict_for_type, use_alphaquant_format)
-        write_chunk_to_file(input_df_subset,tmpfile_large, header, write_index=True)
+        input_df_subset = adapt_subtable(
+            input_df_subset, config_dict_for_type, use_alphaquant_format
+        )
+        write_chunk_to_file(input_df_subset, tmpfile_large, header, write_index=True)
         header = False
 
-    process_with_dask(tmpfile_columnfilt=tmpfile_large , outfile_name = outfile_name, config_dict_for_type=config_dict_for_type, use_alphaquant_format=use_alphaquant_format)
+    process_with_dask(
+        tmpfile_columnfilt=tmpfile_large,
+        outfile_name=outfile_name,
+        config_dict_for_type=config_dict_for_type,
+        use_alphaquant_format=use_alphaquant_format,
+    )
+
 
 def get_tmpfile_location(input_file):
-    return f"{input_file}.tmp.longformat.columnfilt.tsv" #only needed when file is large
+    return (
+        f"{input_file}.tmp.longformat.columnfilt.tsv"  # only needed when file is large
+    )
+
 
 def remove_possible_old_tmpfiles(tmpfile_large, outfile_name):
-    #remove potential leftovers from previous processings
+    # remove potential leftovers from previous processings
     if os.path.exists(tmpfile_large):
         os.remove(tmpfile_large)
     if os.path.exists(outfile_name):
         os.remove(outfile_name)
 
 
-def process_in_memory(input_file, outfile_name, config_dict_for_type, sep = "\t",decimal = ".",
-                                                     chunksize =1000_000, use_alphaquant_format = False):
-
-    relevant_cols = config_dict_loader.get_relevant_columns_config_dict(config_dict_for_type)
-    input_df_it = pd.read_csv(input_file, sep = sep, decimal=decimal, usecols = relevant_cols, encoding ='latin1', chunksize = chunksize)
+def process_in_memory(
+    input_file,
+    outfile_name,
+    config_dict_for_type,
+    sep="\t",
+    decimal=".",
+    chunksize=1000_000,
+    use_alphaquant_format=False,
+):
+    relevant_cols = config_dict_loader.get_relevant_columns_config_dict(
+        config_dict_for_type
+    )
+    input_df_it = pd.read_csv(
+        input_file,
+        sep=sep,
+        decimal=decimal,
+        usecols=relevant_cols,
+        encoding="latin1",
+        chunksize=chunksize,
+    )
     input_df_list = []
     for input_df_subset in input_df_it:
-        input_df_subset = adapt_subtable(input_df_subset, config_dict_for_type, use_alphaquant_format)
+        input_df_subset = adapt_subtable(
+            input_df_subset, config_dict_for_type, use_alphaquant_format
+        )
         input_df_list.append(input_df_subset)
 
     input_df = pd.concat(input_df_list)
     input_reshaped = reshape_input_df(input_df, config_dict_for_type)
-    input_reshaped.to_csv(outfile_name, sep = "\t", index = None)
+    input_reshaped.to_csv(outfile_name, sep="\t", index=None)
 
 
 def adapt_subtable(input_df_subset, config_dict, use_alphaquant_format):
-    input_df_subset = quantreader_utils.filter_input(config_dict.get("filters", {}), input_df_subset)
+    input_df_subset = quantreader_utils.filter_input(
+        config_dict.get("filters", {}), input_df_subset
+    )
     if "ion_hierarchy" in config_dict.keys():
-        return table_reformatter.merge_protein_cols_and_config_dict(input_df_subset, config_dict, use_alphaquant_format)
+        return table_reformatter.merge_protein_cols_and_config_dict(
+            input_df_subset, config_dict, use_alphaquant_format
+        )
     else:
-        return table_reformatter.merge_protein_and_ion_cols(input_df_subset, config_dict)
+        return table_reformatter.merge_protein_and_ion_cols(
+            input_df_subset, config_dict
+        )
 
-def write_chunk_to_file(chunk, filepath ,write_header, write_index):
+
+def write_chunk_to_file(chunk, filepath, write_header, write_index):
     """write chunk of pandas dataframe to a file"""
-    chunk.to_csv(filepath, header=write_header, mode='a', sep = "\t", index = write_index)
+    chunk.to_csv(filepath, header=write_header, mode="a", sep="\t", index=write_index)
+
 
 def reshape_input_df(input_df, config_dict):
-    input_df = input_df.astype({'quant_val': 'float'})
-    input_df = plexdia_reformatter.adapt_input_df_columns_in_case_of_mDIA(input_df=input_df, config_dict_for_type=config_dict)
+    input_df = input_df.astype({"quant_val": "float"})
+    input_df = plexdia_reformatter.adapt_input_df_columns_in_case_of_mDIA(
+        input_df=input_df, config_dict_for_type=config_dict
+    )
     column_names = get_column_names(input_df)
     input_df = adapt_input_df(input_df, column_names)
-    input_reshaped = pd.pivot_table(input_df, index = ['protein', 'quant_id']+column_names, columns = config_dict.get("sample_ID"), values = 'quant_val', fill_value=0)
+    input_reshaped = pd.pivot_table(
+        input_df,
+        index=["protein", "quant_id"] + column_names,
+        columns=config_dict.get("sample_ID"),
+        values="quant_val",
+        fill_value=0,
+    )
     input_reshaped = input_reshaped.reset_index()
     return input_reshaped
 
+
 def get_column_names(input_df):
     if input_df.index.names[0] is None:
         return []
     else:
         return input_df.index.names
 
+
 def adapt_input_df(input_df, column_names):
-    if len(column_names)==0:
+    if len(column_names) == 0:
         return input_df.reset_index()
     else:
         input_df = input_df.reset_index()
         input_df[column_names] = input_df[column_names].astype(str)
         return input_df
 
 
-
-
-def process_with_dask(*, tmpfile_columnfilt, outfile_name, config_dict_for_type, use_alphaquant_format):
-    df = dd.read_csv(tmpfile_columnfilt, sep = "\t")
-    allcols = df[config_dict_for_type.get("sample_ID")].drop_duplicates().compute() # the columns of the output table are the sample IDs
-    allcols = plexdia_reformatter.extend_sample_allcolumns_for_mDIA_case(allcols_samples=allcols, config_dict_for_type=config_dict_for_type)
-    allcols = ['protein', 'quant_id'] + sorted(allcols)
+def process_with_dask(
+    *, tmpfile_columnfilt, outfile_name, config_dict_for_type, use_alphaquant_format
+):
+    df = dd.read_csv(tmpfile_columnfilt, sep="\t")
+    allcols = (
+        df[config_dict_for_type.get("sample_ID")].drop_duplicates().compute()
+    )  # the columns of the output table are the sample IDs
+    allcols = plexdia_reformatter.extend_sample_allcolumns_for_mDIA_case(
+        allcols_samples=allcols, config_dict_for_type=config_dict_for_type
+    )
+    allcols = ["protein", "quant_id"] + sorted(allcols)
 
     if not use_alphaquant_format:
         hierarchy_columns = get_hierarchy_names_from_config_dict(config_dict_for_type)
         allcols = allcols + hierarchy_columns
-    df = df.set_index('protein')
+    df = df.set_index("protein")
     sorted_filedir = f"{tmpfile_columnfilt}_sorted"
-    df.to_csv(sorted_filedir, sep = "\t")
-    #now the files are sorted and can be pivoted chunkwise (multiindex pivoting at the moment not possible in dask)
+    df.to_csv(sorted_filedir, sep="\t")
+    # now the files are sorted and can be pivoted chunkwise (multiindex pivoting at the moment not possible in dask)
     files_dask = glob.glob(f"{sorted_filedir}/*part")
     header = True
     for file in files_dask:
         if use_alphaquant_format:
-            input_df = pd.read_csv(file, sep = "\t")
+            input_df = pd.read_csv(file, sep="\t")
         else:
-            input_df = pd.read_csv(file, sep = "\t", index_col=hierarchy_columns)
-        if len(input_df.index) <2:
+            input_df = pd.read_csv(file, sep="\t", index_col=hierarchy_columns)
+        if len(input_df.index) < 2:
             continue
         input_reshaped = reshape_input_df(input_df, config_dict_for_type)
         input_reshaped = sort_and_add_columns(input_reshaped, allcols)
-        write_chunk_to_file(input_reshaped, outfile_name, header, write_index = False)
+        write_chunk_to_file(input_reshaped, outfile_name, header, write_index=False)
         header = False
     os.remove(tmpfile_columnfilt)
     shutil.rmtree(sorted_filedir)
 
+
 def get_hierarchy_names_from_config_dict(config_dict_for_type):
     hierarchy_names = []
     if "ion_hierarchy" in config_dict_for_type.keys():
         ion_hierarchy = config_dict_for_type.get("ion_hierarchy")
         for hierarchy_type in ion_hierarchy.keys():
             hierarchy_names += ion_hierarchy.get(hierarchy_type).get("order")
         return list(set(hierarchy_names))
     else:
         return []
-    
+
 
 def sort_and_add_columns(input_reshaped, allcols):
     missing_cols = set(allcols) - set(input_reshaped.columns)
     input_reshaped[list(missing_cols)] = 0
     input_reshaped = input_reshaped[allcols]
     return input_reshaped
-
-
-
-
-
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/plexdia_reformatter.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/plexdia_reformatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,77 @@
+import re
+
+
 def extend_sample_allcolumns_for_mDIA_case(allcols_samples, config_dict_for_type):
     if is_mDIA_table(config_dict_for_type):
         new_allcols = []
-        channels = ['Dimethyl-n-0', 'Dimethyl-n-4', 'Dimethyl-n-8']
+        channels = ["Dimethyl-n-0", "Dimethyl-n-4", "Dimethyl-n-8"]
         for channel in channels:
             for sample in allcols_samples:
                 new_allcols.append(merge_channel_and_sample_string(sample, channel))
         return new_allcols
     else:
         return allcols_samples
 
 
 # Cell
-#mDIA case
+# mDIA case
 
-def adapt_input_df_columns_in_case_of_mDIA(input_df,config_dict_for_type):
+
+def adapt_input_df_columns_in_case_of_mDIA(input_df, config_dict_for_type):
     if is_mDIA_table(config_dict_for_type):
         input_df = extend_sampleID_column_for_mDIA_case(input_df, config_dict_for_type)
         input_df = set_mtraq_reduced_ion_column_into_dataframe(input_df)
         return input_df
     else:
         return input_df
 
 
-def extend_sampleID_column_for_mDIA_case(input_df,config_dict_for_type):
+def extend_sampleID_column_for_mDIA_case(input_df, config_dict_for_type):
     channels_per_peptide = parse_channel_from_peptide_column(input_df)
-    return merge_sample_id_and_channels(input_df, channels_per_peptide, config_dict_for_type)
+    return merge_sample_id_and_channels(
+        input_df, channels_per_peptide, config_dict_for_type
+    )
 
 
 def set_mtraq_reduced_ion_column_into_dataframe(input_df):
-    new_ions = remove_mtraq_modifications_from_ion_ids(input_df['quant_id'])
-    input_df['quant_id'] = new_ions
+    new_ions = remove_mtraq_modifications_from_ion_ids(input_df["quant_id"])
+    input_df["quant_id"] = new_ions
     return input_df
 
+
 def remove_mtraq_modifications_from_ion_ids(ions):
     new_ions = []
     for ion in ions:
-        new_ions.append( re.sub("\(Dimethyl-\w-\d\)","", ion))
+        new_ions.append(re.sub("\(Dimethyl-\w-\d\)", "", ion))
     return new_ions
 
 
 def is_mDIA_table(config_dict_for_type):
-    return config_dict_for_type.get('channel_ID') == ['Channel.0', 'Channel.4']
+    return config_dict_for_type.get("channel_ID") == ["Channel.0", "Channel.4"]
 
 
-import re
 def parse_channel_from_peptide_column(input_df):
     channels = []
-    for pep in input_df['Modified.Sequence']:
+    for pep in input_df["Modified.Sequence"]:
         pattern = "(.*)(\(Dimethyl-n-.\))(.*)"
         matched = re.match(pattern, pep)
         num_appearances = pep.count("Dimethyl-n-")
-        if matched and num_appearances==1:
+        if matched and num_appearances == 1:
             channels.append(matched.group(2))
         else:
             channels.append("NA")
     return channels
 
+
 def merge_sample_id_and_channels(input_df, channels, config_dict_for_type):
     sample_id = config_dict_for_type.get("sample_ID")
     sample_ids = list(input_df[sample_id])
-    input_df[sample_id] = [merge_channel_and_sample_string(sample_ids[idx], channels[idx]) for idx in range(len(sample_ids))]
+    input_df[sample_id] = [
+        merge_channel_and_sample_string(sample_ids[idx], channels[idx])
+        for idx in range(len(sample_ids))
+    ]
     return input_df
 
+
 def merge_channel_and_sample_string(sample, channel):
     return f"{sample}_{channel}"
-
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/quant_reader_manager.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/quant_reader_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 import pandas as pd
 from . import config_dict_loader
 from . import longformat_reader
 from . import wideformat_reader
 
 
-def import_data(input_file, input_type_to_use = None, samples_subset = None, results_dir = None, use_alphaquant_format = False):
+def import_data(
+    input_file,
+    input_type_to_use=None,
+    samples_subset=None,
+    results_dir=None,
+    use_alphaquant_format=False,
+):
     """
     Function to import peptide level data. Depending on available columns in the provided file,
     the function identifies the type of input used (e.g. Spectronaut, MaxQuant, DIA-NN), reformats if necessary
     and returns a generic wide-format dataframe
     :param file input_file: quantified peptide/ion -level data
     :param file results_folder: the folder where the directlfq outputs are stored
     """
 
     samples_subset = add_ion_protein_headers_if_applicable(samples_subset)
     if "aq_reformat" in input_file:
         file_to_read = input_file
     else:
-        file_to_read = reformat_and_save_input_file(input_file=input_file, input_type_to_use=input_type_to_use, use_alphaquant_format = use_alphaquant_format)
-    
-    input_reshaped = pd.read_csv(file_to_read, sep = "\t", encoding = 'latin1', usecols=samples_subset)
-    input_reshaped = input_reshaped.drop_duplicates(subset='quant_id')
+        file_to_read = reformat_and_save_input_file(
+            input_file=input_file,
+            input_type_to_use=input_type_to_use,
+            use_alphaquant_format=use_alphaquant_format,
+        )
+
+    input_reshaped = pd.read_csv(
+        file_to_read, sep="\t", encoding="latin1", usecols=samples_subset
+    )
+    input_reshaped = input_reshaped.drop_duplicates(subset="quant_id")
     return input_reshaped
 
+
 def add_ion_protein_headers_if_applicable(samples_subset):
     if samples_subset is not None:
         return samples_subset + ["quant_id", "protein"]
     else:
         return None
 
-def reformat_and_save_input_file(input_file, input_type_to_use = None, use_alphaquant_format = False):
-    
-    input_type, config_dict_for_type, sep = config_dict_loader.get_input_type_and_config_dict(input_file, input_type_to_use)
+
+def reformat_and_save_input_file(
+    input_file, input_type_to_use=None, use_alphaquant_format=False
+):
+    input_type, config_dict_for_type, sep = (
+        config_dict_loader.get_input_type_and_config_dict(input_file, input_type_to_use)
+    )
     print(f"using input type {input_type}")
-    format = config_dict_for_type.get('format')
+    format = config_dict_for_type.get("format")
     outfile_name = f"{input_file}.{input_type}.aq_reformat.tsv"
 
     if format == "longtable":
-        longformat_reader.reformat_and_write_longtable_according_to_config(input_file, outfile_name,config_dict_for_type, sep = sep, use_alphaquant_format=use_alphaquant_format)
+        longformat_reader.reformat_and_write_longtable_according_to_config(
+            input_file,
+            outfile_name,
+            config_dict_for_type,
+            sep=sep,
+            use_alphaquant_format=use_alphaquant_format,
+        )
     elif format == "widetable":
-        wideformat_reader.reformat_and_write_wideformat_table(input_file, outfile_name, config_dict_for_type)
+        wideformat_reader.reformat_and_write_wideformat_table(
+            input_file, outfile_name, config_dict_for_type
+        )
     else:
-        raise Exception('Format not recognized!')
+        raise Exception("Format not recognized!")
     return outfile_name
 
+
 def set_quanttable_config_location(quanttable_config_file):
     config_dict_loader.INTABLE_CONFIG = quanttable_config_file
-
-
-
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/quantreader_utils.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/quantreader_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 def filter_input(filter_dict, input):
-    if filter_dict == None:
+    if filter_dict is None:
         return input
-    for filtname,filterconf in filter_dict.items():
-        param = filterconf.get('param')
-        comparator = filterconf.get('comparator')
-        value = filterconf.get('value')
+    for filtname, filterconf in filter_dict.items():
+        param = filterconf.get("param")
+        comparator = filterconf.get("comparator")
+        value = filterconf.get("value")
+
+        if comparator not in [">", ">=", "<", "<=", "==", "!="]:
+            raise TypeError(
+                f"cannot identify the filter comparator of {filtname} given in the longtable config yaml!"
+            )
 
-        if comparator not in [">",">=", "<", "<=", "==", "!="]:
-            raise TypeError(f"cannot identify the filter comparator of {filtname} given in the longtable config yaml!")
-
-        if comparator=="==":
-            input = input[input[param] ==value]
+        if comparator == "==":
+            input = input[input[param] == value]
             continue
         try:
-            input = input.astype({f"{param}" : "float"})
-        except:
+            input = input.astype({f"{param}": "float"})
+        except Exception:
             pass
 
-        if comparator==">":
-            input = input[input[param].astype(type(value)) >value]
+        if comparator == ">":
+            input = input[input[param].astype(type(value)) > value]
 
-        if comparator==">=":
-            input = input[input[param].astype(type(value)) >=value]
+        if comparator == ">=":
+            input = input[input[param].astype(type(value)) >= value]
 
-        if comparator=="<":
-            input = input[input[param].astype(type(value)) <value]
+        if comparator == "<":
+            input = input[input[param].astype(type(value)) < value]
 
-        if comparator=="<=":
-            input = input[input[param].astype(type(value)) <=value]
+        if comparator == "<=":
+            input = input[input[param].astype(type(value)) <= value]
 
-        if comparator=="!=":
-            input = input[input[param].astype(type(value)) !=value]
+        if comparator == "!=":
+            input = input[input[param].astype(type(value)) != value]
 
-    return input
+    return input
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/table_reformatter.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/table_reformatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,151 +1,185 @@
-import itertools
 import pandas as pd
 import copy
 
-def merge_protein_cols_and_config_dict(input_df, config_dict, use_alphaquant_format = False):
+
+def merge_protein_cols_and_config_dict(
+    input_df, config_dict, use_alphaquant_format=False
+):
     """[summary]
-    
+
     Args:
         input_df ([pandas dataframe]): longtable containing peptide intensity data
         confid_dict ([dict[String[]]]): nested dict containing the parse information. derived from yaml file
 
     Returns:
         pandas dataframe: longtable with newly assigned "protein" and "ion" columns
     """
     protein_cols = config_dict.get("protein_cols")
     ion_hierarchy = config_dict.get("ion_hierarchy")
-    splitcol2sep = config_dict.get('split_cols')
-    quant_id_dict = config_dict.get('quant_ID')
+    splitcol2sep = config_dict.get("split_cols")
+    quant_id_dict = config_dict.get("quant_ID")
 
     ion_dfs = []
-    input_df['protein'] = join_columns(input_df, protein_cols)
+    input_df["protein"] = join_columns(input_df, protein_cols)
 
-    input_df = input_df.drop(columns = [x for x in protein_cols if x!='protein'])
+    input_df = input_df.drop(columns=[x for x in protein_cols if x != "protein"])
     index_names = []
     for hierarchy_type in ion_hierarchy.keys():
         df_subset = input_df.copy()
         ion_hierarchy_local = ion_hierarchy.get(hierarchy_type).get("order")
-        ion_headers_merged, ion_headers_grouped = get_ionname_columns(ion_hierarchy.get(hierarchy_type).get("mapping"), ion_hierarchy_local) #ion headers merged is just a helper to select all relevant rows, ionheaders grouped contains the sets of ionstrings to be merged into a list eg [[SEQ, MOD], [CH]]
-        quant_columns = get_quantitative_columns(df_subset, hierarchy_type, config_dict, ion_headers_merged)
-        headers = list(set(ion_headers_merged + quant_columns + ['protein']))
+        ion_headers_merged, ion_headers_grouped = get_ionname_columns(
+            ion_hierarchy.get(hierarchy_type).get("mapping"), ion_hierarchy_local
+        )  # ion headers merged is just a helper to select all relevant rows, ionheaders grouped contains the sets of ionstrings to be merged into a list eg [[SEQ, MOD], [CH]]
+        quant_columns = get_quantitative_columns(
+            df_subset, hierarchy_type, config_dict, ion_headers_merged
+        )
+        headers = list(set(ion_headers_merged + quant_columns + ["protein"]))
         if "sample_ID" in config_dict.keys():
-            headers+=[config_dict.get("sample_ID")]
+            headers += [config_dict.get("sample_ID")]
         df_subset = df_subset[headers].drop_duplicates()
 
         if splitcol2sep is not None:
-            if quant_columns[0] in splitcol2sep.keys(): #in the case that quantitative values are stored grouped in one column (e.g. msiso1,msiso2,msiso3, etc.), reformat accordingly
+            if (
+                quant_columns[0] in splitcol2sep.keys()
+            ):  # in the case that quantitative values are stored grouped in one column (e.g. msiso1,msiso2,msiso3, etc.), reformat accordingly
                 df_subset = split_extend_df(df_subset, splitcol2sep)
-            ion_headers_grouped = adapt_headers_on_extended_df(ion_headers_grouped, splitcol2sep)
-
-        #df_subset = df_subset.set_index(quant_columns)
-
-        df_subset = add_index_and_metadata_columns(df_subset, ion_hierarchy_local, ion_headers_grouped, quant_id_dict, hierarchy_type)
+            ion_headers_grouped = adapt_headers_on_extended_df(
+                ion_headers_grouped, splitcol2sep
+            )
+
+        # df_subset = df_subset.set_index(quant_columns)
+
+        df_subset = add_index_and_metadata_columns(
+            df_subset,
+            ion_hierarchy_local,
+            ion_headers_grouped,
+            quant_id_dict,
+            hierarchy_type,
+        )
         index_names += df_subset.index.names
-        #add_merged_ionnames(df_subset, ion_hierarchy_local, ion_headers_grouped, quant_id_dict, hierarchy_type)
+        # add_merged_ionnames(df_subset, ion_hierarchy_local, ion_headers_grouped, quant_id_dict, hierarchy_type)
         ion_dfs.append(df_subset.reset_index())
-    
+
     input_df = pd.concat(ion_dfs, ignore_index=True)
     if use_alphaquant_format:
         input_df = input_df.drop(columns=list(set(index_names)))
     else:
         input_df = input_df.set_index(list(set(index_names)))
 
     return input_df
 
-def join_columns(df, columns, separator='_'):
+
+def join_columns(df, columns, separator="_"):
     if len(columns) == 1:
-        return df[columns[0]].fillna('nan').astype(str)
+        return df[columns[0]].fillna("nan").astype(str)
     else:
-        return df[columns].fillna('nan').astype(str).agg(separator.join, axis=1)
-
+        return df[columns].fillna("nan").astype(str).agg(separator.join, axis=1)
 
 
 def get_ionname_columns(ion_dict, ion_hierarchy_local):
     ion_headers_merged = []
     ion_headers_grouped = []
     for lvl in ion_hierarchy_local:
         vals = ion_dict.get(lvl)
         ion_headers_merged.extend(vals)
         ion_headers_grouped.append(vals)
     return ion_headers_merged, ion_headers_grouped
 
+
 def get_quantitative_columns(input_df, hierarchy_type, config_dict, ion_headers_merged):
-    naming_columns = ion_headers_merged + ['protein']
-    if config_dict.get("format") == 'longtable':
+    naming_columns = ion_headers_merged + ["protein"]
+    if config_dict.get("format") == "longtable":
         quantcol = config_dict.get("quant_ID").get(hierarchy_type)
         return [quantcol]
 
-    if config_dict.get("format") == 'widetable':
-        quantcolumn_candidates = [x for x in input_df.columns if x not in naming_columns]
+    if config_dict.get("format") == "widetable":
+        quantcolumn_candidates = [
+            x for x in input_df.columns if x not in naming_columns
+        ]
         if "quant_pre_or_suffix" in config_dict.keys():
-            return [x for x in quantcolumn_candidates if x.startswith(config_dict.get("quant_pre_or_suffix")) or x.endswith(config_dict.get("quant_pre_or_suffix"))] # in the case that the quantitative columns have a prefix (like "Intensity " in MQ peptides.txt), only columns with the prefix are filtered
+            return [
+                x
+                for x in quantcolumn_candidates
+                if x.startswith(config_dict.get("quant_pre_or_suffix"))
+                or x.endswith(config_dict.get("quant_pre_or_suffix"))
+            ]  # in the case that the quantitative columns have a prefix (like "Intensity " in MQ peptides.txt), only columns with the prefix are filtered
         else:
-            return quantcolumn_candidates #in this case, we assume that all non-ionname/proteinname columns are quantitative columns
+            return quantcolumn_candidates  # in this case, we assume that all non-ionname/proteinname columns are quantitative columns
 
 
 def split_extend_df(input_df, splitcol2sep, value_threshold=10):
     """reformats data that is stored in a condensed way in a single column. For example isotope1_intensity;isotope2_intensity etc. in Spectronaut
 
     Args:
         input_df ([type]): [description]
         splitcol2sep ([type]): [description]
         value_threshold([type]): [description]
 
     Returns:
         Pandas Dataframe: Pandas dataframe with the condensed items expanded to long format
     """
-    if splitcol2sep==None:
+    if splitcol2sep is None:
         return input_df
 
     for split_col, separator in splitcol2sep.items():
         idx_name = f"{split_col}_idxs"
         split_col_series = input_df[split_col].str.split(separator)
-        input_df = input_df.drop(columns = [split_col])
+        input_df = input_df.drop(columns=[split_col])
 
         input_df[idx_name] = [list(range(len(x))) for x in split_col_series]
         exploded_input = input_df.explode(idx_name)
         exploded_split_col_series = split_col_series.explode()
 
-        exploded_input[split_col] = exploded_split_col_series.replace('', 0) #the column with the intensities has to come after to column with the idxs
+        exploded_input[split_col] = exploded_split_col_series.replace(
+            "", 0
+        )  # the column with the intensities has to come after to column with the idxs
 
         exploded_input = exploded_input.astype({split_col: float})
-        exploded_input = exploded_input[exploded_input[split_col]>value_threshold]
-        #exploded_input = exploded_input.rename(columns = {'var1': split_col})
+        exploded_input = exploded_input[exploded_input[split_col] > value_threshold]
+        # exploded_input = exploded_input.rename(columns = {'var1': split_col})
     return exploded_input
 
+
 def adapt_headers_on_extended_df(ion_headers_grouped, splitcol2sep):
-    #in the case that one column has been split, we need to designate the "naming" column
+    # in the case that one column has been split, we need to designate the "naming" column
     ion_headers_grouped_copy = copy.deepcopy(ion_headers_grouped)
     for vals in ion_headers_grouped_copy:
         if splitcol2sep is not None:
             for idx in range(len(vals)):
                 if vals[idx] in splitcol2sep.keys():
                     vals[idx] = vals[idx] + "_idxs"
     return ion_headers_grouped_copy
 
 
 def merge_protein_and_ion_cols(input_df, config_dict):
-    protein_cols =  config_dict.get("protein_cols")
+    protein_cols = config_dict.get("protein_cols")
     ion_cols = config_dict.get("ion_cols")
-    input_df['protein'] = join_columns(input_df, protein_cols)
-    input_df['quant_id'] = join_columns(input_df, ion_cols)
-    input_df = input_df.rename(columns = {config_dict.get('quant_ID') : "quant_val"})
+    input_df["protein"] = join_columns(input_df, protein_cols)
+    input_df["quant_id"] = join_columns(input_df, ion_cols)
+    input_df = input_df.rename(columns={config_dict.get("quant_ID"): "quant_val"})
     return input_df
 
 
-def add_index_and_metadata_columns(df_subset, ion_hierarchy_local, ion_headers_grouped, quant_id_dict, hierarchy_type):
+def add_index_and_metadata_columns(
+    df_subset, ion_hierarchy_local, ion_headers_grouped, quant_id_dict, hierarchy_type
+):
     """puts together the hierarchical ion names as a column in a given input dataframe"""
-    
+
     for idx in range(len(ion_hierarchy_local)):
         hierarchy_name = ion_hierarchy_local[idx]
         headers = ion_headers_grouped[idx]
-        df_subset[hierarchy_name] = join_columns(df_subset, headers)# df_subset[headers].apply(lambda x: '_'.join(x.astype(str)), axis=1)
-        df_subset[hierarchy_name] = f"{hierarchy_name}_" +df_subset[hierarchy_name]
-    
-    df_subset['quant_id'] = join_columns(df_subset, ion_hierarchy_local, separator='_')# df_subset[ion_hierarchy_local].apply(lambda x: '_AND_'.join(x.astype(str)), axis=1)
-
+        df_subset[hierarchy_name] = join_columns(
+            df_subset, headers
+        )  # df_subset[headers].apply(lambda x: '_'.join(x.astype(str)), axis=1)
+        df_subset[hierarchy_name] = f"{hierarchy_name}_" + df_subset[hierarchy_name]
+
+    df_subset["quant_id"] = join_columns(
+        df_subset, ion_hierarchy_local, separator="_"
+    )  # df_subset[ion_hierarchy_local].apply(lambda x: '_AND_'.join(x.astype(str)), axis=1)
 
     df_subset = df_subset.set_index(ion_hierarchy_local)
-    if quant_id_dict!= None:
-        df_subset = df_subset.rename(columns = {quant_id_dict.get(hierarchy_type) : "quant_val"})
-    return df_subset
+    if quant_id_dict is not None:
+        df_subset = df_subset.rename(
+            columns={quant_id_dict.get(hierarchy_type): "quant_val"}
+        )
+    return df_subset
```

### Comparing `alphabase-1.2.3/alphabase/quantification/quant_reader/wideformat_reader.py` & `alphabase-1.2.4/alphabase/quantification/quant_reader/wideformat_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import pandas as pd
 from . import quantreader_utils
 from . import table_reformatter
 
 
 def reformat_and_write_wideformat_table(peptides_tsv, outfile_name, config_dict):
-    input_df = pd.read_csv(peptides_tsv,sep="\t", encoding ='latin1')
+    input_df = pd.read_csv(peptides_tsv, sep="\t", encoding="latin1")
     filter_dict = config_dict.get("filters")
-    protein_cols = config_dict.get("protein_cols")
-    ion_cols = config_dict.get("ion_cols")
+
     input_df = quantreader_utils.filter_input(filter_dict, input_df)
-    #input_df = merge_protein_and_ion_cols(input_df, config_dict)
-    input_df = table_reformatter.merge_protein_cols_and_config_dict(input_df, config_dict)
-    if 'quant_pre_or_suffix' in config_dict.keys():
-        quant_pre_or_suffix = config_dict.get('quant_pre_or_suffix')
-        headers = ['protein', 'quant_id'] + list(filter(lambda x: x.startswith(quant_pre_or_suffix) or x.endswith(quant_pre_or_suffix), input_df.columns))
+    # input_df = merge_protein_and_ion_cols(input_df, config_dict)
+    input_df = table_reformatter.merge_protein_cols_and_config_dict(
+        input_df, config_dict
+    )
+    if "quant_pre_or_suffix" in config_dict.keys():
+        quant_pre_or_suffix = config_dict.get("quant_pre_or_suffix")
+        headers = ["protein", "quant_id"] + list(
+            filter(
+                lambda x: x.startswith(quant_pre_or_suffix)
+                or x.endswith(quant_pre_or_suffix),
+                input_df.columns,
+            )
+        )
         input_df = input_df[headers]
-        input_df = input_df.rename(columns = lambda x : x.replace(quant_pre_or_suffix, ""))
+        input_df = input_df.rename(columns=lambda x: x.replace(quant_pre_or_suffix, ""))
+
+    # input_df = input_df.reset_index()
 
-    #input_df = input_df.reset_index()
-    
-    input_df.to_csv(outfile_name, sep = '\t', index = None)
+    input_df.to_csv(outfile_name, sep="\t", index=None)
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/base.py` & `alphabase-1.2.4/alphabase/spectral_library/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,33 @@
 import numpy as np
 import typing
 import logging
 import copy
 import warnings
 import re
 
-import alphabase.peptide.fragment as fragment
-import alphabase.peptide.precursor as precursor
+from alphabase.peptide.fragment import (
+    create_fragment_mz_dataframe,
+    calc_fragment_count,
+    filter_fragment_number,
+    join_left,
+    remove_unused_fragments,
+)
+from alphabase.peptide.precursor import (
+    update_precursor_mz,
+    refine_precursor_df,
+    calc_precursor_isotope_intensity_mp,
+    calc_precursor_isotope_intensity,
+    calc_precursor_isotope_info_mp,
+    calc_precursor_isotope_info,
+    hash_precursor_df,
+)
 from alphabase.io.hdf import HDF_File
 
+
 class SpecLibBase(object):
     """
     Base spectral library in alphabase and alphapeptdeep.
 
     Attributes
     ----------
     charged_frag_types : list
@@ -25,181 +40,191 @@
     max_precursor_mz : float
         same as `precursor_mz_max` in Parameters in :meth:`__init__`.
 
     decoy : str
         same as `decoy` in Parameters in :meth:`__init__`.
     """
 
-    key_numeric_columns:list = [
-        'ccs_pred', 'charge', 
-        'decoy',
-        'frag_stop_idx', 'frag_start_idx',
-        'isotope_m1_intensity', 'isotope_m1_mz',
-        'isotope_apex_mz', 'isotope_apex_intensity',
-        'isotope_apex_offset',
-        'isotope_right_most_mz', 'isotope_right_most_intensity',
-        'isotope_right_most_offset',
-        'miss_cleavage', 
-        'mobility_pred', 'mobility',
-        'nAA', 'precursor_mz', 
-        'rt_pred', 'rt_norm_pred', 'rt',
-        'labeling_channel',
+    key_numeric_columns: list = [
+        "ccs_pred",
+        "charge",
+        "decoy",
+        "frag_stop_idx",
+        "frag_start_idx",
+        "isotope_m1_intensity",
+        "isotope_m1_mz",
+        "isotope_apex_mz",
+        "isotope_apex_intensity",
+        "isotope_apex_offset",
+        "isotope_right_most_mz",
+        "isotope_right_most_intensity",
+        "isotope_right_most_offset",
+        "miss_cleavage",
+        "mobility_pred",
+        "mobility",
+        "nAA",
+        "precursor_mz",
+        "rt_pred",
+        "rt_norm_pred",
+        "rt",
+        "labeling_channel",
     ]
     """
-    list of str: Key numeric columns to be saved 
-    into library/precursor_df in the hdf file for fast loading, 
+    list of str: Key numeric columns to be saved
+    into library/precursor_df in the hdf file for fast loading,
     others will be saved into library/mod_seq_df instead.
     """
 
-    def __init__(self,
-        # ['b_z1','b_z2','y_z1','y_modloss_z1', ...]; 
-        # 'b_z1': 'b' is the fragment type and 
+    def __init__(
+        self,
+        # ['b_z1','b_z2','y_z1','y_modloss_z1', ...];
+        # 'b_z1': 'b' is the fragment type and
         # 'z1' is the charge state z=1.
-        charged_frag_types:typing.List[str] = [
-            'b_z1','b_z2','y_z1', 'y_z2'
-        ], 
-        precursor_mz_min = 400, precursor_mz_max = 6000,
-        decoy:str = None,
+        charged_frag_types: typing.List[str] = ["b_z1", "b_z2", "y_z1", "y_z2"],
+        precursor_mz_min=400,
+        precursor_mz_max=6000,
+        decoy: str = None,
     ):
         """
         Parameters
         ----------
         charged_frag_types : typing.List[str], optional
-            fragment types with charge. 
+            fragment types with charge.
             Defaults to [ 'b_z1','b_z2','y_z1', 'y_z2' ].
 
         precursor_mz_min : int, optional
-            Use this to clip precursor df. 
+            Use this to clip precursor df.
             Defaults to 400.
 
         precursor_mz_max : int, optional
-            Use this to clip precursor df. 
+            Use this to clip precursor df.
             Defaults to 6000.
 
         decoy : str, optional
             Decoy methods, could be "pseudo_reverse" or "diann".
             Defaults to None.
         """
         self.charged_frag_types = charged_frag_types
         self._precursor_df = pd.DataFrame()
         self._fragment_intensity_df = pd.DataFrame()
         self._fragment_mz_df = pd.DataFrame()
         self.min_precursor_mz = precursor_mz_min
         self.max_precursor_mz = precursor_mz_max
 
         self.decoy = decoy
-    
+
     @property
-    def precursor_df(self)->pd.DataFrame:
+    def precursor_df(self) -> pd.DataFrame:
         """
         Precursor dataframe with columns
         'sequence', 'mods', 'mod_sites', 'charge', etc,
         identical to :attr:`peptide_df`.
         """
         return self._precursor_df
 
     @precursor_df.setter
-    def precursor_df(self, df:pd.DataFrame):
+    def precursor_df(self, df: pd.DataFrame):
         self._precursor_df = df
-        precursor.refine_precursor_df(
+        refine_precursor_df(
             self._precursor_df,
             drop_frag_idx=False,
             ensure_data_validity=True,
         )
 
     @property
-    def peptide_df(self)->pd.DataFrame:
+    def peptide_df(self) -> pd.DataFrame:
         """
         Peptide dataframe with columns
         'sequence', 'mods', 'mod_sites', 'charge', etc,
-        identical to :attr:`precursor_df`. 
+        identical to :attr:`precursor_df`.
         """
         return self._precursor_df
 
     @peptide_df.setter
-    def peptide_df(self, df:pd.DataFrame):
+    def peptide_df(self, df: pd.DataFrame):
         self.precursor_df = df
 
     @property
-    def fragment_mz_df(self)->pd.DataFrame:
+    def fragment_mz_df(self) -> pd.DataFrame:
         """
-        The fragment mz dataframe with 
+        The fragment mz dataframe with
         fragment types as columns (['b_z1', 'y_z2', ...])
         """
         return self._fragment_mz_df
 
     @property
-    def fragment_intensity_df(self)->pd.DataFrame:
+    def fragment_intensity_df(self) -> pd.DataFrame:
         """
-        The fragment intensity dataframe with 
+        The fragment intensity dataframe with
         fragment types as columns (['b_z1', 'y_z2', ...])
         """
         return self._fragment_intensity_df
-    
 
-    def available_dense_fragment_dfs(self)->list:
+    def available_dense_fragment_dfs(self) -> list:
         """
         Return the available dense fragment dataframes
         By dynamically checking the attributes of the object.
         a fragment dataframe is matched with the pattern '_fragment_[attribute_name]_df'
 
         Returns
         -------
         list
             List of available fragment dataframes
         """
-        return [
-            attr for attr in dir(self) 
-            if re.match(r'_fragment_.*_df', attr)
-        ]
-    
+        return [attr for attr in dir(self) if re.match(r"_fragment_.*_df", attr)]
+
     def copy(self):
         """
         Return a copy of the spectral library object.
-        
+
         Returns
         -------
         SpecLibBase
             A copy of the spectral library object.
         """
         new_instance = self.__class__()
         new_instance.__dict__ = copy.deepcopy(self.__dict__)
 
         return new_instance
-    
+
     def append(
-            self, 
-            other : 'SpecLibBase',
-            dfs_to_append : typing.List[str] = ['_precursor_df','_fragment_intensity_df', '_fragment_mz_df','_fragment_intensity_predicted_df'],
-            remove_unused_dfs:bool = True,
-        ):
+        self,
+        other: "SpecLibBase",
+        dfs_to_append: typing.List[str] = [
+            "_precursor_df",
+            "_fragment_intensity_df",
+            "_fragment_mz_df",
+            "_fragment_intensity_predicted_df",
+        ],
+        remove_unused_dfs: bool = True,
+    ):
         """
 
-        Append another SpecLibBase object to the current one in place. 
+        Append another SpecLibBase object to the current one in place.
         All matching dataframes in the second object will be appended to the current one. Dataframes missing in the current object will be ignored.
         All matching columns in the second object will be appended to the current one. Columns missing in the current object will be ignored.
         Dataframes and columns missing in the second object will raise an error.
-        
+
         Parameters
         ----------
         other : SpecLibBase
             Second SpecLibBase object to be appended.
-            
+
         dfs_to_append : list, optional
             List of dataframes to be appended.
             Defaults to ['_precursor_df','_fragment_intensity_df', '_fragment_mz_df','_fragment_intensity_predicted_df'].
 
         remove_unused_dfs : bool, optional
             Remove dataframes from the current library that are not used in the append, this is crucial when using the remove unused fragments function
             after appending a library, inorder to have all fragment dataframes of the same size. When set to false the unused dataframes will be kept.
-            
+
         Returns
         -------
         None
-            
+
         """
         if remove_unused_dfs:
             current_frag_dfs = self.available_dense_fragment_dfs()
             for attr in current_frag_dfs:
                 if attr not in dfs_to_append:
                     delattr(self, attr)
 
@@ -208,393 +233,340 @@
             # the first dataframe should have all the columns of the second dataframe, otherwise raise error
             # the second dataframe may have more columns, but they will be dropped with a warning
             missing_columns = set(df1.columns) - set(df2.columns)
             if len(missing_columns) > 0:
                 raise ValueError(
                     f"The columns are not compatible. {missing_columns} are missing in the dataframe which should be appended."
                 )
-            
+
             missing_columns = set(df2.columns) - set(df1.columns)
             if len(missing_columns) > 0:
                 warnings.warn(
                     f"Unmatched columns in second dataframe will be dropped: {missing_columns}."
                 )
 
             return df1.columns.values
-        
+
         # get subset of dataframes and columns to append
         # will fail if the speclibs are not compatible
         matching_columns = []
         for attr in dfs_to_append:
             if hasattr(self, attr) and hasattr(other, attr):
                 matching_columns.append(
-                    check_matching_columns(
-                        getattr(self, attr), getattr(other, attr)
-                    )
+                    check_matching_columns(getattr(self, attr), getattr(other, attr))
                 )
             elif hasattr(self, attr) and not hasattr(other, attr):
                 raise ValueError(
                     f"The libraries can't be appended as {attr} is missing in the second library."
                 )
             else:
                 matching_columns.append([])
 
         n_fragments = []
         # get subset of dfs_to_append starting with _fragment
         for attr in dfs_to_append:
-            if attr.startswith('_fragment'):
+            if attr.startswith("_fragment"):
                 if hasattr(self, attr):
                     n_current_fragments = len(getattr(self, attr))
                     if n_current_fragments > 0:
                         n_fragments += [n_current_fragments]
 
         if not np.all(np.array(n_fragments) == n_fragments[0]):
             raise ValueError(
-                f"The libraries can't be appended as the number of fragments in the current libraries are not the same."
+                "The libraries can't be appended as the number of fragments in the current libraries are not the same."
             )
-        
-        for attr, matching_columns in zip(
-            dfs_to_append,
-            matching_columns
-        ):
+
+        for attr, matching_columns in zip(dfs_to_append, matching_columns):
             if hasattr(self, attr) and hasattr(other, attr):
-                
                 current_df = getattr(self, attr)
 
                 # copy dataframes to avoid changing the original ones
                 other_df = getattr(other, attr)[matching_columns].copy()
 
-                if attr.startswith('_precursor'):
-                    
+                if attr.startswith("_precursor"):
                     frag_idx_increment = 0
-                    for fragment_df in ['_fragment_intensity_df', '_fragment_mz_df']:
+                    for fragment_df in ["_fragment_intensity_df", "_fragment_mz_df"]:
                         if hasattr(self, fragment_df):
                             if len(getattr(self, fragment_df)) > 0:
                                 frag_idx_increment = len(getattr(self, fragment_df))
-   
-                    if 'frag_start_idx' in other_df.columns:
-                        other_df['frag_start_idx'] += frag_idx_increment
 
-                    if 'frag_stop_idx' in other_df.columns:
-                        other_df['frag_stop_idx'] += frag_idx_increment
+                    if "frag_start_idx" in other_df.columns:
+                        other_df["frag_start_idx"] += frag_idx_increment
+
+                    if "frag_stop_idx" in other_df.columns:
+                        other_df["frag_stop_idx"] += frag_idx_increment
 
                 setattr(
-                    self, attr,
+                    self,
+                    attr,
                     pd.concat(
-                        [
-                            current_df,
-                            other_df
-                        ],
-                        axis=0,
-                        ignore_index=True,
-                        sort=False
-                    ).reset_index(drop=True)
+                        [current_df, other_df], axis=0, ignore_index=True, sort=False
+                    ).reset_index(drop=True),
                 )
 
     def refine_df(self):
         """
         Sort nAA and reset_index for faster calculation (or prediction)
         """
-        precursor.refine_precursor_df(
-            self._precursor_df
-        )
+        refine_precursor_df(self._precursor_df)
 
     def append_decoy_sequence(self):
         """
         Append decoy sequence into precursor_df.
         Decoy method is based on self.decoy(str).
         ```
         >>> decoy_lib = (decoy_lib_provider.get_decoy_lib( self.decoy, self))
         >>> decoy_lib.decoy_sequence()
         >>> decoy_lib.append_to_target_lib()
         ...
         ```
         """
-        from alphabase.spectral_library.decoy import (
-            decoy_lib_provider
-        )
+        from alphabase.spectral_library.decoy import decoy_lib_provider
+
         # register 'protein_reverse' to the decoy_lib_provider
-        import alphabase.protein.protein_level_decoy
+        from alphabase.protein.protein_level_decoy import register_decoy
 
-        decoy_lib = (
-            decoy_lib_provider.get_decoy_lib(
-                self.decoy, self
-            )
-        )
-        if decoy_lib is None: return None
+        register_decoy()
+
+        decoy_lib = decoy_lib_provider.get_decoy_lib(self.decoy, self)
+        if decoy_lib is None:
+            return None
         decoy_lib.decoy_sequence()
         decoy_lib.append_to_target_lib()
 
     def clip_by_precursor_mz_(self):
-        ''' 
+        """
         Clip self._precursor_df inplace by self.min_precursor_mz and self.max_precursor_mz
-        '''
+        """
         self._precursor_df.drop(
             self._precursor_df.loc[
-                (self._precursor_df['precursor_mz']<self.min_precursor_mz)|
-                (self._precursor_df['precursor_mz']>self.max_precursor_mz)
-            ].index, inplace=True
+                (self._precursor_df["precursor_mz"] < self.min_precursor_mz)
+                | (self._precursor_df["precursor_mz"] > self.max_precursor_mz)
+            ].index,
+            inplace=True,
         )
         self._precursor_df.reset_index(drop=True, inplace=True)
 
     def calc_precursor_mz(self):
         """
         Calculate precursor mz for self._precursor_df
         """
-        fragment.update_precursor_mz(self._precursor_df)
+        update_precursor_mz(self._precursor_df)
 
     def calc_and_clip_precursor_mz(self):
         """
         Calculate precursor mz for self._precursor_df,
         and clip the self._precursor_df using `self.clip_by_precursor_mz_`
         """
         self.calc_precursor_mz()
         self.clip_by_precursor_mz_()
 
-    def calc_precursor_isotope_intensity(self,
-        max_isotope = 6,
-        min_right_most_intensity = 0.001,
-        mp_batch_size = 10000,
-        mp_process_num = 8,
-        normalize:typing.Literal['mono','sum'] = "sum",
+    def calc_precursor_isotope_intensity(
+        self,
+        max_isotope=6,
+        min_right_most_intensity=0.001,
+        mp_batch_size=10000,
+        mp_process_num=8,
+        normalize: typing.Literal["mono", "sum"] = "sum",
     ):
         """
         Calculate and append the isotope intensity columns into self.precursor_df.
-        See `alphabase.peptide.precursor.calc_precursor_isotope_intensity` for details.
-    
+        See `alphabase.peptide.calc_precursor_isotope_intensity` for details.
+
         Parameters
         ----------
 
         max_isotope : int, optional
             The maximum isotope to calculate.
 
         min_right_most_intensity : float, optional
             The minimum intensity of the right most isotope.
 
         mp_batch_size : int, optional
             The batch size for multiprocessing.
 
         mp_processes : int, optional
             The number of processes for multiprocessing.
-        
+
         """
 
-        if 'precursor_mz' not in self._precursor_df.columns:
+        if "precursor_mz" not in self._precursor_df.columns:
             self.calc_and_clip_precursor_mz()
 
-        if mp_process_num>1 and len(self.precursor_df)>mp_batch_size:
-            (
-                self._precursor_df
-            ) = precursor.calc_precursor_isotope_intensity_mp(
-                self.precursor_df, 
-                max_isotope = max_isotope,
-                min_right_most_intensity = min_right_most_intensity,
+        if mp_process_num > 1 and len(self.precursor_df) > mp_batch_size:
+            (self._precursor_df) = calc_precursor_isotope_intensity_mp(
+                self.precursor_df,
+                max_isotope=max_isotope,
+                min_right_most_intensity=min_right_most_intensity,
                 normalize=normalize,
-                mp_process_num = mp_process_num,
+                mp_process_num=mp_process_num,
                 mp_batch_size=mp_batch_size,
             )
         else:
-            (
-                self._precursor_df
-            ) = precursor.calc_precursor_isotope_intensity(
-                self.precursor_df, 
-                max_isotope = max_isotope,
+            (self._precursor_df) = calc_precursor_isotope_intensity(
+                self.precursor_df,
+                max_isotope=max_isotope,
                 normalize=normalize,
-                min_right_most_intensity = min_right_most_intensity,
+                min_right_most_intensity=min_right_most_intensity,
             )
 
-    def calc_precursor_isotope(self,
-        max_isotope = 6,
-        min_right_most_intensity = 0.001,
-        mp_batch_size = 10000,
-        mp_process_num = 8,
-        normalize:typing.Literal['mono','sum'] = "sum",
+    def calc_precursor_isotope(
+        self,
+        max_isotope=6,
+        min_right_most_intensity=0.001,
+        mp_batch_size=10000,
+        mp_process_num=8,
+        normalize: typing.Literal["mono", "sum"] = "sum",
     ):
         return self.calc_precursor_isotope_intensity(
             max_isotope=max_isotope,
             min_right_most_intensity=min_right_most_intensity,
             normalize=normalize,
             mp_batch_size=mp_batch_size,
             mp_process_num=mp_process_num,
-        )     
-    
-    def calc_precursor_isotope_info(self, 
-        mp_process_num:int=8,
+        )
+
+    def calc_precursor_isotope_info(
+        self,
+        mp_process_num: int = 8,
         mp_process_bar=None,
-        mp_batch_size = 10000,
+        mp_batch_size=10000,
     ):
         """
         Append isotope columns into self.precursor_df.
-        See `alphabase.peptide.precursor.calc_precursor_isotope` for details.
+        See `alphabase.peptide.calc_precursor_isotope` for details.
         """
-        if 'precursor_mz' not in self._precursor_df.columns:
+        if "precursor_mz" not in self._precursor_df.columns:
             self.calc_and_clip_precursor_mz()
-        if (
-            mp_process_num > 1 and 
-            len(self.precursor_df)>mp_batch_size
-        ):
-            (
-                self._precursor_df
-            ) = precursor.calc_precursor_isotope_info_mp(
-                self.precursor_df, 
+        if mp_process_num > 1 and len(self.precursor_df) > mp_batch_size:
+            (self._precursor_df) = calc_precursor_isotope_info_mp(
+                self.precursor_df,
                 processes=mp_process_num,
                 process_bar=mp_process_bar,
             )
         else:
-            (
-                self._precursor_df
-            ) = precursor.calc_precursor_isotope_info(
-                self.precursor_df
-            )
+            (self._precursor_df) = calc_precursor_isotope_info(self.precursor_df)
 
     def calc_fragment_mz_df(self):
         """
         TODO: use multiprocessing here or in the
         `create_fragment_mz_dataframe` function.
         """
-        if (
-            self.charged_frag_types is not None 
-            or len(self.charged_frag_types)
-        ):
-            (
-                self._fragment_mz_df
-            ) = fragment.create_fragment_mz_dataframe(
-                self.precursor_df, self.charged_frag_types,
+        if self.charged_frag_types is not None or len(self.charged_frag_types):
+            (self._fragment_mz_df) = create_fragment_mz_dataframe(
+                self.precursor_df,
+                self.charged_frag_types,
             )
         else:
-            print('Skip fragment calculation as self.charged_frag_types is None or empty')
+            print(
+                "Skip fragment calculation as self.charged_frag_types is None or empty"
+            )
 
     def hash_precursor_df(self):
         """Insert hash codes for peptides and precursors"""
-        precursor.hash_precursor_df(
-            self._precursor_df
-        )
-    
-    def annotate_fragments_from_speclib(self, 
-        donor_speclib, 
-        verbose = True
-    ):
+        hash_precursor_df(self._precursor_df)
+
+    def annotate_fragments_from_speclib(self, donor_speclib, verbose=True):
         """
         Annotate self.precursor_df with fragments from donor_speclib.
         The donor_speclib must have a fragment_mz_df and can optionally have a fragment_intensity_df.
         Fragment dataframes are updated inplace and overwritten.
 
         Parameters
         ----------
         donor_speclib : SpecLibBase
             The donor library to annotate fragments from.
 
         verbose : bool, optional
             Print progress, by default True, for example::
-            
+
                 2022-12-16 00:52:08> Speclib with 4 precursors will be reannotated with speclib with 12 precursors and 504 fragments
                 2022-12-16 00:52:08> A total of 4 precursors were succesfully annotated, 0 precursors were not matched
-            
-            
+
+
         """
-        self = annotate_fragments_from_speclib(
-            self, donor_speclib, verbose = verbose
-        )
-    
+        self = annotate_fragments_from_speclib(self, donor_speclib, verbose=verbose)
+
     def remove_unused_fragments(self):
         """
         Remove unused fragments from all available fragment dataframes.
         Fragment dataframes are updated inplace and overwritten.
         """
 
         available_fragments_df = self.available_dense_fragment_dfs()
         non_zero_dfs = [
-            df for df in available_fragments_df 
-            if len(getattr(self, df)) > 0
+            df for df in available_fragments_df if len(getattr(self, df)) > 0
         ]
-        to_compress = [
-            getattr(self, df) for df in non_zero_dfs
-        ]
-        self._precursor_df, compressed_dfs = fragment.remove_unused_fragments(
+        to_compress = [getattr(self, df) for df in non_zero_dfs]
+        self._precursor_df, compressed_dfs = remove_unused_fragments(
             self._precursor_df, to_compress
         )
 
         for df, compressed_df in zip(non_zero_dfs, compressed_dfs):
             setattr(self, df, compressed_df)
 
-
     def calc_fragment_count(self):
         """
-        Count the number of non-zero fragments for each precursor.
+        Count the number of non-zero fragments for each
         Creates the column 'n_fragments' in self._precursor_df.
         """
 
-        self._precursor_df['n_fragments'] = fragment.calc_fragment_count(
-            self._precursor_df,
-            self._fragment_intensity_df
+        self._precursor_df["n_fragments"] = calc_fragment_count(
+            self._precursor_df, self._fragment_intensity_df
         )
-    
+
     def filter_fragment_number(
-            self, 
-            n_fragments_allowed_column_name='n_fragments_allowed', 
-            n_allowed=999
-        ):
+        self, n_fragments_allowed_column_name="n_fragments_allowed", n_allowed=999
+    ):
         """
         Filter the top k fragments for each precursor based on a global setting and a precursor wise column.
         The smaller one will be used. Can be used to make sure that target and decoy have the same number of fragments.
 
         Parameters
         ----------
         n_fragments_allowed_column_name : str, optional, default 'n_fragments_allowed'
-            The column name in self._precursor_df that contains the number of fragments allowed for each precursor.
+            The column name in self._precursor_df that contains the number of fragments allowed for each
 
         n_allowed : int, optional, default 999
-            The global setting for the number of fragments allowed for each precursor.
+            The global setting for the number of fragments allowed for each
         """
 
-        fragment.filter_fragment_number(
+        filter_fragment_number(
             self._precursor_df,
             self._fragment_intensity_df,
             n_fragments_allowed_column_name=n_fragments_allowed_column_name,
-            n_allowed=n_allowed
+            n_allowed=n_allowed,
         )
 
-    def _get_hdf_to_save(self, 
-        hdf_file, 
-        delete_existing=False
-    ):
+    def _get_hdf_to_save(self, hdf_file, delete_existing=False):
         """Internal function to get a HDF group to write"""
         _hdf = HDF_File(
-            hdf_file, 
-            read_only=False, 
-            truncate=True,
-            delete_existing=delete_existing
+            hdf_file, read_only=False, truncate=True, delete_existing=delete_existing
         )
         return _hdf.library
 
-    def _get_hdf_to_load(self,
-        hdf_file, 
+    def _get_hdf_to_load(
+        self,
+        hdf_file,
     ):
         """Internal function to get a HDF group to read"""
         _hdf = HDF_File(
             hdf_file,
         )
         return _hdf.library
 
-    def save_df_to_hdf(self, 
-        hdf_file:str, 
-        df_key: str,
-        df: pd.DataFrame,
-        delete_existing=False
+    def save_df_to_hdf(
+        self, hdf_file: str, df_key: str, df: pd.DataFrame, delete_existing=False
     ):
         """Save a new HDF group or dataset into existing HDF file"""
-        self._get_hdf_to_save(
-            hdf_file, 
-            delete_existing=delete_existing
-        ).add_group(df_key, df)
-
-    def load_df_from_hdf(self, 
-        hdf_file:str, 
-        df_name: str
-    )->pd.DataFrame:
+        self._get_hdf_to_save(hdf_file, delete_existing=delete_existing).add_group(
+            df_key, df
+        )
+
+    def load_df_from_hdf(self, hdf_file: str, df_name: str) -> pd.DataFrame:
         """Load specific dataset (dataframe) from hdf_file.
 
         Parameters
         ----------
         hdf_file : str
             The hdf file name
 
@@ -602,173 +574,172 @@
             The dataset/dataframe name in the hdf file
 
         Returns
         -------
         pd.DataFrame
             Loaded dataframe
         """
-        return self._get_hdf_to_load(
-            hdf_file
-        ).__getattribute__(df_name).values
+        return self._get_hdf_to_load(hdf_file).__getattribute__(df_name).values
 
-    def save_hdf(self, hdf_file:str):
+    def save_hdf(self, hdf_file: str):
         """Save library dataframes into hdf_file.
         For `self.precursor_df`, this method will save it into two hdf groups in hdf_file:
         `library/precursor_df` and `library/mod_seq_df`.
 
-        `library/precursor_df` contains all essential numberic columns those 
+        `library/precursor_df` contains all essential numberic columns those
         can be loaded faster from hdf file into memory:
 
         'precursor_mz', 'charge', 'mod_seq_hash', 'mod_seq_charge_hash',
         'frag_start_idx', 'frag_stop_idx', 'decoy', 'rt_pred', 'ccs_pred',
-        'mobility_pred', 'miss_cleave', 'nAA', 
+        'mobility_pred', 'miss_cleave', 'nAA',
         ['isotope_mz_m1', 'isotope_intensity_m1'], ...
 
-        `library/mod_seq_df` contains all string columns and the other 
+        `library/mod_seq_df` contains all string columns and the other
         not essential columns:
         'sequence','mods','mod_sites', ['proteins', 'genes']...
-        as well as 'mod_seq_hash', 'mod_seq_charge_hash' columns to map 
+        as well as 'mod_seq_hash', 'mod_seq_charge_hash' columns to map
         back to `precursor_df`
 
         Parameters
         ----------
         hdf_file : str
             the hdf file path to save
-            
+
         """
-        _hdf = HDF_File(
-            hdf_file, 
-            read_only=False, 
-            truncate=True,
-            delete_existing=True
-        )
-        if 'mod_seq_charge_hash' not in self._precursor_df.columns:
+        _hdf = HDF_File(hdf_file, read_only=False, truncate=True, delete_existing=True)
+        if "mod_seq_charge_hash" not in self._precursor_df.columns:
             self.hash_precursor_df()
 
-        key_columns = self.key_numeric_columns+[
-            'mod_seq_hash', 'mod_seq_charge_hash'
-        ]
+        key_columns = self.key_numeric_columns + ["mod_seq_hash", "mod_seq_charge_hash"]
 
         _hdf.library = {
-            'mod_seq_df': self._precursor_df[
+            "mod_seq_df": self._precursor_df[
                 [
-                    col for col in self._precursor_df.columns 
+                    col
+                    for col in self._precursor_df.columns
                     if col not in self.key_numeric_columns
                 ]
             ],
-            'precursor_df': self._precursor_df[
-                [
-                    col for col in self._precursor_df.columns 
-                    if col in key_columns
-                ]
+            "precursor_df": self._precursor_df[
+                [col for col in self._precursor_df.columns if col in key_columns]
             ],
-            'fragment_mz_df': self._fragment_mz_df,
-            'fragment_intensity_df': self._fragment_intensity_df,
+            "fragment_mz_df": self._fragment_mz_df,
+            "fragment_intensity_df": self._fragment_intensity_df,
         }
-        
-    def load_hdf(self, hdf_file:str, load_mod_seq:bool=False):
+
+    def load_hdf(self, hdf_file: str, load_mod_seq: bool = False):
         """Load the hdf library from hdf_file
 
         Parameters
         ----------
         hdf_file : str
             hdf library path to load
 
         load_mod_seq : bool, optional
-            if also load mod_seq_df. 
+            if also load mod_seq_df.
             Defaults to False.
-            
+
         """
         _hdf = HDF_File(
             hdf_file,
         )
-        self._precursor_df:pd.DataFrame = _hdf.library.precursor_df.values
+        self._precursor_df: pd.DataFrame = _hdf.library.precursor_df.values
         if load_mod_seq:
-            key_columns = self.key_numeric_columns+[
-                'mod_seq_hash', 'mod_seq_charge_hash'
+            key_columns = self.key_numeric_columns + [
+                "mod_seq_hash",
+                "mod_seq_charge_hash",
             ]
             mod_seq_df = _hdf.library.mod_seq_df.values
-            cols = [
-                col for col in mod_seq_df.columns 
-                if col not in key_columns
-            ]
+            cols = [col for col in mod_seq_df.columns if col not in key_columns]
             self._precursor_df[cols] = mod_seq_df[cols]
-            
+
         self._fragment_mz_df = _hdf.library.fragment_mz_df.values
         self._fragment_intensity_df = _hdf.library.fragment_intensity_df.values
 
         self._fragment_mz_df = self._fragment_mz_df[
             [
-                frag for frag in self.charged_frag_types 
+                frag
+                for frag in self.charged_frag_types
                 if frag in self._fragment_mz_df.columns
             ]
         ]
         self._fragment_intensity_df = self._fragment_intensity_df[
             [
-                frag for frag in self.charged_frag_types 
+                frag
+                for frag in self.charged_frag_types
                 if frag in self._fragment_intensity_df.columns
             ]
         ]
-        
+
+
 def annotate_fragments_from_speclib(
-    speclib: SpecLibBase, 
+    speclib: SpecLibBase,
     fragment_speclib: SpecLibBase,
-    verbose = True,
-)->SpecLibBase:
+    verbose=True,
+) -> SpecLibBase:
     """Reannotate an SpecLibBase library with fragments from a different SpecLibBase.
-    
+
     Parameters
     ----------
     speclib: alphabase.spectral_library.library_base.SpecLibBase
         Spectral library which contains the precursors to be annotated. All fragments mz and fragment intensities will be removed.
 
     fragment_speclib: alphabase.spectral_library.library_base.SpecLibBase
         Spectral library which contains the donor precursors whose fragments should be used.
 
     Returns
     -------
 
     alphabase.spectral_library.library_base.SpecLibBase
         newly annotated spectral library
- 
+
     """
     if verbose:
         num_precursor_left = len(speclib.precursor_df)
         num_precursor_right = len(fragment_speclib.precursor_df)
-        num_fragments_right = len(fragment_speclib.fragment_mz_df) * len(fragment_speclib.fragment_mz_df.columns)
-        logging.info(f'Speclib with {num_precursor_left:,} precursors will be reannotated with speclib with {num_precursor_right:,} precursors and {num_fragments_right:,} fragments')
+        num_fragments_right = len(fragment_speclib.fragment_mz_df) * len(
+            fragment_speclib.fragment_mz_df.columns
+        )
+        logging.info(
+            f"Speclib with {num_precursor_left:,} precursors will be reannotated with speclib with {num_precursor_right:,} precursors and {num_fragments_right:,} fragments"
+        )
 
     # reannotation is based on mod_seq_hash column
-    hash_column_name = 'mod_seq_hash'
+    hash_column_name = "mod_seq_hash"
 
     # create hash columns if missing
     if hash_column_name not in speclib.precursor_df.columns:
         speclib.hash_precursor_df()
 
     if fragment_speclib not in fragment_speclib.precursor_df.columns:
         fragment_speclib.hash_precursor_df()
 
     speclib_hash = speclib.precursor_df[hash_column_name].values
     fragment_speclib_hash = fragment_speclib.precursor_df[hash_column_name].values
 
-    speclib_indices = fragment.join_left(speclib_hash, fragment_speclib_hash)
+    speclib_indices = join_left(speclib_hash, fragment_speclib_hash)
 
-    matched_mask = (speclib_indices >= 0)
+    matched_mask = speclib_indices >= 0
 
     if verbose:
         matched_count = np.sum(matched_mask)
         not_matched_count = np.sum(~matched_mask)
-    
-        logging.info(f'A total of {matched_count:,} precursors were succesfully annotated, {not_matched_count:,} precursors were not matched')
 
+        logging.info(
+            f"A total of {matched_count:,} precursors were succesfully annotated, {not_matched_count:,} precursors were not matched"
+        )
+
+    frag_start_idx = fragment_speclib.precursor_df["frag_start_idx"].values[
+        speclib_indices
+    ]
+    frag_stop_idx = fragment_speclib.precursor_df["frag_stop_idx"].values[
+        speclib_indices
+    ]
 
-    frag_start_idx = fragment_speclib.precursor_df['frag_start_idx'].values[speclib_indices]
-    frag_stop_idx = fragment_speclib.precursor_df['frag_stop_idx'].values[speclib_indices]
-    
     speclib._precursor_df = speclib._precursor_df[matched_mask].copy()
-    speclib._precursor_df['frag_start_idx'] = frag_start_idx[matched_mask]
-    speclib._precursor_df['frag_stop_idx'] = frag_stop_idx[matched_mask]
+    speclib._precursor_df["frag_start_idx"] = frag_start_idx[matched_mask]
+    speclib._precursor_df["frag_stop_idx"] = frag_stop_idx[matched_mask]
 
     speclib._fragment_mz_df = fragment_speclib._fragment_mz_df.copy()
     speclib._fragment_intensity_df = fragment_speclib._fragment_intensity_df.copy()
 
-    return speclib
+    return speclib
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/decoy.py` & `alphabase-1.2.4/alphabase/spectral_library/decoy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,125 +1,128 @@
 import copy
 from typing import Any
 import pandas as pd
 import multiprocessing as mp
-from functools import partial
 from alphabase.spectral_library.base import SpecLibBase
-from alphabase.io.hdf import HDF_File
+
 
 def _batchify_series(series, mp_batch_size):
     """Internal funciton for multiprocessing"""
     for i in range(0, len(series), mp_batch_size):
-        yield series.iloc[i:i+mp_batch_size]
+        yield series.iloc[i : i + mp_batch_size]
+
+
 class BaseDecoyGenerator(object):
     """
     Base class for decoy generator.
     A class is used instead of a function to make as it needs to be pickled for multiprocessing.
     """
+
     def __call__(self, series: pd.Series) -> pd.Series:
         """
         Main entry of this class, it calls follows methods:
         - self._decoy()
         """
 
         return series.apply(self._decoy)
 
-    def _decoy(self, sequence:str) -> str:
-        raise NotImplementedError('Subclass should implement this method.')
+    def _decoy(self, sequence: str) -> str:
+        raise NotImplementedError("Subclass should implement this method.")
 
-class DIANNDecoyGenerator(BaseDecoyGenerator):
-    def __init__(self, 
-            raw_AAs:str = 'GAVLIFMPWSCTYHKRQENDBJOUXZ',
-            mutated_AAs:str = 'LLLVVLLLLTSSSSLLNDQEVVVVVV'
-        ):
 
+class DIANNDecoyGenerator(BaseDecoyGenerator):
+    def __init__(
+        self,
+        raw_AAs: str = "GAVLIFMPWSCTYHKRQENDBJOUXZ",
+        mutated_AAs: str = "LLLVVLLLLTSSSSLLNDQEVVVVVV",
+    ):
         """
         DiaNN-like decoy peptide generator
 
         Parameters
         ----------
 
         raw_AAs : str, optional
-            AAs those DiaNN decoy from. 
+            AAs those DiaNN decoy from.
             Defaults to 'GAVLIFMPWSCTYHKRQENDBJOUXZ'.
 
         mutated_AAs : str, optional
-            AAs those DiaNN decoy to. 
+            AAs those DiaNN decoy to.
             Defaults to 'LLLVVLLLLTSSSSLLNDQEVVVVVV'.
-            
+
         """
         self.raw_AAs = raw_AAs
         self.mutated_AAs = mutated_AAs
 
-
     def _decoy(self, sequence: str) -> str:
-        return sequence[0]+ \
-        self.mutated_AAs[self.raw_AAs.index(sequence[1])]+ \
-        sequence[2:-2]+ \
-        self.mutated_AAs[self.raw_AAs.index(sequence[-2])]+ \
-        sequence[-1]
+        return (
+            sequence[0]
+            + self.mutated_AAs[self.raw_AAs.index(sequence[1])]
+            + sequence[2:-2]
+            + self.mutated_AAs[self.raw_AAs.index(sequence[-2])]
+            + sequence[-1]
+        )
+
 
 class PseudoReverseDecoyGenerator(BaseDecoyGenerator):
-    def __init__(self, fix_C_term:bool=True):
+    def __init__(self, fix_C_term: bool = True):
         """
         Pseudo-reverse decoy generator.
 
         Parameters
         ----------
 
         fix_C_term : bool, optional
-            If fix C-term AA when decoy. 
+            If fix C-term AA when decoy.
             Defaults to True.
         """
 
         self.fix_C_term = fix_C_term
 
     def _decoy(self, sequence: str) -> str:
         if self.fix_C_term:
-            return (sequence[:-1][::-1] + sequence[-1])
+            return sequence[:-1][::-1] + sequence[-1]
         else:
             return sequence[::-1]
 
+
 class SpecLibDecoy(SpecLibBase):
     """
     Pseudo-reverse peptide decoy generator.
     """
 
-    def __init__(self, 
-        target_lib:SpecLibBase,
+    def __init__(
+        self,
+        target_lib: SpecLibBase,
         decoy_generator: Any = PseudoReverseDecoyGenerator,
         **kwargs,
     ):
         """
         Parameters
         ----------
         target_lib : SpecLibBase
             Target library to decoy.
 
         fix_C_term : bool, optional
-            If fix C-term AA when decoy. 
+            If fix C-term AA when decoy.
             Defaults to True.
-        
+
         Attributes
         ----------
         target_lib : SpecLibBase
             same as 'target_lib' in Args.
         """
         self.__dict__ = copy.deepcopy(target_lib.__dict__)
         self.target_lib = target_lib
 
-        self.generator = decoy_generator(
-            **kwargs
-        )
+        self.generator = decoy_generator(**kwargs)
 
     def translate_to_decoy(
-            self, 
-            multiprocessing : bool = True,
-            mp_batch_size=10000, 
-            mp_process_num: int = 8):
+        self, multiprocessing: bool = True, mp_batch_size=10000, mp_process_num: int = 8
+    ):
         """
         Main entry of this class, it calls follows methods:
         - self.decoy_sequence()
 
         Parameters
         ----------
 
@@ -130,42 +133,38 @@
         mp_batch_size : int, optional
             Batch size for multiprocessing.
             Defaults to 10000.
 
         mp_process_num : int, optional
             Number of processes for multiprocessing.
             Defaults to 8.
-            
+
         """
         self.decoy_sequence(
             multiprocessing=multiprocessing,
             mp_batch_size=mp_batch_size,
-            mp_process_num=mp_process_num
+            mp_process_num=mp_process_num,
         )
 
     def append_to_target_lib(self):
         """
         A decoy method should define how to append itself to target_lib.
-        Sub-classes should override this method when necessary. 
+        Sub-classes should override this method when necessary.
         """
         self._remove_target_seqs()
-        self._precursor_df['decoy'] = 1
-        self.target_lib._precursor_df['decoy'] = 0
-        self.target_lib._precursor_df = pd.concat((
-            self.target_lib._precursor_df,
-            self._precursor_df
-        ), ignore_index=True)
+        self._precursor_df["decoy"] = 1
+        self.target_lib._precursor_df["decoy"] = 0
+        self.target_lib._precursor_df = pd.concat(
+            (self.target_lib._precursor_df, self._precursor_df), ignore_index=True
+        )
         self.target_lib.refine_df()
 
     def decoy_sequence(
-            self, 
-            multiprocessing: bool = True, 
-            mp_batch_size=10000, 
-            mp_process_num: int = 8
-        ):
+        self, multiprocessing: bool = True, mp_batch_size=10000, mp_process_num: int = 8
+    ):
         """
         Generate decoy sequences from `self.target_lib`.
         Sub-classes should override the `_decoy_seq` method when necessary.
 
         Parameters
         ----------
 
@@ -179,86 +178,81 @@
 
         mp_process_num : int, optional
             Number of processes for multiprocessing.
             Defaults to 8.
         """
 
         if not multiprocessing or self._precursor_df.shape[0] < mp_batch_size:
-            self._precursor_df['sequence'] = self.generator(self._precursor_df['sequence'])
+            self._precursor_df["sequence"] = self.generator(
+                self._precursor_df["sequence"]
+            )
             self._remove_target_seqs()
             return
-            
-        sequence_batches = list(_batchify_series(
-            self._precursor_df['sequence'], mp_batch_size
-        ))
+
+        sequence_batches = list(
+            _batchify_series(self._precursor_df["sequence"], mp_batch_size)
+        )
 
         series_list = []
         with mp.get_context("spawn").Pool(mp_process_num) as p:
-            processing = p.imap(
-                self.generator,
-                sequence_batches
-            )
+            processing = p.imap(self.generator, sequence_batches)
             for df in processing:
                 series_list.append(df)
-        self._precursor_df['sequence'] = pd.concat(series_list)
+        self._precursor_df["sequence"] = pd.concat(series_list)
         self._remove_target_seqs()
 
     def _remove_target_seqs(self):
-        target_seqs = set(
-            self.target_lib._precursor_df.sequence.values
-        )
+        target_seqs = set(self.target_lib._precursor_df.sequence.values)
         self._precursor_df.drop(
-            self._precursor_df.loc[
-                self._precursor_df.sequence.isin(target_seqs)
-            ].index, inplace=True
+            self._precursor_df.loc[self._precursor_df.sequence.isin(target_seqs)].index,
+            inplace=True,
         )
 
+
 class SpecLibDecoyProvider(object):
     def __init__(self):
         self.decoy_dict = {}
 
-    def register(self, name:str, decoy_class:SpecLibDecoy):
+    def register(self, name: str, decoy_class: SpecLibDecoy):
         """Register a new decoy class"""
         self.decoy_dict[name.lower()] = decoy_class
 
-    def get_decoy_lib(self, 
-        name:str, 
-        target_lib:SpecLibBase, 
-        **kwargs
-    )->SpecLibDecoy:
-        """Get an object of a subclass of `SpecLibDecoy` based on 
+    def get_decoy_lib(
+        self, name: str, target_lib: SpecLibBase, **kwargs
+    ) -> SpecLibDecoy:
+        """Get an object of a subclass of `SpecLibDecoy` based on
         registered name.
 
         Parameters
         ----------
         name : str
             Registered decoy class name
-            
+
         target_lib : SpecLibBase
             Target library for decoy generation
 
         Returns
         -------
         SpecLibDecoy
             Decoy library object
         """
-        if not name: return None
+        if not name:
+            return None
         name = name.lower()
         if name == "none" or name == "null":
             return None
         if name in self.decoy_dict:
             return SpecLibDecoy(
-                target_lib,
-                decoy_generator = self.decoy_dict[name],
-                **kwargs
+                target_lib, decoy_generator=self.decoy_dict[name], **kwargs
             )
         else:
-            raise ValueError(f'Decoy method {name} not found.')
+            raise ValueError(f"Decoy method {name} not found.")
+
 
-decoy_lib_provider:SpecLibDecoyProvider = SpecLibDecoyProvider()
+decoy_lib_provider: SpecLibDecoyProvider = SpecLibDecoyProvider()
 """
-Factory object of `SpecLibDecoyProvider` to 
+Factory object of `SpecLibDecoyProvider` to
 register and get different types of decoy methods.
 """
 
-decoy_lib_provider.register('pseudo_reverse', PseudoReverseDecoyGenerator)
-decoy_lib_provider.register('diann', DIANNDecoyGenerator)
+decoy_lib_provider.register("pseudo_reverse", PseudoReverseDecoyGenerator)
+decoy_lib_provider.register("diann", DIANNDecoyGenerator)
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/flat.py` & `alphabase-1.2.4/alphabase/spectral_library/flat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,214 +1,214 @@
 import pandas as pd
 import numpy as np
 import warnings
 
-from alphabase.spectral_library.base import (
-    SpecLibBase
-)
-from alphabase.peptide.fragment import (
-    flatten_fragments
-)
+from alphabase.spectral_library.base import SpecLibBase
+from alphabase.peptide.fragment import flatten_fragments, remove_unused_fragments
 
 from alphabase.io.hdf import HDF_File
 
-import alphabase.peptide.precursor as precursor
 
 class SpecLibFlat(SpecLibBase):
-    """ 
+    """
     Flatten the spectral library (SpecLibBase) by using :meth:`parse_base_library`.
 
     Attributes
     ----------
     custom_fragment_df_columns : list of str
-        'mz' and 'intensity' columns are required in :attr:`fragment_df`, 
-        others could be customized. 
+        'mz' and 'intensity' columns are required in :attr:`fragment_df`,
+        others could be customized.
         It can include ['type','number','position','charge','loss_type'].
 
     min_fragment_intensity : float
         minimal intensity to keep in :attr:`fragment_df`.
 
     keep_top_k_fragments : float
         top k highest peaks to keep in :attr:`fragment_df`.
-    
+
     """
 
-    key_numeric_columns = SpecLibBase.key_numeric_columns+[
-        'flat_frag_start_idx','flat_frag_stop_idx'
+    key_numeric_columns = SpecLibBase.key_numeric_columns + [
+        "flat_frag_start_idx",
+        "flat_frag_stop_idx",
     ]
-    """ 
-    :obj:`SpecLibBase.key_numeric_columns <alphabase.spectral_library.base.SpecLibBase.key_numeric_columns>` 
+    """
+    :obj:`SpecLibBase.key_numeric_columns <alphabase.spectral_library.base.SpecLibBase.key_numeric_columns>`
     + `['flat_frag_start_idx','flat_frag_stop_idx']`.
     """
 
-    def __init__(self,
-        charged_frag_types:list = ['b_z1','b_z2','y_z1','y_z2'],
-        min_fragment_intensity:float = 0.001,
-        keep_top_k_fragments:int = 1000,
-        custom_fragment_df_columns:list = [
-            'type','number','position','charge','loss_type'
+    def __init__(
+        self,
+        charged_frag_types: list = ["b_z1", "b_z2", "y_z1", "y_z2"],
+        min_fragment_intensity: float = 0.001,
+        keep_top_k_fragments: int = 1000,
+        custom_fragment_df_columns: list = [
+            "type",
+            "number",
+            "position",
+            "charge",
+            "loss_type",
         ],
-        **kwargs
+        **kwargs,
     ):
         """
         Parameters
         ----------
         min_fragment_intensity : float, optional
             minimal intensity to keep, by default 0.001
 
         keep_top_k_fragments : int, optional
             top k highest peaks to keep, by default 1000
 
         custom_fragment_df_columns : list, optional
-            See :attr:`custom_fragment_df_columns`, 
+            See :attr:`custom_fragment_df_columns`,
             defaults to ['type','number','position','charge','loss_type']
         """
         super().__init__(charged_frag_types=charged_frag_types)
         self.min_fragment_intensity = min_fragment_intensity
         self.keep_top_k_fragments = keep_top_k_fragments
 
         self.custom_fragment_df_columns = custom_fragment_df_columns
 
     @property
-    def fragment_df(self)->pd.DataFrame:
+    def fragment_df(self) -> pd.DataFrame:
         """The flat fragment dataframe with columns
         (['mz', 'intensity'] + :attr:`custom_fragment_df_columns`.)
         """
         return self._fragment_df
 
     @property
-    def protein_df(self)->pd.DataFrame:
-        """ Protein dataframe """
+    def protein_df(self) -> pd.DataFrame:
+        """Protein dataframe"""
         return self._protein_df
-    
+
     def available_dense_fragment_dfs(self):
         """Return the available dense fragment dataframes.
         This method is inherited from :class:`SpecLibBase` and will return an empty list for a flat library.
         """
         return []
-    
+
     def remove_unused_fragments(self):
         """Remove unused fragments from fragment_df.
         This method is inherited from :class:`SpecLibBase` and has not been implemented for a flat library.
         """
-        raise NotImplementedError("remove_unused_fragments is not implemented for a flat library")
-    
-    def parse_base_library(self, 
-        library:SpecLibBase,
-        keep_original_frag_dfs:bool=False,
-        copy_precursor_df:bool=False,
-        **kwargs
+        self._precursor_df, (self._fragment_df,) = remove_unused_fragments(
+            self._precursor_df,
+            (self._fragment_df,),
+            frag_start_col="flat_frag_start_idx",
+            frag_stop_col="flat_frag_stop_idx",
+        )
+
+    def parse_base_library(
+        self,
+        library: SpecLibBase,
+        keep_original_frag_dfs: bool = False,
+        copy_precursor_df: bool = False,
+        **kwargs,
     ):
-        """ 
-        Flatten an library object of SpecLibBase or its inherited class. 
+        """
+        Flatten an library object of SpecLibBase or its inherited class.
         This method will generate :attr:`precursor_df` and :attr:`fragment_df`
-        The fragments in fragment_df can be located by 
-        `flat_frag_start_idx` and `flat_frag_stop_idx` in precursor_df. 
+        The fragments in fragment_df can be located by
+        `flat_frag_start_idx` and `flat_frag_stop_idx` in precursor_df.
 
         Parameters
         ----------
         library : SpecLibBase
             A library object with attributes
             `precursor_df`, `fragment_mz_df` and `fragment_intensity_df`.
-        
+
         keep_original_frag_dfs : bool, default True
-            If `fragment_mz_df` and `fragment_intensity_df` are 
+            If `fragment_mz_df` and `fragment_intensity_df` are
             kept in this library.
 
         copy_precursor_df : bool, default False
-            If True, make a copy of `precursor_df` from `library`, 
-            otherwise `flat_frag_start_idx` and `flat_frag_stop_idx` 
+            If True, make a copy of `precursor_df` from `library`,
+            otherwise `flat_frag_start_idx` and `flat_frag_stop_idx`
             columns will also append to the `library`.
         """
         self._precursor_df, self._fragment_df = flatten_fragments(
-            library.precursor_df.copy() if copy_precursor_df else library.precursor_df, 
-            library.fragment_mz_df, 
+            library.precursor_df.copy() if copy_precursor_df else library.precursor_df,
+            library.fragment_mz_df,
             library.fragment_intensity_df,
             min_fragment_intensity=self.min_fragment_intensity,
             keep_top_k_fragments=self.keep_top_k_fragments,
             custom_columns=self.custom_fragment_df_columns,
-            **kwargs
+            **kwargs,
         )
-        
-        if hasattr(library, 'protein_df'):
+
+        if hasattr(library, "protein_df"):
             self._protein_df = library.protein_df
         else:
             self._protein_df = pd.DataFrame()
 
         if keep_original_frag_dfs:
-
             self.charged_frag_types = library.fragment_mz_df.columns.values
             for dense_frag_df in library.available_dense_fragment_dfs():
                 setattr(self, dense_frag_df, getattr(library, dense_frag_df))
 
             warnings.warn(
                 "The SpecLibFlat object will have a strictly flat representation in the future. keep_original_frag_dfs=True will be deprecated.",
-                DeprecationWarning
+                DeprecationWarning,
             )
 
-
-    def save_hdf(self, hdf_file:str):
+    def save_hdf(self, hdf_file: str):
         """Save library dataframes into hdf_file.
         For `self.precursor_df`, this method will save it into two hdf groups:
         hdf_file: `library/precursor_df` and `library/mod_seq_df`.
 
-        `library/precursor_df` contains all essential numberic columns those 
+        `library/precursor_df` contains all essential numberic columns those
         can be loaded faster from hdf file into memory:
         `['precursor_mz', 'charge', 'mod_seq_hash', 'mod_seq_charge_hash',
-        'frag_start_idx', 'frag_stop_idx', 'flat_frag_start_idx', 'flat_frag_stop_idx', 
-        'decoy', 'rt_pred', 'ccs_pred', 'mobility_pred', 'miss_cleave', 'nAA', 
+        'frag_start_idx', 'frag_stop_idx', 'flat_frag_start_idx', 'flat_frag_stop_idx',
+        'decoy', 'rt_pred', 'ccs_pred', 'mobility_pred', 'miss_cleave', 'nAA',
         'isotope_mz_m1', 'isotope_intensity_m1', ...]`
 
-        `library/mod_seq_df` contains all string columns and the other 
+        `library/mod_seq_df` contains all string columns and the other
         not essential columns:
         'sequence','mods','mod_sites', ['proteins', 'genes']...
-        as well as 'mod_seq_hash', 'mod_seq_charge_hash' columns to map 
+        as well as 'mod_seq_hash', 'mod_seq_charge_hash' columns to map
         back to `precursor_df`
 
         Parameters
         ----------
         hdf_file : str
             the hdf file path to save
-            
+
         """
         super().save_hdf(hdf_file)
-        _hdf = HDF_File(
-            hdf_file,
-            read_only=False,
-            truncate=True,
-            delete_existing=False
-        )
+        _hdf = HDF_File(hdf_file, read_only=False, truncate=True, delete_existing=False)
         _hdf.library.fragment_df = self.fragment_df
         _hdf.library.protein_df = self.protein_df
         _hdf.library.fragment_mz_df = self.fragment_mz_df
         _hdf.library.fragment_intensity_df = self.fragment_intensity_df
-        
-    def load_hdf(self, hdf_file:str, load_mod_seq:bool=False):
+
+    def load_hdf(self, hdf_file: str, load_mod_seq: bool = False):
         """Load the hdf library from hdf_file
 
         Parameters
         ----------
         hdf_file : str
             hdf library path to load
 
         load_mod_seq : bool, optional
-            if also load mod_seq_df. 
+            if also load mod_seq_df.
             Defaults to False.
-            
+
         """
         super().load_hdf(hdf_file, load_mod_seq=load_mod_seq)
         _hdf = HDF_File(
             hdf_file,
         )
         self._fragment_df = _hdf.library.fragment_df.values
         self._protein_df = _hdf.library.protein_df.values
         self._fragment_mz_df = _hdf.library.fragment_mz_df.values
         self._fragment_intensity_df = _hdf.library.fragment_intensity_df.values
-        
-    def get_full_charged_types(self,frag_df:pd.DataFrame) -> list:
+
+    def get_full_charged_types(self, frag_df: pd.DataFrame) -> list:
         """
         Infer the full set of charged fragment types from the fragment dataframe
         by full we mean a complete set of fragment types for each charge
         so if we have a fragment b_z1 we should also have a fragment y_z1 and vice versa
 
         Parameters
         ----------
@@ -217,145 +217,181 @@
 
         Returns
         -------
         charged_frag_types : list
             The full set of charged fragment types in the form of a list of strings such as ['a_z1','b_z1','c_z1','x_z1','y_z1','z_z1']
 
         """
-        unique_charge_type_pairs = frag_df[['type','loss_type','charge']].drop_duplicates()
-        #Fragtypes from ascii to char
-        self.frag_types_as_char = {i: chr(i) for i in unique_charge_type_pairs['type'].unique()}
+        unique_charge_type_pairs = frag_df[
+            ["type", "loss_type", "charge"]
+        ].drop_duplicates()
+        # Fragtypes from ascii to char
+        self.frag_types_as_char = {
+            i: chr(i) for i in unique_charge_type_pairs["type"].unique()
+        }
 
         charged_frag_types = set()
         # Now if we have a fragment type that is a,b,c we should have the corresponding x,y,z
-        
-        corresponding = {
-            'a':'x',
-            'b':'y',
-            'c':'z',
-            'x':'a',
-            'y':'b',
-            'z':'c'
-        }
-        loss_number_to_type = {0: '', 18: '_H2O', 17: '_NH3',98: '_modloss'}
-        for type,loss,max_charge in unique_charge_type_pairs.values:
-            for possible_charge  in range(1,max_charge+1):
+
+        corresponding = {"a": "x", "b": "y", "c": "z", "x": "a", "y": "b", "z": "c"}
+        loss_number_to_type = {0: "", 18: "_H2O", 17: "_NH3", 98: "_modloss"}
+        for type, loss, max_charge in unique_charge_type_pairs.values:
+            for possible_charge in range(1, max_charge + 1):
                 # Add the string for this pair
-                charged_frag_types.add(f"{self.frag_types_as_char[type]}{loss_number_to_type[loss]}_z{possible_charge}")
+                charged_frag_types.add(
+                    f"{self.frag_types_as_char[type]}{loss_number_to_type[loss]}_z{possible_charge}"
+                )
                 # Add the string for the corresponding pair
-                charged_frag_types.add(f"{corresponding[self.frag_types_as_char[type]]}{loss_number_to_type[loss]}_z{possible_charge}")
+                charged_frag_types.add(
+                    f"{corresponding[self.frag_types_as_char[type]]}{loss_number_to_type[loss]}_z{possible_charge}"
+                )
         return list(charged_frag_types)
+
     def to_SpecLibBase(self) -> SpecLibBase:
         """
         Convert the flat library to SpecLibBase object.
 
         Returns:
         --------
         SpecLibBase
-            A SpecLibBase object with `precursor_df`, `fragment_mz_df` and `fragment_intensity_df`, and 
+            A SpecLibBase object with `precursor_df`, `fragment_mz_df` and `fragment_intensity_df`, and
             '_additional_fragment_columns_df' if there was more than mz and intensity in the original fragment_df.
         """
         # Check that fragment_df has the following columns ['mz', 'intensity', 'type', 'charge', 'position', 'loss_type']
-        assert  set(['mz', 'intensity', 'type', 'charge', 'position', 'loss_type']).issubset(self._fragment_df.columns), f'fragment_df does not have the following columns: {set(["mz", "intensity", "type", "charge", "position", "loss_type"]) - set(self._fragment_df.columns)}'
-        self.charged_frag_types = self.get_full_charged_types(self._fragment_df) # Infer the full set of charged fragment types from data
+        assert set(
+            ["mz", "intensity", "type", "charge", "position", "loss_type"]
+        ).issubset(
+            self._fragment_df.columns
+        ), f'fragment_df does not have the following columns: {set(["mz", "intensity", "type", "charge", "position", "loss_type"]) - set(self._fragment_df.columns)}'
+        self.charged_frag_types = self.get_full_charged_types(
+            self._fragment_df
+        )  # Infer the full set of charged fragment types from data
         # charged_frag_types = self.charged_frag_types #Use pre-defined charged_frag_types
-        frag_type_to_col_dict = dict(zip(
-            self.charged_frag_types,  
-            range(len(self.charged_frag_types))
-        ))
-        loss_number_to_type = {0: '', 18: '_H2O', 17: '_NH3',98: '_modloss'}
-    
-        available_frag_types = self._fragment_df['type'].unique()
+        frag_type_to_col_dict = dict(
+            zip(self.charged_frag_types, range(len(self.charged_frag_types)))
+        )
+        loss_number_to_type = {0: "", 18: "_H2O", 17: "_NH3", 98: "_modloss"}
+
+        available_frag_types = self._fragment_df["type"].unique()
         self.frag_types_as_char = {i: chr(i) for i in available_frag_types}
 
         frag_types_z_charge = (
-            self._fragment_df['type'].map(self.frag_types_as_char) + 
-            self._fragment_df['loss_type'].map(loss_number_to_type) + 
-            '_z' + 
-            self._fragment_df['charge'].astype(str)
+            self._fragment_df["type"].map(self.frag_types_as_char)
+            + self._fragment_df["loss_type"].map(loss_number_to_type)
+            + "_z"
+            + self._fragment_df["charge"].astype(str)
         )
 
-        #Print number of nAA less 1
-        accumlated_nAA = (self._precursor_df['nAA']-1).cumsum()
+        # Print number of nAA less 1
+        accumlated_nAA = (self._precursor_df["nAA"] - 1).cumsum()
         # Define intensity and mz as a matrix of shape (accumlated_nAA[-1], len(self.charged_frag_types), 2) - 2 for mz and intensity
-        intensity_and_mz = np.zeros((accumlated_nAA.iloc[-1], len(self.charged_frag_types), 2))
+        intensity_and_mz = np.zeros(
+            (accumlated_nAA.iloc[-1], len(self.charged_frag_types), 2)
+        )
 
         # Start indices for each precursor is the accumlated nAA of the previous precursor and for the first precursor is 0
         start_indexes = accumlated_nAA.shift(1).fillna(0).astype(int)
-        
-        
+
         column_indices = frag_types_z_charge.map(frag_type_to_col_dict)
 
         # We need to calculate for each fragment the precursor_idx that maps a fragment to a precursor
         drop_precursor_idx = False
-        if 'precursor_idx' not in self._fragment_df.columns:        
-            drop_precursor_idx = True    
+        if "precursor_idx" not in self._fragment_df.columns:
+            drop_precursor_idx = True
             # Sort precursor_df by 'flat_frag_start_idx'
-            self._precursor_df = self._precursor_df.sort_values('flat_frag_start_idx')
+            self._precursor_df = self._precursor_df.sort_values("flat_frag_start_idx")
             # Add precursor_idx to precursor_df as 0,1,2,3...
-            self._precursor_df['precursor_idx'] = range(self._precursor_df.shape[0])
+            self._precursor_df["precursor_idx"] = range(self._precursor_df.shape[0])
 
             # Add precursor_idx to fragment_df
-            frag_precursor_idx = np.repeat(self._precursor_df['precursor_idx'], self._precursor_df['flat_frag_stop_idx'] - self._precursor_df['flat_frag_start_idx'])
+            frag_precursor_idx = np.repeat(
+                self._precursor_df["precursor_idx"],
+                self._precursor_df["flat_frag_stop_idx"]
+                - self._precursor_df["flat_frag_start_idx"],
+            )
+
+            assert (
+                len(frag_precursor_idx) == self._fragment_df.shape[0]
+            ), f"Number of fragments {len(frag_precursor_idx)} is not equal to the number of rows in fragment_df {self._fragment_df.shape[0]}"
+
+            self._fragment_df["precursor_idx"] = frag_precursor_idx.values
+
+        # Row indices of a fragment being the accumlated nAA of the precursor + fragment position -1
+        precursor_idx_to_accumlated_nAA = dict(
+            zip(self._precursor_df["precursor_idx"], start_indexes)
+        )
+        row_indices = (
+            self._fragment_df["precursor_idx"].map(
+                precursor_idx_to_accumlated_nAA, na_action="ignore"
+            )
+            + self._fragment_df["position"]
+        )
 
-            assert len(frag_precursor_idx) == self._fragment_df.shape[0], f'Number of fragments {len(frag_precursor_idx)} is not equal to the number of rows in fragment_df {self._fragment_df.shape[0]}'
-        
-            self._fragment_df['precursor_idx'] = frag_precursor_idx.values
-
-        #Row indices of a fragment being the accumlated nAA of the precursor + fragment position -1
-        precursor_idx_to_accumlated_nAA = dict(zip(self._precursor_df['precursor_idx'], start_indexes))
-        row_indices = self._fragment_df['precursor_idx'].map(precursor_idx_to_accumlated_nAA,na_action = 'ignore') + self._fragment_df['position'] 
-        
         # Drop elements were the column_indices is nan and drop them from both row_indices and column_indices
         nan_indices = column_indices.index[column_indices.isna()]
         row_indices = row_indices.drop(nan_indices)
         column_indices = column_indices.drop(nan_indices)
 
-        assert row_indices.shape[0] == column_indices.shape[0], f'row_indices {row_indices.shape[0]} is not equal to column_indices {column_indices.shape[0]}'
+        assert (
+            row_indices.shape[0] == column_indices.shape[0]
+        ), f"row_indices {row_indices.shape[0]} is not equal to column_indices {column_indices.shape[0]}"
+
+        assert (
+            np.max(row_indices) <= intensity_and_mz.shape[0]
+        ), f"row_indices {np.max(row_indices)} is greater than the number of fragments {intensity_and_mz.shape[0]}"
 
-
-        assert np.max(row_indices) <= intensity_and_mz.shape[0], f'row_indices {np.max(row_indices)} is greater than the number of fragments {intensity_and_mz.shape[0]}'
-        
         # Assign the intensity and mz to the correct position in the matrix
-        intensity_indices = np.array((row_indices, column_indices,np.zeros_like(row_indices)), dtype=int).tolist()
-        mz_indices = np.array((row_indices, column_indices,np.ones_like(row_indices)), dtype=int).tolist()
-        
-        intensity_and_mz[tuple(intensity_indices)] = self._fragment_df['intensity']
-        intensity_and_mz[tuple(mz_indices)] = self._fragment_df['mz']
-
-        #Create fragment_mz_df and fragment_intensity_df
-        fragment_mz_df = pd.DataFrame(intensity_and_mz[:,:,1], columns = self.charged_frag_types)
-        fragment_intensity_df = pd.DataFrame(intensity_and_mz[:,:,0], columns = self.charged_frag_types)
-
-        #Add columns frag_start_idx and frag_stop_idx to the precursor_df
-        self._precursor_df['frag_start_idx'] = start_indexes
-        self._precursor_df['frag_stop_idx'] = accumlated_nAA
+        intensity_indices = np.array(
+            (row_indices, column_indices, np.zeros_like(row_indices)), dtype=int
+        ).tolist()
+        mz_indices = np.array(
+            (row_indices, column_indices, np.ones_like(row_indices)), dtype=int
+        ).tolist()
+
+        intensity_and_mz[tuple(intensity_indices)] = self._fragment_df["intensity"]
+        intensity_and_mz[tuple(mz_indices)] = self._fragment_df["mz"]
+
+        # Create fragment_mz_df and fragment_intensity_df
+        fragment_mz_df = pd.DataFrame(
+            intensity_and_mz[:, :, 1], columns=self.charged_frag_types
+        )
+        fragment_intensity_df = pd.DataFrame(
+            intensity_and_mz[:, :, 0], columns=self.charged_frag_types
+        )
 
-        #Drop precursor Idx from both fragment_df and precursor_df
-        if drop_precursor_idx:
-            self._fragment_df = self._fragment_df.drop(columns = ['precursor_idx'])
-            self._precursor_df = self._precursor_df.drop(columns = ['precursor_idx'])
+        # Add columns frag_start_idx and frag_stop_idx to the precursor_df
+        self._precursor_df["frag_start_idx"] = start_indexes
+        self._precursor_df["frag_stop_idx"] = accumlated_nAA
 
+        # Drop precursor Idx from both fragment_df and precursor_df
+        if drop_precursor_idx:
+            self._fragment_df = self._fragment_df.drop(columns=["precursor_idx"])
+            self._precursor_df = self._precursor_df.drop(columns=["precursor_idx"])
 
-        #Drop flat indices from precursor_df
-        self._precursor_df = self._precursor_df.drop(columns = ['flat_frag_start_idx','flat_frag_stop_idx'])
-        
-         
+        # Drop flat indices from precursor_df
+        self._precursor_df = self._precursor_df.drop(
+            columns=["flat_frag_start_idx", "flat_frag_stop_idx"]
+        )
 
-        #Create SpecLibBase object
+        # Create SpecLibBase object
         spec_lib_base = SpecLibBase()
         spec_lib_base._precursor_df = self._precursor_df
         spec_lib_base._fragment_mz_df = fragment_mz_df
         spec_lib_base._fragment_intensity_df = fragment_intensity_df
         spec_lib_base.charged_frag_types = self.charged_frag_types
-        
+
         #  Add additional columns from frag_df that were not mz and intensity
-        additional_columns = set(self._fragment_df.columns) - set(['mz','intensity','type','charge','position','loss_type'])
+        additional_columns = set(self._fragment_df.columns) - set(
+            ["mz", "intensity", "type", "charge", "position", "loss_type"]
+        )
         for col in additional_columns:
-            additional_matrix = np.zeros((accumlated_nAA.iloc[-1], len(self.charged_frag_types)))
+            additional_matrix = np.zeros(
+                (accumlated_nAA.iloc[-1], len(self.charged_frag_types))
+            )
             data_indices = np.array((row_indices, column_indices), dtype=int).tolist()
             additional_matrix[tuple(data_indices)] = self._fragment_df[col]
-            additional_df = pd.DataFrame(additional_matrix, columns = self.charged_frag_types)
-            setattr(spec_lib_base,f'_fragment_{col}_df',additional_df)
+            additional_df = pd.DataFrame(
+                additional_matrix, columns=self.charged_frag_types
+            )
+            setattr(spec_lib_base, f"_fragment_{col}_df", additional_df)
 
-        
-        return spec_lib_base
+        return spec_lib_base
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/reader.py` & `alphabase-1.2.4/alphabase/spectral_library/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 import typing
-import os
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from alphabase.peptide.mobility import mobility_to_ccs_for_df
-from alphabase.io.psm_reader.dia_search_reader import SpectronautReader
-from alphabase.io.psm_reader.maxquant_reader import MaxQuantReader
+from alphabase.psm_reader.maxquant_reader import MaxQuantReader
 from alphabase.spectral_library.base import SpecLibBase
 from alphabase.psm_reader.psm_reader import psm_reader_yaml
 from alphabase.psm_reader import psm_reader_provider
 
-from alphabase.constants._const import CONST_FILE_FOLDER, PEAK_INTENSITY_DTYPE
-from alphabase.yaml_utils import load_yaml
+from alphabase.constants._const import PEAK_INTENSITY_DTYPE
+
 
 class LibraryReaderBase(MaxQuantReader, SpecLibBase):
-    def __init__(self,
-        charged_frag_types:typing.List[str] = [
-            'b_z1','b_z2','y_z1', 'y_z2', 
-            'b_modloss_z1','b_modloss_z2',
-            'y_modloss_z1', 'y_modloss_z2'
+    def __init__(
+        self,
+        charged_frag_types: typing.List[str] = [
+            "b_z1",
+            "b_z2",
+            "y_z1",
+            "y_z2",
+            "b_modloss_z1",
+            "b_modloss_z2",
+            "y_modloss_z1",
+            "y_modloss_z2",
         ],
-        column_mapping:dict = None,
-        modification_mapping:dict = None,
-        fdr = 0.01,
-        fixed_C57 = False,
-        mod_seq_columns=psm_reader_yaml[
-            'library_reader_base'
-        ]['mod_seq_columns'],
-        rt_unit='irt',
-        precursor_mz_min:float = 400,
-        precursor_mz_max:float = 2000,
-        decoy:str = None,
-        **kwargs
+        column_mapping: dict = None,
+        modification_mapping: dict = None,
+        fdr=0.01,
+        fixed_C57=False,
+        mod_seq_columns=psm_reader_yaml["library_reader_base"]["mod_seq_columns"],
+        rt_unit="irt",
+        precursor_mz_min: float = 400,
+        precursor_mz_max: float = 2000,
+        decoy: str = None,
+        **kwargs,
     ):
         """
 
         Base class for reading spectral libraries from long format csv files.
 
         Parameters
         ----------
 
         charged_frag_types: list of str
             List of fragment types to be used in the spectral library.
             The default is ['b_z1','b_z2','y_z1', 'y_z2', 'b_modloss_z1','b_modloss_z2','y_modloss_z1', 'y_modloss_z2']
 
         column_mapping: dict
             Dictionary mapping the column names in the csv file to the column names in the spectral library.
-            The default is None, which uses the `library_reader_base` column mapping in `psm_reader.yaml` 
+            The default is None, which uses the `library_reader_base` column mapping in `psm_reader.yaml`
 
         modification_mapping: dict
             Dictionary mapping the modification names in the csv file to the modification names in the spectral library.
 
         fdr: float
             False discovery rate threshold for filtering the spectral library.
             default is 0.01
 
         fixed_C57: bool
-    
+
         mod_seq_columns: list of str
             List of column names in the csv file containing the modified sequence.
             By default the mapping is taken from `psm_reader.yaml`
 
         rt_unit: str
             Unit of the retention time column in the csv file.
             The default is 'irt'
@@ -73,269 +75,267 @@
             Maximum precursor m/z value for filtering the spectral library.
 
         decoy: str
             Decoy type for the spectral library.
             Can be either `pseudo_reverse` or `diann`
 
         """
-        SpecLibBase.__init__(self,
-            charged_frag_types = charged_frag_types,
+        SpecLibBase.__init__(
+            self,
+            charged_frag_types=charged_frag_types,
             precursor_mz_min=precursor_mz_min,
             precursor_mz_max=precursor_mz_max,
-            decoy=decoy
+            decoy=decoy,
         )
 
-        MaxQuantReader.__init__(self, 
-            column_mapping = column_mapping,
-            modification_mapping = modification_mapping,
-            fdr = fdr,
-            keep_decoy = False,
-            fixed_C57 = fixed_C57,
+        MaxQuantReader.__init__(
+            self,
+            column_mapping=column_mapping,
+            modification_mapping=modification_mapping,
+            fdr=fdr,
+            keep_decoy=False,
+            fixed_C57=fixed_C57,
             mod_seq_columns=mod_seq_columns,
             rt_unit=rt_unit,
         )
 
     def _init_column_mapping(self):
         """
         Initialize the column mapping from the `psm_reader.yaml` file.
         """
-        self.column_mapping = psm_reader_yaml[
-            'library_reader_base'
-        ]['column_mapping']
-
-    def _find_key_columns(self, lib_df:pd.DataFrame):
+        self.column_mapping = psm_reader_yaml["library_reader_base"]["column_mapping"]
 
+    def _find_key_columns(self, lib_df: pd.DataFrame):
         """
         Find and create the key columns for the spectral library.
 
         Parameters
         ----------
 
         lib_df: pd.DataFrame
             Dataframe containing the spectral library.
-        
+
         """
-        if 'fragment_loss_type' not in lib_df.columns:
-            lib_df['fragment_loss_type'] = ''
+        if "fragment_loss_type" not in lib_df.columns:
+            lib_df["fragment_loss_type"] = ""
 
-        lib_df.fillna({'fragment_loss_type':''}, inplace=True)
+        lib_df.fillna({"fragment_loss_type": ""}, inplace=True)
         lib_df.replace(
-            {'fragment_loss_type':'noloss'},
-            {'fragment_loss_type':''},inplace=True
+            {"fragment_loss_type": "noloss"}, {"fragment_loss_type": ""}, inplace=True
         )
 
-        if 'mods' not in lib_df.columns:
-            lib_df['mods'] = ''
+        if "mods" not in lib_df.columns:
+            lib_df["mods"] = ""
 
-        if 'mod_sites' not in lib_df.columns:
-            lib_df['mod_sites'] = ''
+        if "mod_sites" not in lib_df.columns:
+            lib_df["mod_sites"] = ""
 
-    def _get_fragment_intensity(self, lib_df:pd.DataFrame):
+    def _get_fragment_intensity(self, lib_df: pd.DataFrame):
         """
 
         Create the self._fragment_intensity dataframe from a given spectral library.
         In the process, the input dataframe is converted from long format to a precursor dataframe and returned.
 
         Parameters
         ----------
         lib_df: pd.DataFrame
             Dataframe containing the spectral library.
 
         Returns
         -------
         precursor_df: pd.DataFrame
             Dataframe containing the fragment intensity.
-        
+
         """
-        frag_col_dict = dict(zip(
-            self.charged_frag_types, 
-            range(len(self.charged_frag_types))
-        ))
+        frag_col_dict = dict(
+            zip(self.charged_frag_types, range(len(self.charged_frag_types)))
+        )
 
         self._find_key_columns(lib_df)
 
         # drop all columns which are all NaN as they prohibit grouping
-        lib_df = lib_df.dropna(axis=1, how='all')
+        lib_df = lib_df.dropna(axis=1, how="all")
 
         precursor_df_list = []
 
         frag_intens_list = []
         nAA_list = []
 
         fragment_columns = [
-            'fragment_mz','fragment_type','fragment_charge','fragment_series','fragment_loss_type','fragment_intensity'
+            "fragment_mz",
+            "fragment_type",
+            "fragment_charge",
+            "fragment_series",
+            "fragment_loss_type",
+            "fragment_intensity",
         ]
 
         # by default, all non-fragment columns are used to group the library
         non_fragment_columns = list(set(lib_df.columns) - set(fragment_columns))
 
-        
-        for keys, df_group in tqdm(lib_df.groupby(
-            non_fragment_columns
-        )):
+        for keys, df_group in tqdm(lib_df.groupby(non_fragment_columns)):
             precursor_columns = dict(zip(non_fragment_columns, keys))
 
-            nAA = len(precursor_columns['sequence'])
+            nAA = len(precursor_columns["sequence"])
 
             intens = np.zeros(
-                (nAA-1, len(self.charged_frag_types)),
+                (nAA - 1, len(self.charged_frag_types)),
                 dtype=PEAK_INTENSITY_DTYPE,
             )
             for frag_type, frag_num, loss_type, frag_charge, inten in df_group[
                 [
-                    'fragment_type','fragment_series','fragment_loss_type',
-                    'fragment_charge','fragment_intensity'
+                    "fragment_type",
+                    "fragment_series",
+                    "fragment_loss_type",
+                    "fragment_charge",
+                    "fragment_intensity",
                 ]
             ].values:
-                if frag_type in 'abc':
+                if frag_type in "abc":
                     frag_num -= 1
-                elif frag_type in 'xyz':
-                    frag_num = nAA-frag_num-1
+                elif frag_type in "xyz":
+                    frag_num = nAA - frag_num - 1
                 else:
                     continue
-                
-                if loss_type == '':
-                    frag_type = f'{frag_type}_z{frag_charge}'
-                elif loss_type == 'H3PO4':
-                    frag_type = f'{frag_type}_modloss_z{frag_charge}'
-                elif loss_type == 'H2O':
-                    frag_type = f'{frag_type}_H2O_z{frag_charge}'
-                elif loss_type == 'NH3':
-                    frag_type = f'{frag_type}_NH3_z{frag_charge}'
-                elif loss_type == 'unknown': # DiaNN+fragger
-                    frag_type = f'{frag_type}_z{frag_charge}'
+
+                if loss_type == "":
+                    frag_type = f"{frag_type}_z{frag_charge}"
+                elif loss_type == "H3PO4":
+                    frag_type = f"{frag_type}_modloss_z{frag_charge}"
+                elif loss_type == "H2O":
+                    frag_type = f"{frag_type}_H2O_z{frag_charge}"
+                elif loss_type == "NH3":
+                    frag_type = f"{frag_type}_NH3_z{frag_charge}"
+                elif loss_type == "unknown":  # DiaNN+fragger
+                    frag_type = f"{frag_type}_z{frag_charge}"
                 else:
                     continue
-                
+
                 if frag_type not in frag_col_dict:
                     continue
                 frag_col_idx = frag_col_dict[frag_type]
                 intens[frag_num, frag_col_idx] = inten
             max_inten = np.max(intens)
-            if max_inten <= 0: continue
+            if max_inten <= 0:
+                continue
             intens /= max_inten
 
-            precursor_df_list.append(precursor_columns) 
+            precursor_df_list.append(precursor_columns)
             frag_intens_list.append(intens)
             nAA_list.append(nAA)
 
         df = pd.DataFrame(precursor_df_list)
 
-
         self._fragment_intensity_df = pd.DataFrame(
-            np.concatenate(frag_intens_list),
-            columns = self.charged_frag_types
+            np.concatenate(frag_intens_list), columns=self.charged_frag_types
         )
 
-        indices = np.zeros(len(nAA_list)+1, dtype=np.int64)
-        indices[1:] = np.array(nAA_list)-1
+        indices = np.zeros(len(nAA_list) + 1, dtype=np.int64)
+        indices[1:] = np.array(nAA_list) - 1
         indices = np.cumsum(indices)
 
-        df['frag_start_idx'] = indices[:-1]
-        df['frag_stop_idx'] = indices[1:]
+        df["frag_start_idx"] = indices[:-1]
+        df["frag_stop_idx"] = indices[1:]
 
         return df
 
-    def _load_file(
-            self, 
-            filename:str
-        ):
+    def _load_file(self, filename: str):
         """
         Load the spectral library from a csv file.
         Reimplementation of `PSMReaderBase._translate_columns`.
         """
 
         csv_sep = self._get_table_delimiter(filename)
 
-        df = pd.read_csv(filename, sep=csv_sep,keep_default_na=False)
+        df = pd.read_csv(filename, sep=csv_sep, keep_default_na=False)
         self._find_mod_seq_column(df)
-        
+
         return df
 
-        
     def _post_process(
-        self, 
-        lib_df:pd.DataFrame,
-    ):  
+        self,
+        lib_df: pd.DataFrame,
+    ):
         """
         Process the spectral library and create the `fragment_intensity`, `fragment_mz`dataframe.
         Reimplementation of `PSMReaderBase._post_process`.
         """
 
         # identify unknown modifications
         len_before = len(self._psm_df)
-        self._psm_df = self._psm_df[
-            ~self._psm_df['mods'].isna()
-        ]
+        self._psm_df = self._psm_df[~self._psm_df["mods"].isna()]
         len_after = len(self._psm_df)
 
         if len_before != len_after:
             print(
-                f'{len_before-len_after} Entries with unknown modifications are removed'
-            ) 
-        
-        if 'nAA' not in self._psm_df.columns:
-            self._psm_df['nAA'] = self._psm_df.sequence.str.len()
+                f"{len_before-len_after} Entries with unknown modifications are removed"
+            )
+
+        if "nAA" not in self._psm_df.columns:
+            self._psm_df["nAA"] = self._psm_df.sequence.str.len()
 
         self._psm_df = self._get_fragment_intensity(self._psm_df)
-        
+
         self.normalize_rt_by_raw_name()
-        
-        if 'mobility' in self._psm_df.columns:
-            self._psm_df['ccs'] = (
-                mobility_to_ccs_for_df(
-                    self._psm_df,
-                    'mobility'
-                )
-            )
 
-        self._psm_df.drop('modified_sequence', axis=1, inplace=True)
+        if "mobility" in self._psm_df.columns:
+            self._psm_df["ccs"] = mobility_to_ccs_for_df(self._psm_df, "mobility")
+
+        self._psm_df.drop("modified_sequence", axis=1, inplace=True)
         self._precursor_df = self._psm_df
 
         self.calc_fragment_mz_df()
 
+
 # legacy
 SWATHLibraryReader = LibraryReaderBase
 
+
 class LibraryReaderFromRawData(SpecLibBase):
-    def __init__(self, 
-        charged_frag_types:typing.List[str] = [
-            'b_z1','b_z2','y_z1', 'y_z2', 
-            'b_modloss_z1','b_modloss_z2',
-            'y_modloss_z1', 'y_modloss_z2'
+    def __init__(
+        self,
+        charged_frag_types: typing.List[str] = [
+            "b_z1",
+            "b_z2",
+            "y_z1",
+            "y_z2",
+            "b_modloss_z1",
+            "b_modloss_z2",
+            "y_modloss_z1",
+            "y_modloss_z2",
         ],
-        precursor_mz_min:float = 400,
-        precursor_mz_max:float = 2000,
-        decoy:str = None,
-        **kwargs
+        precursor_mz_min: float = 400,
+        precursor_mz_max: float = 2000,
+        decoy: str = None,
+        **kwargs,
     ):
         super().__init__(
             charged_frag_types=charged_frag_types,
             precursor_mz_min=precursor_mz_min,
             precursor_mz_max=precursor_mz_max,
             decoy=decoy,
         )
-    
-    def import_psms(self, psm_files:list, psm_type:str):
+
+    def import_psms(self, psm_files: list, psm_type: str):
         psm_reader = psm_reader_provider.get_reader(psm_type)
         if isinstance(psm_files, str):
             self._precursor_df = psm_reader.import_file(psm_files)
             self._psm_df = self._precursor_df
         else:
             psm_df_list = []
             for psm_file in psm_files:
                 psm_df_list.append(psm_reader.import_file(psm_file))
             self._precursor_df = pd.concat(psm_df_list, ignore_index=True)
             self._psm_df = self._precursor_df
 
-    def extract_fragments(self, raw_files:list):
-        """ Include two steps:
+    def extract_fragments(self, raw_files: list):
+        """Include two steps:
             1. self.calc_fragment_mz_df() to generate self.fragment_mz_df
             2. Extract self.fragment_intensity_df from RAW files using AlphaRAW
 
         Parameters
         ----------
         raw_files : list
             RAW file paths
         """
         self.calc_fragment_mz_df()
-        # TODO Use AlphaRAW to extract fragment intensities
+        # TODO Use AlphaRAW to extract fragment intensities
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/translate.py` & `alphabase-1.2.4/alphabase/spectral_library/translate.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 from alphabase.constants.modification import MOD_DF
 
 from alphabase.spectral_library.base import SpecLibBase
 
 from alphabase.utils import explode_multiple_columns
 
-#@numba.njit #(cannot use numba for pd.Series)
+
+# @numba.njit #(cannot use numba for pd.Series)
 def create_modified_sequence(
-    seq_mods_sites:typing.Tuple, # must be ('sequence','mods','mod_sites')
-    translate_mod_dict:dict=None,
-    mod_sep='[]',
-    nterm = '_',
-    cterm = '_'
+    seq_mods_sites: typing.Tuple,  # must be ('sequence','mods','mod_sites')
+    translate_mod_dict: dict = None,
+    mod_sep="[]",
+    nterm="_",
+    cterm="_",
 ):
-    '''
+    """
     Translate `(sequence, mods, mod_sites)` into a modified sequence. Used by `df.apply()`.
     For example, `('ABCDEFG','Mod1@A;Mod2@E','1;5')`->`_A[Mod1@A]BCDE[Mod2@E]FG_`.
 
     Parameters
     ----------
     seq_mods_sites : List
         must be `(sequence, mods, mod_sites)`
@@ -32,101 +33,110 @@
         A dict to map AlphaX modification names to other software,
         use unimod name if None.
         Defaults to None.
 
     mod_sep : str
         '[]' or '()', default '[]'
 
-    '''
+    """
     mod_seq, mods, mod_sites = seq_mods_sites
     if mods:
-        mods = mods.split(';')
-        mod_sites = [int(i) for i in mod_sites.split(';')]
+        mods = mods.split(";")
+        mod_sites = [int(i) for i in mod_sites.split(";")]
         rev_order = np.argsort(mod_sites)[::-1]
         mod_sites = [mod_sites[rev_order[i]] for i in range(len(mod_sites))]
         mods = [mods[rev_order[i]] for i in range(len(mods))]
         if translate_mod_dict is None:
-            mods = [mod[:mod.find('@')] for mod in mods]
+            mods = [mod[: mod.find("@")] for mod in mods]
         else:
             mods = [translate_mod_dict[mod] for mod in mods]
         for _site, mod in zip(mod_sites, mods):
             if _site > 0:
-                mod_seq = mod_seq[:_site] + mod_sep[0]+mod+mod_sep[1] + mod_seq[_site:]
+                mod_seq = (
+                    mod_seq[:_site] + mod_sep[0] + mod + mod_sep[1] + mod_seq[_site:]
+                )
             elif _site == -1:
-                cterm += mod_sep[0]+mod+mod_sep[1]
+                cterm += mod_sep[0] + mod + mod_sep[1]
             elif _site == 0:
-                nterm += mod_sep[0]+mod+mod_sep[1]
+                nterm += mod_sep[0] + mod + mod_sep[1]
             else:
-                mod_seq = mod_seq[:_site] + mod_sep[0]+mod+mod_sep[1] + mod_seq[_site:]
+                mod_seq = (
+                    mod_seq[:_site] + mod_sep[0] + mod + mod_sep[1] + mod_seq[_site:]
+                )
     return nterm + mod_seq + cterm
 
+
 @numba.njit
-def _get_frag_info_from_column_name(column:str):
-    '''
+def _get_frag_info_from_column_name(column: str):
+    """
     Only used when converting alphabase libraries into other libraries
-    '''
-    idx = column.rfind('_')
+    """
+    idx = column.rfind("_")
     frag_type = column[:idx]
-    charge = column[idx+2:]
-    if len(frag_type)==1:
-        loss_type = 'noloss'
+    charge = column[idx + 2 :]
+    if len(frag_type) == 1:
+        loss_type = "noloss"
     else:
-        idx = frag_type.find('_')
-        loss_type = frag_type[idx+1:]
+        idx = frag_type.find("_")
+        loss_type = frag_type[idx + 1 :]
         frag_type = frag_type[0]
     return frag_type, loss_type, charge
 
+
 def _get_frag_num(columns, rows, frag_len):
     frag_nums = []
-    for r,c in zip(rows, columns):
+    for r, c in zip(rows, columns):
         if is_nterm_frag(c):
-            frag_nums.append(r+1)
+            frag_nums.append(r + 1)
         else:
-            frag_nums.append(frag_len-r)
+            frag_nums.append(frag_len - r)
     return frag_nums
 
+
 def merge_precursor_fragment_df(
-    precursor_df:pd.DataFrame, 
-    fragment_mz_df:pd.DataFrame, 
-    fragment_inten_df:pd.DataFrame, 
-    top_n_inten:int,
-    frag_type_head:str='FragmentType',
-    frag_mass_head:str='FragmentMz',
-    frag_inten_head:str='RelativeIntensity',
-    frag_charge_head:str='FragmentCharge',
-    frag_series_head:str='FragmentNumber',
-    frag_loss_head:str='FragmentLossType',
+    precursor_df: pd.DataFrame,
+    fragment_mz_df: pd.DataFrame,
+    fragment_inten_df: pd.DataFrame,
+    top_n_inten: int,
+    frag_type_head: str = "FragmentType",
+    frag_mass_head: str = "FragmentMz",
+    frag_inten_head: str = "RelativeIntensity",
+    frag_charge_head: str = "FragmentCharge",
+    frag_series_head: str = "FragmentNumber",
+    frag_loss_head: str = "FragmentLossType",
     verbose=True,
 ):
-    '''
-    Convert alphabase library into a single dataframe. 
-    This method is not important, as it will be only 
+    """
+    Convert alphabase library into a single dataframe.
+    This method is not important, as it will be only
     used by DiaNN, or spectronaut, or others
-    '''
+    """
     df = precursor_df.copy()
-    frag_columns = fragment_mz_df.columns.values.astype('U')
+    frag_columns = fragment_mz_df.columns.values.astype("U")
     frag_type_list = []
     frag_loss_list = []
     frag_charge_list = []
     frag_mass_list = []
     frag_inten_list = []
     frag_num_list = []
-    iters =  enumerate(df[['frag_start_idx','frag_stop_idx']].values)
+    iters = enumerate(df[["frag_start_idx", "frag_stop_idx"]].values)
     if verbose:
         iters = tqdm.tqdm(iters)
-    for i,(start, end) in iters:
-        intens = fragment_inten_df.iloc[start:end,:].to_numpy(copy=True) # is loc[start:end-1,:] faster?
+    for i, (start, end) in iters:
+        intens = fragment_inten_df.iloc[start:end, :].to_numpy(
+            copy=True
+        )  # is loc[start:end-1,:] faster?
         max_inten = np.amax(intens)
         if max_inten > 0:
             intens /= max_inten
-        masses = fragment_mz_df.iloc[start:end,:].values
+        masses = fragment_mz_df.iloc[start:end, :].values
         sorted_idx = np.argsort(intens.reshape(-1))[-top_n_inten:][::-1]
         idx_in_df = np.unravel_index(sorted_idx, masses.shape)
 
-        frag_len = end-start
+        frag_len = end - start
         rows = np.arange(frag_len, dtype=np.int32)[idx_in_df[0]]
         columns = frag_columns[idx_in_df[1]]
 
         frag_types, loss_types, charges = zip(
             *[_get_frag_info_from_column_name(_) for _ in columns]
         )
 
@@ -134,31 +144,32 @@
 
         frag_type_list.append(frag_types)
         frag_loss_list.append(loss_types)
         frag_charge_list.append(charges)
         frag_mass_list.append(masses[idx_in_df])
         frag_inten_list.append(intens[idx_in_df])
         frag_num_list.append(frag_nums)
-    
+
     df[frag_type_head] = frag_type_list
     df[frag_mass_head] = frag_mass_list
     df[frag_inten_head] = frag_inten_list
     df[frag_charge_head] = frag_charge_list
     df[frag_series_head] = frag_num_list
     df[frag_loss_head] = frag_loss_list
 
-    return explode_multiple_columns(df, 
+    return explode_multiple_columns(
+        df,
         [
             frag_type_head,
             frag_mass_head,
             frag_inten_head,
             frag_charge_head,
             frag_series_head,
             frag_loss_head,
-        ]
+        ],
     )
 
     # try:
     #     return df.explode([
     #         frag_type_head,
     #         frag_mass_head,
     #         frag_inten_head,
@@ -173,287 +184,300 @@
     #     df[frag_mass_head] = _flatten(frag_mass_list)
     #     df[frag_inten_head] = _flatten(frag_inten_list)
     #     df[frag_charge_head] = _flatten(frag_charge_list)
     #     df[frag_loss_head] = _flatten(frag_loss_list)
     #     df[frag_num_head] = _flatten(frag_num_list)
     #     return df
 
+
 mod_to_unimod_dict = {}
-for mod_name,unimod_id in MOD_DF[['mod_name','unimod_id']].values:
-    if unimod_id==-1 or unimod_id=='-1': continue
+for mod_name, unimod_id in MOD_DF[["mod_name", "unimod_id"]].values:
+    if unimod_id == -1 or unimod_id == "-1":
+        continue
     mod_to_unimod_dict[mod_name] = f"UniMod:{unimod_id}"
 
-def is_nterm_frag(frag_type:str):
-    return frag_type[0] in 'abc'
+
+def is_nterm_frag(frag_type: str):
+    return frag_type[0] in "abc"
+
 
 def mask_fragment_intensity_by_mz_(
-    fragment_mz_df:pd.DataFrame, 
-    fragment_intensity_df:pd.DataFrame,
-    min_frag_mz, max_frag_mz
+    fragment_mz_df: pd.DataFrame,
+    fragment_intensity_df: pd.DataFrame,
+    min_frag_mz,
+    max_frag_mz,
 ):
     fragment_intensity_df.mask(
-        (fragment_mz_df>max_frag_mz)|(fragment_mz_df<min_frag_mz),
-        0, inplace=True
+        (fragment_mz_df > max_frag_mz) | (fragment_mz_df < min_frag_mz), 0, inplace=True
     )
 
+
 def mask_fragment_intensity_by_frag_nAA(
-    fragment_intensity_df:pd.DataFrame,
-    precursor_df:pd.DataFrame,
-    max_mask_frag_nAA
+    fragment_intensity_df: pd.DataFrame, precursor_df: pd.DataFrame, max_mask_frag_nAA
 ):
-    if max_mask_frag_nAA <= 0: return
-    b_mask = np.zeros(
-        len(fragment_intensity_df), 
-        dtype=np.bool_
-    )
+    if max_mask_frag_nAA <= 0:
+        return
+    b_mask = np.zeros(len(fragment_intensity_df), dtype=np.bool_)
     y_mask = b_mask.copy()
     for i_frag in range(max_mask_frag_nAA):
-        b_mask[precursor_df.frag_start_idx.values+i_frag] = True
-        y_mask[precursor_df.frag_stop_idx.values-i_frag-1] = True
-    
+        b_mask[precursor_df.frag_start_idx.values + i_frag] = True
+        y_mask[precursor_df.frag_stop_idx.values - i_frag - 1] = True
+
     masks = np.zeros(
-        (
-            len(fragment_intensity_df),
-            len(fragment_intensity_df.columns)
-        ), dtype=np.bool_
+        (len(fragment_intensity_df), len(fragment_intensity_df.columns)), dtype=np.bool_
     )
-    for i,col in enumerate(fragment_intensity_df.columns.values):
+    for i, col in enumerate(fragment_intensity_df.columns.values):
         if is_nterm_frag(col):
-            masks[:,i] = b_mask
+            masks[:, i] = b_mask
         else:
-            masks[:,i] = y_mask
-    
-    fragment_intensity_df.mask(
-        masks, 0, inplace=True
-    )
+            masks[:, i] = y_mask
+
+    fragment_intensity_df.mask(masks, 0, inplace=True)
+
 
 def speclib_to_single_df(
-    speclib:SpecLibBase,
+    speclib: SpecLibBase,
     *,
-    translate_mod_dict:dict = None,
-    keep_k_highest_fragments:int=12,
-    min_frag_mz = 200,
-    max_frag_mz = 2000,
-    min_frag_intensity = 0.01,
-    min_frag_nAA = 0,
-    modloss:str='H3PO4',
-    frag_type_head:str='FragmentType',
-    frag_mass_head:str='FragmentMz',
-    frag_inten_head:str='RelativeIntensity',
-    frag_charge_head:str='FragmentCharge',
-    frag_loss_head:str='FragmentLossType',
-    frag_series_head:str='FragmentNumber',
-    verbose = True,
-)->pd.DataFrame:
-    '''
+    translate_mod_dict: dict = None,
+    keep_k_highest_fragments: int = 12,
+    min_frag_mz=200,
+    max_frag_mz=2000,
+    min_frag_intensity=0.01,
+    min_frag_nAA=0,
+    modloss: str = "H3PO4",
+    frag_type_head: str = "FragmentType",
+    frag_mass_head: str = "FragmentMz",
+    frag_inten_head: str = "RelativeIntensity",
+    frag_charge_head: str = "FragmentCharge",
+    frag_loss_head: str = "FragmentLossType",
+    frag_series_head: str = "FragmentNumber",
+    verbose=True,
+) -> pd.DataFrame:
+    """
     Convert alphabase library to diann (or Spectronaut) library dataframe
-    This method is not important, as it will be only 
+    This method is not important, as it will be only
     used by DiaNN, or spectronaut, or others
 
     Parameters
     ----------
     translate_mod_dict : dict
         A dict to map AlphaX modification names to other software,
         use unimod name if None.
         Defaults to None.
-    
+
     keep_k_highest_peaks : int
         only keep highest fragments for each precursor. Default: 12
 
     Returns
     -------
     pd.DataFrame
         a single dataframe in the SWATH-like format
 
-    '''
+    """
     df = pd.DataFrame()
-    df['ModifiedPeptide'] = speclib._precursor_df[
-        ['sequence','mods','mod_sites']
+    df["ModifiedPeptide"] = speclib._precursor_df[
+        ["sequence", "mods", "mod_sites"]
     ].apply(
-        create_modified_sequence, 
+        create_modified_sequence,
         axis=1,
         translate_mod_dict=translate_mod_dict,
-        mod_sep='[]'
+        mod_sep="[]",
     )
 
-    df['frag_start_idx'] = speclib._precursor_df['frag_start_idx']
-    df['frag_stop_idx'] = speclib._precursor_df['frag_stop_idx']
-    
-    df['PrecursorCharge'] = speclib._precursor_df['charge']
+    df["frag_start_idx"] = speclib._precursor_df["frag_start_idx"]
+    df["frag_stop_idx"] = speclib._precursor_df["frag_stop_idx"]
 
-    for rt_col in ['irt_pred','rt_pred','rt','irt','rt_norm']:
+    df["PrecursorCharge"] = speclib._precursor_df["charge"]
+
+    for rt_col in ["irt_pred", "rt_pred", "rt", "irt", "rt_norm"]:
         if rt_col in speclib.precursor_df.columns:
-            df['RT'] = speclib.precursor_df[rt_col]
+            df["RT"] = speclib.precursor_df[rt_col]
             break
-    if 'RT' not in df.columns:
-        raise ValueError('precursor_df must contain the RT columns')
+    if "RT" not in df.columns:
+        raise ValueError("precursor_df must contain the RT columns")
     # if 'irt_pred' in speclib._precursor_df.columns:
     #     df['RT'] = speclib._precursor_df['irt_pred']
     # elif 'rt_pred' in speclib._precursor_df.columns:
     #     df['RT'] = speclib._precursor_df['rt_pred']
     # elif 'rt_norm' in speclib._precursor_df.columns:
     #     df['RT'] = speclib._precursor_df['rt_norm']
     # else:
     #     raise ValueError('precursor_df must contain the "rt_pred" or "rt_norm" column')
 
-    for im_col in ['mobility_pred','mobility']:
+    for im_col in ["mobility_pred", "mobility"]:
         if im_col in speclib.precursor_df.columns:
-            df['IonMobility'] = speclib.precursor_df[im_col]
+            df["IonMobility"] = speclib.precursor_df[im_col]
             break
     # if 'mobility_pred' in speclib._precursor_df.columns:
     #     df['IonMobility'] = speclib._precursor_df.mobility_pred
     # elif 'mobility' in speclib._precursor_df.columns:
     #     df['IonMobility'] = speclib._precursor_df.mobility
-    
+
     # df['LabelModifiedSequence'] = df['ModifiedPeptide']
-    df['StrippedPeptide'] = speclib.precursor_df['sequence']
+    df["StrippedPeptide"] = speclib.precursor_df["sequence"]
 
-    if 'precursor_mz' not in speclib._precursor_df.columns:
+    if "precursor_mz" not in speclib._precursor_df.columns:
         speclib.calc_precursor_mz()
-    df['PrecursorMz'] = speclib._precursor_df['precursor_mz']
+    df["PrecursorMz"] = speclib._precursor_df["precursor_mz"]
 
-    for prot_col in ['uniprot_ids','proteins']:
+    for prot_col in ["uniprot_ids", "proteins"]:
         if prot_col in speclib.precursor_df.columns:
-            df['ProteinID'] = speclib.precursor_df[prot_col]
+            df["ProteinID"] = speclib.precursor_df[prot_col]
             break
     # if 'uniprot_ids' in speclib._precursor_df.columns:
     #     df['ProteinID'] = speclib._precursor_df.uniprot_ids
     # elif 'proteins' in speclib._precursor_df.columns:
     #     df['ProteinID'] = speclib._precursor_df.proteins
 
-    if 'genes' in speclib._precursor_df.columns:
-        df['Genes'] = speclib._precursor_df['genes']
+    if "genes" in speclib._precursor_df.columns:
+        df["Genes"] = speclib._precursor_df["genes"]
 
-    if 'decoy' in speclib._precursor_df.columns:
-        df['Decoy'] = speclib._precursor_df['decoy']
+    if "decoy" in speclib._precursor_df.columns:
+        df["Decoy"] = speclib._precursor_df["decoy"]
 
     # if 'protein_group' in speclib._precursor_df.columns:
     #     df['ProteinGroups'] = speclib._precursor_df['protein_group']
 
     if min_frag_mz > 0 or max_frag_mz > 0:
         mask_fragment_intensity_by_mz_(
             speclib._fragment_mz_df,
             speclib._fragment_intensity_df,
-            min_frag_mz, max_frag_mz
+            min_frag_mz,
+            max_frag_mz,
         )
 
     if min_frag_nAA > 0:
         mask_fragment_intensity_by_frag_nAA(
             speclib._fragment_intensity_df,
             speclib._precursor_df,
-            max_mask_frag_nAA=min_frag_nAA-1
+            max_mask_frag_nAA=min_frag_nAA - 1,
         )
 
     df = merge_precursor_fragment_df(
         df,
         speclib._fragment_mz_df,
         speclib._fragment_intensity_df,
         top_n_inten=keep_k_highest_fragments,
         frag_type_head=frag_type_head,
         frag_mass_head=frag_mass_head,
         frag_inten_head=frag_inten_head,
         frag_charge_head=frag_charge_head,
         frag_loss_head=frag_loss_head,
         frag_series_head=frag_series_head,
-        verbose=verbose
+        verbose=verbose,
     )
-    df = df[df['RelativeIntensity']>min_frag_intensity]
-    df.loc[df[frag_loss_head]=='modloss',frag_loss_head] = modloss
+    df = df[df["RelativeIntensity"] > min_frag_intensity]
+    df.loc[df[frag_loss_head] == "modloss", frag_loss_head] = modloss
+
+    return df.drop(["frag_start_idx", "frag_stop_idx"], axis=1)
 
-    return df.drop(['frag_start_idx','frag_stop_idx'], axis=1)
 
 def speclib_to_swath_df(
-    speclib:SpecLibBase,
+    speclib: SpecLibBase,
     *,
-    keep_k_highest_fragments:int=12,
-    min_frag_mz = 200,
-    max_frag_mz = 2000,
-    min_frag_intensity = 0.01,
-)->pd.DataFrame:
+    keep_k_highest_fragments: int = 12,
+    min_frag_mz=200,
+    max_frag_mz=2000,
+    min_frag_intensity=0.01,
+) -> pd.DataFrame:
     speclib_to_single_df(
-        speclib, 
+        speclib,
         translate_mod_dict=None,
         keep_k_highest_fragments=keep_k_highest_fragments,
-        min_frag_mz = min_frag_mz,
-        max_frag_mz = max_frag_mz,
-        min_frag_intensity = min_frag_intensity,
+        min_frag_mz=min_frag_mz,
+        max_frag_mz=max_frag_mz,
+        min_frag_intensity=min_frag_intensity,
     )
 
+
 class WritingProcess(mp.Process):
     def __init__(self, task_queue, tsv, *args, **kwargs):
-        self.task_queue:mp.Queue = task_queue
+        self.task_queue: mp.Queue = task_queue
         self.tsv = tsv
         super().__init__(*args, **kwargs)
 
     def run(self):
         while True:
             df, batch = self.task_queue.get()
-            if df is None: break
-            if tuple([int(i) for i in pd.__version__.split(".")[:2]]) >= (1,5):
-                newline=dict(lineterminator="\n")
+            if df is None:
+                break
+            if tuple([int(i) for i in pd.__version__.split(".")[:2]]) >= (1, 5):
+                newline = dict(lineterminator="\n")
             else:
-                newline=dict(line_terminator="\n")
-            df.to_csv(self.tsv, header=(batch==0), sep="\t", mode="a", index=False, **newline)
+                newline = dict(line_terminator="\n")
+            df.to_csv(
+                self.tsv,
+                header=(batch == 0),
+                sep="\t",
+                mode="a",
+                index=False,
+                **newline,
+            )
+
 
 def translate_to_tsv(
-    speclib:SpecLibBase,
-    tsv:str,
+    speclib: SpecLibBase,
+    tsv: str,
     *,
-    keep_k_highest_fragments:int=12,
-    min_frag_mz:float = 200,
-    max_frag_mz:float = 2000,
-    min_frag_intensity:float = 0.01,
-    min_frag_nAA:int = 0,
-    batch_size:int = 100000,
-    translate_mod_dict:dict = None,
-    multiprocessing:bool=True
+    keep_k_highest_fragments: int = 12,
+    min_frag_mz: float = 200,
+    max_frag_mz: float = 2000,
+    min_frag_intensity: float = 0.01,
+    min_frag_nAA: int = 0,
+    batch_size: int = 100000,
+    translate_mod_dict: dict = None,
+    multiprocessing: bool = True,
 ):
     if multiprocessing:
-        queue_size = 1000000//batch_size
+        queue_size = 1000000 // batch_size
         if queue_size < 2:
             queue_size = 2
         elif queue_size > 10:
             queue_size = 10
         df_head_queue = mp.Queue(maxsize=queue_size)
         writing_process = WritingProcess(df_head_queue, tsv)
         writing_process.start()
     mask_fragment_intensity_by_mz_(
         speclib._fragment_mz_df,
         speclib._fragment_intensity_df,
-        min_frag_mz, max_frag_mz
+        min_frag_mz,
+        max_frag_mz,
     )
     if min_frag_nAA > 0:
         mask_fragment_intensity_by_frag_nAA(
             speclib._fragment_intensity_df,
             speclib._precursor_df,
-            max_mask_frag_nAA=min_frag_nAA-1
+            max_mask_frag_nAA=min_frag_nAA - 1,
         )
     if isinstance(tsv, str):
-        with open(tsv, "w"): pass
+        with open(tsv, "w"):
+            pass
     _speclib = SpecLibBase()
     _speclib._fragment_intensity_df = speclib._fragment_intensity_df
     _speclib._fragment_mz_df = speclib._fragment_mz_df
     precursor_df = speclib._precursor_df
     for i in tqdm.tqdm(range(0, len(precursor_df), batch_size)):
-        _speclib._precursor_df = precursor_df.iloc[i:i+batch_size]
+        _speclib._precursor_df = precursor_df.iloc[i : i + batch_size]
         df = speclib_to_single_df(
-            _speclib, translate_mod_dict=translate_mod_dict,
+            _speclib,
+            translate_mod_dict=translate_mod_dict,
             keep_k_highest_fragments=keep_k_highest_fragments,
             min_frag_mz=0,
             max_frag_mz=0,
             min_frag_intensity=min_frag_intensity,
             min_frag_nAA=0,
-            verbose=False
+            verbose=False,
         )
         if multiprocessing:
             df_head_queue.put((df, i))
         else:
-            if tuple([int(i) for i in pd.__version__.split(".")[:2]]) >= (1,5):
-                newline=dict(lineterminator="\n")
+            if tuple([int(i) for i in pd.__version__.split(".")[:2]]) >= (1, 5):
+                newline = dict(lineterminator="\n")
             else:
-                newline=dict(line_terminator="\n")
-            df.to_csv(tsv, header=(i==0), sep="\t", mode='a', index=False, **newline)
+                newline = dict(line_terminator="\n")
+            df.to_csv(tsv, header=(i == 0), sep="\t", mode="a", index=False, **newline)
     if multiprocessing:
         df_head_queue.put((None, None))
-        print("Translation finished, it will take several minutes to export the rest precursors to the tsv file...")
+        print(
+            "Translation finished, it will take several minutes to export the rest precursors to the tsv file..."
+        )
         writing_process.join()
-
```

### Comparing `alphabase-1.2.3/alphabase/spectral_library/validate.py` & `alphabase-1.2.4/alphabase/spectral_library/validate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pandas as pd
 import numpy as np
 
 from typing import Union, List
 
-class Column():
+
+class Column:
     def __init__(
-            self, 
-            name : str, 
-            type : Union[str, type, np.dtype], 
-            allow_NaN : bool = False, 
-            allow_inf : bool = False
-        ):
+        self,
+        name: str,
+        type: Union[str, type, np.dtype],
+        allow_NaN: bool = False,
+        allow_inf: bool = False,
+    ):
         """
         Base class for validating a single column.
         The column is safely cast to the specified type inplace.
         NaN and inf values are checked.
 
         Parameters
         ----------
@@ -35,101 +36,104 @@
         ----------
 
         name: str
             Name of the column
 
         type: Union[type, np.dtype]
             Type of the column
-        
+
         """
 
         self.name = name
 
         if isinstance(type, str):
             self.type = np.dtype(type)
         else:
             self.type = type
 
         self.allow_NaN = allow_NaN
         self.allow_inf = allow_inf
 
-    def __call__(
-            self, 
-            df : pd.DataFrame
-            ):
+    def __call__(self, df: pd.DataFrame):
         """
         Validates the column.
 
         Parameters
         ----------
 
         df: pd.DataFrame
             Dataframe which contains the column.
 
         """
         if df[self.name].dtype != self.type:
             if np.can_cast(df[self.name].dtype, self.type):
                 df[self.name] = df[self.name].astype(self.type)
             else:
-                raise ValueError(f"Validation failed: Column {self.name} of type {_get_type_name(df[self.name].dtype)} cannot be cast to {_get_type_name(self.type)}")
-            
+                raise ValueError(
+                    f"Validation failed: Column {self.name} of type {_get_type_name(df[self.name].dtype)} cannot be cast to {_get_type_name(self.type)}"
+                )
+
         if not self.allow_NaN:
             if df[self.name].isna().any():
-                raise ValueError(f"Validation failed: Column {self.name} contains NaN values")
-            
+                raise ValueError(
+                    f"Validation failed: Column {self.name} contains NaN values"
+                )
+
         if not self.allow_inf:
             if not np.isfinite(df[self.name]).all():
-                raise ValueError(f"Validation failed: Column {self.name} contains inf values")
+                raise ValueError(
+                    f"Validation failed: Column {self.name} contains inf values"
+                )
+
 
 class Optional(Column):
     """
     Optional column to be validated.
     If the column is not present in the dataframe, the validation is skipped.
     """
+
     def __init__(self, *args, **kwargs):
         """
         Optional column
-        
+
         Parameters
         ----------
-        
+
         name: str
             Name of the column
-                
+
         type: type
             Type of the column
-            
+
         """
 
-        super().__init__( *args, **kwargs)
-        
+        super().__init__(*args, **kwargs)
 
-    def __call__(
-            self, 
-            df : pd.DataFrame
-        ):
+    def __call__(self, df: pd.DataFrame):
         """
         Casts the column to the specified type if it is present in the dataframe
 
         Parameters
         ----------
 
         df: pd.DataFrame
             Dataframe to validate
 
         """
 
         if self.name in df.columns:
             super().__call__(df)
 
+
 class Required(Column):
     """
     Required column to be validated.
     If the column is not present in the dataframe, the validation fails.
     """
+
     def __init__(self, *args, **kwargs):
         """
         Required column
 
         Parameters
         ----------
 
@@ -138,39 +142,36 @@
 
         type: type
             Type of the column
 
         """
         super().__init__(*args, **kwargs)
 
-    def __call__(
-            self, 
-            df : pd.DataFrame
-        ):
+    def __call__(self, df: pd.DataFrame):
         """
         Casts the column to the specified type if it is present in the dataframe
 
         Parameters
         ----------
 
         df: pd.DataFrame
             Dataframe to validate
 
         """
 
-        if self.name in df.columns:       
+        if self.name in df.columns:
             super().__call__(df)
         else:
-            raise ValueError(f"Validation failed: Column {self.name} is not present in the dataframe")
+            raise ValueError(
+                f"Validation failed: Column {self.name} is not present in the dataframe"
+            )
 
-class Schema():
-    def __init__(
-            self, 
-            name : str, 
-            properties: List[Column]):
+
+class Schema:
+    def __init__(self, name: str, properties: List[Column]):
         """
         Schema for validating dataframes
 
         Parameters
         ----------
 
         name: str
@@ -181,15 +182,15 @@
 
         """
 
         self.name = name
         self.schema = properties
         for column in self.schema:
             if not isinstance(column, Column):
-                raise ValueError(f"Schema must contain only Property objects")
+                raise ValueError("Schema must contain only Property objects")
 
     def __call__(self, df):
         """
         Validates the dataframe
 
         Parameters
         ----------
@@ -198,16 +199,16 @@
             Dataframe to validate
 
         """
 
         for column in self.schema:
             column(df)
 
-def _get_type_name(
-        type : Union[str, type, np.dtype]) -> str:
+
+def _get_type_name(type: Union[str, type, np.dtype]) -> str:
     """
     Returns the human readable name of the type
 
     Parameters
     ----------
 
     type: Union[str, type, np.dtype]
@@ -221,8 +222,8 @@
 
     """
     if isinstance(type, str):
         return type
     elif isinstance(type, np.dtype):
         return type.name
     else:
-        return type.__name__
+        return type.__name__
```

### Comparing `alphabase-1.2.3/alphabase/utils.py` & `alphabase-1.2.4/alphabase/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import tqdm
-import os
-import sys
 import pandas as pd
 import itertools
 import io
 
+
 # from alphatims
 def process_bar(iterator, len_iter):
     with tqdm.tqdm(total=len_iter) as bar:
         i = 0
-        for i,iter in enumerate(iterator):
+        for i, iter in enumerate(iterator):
             yield iter
             bar.update()
-        bar.update(len_iter-i-1)
+        bar.update(len_iter - i - 1)
+
 
 def _flatten(list_of_lists):
-    '''
+    """
     Flatten a list of lists
-    '''
-    return list(
-        itertools.chain.from_iterable(list_of_lists)
-    )
+    """
+    return list(itertools.chain.from_iterable(list_of_lists))
+
 
-def explode_multiple_columns(df:pd.DataFrame, columns:list):
+def explode_multiple_columns(df: pd.DataFrame, columns: list):
     try:
         return df.explode(columns)
     except ValueError:
         # pandas < 1.3.0
-        print(f'pandas=={pd.__version__} cannot explode multiple columns')
+        print(f"pandas=={pd.__version__} cannot explode multiple columns")
         ret_df = df.explode(columns[0])
         for col in columns[1:]:
             ret_df[col] = _flatten(df[col].values)
         return ret_df
 
-def get_delimiter(tsv_file:str):
+
+def get_delimiter(tsv_file: str):
     if isinstance(tsv_file, io.StringIO):
         # for unit tests
         line = tsv_file.readline().strip()
         tsv_file.seek(0)
     else:
         with open(tsv_file, "r") as f:
             line = f.readline().strip()
-    if '\t' in line: return '\t'
-    elif ',' in line: return ','
-    else: return '\t'
+    if "\t" in line:
+        return "\t"
+    elif "," in line:
+        return ","
+    else:
+        return "\t"
```

### Comparing `alphabase-1.2.3/alphabase.egg-info/PKG-INFO` & `alphabase-1.2.4/alphabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabase
-Version: 1.2.3
+Version: 1.2.4
 Summary: An infrastructure Python package of the AlphaX ecosystem
 Home-page: https://github.com/MannLabs/alphabase
 Author: Mann Labs
 Author-email: jalew188@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
@@ -33,22 +33,23 @@
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn
 Requires-Dist: regex
 Requires-Dist: dask
 Requires-Dist: dask_expr
 Requires-Dist: pyahocorasick
+Requires-Dist: pyteomics
+Requires-Dist: lxml
 Requires-Dist: pywin32; sys_platform == "win32"
 Provides-Extra: development-stable
 Requires-Dist: jupyter; extra == "development-stable"
 Requires-Dist: twine; extra == "development-stable"
 Requires-Dist: bumpversion; extra == "development-stable"
 Requires-Dist: pipdeptree; extra == "development-stable"
 Requires-Dist: ipykernel; extra == "development-stable"
-Requires-Dist: nbdev; extra == "development-stable"
 Requires-Dist: pyteomics; extra == "development-stable"
 Requires-Dist: scikit-learn; extra == "development-stable"
 Requires-Dist: matplotlib; extra == "development-stable"
 Requires-Dist: autodocsumm; extra == "development-stable"
 Requires-Dist: myst_parser; extra == "development-stable"
 Requires-Dist: sphinx; extra == "development-stable"
 Requires-Dist: nbsphinx; extra == "development-stable"
@@ -65,21 +66,22 @@
 Requires-Dist: h5py; extra == "development-stable"
 Requires-Dist: contextlib2; extra == "development-stable"
 Requires-Dist: xxhash; extra == "development-stable"
 Requires-Dist: regex; extra == "development-stable"
 Requires-Dist: pydivsufsort; extra == "development-stable"
 Requires-Dist: pyahocorasick; extra == "development-stable"
 Requires-Dist: pytest; extra == "development-stable"
+Requires-Dist: pre-commit==3.7.0; extra == "development-stable"
+Requires-Dist: nbmake==1.5.3; extra == "development-stable"
 Provides-Extra: development
 Requires-Dist: jupyter; extra == "development"
 Requires-Dist: twine; extra == "development"
 Requires-Dist: bumpversion; extra == "development"
 Requires-Dist: pipdeptree; extra == "development"
 Requires-Dist: ipykernel; extra == "development"
-Requires-Dist: nbdev; extra == "development"
 Requires-Dist: pyteomics; extra == "development"
 Requires-Dist: scikit-learn; extra == "development"
 Requires-Dist: matplotlib; extra == "development"
 Requires-Dist: autodocsumm; extra == "development"
 Requires-Dist: myst_parser; extra == "development"
 Requires-Dist: sphinx; extra == "development"
 Requires-Dist: nbsphinx; extra == "development"
@@ -96,14 +98,16 @@
 Requires-Dist: h5py; extra == "development"
 Requires-Dist: contextlib2; extra == "development"
 Requires-Dist: xxhash; extra == "development"
 Requires-Dist: regex; extra == "development"
 Requires-Dist: pydivsufsort; extra == "development"
 Requires-Dist: pyahocorasick; extra == "development"
 Requires-Dist: pytest; extra == "development"
+Requires-Dist: pre-commit; extra == "development"
+Requires-Dist: nbmake; extra == "development"
 Provides-Extra: stable
 Requires-Dist: numba; extra == "stable"
 Requires-Dist: numpy; extra == "stable"
 Requires-Dist: pyyaml; extra == "stable"
 Requires-Dist: pandas; extra == "stable"
 Requires-Dist: h5py; extra == "stable"
 Requires-Dist: contextlib2; extra == "stable"
@@ -112,14 +116,16 @@
 Requires-Dist: psutil; extra == "stable"
 Requires-Dist: tqdm; extra == "stable"
 Requires-Dist: scikit-learn; extra == "stable"
 Requires-Dist: regex; extra == "stable"
 Requires-Dist: dask; extra == "stable"
 Requires-Dist: dask_expr; extra == "stable"
 Requires-Dist: pyahocorasick; extra == "stable"
+Requires-Dist: pyteomics; extra == "stable"
+Requires-Dist: lxml; extra == "stable"
 
 # AlphaBase
 
 ![Pip installation](https://github.com/MannLabs/alphabase/workflows/Default%20installation%20and%20tests/badge.svg)
 ![PyPi releases](https://github.com/MannLabs/alphabase/workflows/Publish%20on%20PyPi%20and%20release%20on%20GitHub/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/alphabase/badge/?version=latest)](https://alphabase.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/alphabase)](https://pypi.org/project/alphabase)
@@ -311,13 +317,27 @@
 a new [issue](https://github.com/MannLabs/alphabase/issues) or clone the
 repository and create a [pull
 request](https://github.com/MannLabs/alphabase/pulls) with a new branch.
 For an even more interactive participation, check out the
 [discussions](https://github.com/MannLabs/alphabase/discussions) and the
 [the Contributors License Agreement](misc/CLA.md).
 
+### Notes for developers
+#### pre-commit hooks
+It is highly recommended to use the provided pre-commit hooks, as the CI pipeline enforces all checks therein to
+pass in order to merge a branch.
+
+The hooks need to be installed once by
+```bash
+pre-commit install
+```
+You can run the checks yourself using:
+```bash
+pre-commit run --all-files
+```
+
 ------------------------------------------------------------------------
 
 ## Changelog
 
 See the [HISTORY.md](HISTORY.md) for a full overview of the changes made
 in each version.
```

### Comparing `alphabase-1.2.3/alphabase.egg-info/SOURCES.txt` & `alphabase-1.2.4/alphabase.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 alphabase/__init__.py
-alphabase/_modidx.py
 alphabase/cli.py
 alphabase/gui.py
 alphabase/utils.py
 alphabase/yaml_utils.py
 alphabase.egg-info/PKG-INFO
 alphabase.egg-info/SOURCES.txt
 alphabase.egg-info/dependency_links.txt
@@ -32,22 +32,14 @@
 alphabase/constants/const_files/nist_element.yaml
 alphabase/constants/const_files/protease.yaml
 alphabase/constants/const_files/psm_reader.yaml
 alphabase/constants/const_files/quant_reader_config.yaml
 alphabase/io/__init__.py
 alphabase/io/hdf.py
 alphabase/io/tempmmap.py
-alphabase/io/psm_reader/__init__.py
-alphabase/io/psm_reader/alphapept_reader.py
-alphabase/io/psm_reader/dia_psm_reader.py
-alphabase/io/psm_reader/dia_search_reader.py
-alphabase/io/psm_reader/maxquant_reader.py
-alphabase/io/psm_reader/msfragger_reader.py
-alphabase/io/psm_reader/pfind_reader.py
-alphabase/io/psm_reader/psm_reader.py
 alphabase/peptide/__init__.py
 alphabase/peptide/fragment.py
 alphabase/peptide/mass_calc.py
 alphabase/peptide/mobility.py
 alphabase/peptide/precursor.py
 alphabase/protein/__init__.py
 alphabase/protein/fasta.py
@@ -65,22 +57,16 @@
 alphabase/quantification/quant_reader/config_dict_loader.py
 alphabase/quantification/quant_reader/longformat_reader.py
 alphabase/quantification/quant_reader/plexdia_reformatter.py
 alphabase/quantification/quant_reader/quant_reader_manager.py
 alphabase/quantification/quant_reader/quantreader_utils.py
 alphabase/quantification/quant_reader/table_reformatter.py
 alphabase/quantification/quant_reader/wideformat_reader.py
-alphabase/scoring/__init__.py
-alphabase/scoring/fdr.py
-alphabase/scoring/feature_extraction_base.py
-alphabase/scoring/ml_scoring.py
 alphabase/spectral_library/__init__.py
 alphabase/spectral_library/base.py
 alphabase/spectral_library/decoy.py
 alphabase/spectral_library/flat.py
 alphabase/spectral_library/reader.py
 alphabase/spectral_library/translate.py
 alphabase/spectral_library/validate.py
-alphabase/statistics/__init__.py
-alphabase/statistics/regression.py
 tests/test_cli.py
 tests/test_gui.py
```

### Comparing `alphabase-1.2.3/alphabase.egg-info/requires.txt` & `alphabase-1.2.4/alphabase.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 psutil
 tqdm
 scikit-learn
 regex
 dask
 dask_expr
 pyahocorasick
+pyteomics
+lxml
 
 [:sys_platform == "win32"]
 pywin32
 
 [development]
 jupyter
 twine
 bumpversion
 pipdeptree
 ipykernel
-nbdev
 pyteomics
 scikit-learn
 matplotlib
 autodocsumm
 myst_parser
 sphinx
 nbsphinx
@@ -44,22 +45,23 @@
 h5py
 contextlib2
 xxhash
 regex
 pydivsufsort
 pyahocorasick
 pytest
+pre-commit
+nbmake
 
 [development-stable]
 jupyter
 twine
 bumpversion
 pipdeptree
 ipykernel
-nbdev
 pyteomics
 scikit-learn
 matplotlib
 autodocsumm
 myst_parser
 sphinx
 nbsphinx
@@ -76,14 +78,16 @@
 h5py
 contextlib2
 xxhash
 regex
 pydivsufsort
 pyahocorasick
 pytest
+pre-commit==3.7.0
+nbmake==1.5.3
 
 [stable]
 numba
 numpy
 pyyaml
 pandas
 h5py
@@ -93,7 +97,9 @@
 psutil
 tqdm
 scikit-learn
 regex
 dask
 dask_expr
 pyahocorasick
+pyteomics
+lxml
```

### Comparing `alphabase-1.2.3/setup.py` & `alphabase-1.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 #!python
 
 # builtin
 import setuptools
 import re
-import os
+
 # local
 import alphabase as package2install
 
-#nbdev2
-# from configparser import ConfigParser
-# nbdev_config = ConfigParser(delimiters=['='])
-# nbdev_config.read('settings.ini')
-# nbdev_cfg = nbdev_config['DEFAULT']
 
 def get_long_description():
     with open("README.md", "r") as readme_file:
         long_description = readme_file.read()
     return long_description
 
 
@@ -30,15 +25,15 @@
             else:
                 extra_stable = "stable"
             extra_requirements[extra_stable] = []
             extra_requirements[extra] = []
             for line in requirements_file:
                 extra_requirements[extra_stable].append(line)
                 # conditional req like: "pywin32==xxx; sys_platform=='win32'"
-                line, *conditions = line.split(';')
+                line, *conditions = line.split(";")
                 requirement, *comparison = re.split("[><=~!]", line)
                 requirement = requirement.strip()
                 requirement = ";".join([requirement] + conditions)
                 extra_requirements[extra].append(requirement)
     requirements = extra_requirements.pop("")
     return requirements, extra_requirements
 
@@ -58,17 +53,17 @@
         project_urls=package2install.__urls__,
         keywords=package2install.__keywords__,
         classifiers=package2install.__classifiers__,
         packages=[package2install.__project__],
         include_package_data=True,
         entry_points={
             "console_scripts": package2install.__console_scripts__,
-            # 'nbdev': [f'{nbdev_cfg.get("lib_path")}={nbdev_cfg.get("lib_path")}._modidx:d'],
         },
-        install_requires=requirements + [
+        install_requires=requirements
+        + [
             # TODO Remove hardcoded requirement?
             "pywin32; sys_platform=='win32'"
         ],
         extras_require=extra_requirements,
         python_requires=package2install.__python_version__,
     )
```

