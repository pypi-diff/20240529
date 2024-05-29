# Comparing `tmp/kan_gpt-1.0.4.tar.gz` & `tmp/kan_gpt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kan_gpt-1.0.4.tar", last modified: Fri May 17 06:32:35 2024, max compression
+gzip compressed data, was "kan_gpt-1.0.5.tar", last modified: Wed May 29 05:21:18 2024, max compression
```

## Comparing `kan_gpt-1.0.4.tar` & `kan_gpt-1.0.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.638014 kan_gpt-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-17 06:32:35.638014 kan_gpt-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.626014 kan_gpt-1.0.4/kan_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/download_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.630015 kan_gpt-1.0.4/kan_gpt/efficient_kan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/efficient_kan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/efficient_kan/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.630015 kan_gpt-1.0.4/kan_gpt/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    57987 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.634014 kan_gpt-1.0.4/kan_gpt/kan/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_3.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_4.png
--rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_0_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_1_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_2_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_3_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.634014 kan_gpt-1.0.4/kan_gpt/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/mingpt/bpe.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20656 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/kan_gpt/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.638014 kan_gpt-1.0.4/kan_gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 06:32:35.000000 kan_gpt-1.0.4/kan_gpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:32:35.638014 kan_gpt-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:35.634014 kan_gpt-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_dataset_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_efficient_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_gpt_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_gpt_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_kan.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 06:32:23.000000 kan_gpt-1.0.4/tests/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.810168 kan_gpt-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-29 05:21:18.810168 kan_gpt-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.802168 kan_gpt-1.0.5/kan_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/download_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.802168 kan_gpt-1.0.5/kan_gpt/efficient_kan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/efficient_kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10580 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/efficient_kan/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.802168 kan_gpt-1.0.5/kan_gpt/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    57987 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16546 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17589 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.806168 kan_gpt-1.0.5/kan_gpt/kan/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    20912 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24594 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20473 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23921 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_0_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_1_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_2_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_3_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.806168 kan_gpt-1.0.5/kan_gpt/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/mingpt/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16530 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20656 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/kan_gpt/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.810168 kan_gpt-1.0.5/kan_gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 05:21:18.000000 kan_gpt-1.0.5/kan_gpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 05:21:18.810168 kan_gpt-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:18.810168 kan_gpt-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_dataset_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_efficient_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_gpt_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_gpt_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-29 05:21:10.000000 kan_gpt-1.0.5/tests/test_train.py
```

### Comparing `kan_gpt-1.0.4/HISTORY.md` & `kan_gpt-1.0.5/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Docs(README): citation. [Aditya NG]
+
+
+1.0.4 (2024-05-17)
+------------------
+- Release: version 1.0.4 🚀 [Aditya NG]
 - Docs(README): total downloads badge. [Aditya NG]
 
 
 1.0.3 (2024-05-17)
 ------------------
 - Release: version 1.0.3 🚀 [Aditya NG]
 - Test(.coveragerc): excluded few files for now. [Aditya NG]
```

### Comparing `kan_gpt-1.0.4/LICENSE` & `kan_gpt-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/PKG-INFO` & `kan_gpt-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -44,14 +44,29 @@
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
+## Citation
+
+If you find our work useful cite us!
+
+```
+@misc{GANESH2024KANGPT,
+  author       = {Aditya Nalgunda Ganesh},
+  title        = {KAN-GPT: The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling},
+  year         = {2024},
+  month        = {May},
+  note         = {Release 1.0.0, 9th May 2024},
+  url          = {https://github.com/AdityaNG/kan-gpt/}
+}
+```
+
 ## Usage
 
 Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
```

### Comparing `kan_gpt-1.0.4/README.md` & `kan_gpt-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,29 @@
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
+## Citation
+
+If you find our work useful cite us!
+
+```
+@misc{GANESH2024KANGPT,
+  author       = {Aditya Nalgunda Ganesh},
+  title        = {KAN-GPT: The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling},
+  year         = {2024},
+  month        = {May},
+  note         = {Release 1.0.0, 9th May 2024},
+  url          = {https://github.com/AdityaNG/kan-gpt/}
+}
+```
+
 ## Usage
 
 Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
