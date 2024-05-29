# Comparing `tmp/figaro-1.6.6.tar.gz` & `tmp/figaro-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.6.tar", last modified: Tue May 14 11:43:09 2024, max compression
+gzip compressed data, was "figaro-1.6.8.tar", last modified: Wed May 29 13:46:36 2024, max compression
```

## Comparing `figaro-1.6.6.tar` & `figaro-1.6.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.524160 figaro-1.6.6/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.6/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.6/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6875 2024-05-14 11:43:09.523892 figaro-1.6.6/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4156 2024-05-14 11:29:40.000000 figaro-1.6.6/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.504094 figaro-1.6.6/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.509467 figaro-1.6.6/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      332 2024-05-08 10:09:00.000000 figaro-1.6.6/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.6/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:08.000000 figaro-1.6.6/docs/source/figaro.rate.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      308 2024-05-10 07:52:32.000000 figaro-1.6.6/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.512403 figaro-1.6.6/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.6/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1804 2024-05-14 11:37:40.000000 figaro-1.6.6/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.519893 figaro-1.6.6/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.6/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.6/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.6/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.522722 figaro-1.6.6/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.6/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    20100 2024-05-13 16:05:40.000000 figaro-1.6.6/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    23562 2024-05-13 16:05:53.000000 figaro-1.6.6/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10988 2024-05-13 16:06:33.000000 figaro-1.6.6/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9798 2024-05-13 16:06:51.000000 figaro-1.6.6/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2822 2024-05-13 14:47:26.000000 figaro-1.6.6/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.6/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.6/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1364 2024-05-10 09:51:02.000000 figaro-1.6.6/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-05-14 11:13:06.000000 figaro-1.6.6/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.6/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    36461 2024-05-14 07:34:00.000000 figaro-1.6.6/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.6/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    55445 2024-05-14 09:03:30.000000 figaro-1.6.6/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.6/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40563 2024-04-26 15:09:38.000000 figaro-1.6.6/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.6/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    12084 2024-04-24 15:08:47.000000 figaro-1.6.6/figaro/rate.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.6/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-05-03 13:41:22.000000 figaro-1.6.6/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.523529 figaro-1.6.6/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6875 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1809 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-05-14 11:43:09.000000 figaro-1.6.6/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-05-14 11:42:50.000000 figaro-1.6.6/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-05-14 11:43:09.524209 figaro-1.6.6/setup.cfg
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-14 11:43:09.523142 figaro-1.6.6/test/
--rw-r--r--   0 rinaldi    (503) staff       (20)     2577 2024-05-14 09:10:42.000000 figaro-1.6.6/test/test_figaro.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.515103 figaro-1.6.8/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.8/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.8/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-29 13:46:36.514861 figaro-1.6.8/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4036 2024-05-26 08:09:23.000000 figaro-1.6.8/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.495303 figaro-1.6.8/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.503625 figaro-1.6.8/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      332 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.8/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/figaro.rate.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      308 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.505981 figaro-1.6.8/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1928 2024-05-26 08:07:27.000000 figaro-1.6.8/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.511801 figaro-1.6.8/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.8/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5033 2024-05-16 07:03:14.000000 figaro-1.6.8/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1604 2024-05-16 06:51:29.000000 figaro-1.6.8/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.513492 figaro-1.6.8/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    20100 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    23562 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10988 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9798 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2822 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.8/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1364 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8385 2024-05-23 11:09:00.000000 figaro-1.6.8/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.8/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    36516 2024-05-29 13:41:29.000000 figaro-1.6.8/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6328 2024-05-16 06:52:05.000000 figaro-1.6.8/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    55447 2024-05-23 11:09:57.000000 figaro-1.6.8/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40609 2024-05-16 06:53:39.000000 figaro-1.6.8/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.8/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    12100 2024-05-16 06:37:26.000000 figaro-1.6.8/figaro/rate.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.8/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16137 2024-05-29 13:43:50.000000 figaro-1.6.8/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.514535 figaro-1.6.8/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1809 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-05-29 13:45:58.000000 figaro-1.6.8/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-05-29 13:46:36.515149 figaro-1.6.8/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.513662 figaro-1.6.8/test/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2577 2024-05-15 12:04:57.000000 figaro-1.6.8/test/test_figaro.py
```

### Comparing `figaro-1.6.6/LICENSE` & `figaro-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/PKG-INFO` & `figaro-1.6.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.6
+Version: 1.6.8
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,14 +57,16 @@
 
 # [FIGARO - Fast Inference for GW Astronomy, Research & Observations](https://www.youtube.com/watch?v=uJeJ4YiVFz8)
 
 FIGARO is an inference code designed to estimate multivariate probability densities given samples from an unknown distribution using a Dirichlet Process Gaussian Mixture Model (DPGMM) as nonparameteric model.
 It is also possible to perform hierarchical inferences: in this case, the model used is (H)DPGMM, described in [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract).
 Differently from other DPGMM implementations relying on variational algorithms, FIGARO does not require the user to specify a priori the maximum allowed number of mixture components. The required number of Gaussian distributions to be included in the mixture is inferred from the data. The documentation and user guide for FIGARO is available at [the documentation page](https://figaro.readthedocs.io).
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06589/status.svg)](https://doi.org/10.21105/joss.06589)
+![Test](https://github.com/sterinaldi/FIGARO/actions/workflows/test.yml/badge.svg)
 ## Getting started
 
 You can install FIGARO either via pip (stable release, recommended) 
 ```
 pip install figaro
 ```
 or from the repository (potentially unstable)
@@ -80,38 +82,34 @@
 * `figaro-hierarchical` reconstructs a probability density given a set of single-event samples, each of them drawn around a sample from the initial probability density.
 
 If you only want to reconstruct some probability density or run a vanilla hierarchical analysis, we strongly recommend using these CLI, which are already tested and optimised. A (hopefully gentle) introduction to them can be found at [this page](https://figaro.readthedocs.io/en/latest/quickstart.html), and a guide on how to use the FIGARO reconstructions is available [here](https://figaro.readthedocs.io/en/latest/use_mixture.html).
 If you want to include FIGARO in your own scripts, an introductive guide can be found [here](https://figaro.readthedocs.io/en/latest/python_script.html): there we show how to to reconstruct a probability density with FIGARO and how to use its products.
 
 ## Acknowledgments
 
-If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2022b)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R/abstract):
-```
-@ARTICLE{2022MNRAS.517L...5R,
+If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2024)](https://joss.theoj.org/papers/10.21105/joss.06589):
+```text
+@ARTICLE{Rinaldi2024,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
-        title = "{Rapid localization of gravitational wave hosts with FIGARO}",
-      journal = {\mnras},
-     keywords = {gravitational waves, methods: data analysis, methods: statistical, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
-         year = 2022,
-        month = nov,
-       volume = {517},
-       number = {1},
-        pages = {L5-L10},
-          doi = {10.1093/mnrasl/slac101},
-archivePrefix = {arXiv},
-       eprint = {2205.07252},
- primaryClass = {astro-ph.IM},
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        title = "{FIGARO: hierarchical non-parametric inference for population studies}",
+      journal = {Journal of Open Source Software},
+    publisher = {The Open Journal},
+         year = 2024,
+        month = may,
+       volume = {9},
+       number = {97},
+        pages = {6589},
+          doi = {10.21105/joss.06589},
+          url = {https://doi.org/10.21105/joss.06589}
 }
 ```
 
-If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
+If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
 
-```
+```text
 @ARTICLE{2022MNRAS.509.5454R,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
         title = "{(H)DPGMM: a hierarchy of Dirichlet process Gaussian mixture models for the inference of the black hole mass function}",
       journal = {\mnras},
      keywords = {gravitational waves, methods: data analysis, methods: statistical, stars: black holes, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
          year = 2022,
         month = feb,
```

### Comparing `figaro-1.6.6/README.md` & `figaro-1.6.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # [FIGARO - Fast Inference for GW Astronomy, Research & Observations](https://www.youtube.com/watch?v=uJeJ4YiVFz8)
 
 FIGARO is an inference code designed to estimate multivariate probability densities given samples from an unknown distribution using a Dirichlet Process Gaussian Mixture Model (DPGMM) as nonparameteric model.
 It is also possible to perform hierarchical inferences: in this case, the model used is (H)DPGMM, described in [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract).
 Differently from other DPGMM implementations relying on variational algorithms, FIGARO does not require the user to specify a priori the maximum allowed number of mixture components. The required number of Gaussian distributions to be included in the mixture is inferred from the data. The documentation and user guide for FIGARO is available at [the documentation page](https://figaro.readthedocs.io).
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06589/status.svg)](https://doi.org/10.21105/joss.06589)
+![Test](https://github.com/sterinaldi/FIGARO/actions/workflows/test.yml/badge.svg)
 ## Getting started
 
 You can install FIGARO either via pip (stable release, recommended) 
 ```
 pip install figaro
 ```
 or from the repository (potentially unstable)
@@ -23,38 +25,34 @@
 * `figaro-hierarchical` reconstructs a probability density given a set of single-event samples, each of them drawn around a sample from the initial probability density.
 
 If you only want to reconstruct some probability density or run a vanilla hierarchical analysis, we strongly recommend using these CLI, which are already tested and optimised. A (hopefully gentle) introduction to them can be found at [this page](https://figaro.readthedocs.io/en/latest/quickstart.html), and a guide on how to use the FIGARO reconstructions is available [here](https://figaro.readthedocs.io/en/latest/use_mixture.html).
 If you want to include FIGARO in your own scripts, an introductive guide can be found [here](https://figaro.readthedocs.io/en/latest/python_script.html): there we show how to to reconstruct a probability density with FIGARO and how to use its products.
 
 ## Acknowledgments
 
-If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2022b)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R/abstract):
-```
-@ARTICLE{2022MNRAS.517L...5R,
+If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2024)](https://joss.theoj.org/papers/10.21105/joss.06589):
+```text
+@ARTICLE{Rinaldi2024,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
-        title = "{Rapid localization of gravitational wave hosts with FIGARO}",
-      journal = {\mnras},
-     keywords = {gravitational waves, methods: data analysis, methods: statistical, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
-         year = 2022,
-        month = nov,
-       volume = {517},
-       number = {1},
-        pages = {L5-L10},
-          doi = {10.1093/mnrasl/slac101},
-archivePrefix = {arXiv},
-       eprint = {2205.07252},
- primaryClass = {astro-ph.IM},
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        title = "{FIGARO: hierarchical non-parametric inference for population studies}",
+      journal = {Journal of Open Source Software},
+    publisher = {The Open Journal},
+         year = 2024,
+        month = may,
+       volume = {9},
+       number = {97},
+        pages = {6589},
+          doi = {10.21105/joss.06589},
+          url = {https://doi.org/10.21105/joss.06589}
 }
 ```
 
-If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
+If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
 
-```
+```text
 @ARTICLE{2022MNRAS.509.5454R,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
         title = "{(H)DPGMM: a hierarchy of Dirichlet process Gaussian mixture models for the inference of the black hole mass function}",
       journal = {\mnras},
      keywords = {gravitational waves, methods: data analysis, methods: statistical, stars: black holes, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
          year = 2022,
         month = feb,
```

### Comparing `figaro-1.6.6/docs/source/index.rst` & `figaro-1.6.8/docs/source/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,20 @@
    sphinx-quickstart on Sat Jul 15 21:24:28 2023.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 FIGARO - Fast Inference for GW Astronomy, Research & Observations
 =================================================================
 
-| This page contains the documentation for `FIGARO <https://github.com/sterinaldi/FIGARO>_`, along with a brief description of how to use it in your research project. Please refer to the `GitHub issue tracker <https://github.com/sterinaldi/FIGARO/issues>`_ for bug reports (extremely appreciated), issues and contributions.
+| This page contains the documentation for `FIGARO <https://github.com/sterinaldi/FIGARO>`_, along with a brief description of how to use it in your research project. Please refer to the `GitHub issue tracker <https://github.com/sterinaldi/FIGARO/issues>`_ for bug reports (extremely appreciated), issues and contributions.
 | If you're curious about the other projects I'm working on or if you want to get in touch with me, feel free to visit `my website <https://sterinaldi.github.io>`_!
 
+.. image:: https://joss.theoj.org/papers/10.21105/joss.06589/status.svg
+   :target: https://doi.org/10.21105/joss.06589
+   
 Statement of need
 -----------------
 | FIGARO is an inference code designed to estimate multivariate probability densities given samples from an unknown distribution using a Dirichlet Process Gaussian Mixture Model (DPGMM) as nonparameteric model, and to perform hierarchical non-parametric inferences: in this case, the model used is (H)DPGMM, described in `Rinaldi & Del Pozzo (2022a) <https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract>`_.
 | This code, originally developed in the context of black hole population studies using gravitational-wave observations, take as input generic data and therefore it can be applied to a variety of studies beyond gravitational wave populations.
 
 .. toctree::
    :maxdepth: 1
```

### Comparing `figaro-1.6.6/figaro/_likelihood.py` & `figaro-1.6.8/figaro/_likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from numba import prange
 from figaro._numba_functions import *
 
 LOG2PI = np.log(2*np.pi)
 
 @njit
 def scalar_product(v, M, n):
     """
```

### Comparing `figaro-1.6.6/figaro/_numba_functions.py` & `figaro-1.6.8/figaro/_numba_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numba import njit, prange
+from numba import njit
 from numba.extending import get_cython_function_address
 import ctypes
 
 @njit
 def inv_jit(M):
   return np.linalg.inv(M)
```

### Comparing `figaro-1.6.6/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.8/figaro/_pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.8/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.8/figaro/_pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/_pipelines/probability_density.py` & `figaro-1.6.8/figaro/_pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/cosmology.py` & `figaro-1.6.8/figaro/cosmology.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/credible_regions.py` & `figaro-1.6.8/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/cumulative.py` & `figaro-1.6.8/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/decorators.py` & `figaro-1.6.8/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/diagnostic.py` & `figaro-1.6.8/figaro/diagnostic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import numpy as np
-
+import matplotlib.pyplot as plt
+import warnings
 from numba import njit, prange
 from pathlib import Path
-
-import matplotlib.pyplot as plt
-from distutils.spawn import find_executable
-
-from figaro.cumulative import fast_cumulative
 from figaro.exceptions import FIGAROException
 from figaro import plot_settings
 
 log2e = np.log2(np.e)
 
 @njit
 def angular_coefficient(x, y):
@@ -219,14 +215,14 @@
     """
     S = compute_entropy(draws, int(n_draws))
     fig, ax = plt.subplots()
     ax.plot(np.arange(1, len(draws)+1)*step, S, ls = '--', marker = '', lw = 0.7)
     if exp_entropy is not None:
         ax.axhline(exp_entropy, lw = 0.5, ls = '--', c = 'r')
     ax.set_xlabel('$N$')
-    ax.set_ylabel('$S(N)\ [\mathrm{bits}]$')
+    ax.set_ylabel('$S(N)\\ [\\mathrm{bits}]$')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, name+'_entropy.pdf'), bbox_inches = 'tight')
     plt.close()
     return S
```

### Comparing `figaro-1.6.6/figaro/exceptions.py` & `figaro-1.6.8/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/load.py` & `figaro-1.6.8/figaro/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 inj_par['s1y']                 = 'spin1y'
 inj_par['s1z']                 = 'spin1z'
 inj_par['s2x']                 = 'spin2x'
 inj_par['s2y']                 = 'spin2y'
 inj_par['s2z']                 = 'spin2z'
 inj_par['luminosity_distance'] = 'distance'
 
-supported_pars = [p for p in GW_par.keys() if not p in ['snr', 'far']]
+supported_pars = [p for p in GW_par.keys() if p not in ['snr', 'far']]
 
 def available_gw_pars():
     """
     Print a list of available GW parameters
     """
     print(supported_pars)
 
@@ -103,32 +103,32 @@
         rdstate = np.random.RandomState(seed = 1)
     else:
         rdstate = np.random.RandomState()
     event = Path(event).resolve()
     name, ext = str(event).split('/')[-1].split('.')
     if volume:
         par = ['ra', 'dec', 'luminosity_distance']
-    if not ext in supported_extensions:
+    if ext not in supported_extensions:
         raise TypeError("File {0}.{1} is not supported".format(name, ext))
-    if not ext in ['h5', 'hdf5']:
+    if ext not in ['h5', 'hdf5']:
         if par is not None:
             warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat/.csv files")
         if n_samples > -1:
             samples = np.atleast_1d(np.loadtxt(event))
             s = int(min([n_samples, len(samples)]))
             out = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
         else:
             out = np.loadtxt(event)
     else:
         # Check that a list of parameters is passed
         if par is None:
             raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
         # Check that all the parametes are loadable
         if not np.all([p in GW_par.keys() for p in par]):
-            wrong_pars = [p for p in par if not p in GW_par.keys()]
+            wrong_pars = [p for p in par if p not in GW_par.keys()]
             raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
         # If everything is ok, load the samples
         else:
             out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold, likelihood = likelihood)
     
     if out is None:
         return out, name
@@ -172,17 +172,17 @@
     for event in tqdm(event_files, desc = 'Loading events', disable = not(verbose)):
         if seed:
             rdstate = np.random.RandomState(seed = 1)
         else:
             rdstate = np.random.RandomState()
         name, ext = str(event).split('/')[-1].split('.')
         names.append(name)
-        if not ext in supported_extensions:
+        if ext not in supported_extensions:
             raise TypeError("File {0}.{1} is not supported".format(name, ext))
-        if not ext in ['h5', 'hdf5']:
+        if ext not in ['h5', 'hdf5']:
             if par is not None:
                 warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat/.csv files")
             if n_samples > -1:
                 samples = np.atleast_1d(np.loadtxt(event))
                 s = int(min([n_samples, len(samples)]))
                 samples_subset = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
                 if len(np.shape(samples_subset)) == 1:
@@ -197,15 +197,15 @@
                 
         else:
             # Check that a list of parameters is passed
             if par is None:
                 raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
             # Check that all the parametes are loadable
             if not np.all([p in GW_par.keys() for p in par]):
-                wrong_pars = [p for p in par if not p in GW_par.keys()]
+                wrong_pars = [p for p in par if p not in GW_par.keys()]
                 raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars)+". Run figaro.load.available_gw_pars() for a list of available parameters.")
             # If everything is ok, load the samples
             else:
                 out = _unpack_gw_posterior(event, par = par, n_samples = n_samples, cosmology = cosmology, rdstate = rdstate, waveform = waveform, snr_threshold = snr_threshold, far_threshold = far_threshold, likelihood = likelihood)
                 if out is not None:
                     if out.shape[-1] == len(par):
                         events.append(out)
@@ -249,26 +249,26 @@
     '''
     if cosmology == 'Planck18':
         omega = Planck18
     elif cosmology == 'Planck15':
         omega = Planck15
     else:
         raise FIGAROException("Cosmology not supported")
-    if not waveform in supported_waveforms:
+    if waveform not in supported_waveforms:
         raise FIGAROException("Unknown waveform: please use 'combined' (default), 'imr' or 'seob'")
     
     if far_threshold is not None and snr_threshold is not None:
         warnings.warn("Both FAR and SNR threshold provided. FAR will be used.")
         snr_threshold = None
     
     if far_threshold is not None:
-        if not 'far' in par:
+        if 'far' not in par:
             par = np.append(par, 'far')
     elif snr_threshold is not None:
-        if not 'snr' in par:
+        if 'snr' not in par:
             par = np.append(par, 'snr')
     
     with h5py.File(Path(event), 'r') as f:
         samples     = []
         loaded_pars = []
         flag_filter = False
         try:
@@ -537,15 +537,16 @@
     elif ext == 'json':
         if len(np.shape(draws)) == 1:
             draws = np.atleast_2d(draws)
         ll = []
         for draws_i in draws:
             list_of_dicts = [dr.__dict__.copy() for dr in draws_i]
             for density in list_of_dicts:
-                density.pop('components')
+                if 'components' in density.keys():
+                    density.pop('components')
                 for key in density.keys():
                     value = density[key]
                     if isinstance(value, np.ndarray):
                         value = value.tolist()
                     else:
                         value = float(value)
                     density[key] = value
@@ -669,30 +670,30 @@
         np.ndarray or callable: detected samples or callable with approximant
         np.ndarray or NoneType: injection pdf (for samples) or None (for approximant)
         int or NoneType:        total number of injections
         double duration:        duration of the observation
     """
     file = Path(file)
     ext  = file.parts[-1].split('.')[1]
-    if not ext in supported_extensions + ['py']:
+    if ext not in supported_extensions + ['py']:
         raise FIGAROException("Selection function file not supported")
     if ext == 'py':
         selfunc_file_name = file.parts[-1].split('.')[0]
         spec              = importlib.util.spec_from_file_location(selfunc_file_name, file)
         selfunc_module    = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(selfunc_module)
         selfunc           = selfunc_module.selection_function
         inj_pdf           = None
         n_total_inj       = None
         try:
             duration      = selfunc_module.duration
         except:
             duration      = 1.
     else:
-        if not ext in ['h5','hdf5']:
+        if ext not in ['h5','hdf5']:
             samples     = np.loadtxt(file)
             det_idx     = samples[:,-1]
             selfunc     = samples[:,:-2][det_idx == 1]
             inj_pdf     = samples[:,-2][det_idx == 1]
             n_total_inj = len(samples)
             duration    = 1.
         else:
@@ -716,15 +717,15 @@
         double duration: duration of the observation
     """
     # Check that a list of parameters is passed
     if par is None:
         raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
     # Check that all the parametes are loadable
     if not np.all([p in loadable_inj_pars for p in par]):
-        wrong_pars = [p for p in par if not p in loadable_inj_pars]
+        wrong_pars = [p for p in par if p not in loadable_inj_pars]
         raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars))
     with h5py.File(file, 'r') as f:
         data = f['injections']
         n_total_inj = int(data.attrs['total_generated'])
         duration    = data.attrs['analysis_time_s']/(60.*60.*24.*365) # Years
         # Detected injections
         far_cwb    = np.array(data['far_cwb'])
```

### Comparing `figaro-1.6.6/figaro/marginal.py` & `figaro-1.6.8/figaro/marginal.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         log_weights[i]    = log_norm(vals, mu2, s22)
     # Weights
     log_weights = mix.log_w + log_weights
     if norm:
         log_weights -= _marginalise(mix, axis = np.arange(mix.dim)[~idx])._logpdf_probit(vals)
     # Filter out components with negligible weights
     idx_filt = [True for _ in range(len(log_weights))]
-    norm_const = 0.
     if filter:
         ww = np.exp(log_weights)
         idx = np.argsort(ww)
         m = np.where(np.cumsum(ww[idx]) > tol*np.sum(ww))[0].min()
         idx_filt = [i in idx[m:] for i in range(len(ww))]
         if norm:
             log_weights -= logsumexp(log_weights[idx_filt])
```

### Comparing `figaro-1.6.6/figaro/mixture.py` & `figaro-1.6.8/figaro/mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,15 +688,15 @@
         int dim:             number of dimensions
         int n_cl:            number of clusters in the mixture
         int n_pts:           number of points used to infer the mixture
         double alpha:        concentration parameter
         bool probit:         whether to use the probit transformation or not
         np.ndarray log_w:    component log weights
         bool make_comp:      make component objects
-        double alpha_factor: evaluated \int pdet(theta)p(theta|lambda) conditioned on the mixture parameters
+        double alpha_factor: evaluated \\int pdet(theta)p(theta|lambda) conditioned on the mixture parameters
     
     Returns:
         mixture: instance of mixture class
     """
     def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, alpha = 1., probit = True, log_w = None, make_comp = True, alpha_factor = 1.):
         self.means = means
         self.covs  = covs
@@ -1412,15 +1412,15 @@
             alpha_factor = 1.
             N_pts = np.exp(N_pts)
         w = dirichlet(N_pts+self.alpha/self.n_cl).rvs()[0]
         return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp, alpha_factor = alpha_factor)
     
     def compute_alpha_factor(self):
         """
-        Compute the integral \int pdet(theta)p(theta|lambda) dtheta conditioned on the specific DPGMM parameters
+        Compute the integral \\int pdet(theta)p(theta|lambda) dtheta conditioned on the specific DPGMM parameters
         
         Returns:
             double: value of the integral
         """
         # Approximant
         if callable(self.selfunc):
             alpha_factor = np.mean(self.selfunc(self.rvs(self.MC_draws)))
```

### Comparing `figaro-1.6.6/figaro/montecarlo.py` & `figaro-1.6.8/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/plot.py` & `figaro-1.6.8/figaro/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from matplotlib.lines import Line2D
 from matplotlib.colors import Normalize
 from matplotlib.gridspec import GridSpec
 
 from figaro import plot_settings
 from figaro.marginal import marginalise
 from figaro.credible_regions import ConfidenceArea
+from figaro.cumulative import fast_cumulative
 from figaro.utils import recursive_grid
 from figaro.mixture import mixture
 
 # Telling python to ignore empty legend warning from matplotlib
 warnings.filterwarnings("ignore", message = "No artists with labels found to put in legend.  Note that artists whose label start with an underscore are ignored when legend() is called with no argument.")
 
 class PPPlot(axes.Axes):
```

### Comparing `figaro-1.6.6/figaro/plot_settings.py` & `figaro-1.6.8/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/rate.py` & `figaro-1.6.8/figaro/rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
+import warnings
 from pathlib import Path
 from collections import Counter
 from scipy.stats import poisson, norm
 from figaro.cosmology import dVdz_approx_planck18
 
 def sample_rate(draws, n_obs, selfunc, T, volume = None, size = None, each = False, n_draws = 1e4, dvdz = None, z_index = -1, normalise_alpha = False):
     """
```

### Comparing `figaro-1.6.6/figaro/transform.py` & `figaro-1.6.8/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/figaro/utils.py` & `figaro-1.6.8/figaro/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
     idx = np.random.choice(np.arange(len(draws)), size = int(size))
     ctr = Counter(idx)
     samples = np.empty(shape = (1, draws[0].dim))
     for i, n in zip(ctr.keys(), ctr.values()):
         samples = np.concatenate((samples, draws[i].rvs(n)))
     return samples[1:]
     
-def make_gaussian_mixture(mu, cov, bounds, out_folder = '.', names = None, save = False, save_samples = False, n_samps = 3000, probit = True, ext = 'json'):
+def make_gaussian_mixture(mu, cov, bounds, out_folder = '.', names = None, save = False, save_samples = False, n_samps = 3000, probit = True, ext = 'json', make_comp = True):
     """
     Builds mixtures composed of equally-weighted Gaussian distribution.
     WARNING: due to the probit coordinate change, a Gaussian distribution in the natural space does not correspond to a Gaussian distribution in the probit space.
     The resulting distributions in probit space, therefore, are just an approximation. This approximation holds for distributions which are far from boundaries.
     In general, a more robust (but slower) approach would be to draw samples from each original Gaussian distribution and to use them to make a hierarchical inference.
     
     Arguments:
@@ -250,14 +250,15 @@
         np.ndarray bounds: boundaries for probit transformation
         str out_folder:    output folder
         bool save:         whether to save the draws or not
         bool save_samples: whether to save the samples or not
         int n_samps:       number of samples to estimate mean and covariance in probit space
         bool probit:       whether to use the probit transformation or not
         str ext:           file extension (pkl or json)
+        bool make_comp:    make component objects
     
     Returns:
         np.ndarray: mixtures
     """
     # Here to avoid circular import
     from figaro.mixture import mixture
     from figaro.load import save_density
@@ -310,15 +311,15 @@
                     samples = np.concatenate((samples, ss))
         if save_samples:
             if names is not None:
                 name = names[i]
             else:
                 name = 'event_{0}'.format(i+1)
             np.savetxt(Path(events_folder, name+'.txt'), samples[1:])
-        mix = mixture(np.atleast_2d(mm), np.atleast_3d(cc), np.ones(len(means))/len(means), bounds, len(bounds), len(means), 0, probit = probit, alpha = 1.)
+        mix = mixture(np.atleast_2d(mm), np.atleast_3d(cc), np.ones(len(means))/len(means), bounds, len(bounds), len(means), 0, probit = probit, alpha = 1., make_comp = make_comp)
         if save:
             save_density([mix], draws_folder, name, ext)
         mixtures.append([mix])
     mixtures = np.array(mixtures)
     
     if save:
         # Circular import
```

### Comparing `figaro-1.6.6/figaro.egg-info/PKG-INFO` & `figaro-1.6.8/figaro.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.6
+Version: 1.6.8
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,14 +57,16 @@
 
 # [FIGARO - Fast Inference for GW Astronomy, Research & Observations](https://www.youtube.com/watch?v=uJeJ4YiVFz8)
 
 FIGARO is an inference code designed to estimate multivariate probability densities given samples from an unknown distribution using a Dirichlet Process Gaussian Mixture Model (DPGMM) as nonparameteric model.
 It is also possible to perform hierarchical inferences: in this case, the model used is (H)DPGMM, described in [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract).
 Differently from other DPGMM implementations relying on variational algorithms, FIGARO does not require the user to specify a priori the maximum allowed number of mixture components. The required number of Gaussian distributions to be included in the mixture is inferred from the data. The documentation and user guide for FIGARO is available at [the documentation page](https://figaro.readthedocs.io).
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06589/status.svg)](https://doi.org/10.21105/joss.06589)
+![Test](https://github.com/sterinaldi/FIGARO/actions/workflows/test.yml/badge.svg)
 ## Getting started
 
 You can install FIGARO either via pip (stable release, recommended) 
 ```
 pip install figaro
 ```
 or from the repository (potentially unstable)
@@ -80,38 +82,34 @@
 * `figaro-hierarchical` reconstructs a probability density given a set of single-event samples, each of them drawn around a sample from the initial probability density.
 
 If you only want to reconstruct some probability density or run a vanilla hierarchical analysis, we strongly recommend using these CLI, which are already tested and optimised. A (hopefully gentle) introduction to them can be found at [this page](https://figaro.readthedocs.io/en/latest/quickstart.html), and a guide on how to use the FIGARO reconstructions is available [here](https://figaro.readthedocs.io/en/latest/use_mixture.html).
 If you want to include FIGARO in your own scripts, an introductive guide can be found [here](https://figaro.readthedocs.io/en/latest/python_script.html): there we show how to to reconstruct a probability density with FIGARO and how to use its products.
 
 ## Acknowledgments
 
-If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2022b)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R/abstract):
-```
-@ARTICLE{2022MNRAS.517L...5R,
+If you use FIGARO in your research, please cite [Rinaldi & Del Pozzo (2024)](https://joss.theoj.org/papers/10.21105/joss.06589):
+```text
+@ARTICLE{Rinaldi2024,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
-        title = "{Rapid localization of gravitational wave hosts with FIGARO}",
-      journal = {\mnras},
-     keywords = {gravitational waves, methods: data analysis, methods: statistical, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
-         year = 2022,
-        month = nov,
-       volume = {517},
-       number = {1},
-        pages = {L5-L10},
-          doi = {10.1093/mnrasl/slac101},
-archivePrefix = {arXiv},
-       eprint = {2205.07252},
- primaryClass = {astro-ph.IM},
-       adsurl = {https://ui.adsabs.harvard.edu/abs/2022MNRAS.517L...5R},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        title = "{FIGARO: hierarchical non-parametric inference for population studies}",
+      journal = {Journal of Open Source Software},
+    publisher = {The Open Journal},
+         year = 2024,
+        month = may,
+       volume = {9},
+       number = {97},
+        pages = {6589},
+          doi = {10.21105/joss.06589},
+          url = {https://doi.org/10.21105/joss.06589}
 }
 ```
 
-If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022a)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
+If you make use of the hierarchical analysis, you should mention (H)DPGMM as the model used and cite [Rinaldi & Del Pozzo (2022)](https://ui.adsabs.harvard.edu/abs/2022MNRAS.509.5454R/abstract):
 
-```
+```text
 @ARTICLE{2022MNRAS.509.5454R,
        author = {{Rinaldi}, Stefano and {Del Pozzo}, Walter},
         title = "{(H)DPGMM: a hierarchy of Dirichlet process Gaussian mixture models for the inference of the black hole mass function}",
       journal = {\mnras},
      keywords = {gravitational waves, methods: data analysis, methods: statistical, stars: black holes, Astrophysics - Instrumentation and Methods for Astrophysics, General Relativity and Quantum Cosmology},
          year = 2022,
         month = feb,
```

### Comparing `figaro-1.6.6/figaro.egg-info/SOURCES.txt` & `figaro-1.6.8/figaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figaro-1.6.6/pyproject.toml` & `figaro-1.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.6'
+version = '1.6.8'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

### Comparing `figaro-1.6.6/test/test_figaro.py` & `figaro-1.6.8/test/test_figaro.py`

 * *Files identical despite different names*