```

### Comparing `kan_gpt-1.0.4/kan_gpt/cli.py` & `kan_gpt-1.0.5/kan_gpt/cli.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/dataset.py` & `kan_gpt-1.0.5/kan_gpt/dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/download_dataset.py` & `kan_gpt-1.0.5/kan_gpt/download_dataset.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/efficient_kan/model.py` & `kan_gpt-1.0.5/kan_gpt/efficient_kan/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/KAN.py` & `kan_gpt-1.0.5/kan_gpt/kan/KAN.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/KANLayer.py` & `kan_gpt-1.0.5/kan_gpt/kan/KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/LBFGS.py` & `kan_gpt-1.0.5/kan_gpt/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/Symbolic_KANLayer.py` & `kan_gpt-1.0.5/kan_gpt/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_1.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_2.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_3.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_0_4.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_0_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_1.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_1.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_2.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_2.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_3.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_3.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_0_1_4.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_0_1_4.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_0_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_0_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_1_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_1_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_2_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_2_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_3_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_3_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/figures/sp_1_4_0.png` & `kan_gpt-1.0.5/kan_gpt/kan/figures/sp_1_4_0.png`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/spline.py` & `kan_gpt-1.0.5/kan_gpt/kan/spline.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/kan/utils.py` & `kan_gpt-1.0.5/kan_gpt/kan/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/mingpt/bpe.py` & `kan_gpt-1.0.5/kan_gpt/mingpt/bpe.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/mingpt/model.py` & `kan_gpt-1.0.5/kan_gpt/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/mingpt/trainer.py` & `kan_gpt-1.0.5/kan_gpt/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/mingpt/utils.py` & `kan_gpt-1.0.5/kan_gpt/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/model.py` & `kan_gpt-1.0.5/kan_gpt/model.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/prompt.py` & `kan_gpt-1.0.5/kan_gpt/prompt.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/sweep.py` & `kan_gpt-1.0.5/kan_gpt/sweep.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt/train.py` & `kan_gpt-1.0.5/kan_gpt/train.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/kan_gpt.egg-info/PKG-INFO` & `kan_gpt-1.0.5/kan_gpt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kan_gpt
-Version: 1.0.4
+Version: 1.0.5
 Summary: Awesome kan_gpt created by AdityaNG
 Home-page: https://github.com/AdityaNG/kan-gpt/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib==3.6.2
 Requires-Dist: numpy==1.24.4
@@ -44,14 +44,29 @@
 
 ## Install it from PyPI
 
 ```bash
 pip install kan_gpt
 ```
 
+## Citation
+
+If you find our work useful cite us!
+
+```
+@misc{GANESH2024KANGPT,
+  author       = {Aditya Nalgunda Ganesh},
+  title        = {KAN-GPT: The PyTorch implementation of Generative Pre-trained Transformers (GPTs) using Kolmogorov-Arnold Networks (KANs) for language modeling},
+  year         = {2024},
+  month        = {May},
+  note         = {Release 1.0.0, 9th May 2024},
+  url          = {https://github.com/AdityaNG/kan-gpt/}
+}
+```
+
 ## Usage
 
 Refer to the [KAN_GPT.ipynb](https://github.com/AdityaNG/kan-gpt/blob/main/KAN_GPT.ipynb) and [kan_gpt/prompt.py](https://github.com/AdityaNG/kan-gpt/blob/main/kan_gpt/prompt.py) for usage examples. The following is an outline of how to use the model:
 
 ```py
 from kan_gpt.model import GPT
 from transformers import GPT2Tokenizer
```

### Comparing `kan_gpt-1.0.4/kan_gpt.egg-info/SOURCES.txt` & `kan_gpt-1.0.5/kan_gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/setup.py` & `kan_gpt-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_dataset_download.py` & `kan_gpt-1.0.5/tests/test_dataset_download.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_efficient_kan.py` & `kan_gpt-1.0.5/tests/test_efficient_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_gpt_kan.py` & `kan_gpt-1.0.5/tests/test_gpt_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_gpt_mlp.py` & `kan_gpt-1.0.5/tests/test_gpt_mlp.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_kan.py` & `kan_gpt-1.0.5/tests/test_kan.py`

 * *Files identical despite different names*

### Comparing `kan_gpt-1.0.4/tests/test_train.py` & `kan_gpt-1.0.5/tests/test_train.py`

 * *Files identical despite different names*

