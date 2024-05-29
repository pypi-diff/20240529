# Comparing `tmp/brainbox-0.0.6.tar.gz` & `tmp/brainbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainbox-0.0.6.tar", last modified: Thu Jun  8 16:35:46 2023, max compression
+gzip compressed data, was "brainbox-0.0.7.tar", last modified: Wed May 29 08:09:03 2024, max compression
```

## Comparing `brainbox-0.0.6.tar` & `brainbox-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620986 brainbox-0.0.6/
--rw-r--r--   0 home       (501) staff       (20)     1068 2021-07-14 10:57:17.000000 brainbox-0.0.6/LICENSE.md
--rw-r--r--   0 home       (501) staff       (20)      485 2023-06-08 16:35:46.621052 brainbox-0.0.6/PKG-INFO
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.610231 brainbox-0.0.6/brainbox/
--rw-r--r--   0 home       (501) staff       (20)       95 2023-02-22 17:29:14.000000 brainbox-0.0.6/brainbox/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.611664 brainbox-0.0.6/brainbox/datasets/
--rw-r--r--   0 home       (501) staff       (20)      291 2022-11-01 19:02:15.000000 brainbox-0.0.6/brainbox/datasets/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     7111 2023-04-24 11:06:24.000000 brainbox-0.0.6/brainbox/datasets/base.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.612465 brainbox-0.0.6/brainbox/datasets/implementations/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/brainbox/datasets/implementations/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1511 2022-06-01 11:16:20.000000 brainbox-0.0.6/brainbox/datasets/implementations/singer.py
--rw-r--r--   0 home       (501) staff       (20)     5977 2023-04-13 11:08:34.000000 brainbox-0.0.6/brainbox/datasets/implementations/taylor.py
--rw-r--r--   0 home       (501) staff       (20)     7192 2023-06-01 15:44:40.000000 brainbox-0.0.6/brainbox/datasets/transforms.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.613247 brainbox-0.0.6/brainbox/models/
--rw-r--r--   0 home       (501) staff       (20)       50 2022-06-01 11:02:04.000000 brainbox-0.0.6/brainbox/models/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1738 2023-04-25 14:47:43.000000 brainbox-0.0.6/brainbox/models/model.py
--rw-r--r--   0 home       (501) staff       (20)     2248 2023-01-19 11:19:22.000000 brainbox-0.0.6/brainbox/models/weight_init.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.613708 brainbox-0.0.6/brainbox/physiology/
--rw-r--r--   0 home       (501) staff       (20)      157 2023-05-31 14:22:23.000000 brainbox-0.0.6/brainbox/physiology/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.614394 brainbox-0.0.6/brainbox/physiology/neural/
--rw-r--r--   0 home       (501) staff       (20)       46 2022-10-27 14:43:04.000000 brainbox-0.0.6/brainbox/physiology/neural/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1979 2023-03-23 16:58:09.000000 brainbox-0.0.6/brainbox/physiology/neural/correlation.py
--rw-r--r--   0 home       (501) staff       (20)     1743 2023-03-16 16:42:25.000000 brainbox-0.0.6/brainbox/physiology/neural/rdm.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.614921 brainbox-0.0.6/brainbox/physiology/rfs/
--rw-r--r--   0 home       (501) staff       (20)       19 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/rfs/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.615545 brainbox-0.0.6/brainbox/physiology/rfs/gabor/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/__init__.py
--rw-r--r--   0 home       (501) staff       (20)    11574 2023-06-02 11:59:50.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/fit.py
--rw-r--r--   0 home       (501) staff       (20)     6962 2023-06-02 12:43:09.000000 brainbox-0.0.6/brainbox/physiology/rfs/gabor/query.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.616122 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-06-01 17:12:08.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/__init__.py
--rw-r--r--   0 home       (501) staff       (20)    10189 2023-06-02 13:59:42.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/fit.py
--rw-r--r--   0 home       (501) staff       (20)     5121 2023-06-02 12:44:44.000000 brainbox-0.0.6/brainbox/physiology/rfs/gaussian/query.py
--rw-r--r--   0 home       (501) staff       (20)     3303 2023-06-02 12:54:56.000000 brainbox-0.0.6/brainbox/physiology/rfs/rfs.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.617859 brainbox-0.0.6/brainbox/physiology/spiking/
--rw-r--r--   0 home       (501) staff       (20)      172 2023-05-31 14:23:15.000000 brainbox-0.0.6/brainbox/physiology/spiking/__init__.py
--rw-r--r--   0 home       (501) staff       (20)      994 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/spiking/burst.py
--rw-r--r--   0 home       (501) staff       (20)     1473 2023-05-31 14:21:02.000000 brainbox-0.0.6/brainbox/physiology/spiking/isi.py
--rw-r--r--   0 home       (501) staff       (20)     1350 2023-05-18 11:53:28.000000 brainbox-0.0.6/brainbox/physiology/spiking/metric.py
--rw-r--r--   0 home       (501) staff       (20)     1916 2022-10-27 14:59:45.000000 brainbox-0.0.6/brainbox/physiology/spiking/rate.py
--rw-r--r--   0 home       (501) staff       (20)     1619 2022-06-07 21:17:20.000000 brainbox-0.0.6/brainbox/physiology/spiking/synchrony.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.618726 brainbox-0.0.6/brainbox/physiology/tuning/
--rw-r--r--   0 home       (501) staff       (20)       40 2022-07-13 13:42:58.000000 brainbox-0.0.6/brainbox/physiology/tuning/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     9769 2023-02-22 17:29:15.000000 brainbox-0.0.6/brainbox/physiology/tuning/fit.py
--rw-r--r--   0 home       (501) staff       (20)     3064 2022-10-27 14:59:45.000000 brainbox-0.0.6/brainbox/physiology/tuning/fitters.py
--rw-r--r--   0 home       (501) staff       (20)     9228 2022-11-25 15:50:08.000000 brainbox-0.0.6/brainbox/physiology/tuning/query.py
--rw-r--r--   0 home       (501) staff       (20)     2363 2022-05-30 04:52:59.000000 brainbox-0.0.6/brainbox/physiology/util.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620055 brainbox-0.0.6/brainbox/trainer/
--rw-r--r--   0 home       (501) staff       (20)      537 2023-02-27 11:23:54.000000 brainbox-0.0.6/brainbox/trainer/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     5616 2023-03-22 15:49:51.000000 brainbox-0.0.6/brainbox/trainer/crossval.py
--rw-r--r--   0 home       (501) staff       (20)     1248 2023-03-25 08:45:35.000000 brainbox-0.0.6/brainbox/trainer/query.py
--rw-r--r--   0 home       (501) staff       (20)     6822 2023-06-08 08:37:21.000000 brainbox-0.0.6/brainbox/trainer/trainer.py
--rw-r--r--   0 home       (501) staff       (20)     2097 2023-05-08 16:21:07.000000 brainbox-0.0.6/brainbox/trainer/validator.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.611009 brainbox-0.0.6/brainbox.egg-info/
--rw-r--r--   0 home       (501) staff       (20)      485 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     1634 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       43 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)       15 2023-06-08 16:35:46.000000 brainbox-0.0.6/brainbox.egg-info/top_level.txt
--rw-r--r--   0 home       (501) staff       (20)       93 2022-05-30 06:26:36.000000 brainbox-0.0.6/pyproject.toml
--rw-r--r--   0 home       (501) staff       (20)      577 2023-06-08 16:35:46.621377 brainbox-0.0.6/setup.cfg
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620289 brainbox-0.0.6/tests/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/tests/__init__.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-06-08 16:35:46.620723 brainbox-0.0.6/tests/physiology/
--rw-r--r--   0 home       (501) staff       (20)        0 2022-05-30 04:44:08.000000 brainbox-0.0.6/tests/physiology/__init__.py
--rw-r--r--   0 home       (501) staff       (20)     1557 2022-05-30 04:52:59.000000 brainbox-0.0.6/tests/physiology/test_spiking.py
--rw-r--r--   0 home       (501) staff       (20)     1439 2022-05-30 04:52:59.000000 brainbox-0.0.6/tests/physiology/test_util.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.589552 brainbox-0.0.7/
+-rw-r--r--   0 home       (501) staff       (20)     1068 2024-04-09 14:42:37.000000 brainbox-0.0.7/LICENSE.md
+-rw-r--r--   0 home       (501) staff       (20)      646 2024-05-29 08:09:03.589490 brainbox-0.0.7/PKG-INFO
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.579728 brainbox-0.0.7/brainbox/
+-rw-r--r--   0 home       (501) staff       (20)       95 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.581447 brainbox-0.0.7/brainbox/datasets/
+-rw-r--r--   0 home       (501) staff       (20)      291 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/datasets/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     7133 2024-04-09 14:44:55.000000 brainbox-0.0.7/brainbox/datasets/base.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.581993 brainbox-0.0.7/brainbox/datasets/implementations/
+-rw-r--r--   0 home       (501) staff       (20)        0 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/datasets/implementations/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1511 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/datasets/implementations/singer.py
+-rw-r--r--   0 home       (501) staff       (20)     5977 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/datasets/implementations/taylor.py
+-rw-r--r--   0 home       (501) staff       (20)     8421 2024-05-14 13:09:24.000000 brainbox-0.0.7/brainbox/datasets/transforms.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.582639 brainbox-0.0.7/brainbox/models/
+-rw-r--r--   0 home       (501) staff       (20)       50 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/models/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1738 2024-04-09 14:55:49.000000 brainbox-0.0.7/brainbox/models/model.py
+-rw-r--r--   0 home       (501) staff       (20)     2248 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/models/weight_init.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.582993 brainbox-0.0.7/brainbox/physiology/
+-rw-r--r--   0 home       (501) staff       (20)      157 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.583588 brainbox-0.0.7/brainbox/physiology/neural/
+-rw-r--r--   0 home       (501) staff       (20)       46 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/neural/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     2381 2024-04-28 15:10:31.000000 brainbox-0.0.7/brainbox/physiology/neural/correlation.py
+-rw-r--r--   0 home       (501) staff       (20)     1500 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/neural/rdm.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.583918 brainbox-0.0.7/brainbox/physiology/rfs/
+-rw-r--r--   0 home       (501) staff       (20)       19 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.584374 brainbox-0.0.7/brainbox/physiology/rfs/gabor/
+-rw-r--r--   0 home       (501) staff       (20)        0 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/gabor/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)    11601 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/gabor/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     6962 2024-04-18 16:49:52.000000 brainbox-0.0.7/brainbox/physiology/rfs/gabor/query.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.584945 brainbox-0.0.7/brainbox/physiology/rfs/gaussian/
+-rw-r--r--   0 home       (501) staff       (20)        0 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/gaussian/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)    10324 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/gaussian/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     4046 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/gaussian/query.py
+-rw-r--r--   0 home       (501) staff       (20)     3303 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/rfs/rfs.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.586294 brainbox-0.0.7/brainbox/physiology/spiking/
+-rw-r--r--   0 home       (501) staff       (20)      188 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/spiking/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)      994 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/spiking/burst.py
+-rw-r--r--   0 home       (501) staff       (20)     1474 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/spiking/isi.py
+-rw-r--r--   0 home       (501) staff       (20)     1350 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/spiking/metric.py
+-rw-r--r--   0 home       (501) staff       (20)     1916 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/spiking/rate.py
+-rw-r--r--   0 home       (501) staff       (20)     2239 2024-05-19 13:41:54.000000 brainbox-0.0.7/brainbox/physiology/spiking/synchrony.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.587225 brainbox-0.0.7/brainbox/physiology/tuning/
+-rw-r--r--   0 home       (501) staff       (20)       40 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/tuning/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     9793 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/tuning/fit.py
+-rw-r--r--   0 home       (501) staff       (20)     3064 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/tuning/fitters.py
+-rw-r--r--   0 home       (501) staff       (20)    10737 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/tuning/query.py
+-rw-r--r--   0 home       (501) staff       (20)     1684 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/physiology/util.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.588225 brainbox-0.0.7/brainbox/trainer/
+-rw-r--r--   0 home       (501) staff       (20)      537 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/trainer/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     6052 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/trainer/crossval.py
+-rw-r--r--   0 home       (501) staff       (20)     1248 2024-04-13 13:59:13.000000 brainbox-0.0.7/brainbox/trainer/query.py
+-rw-r--r--   0 home       (501) staff       (20)     6822 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/trainer/trainer.py
+-rw-r--r--   0 home       (501) staff       (20)     2097 2024-04-09 14:42:37.000000 brainbox-0.0.7/brainbox/trainer/validator.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.589191 brainbox-0.0.7/brainbox.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)      646 2024-05-29 08:09:03.000000 brainbox-0.0.7/brainbox.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     1634 2024-05-29 08:09:03.000000 brainbox-0.0.7/brainbox.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2024-05-29 08:09:03.000000 brainbox-0.0.7/brainbox.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       56 2024-05-29 08:09:03.000000 brainbox-0.0.7/brainbox.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)       15 2024-05-29 08:09:03.000000 brainbox-0.0.7/brainbox.egg-info/top_level.txt
+-rw-r--r--   0 home       (501) staff       (20)       93 2024-04-09 14:42:37.000000 brainbox-0.0.7/pyproject.toml
+-rw-r--r--   0 home       (501) staff       (20)      591 2024-05-29 08:09:03.589890 brainbox-0.0.7/setup.cfg
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.588396 brainbox-0.0.7/tests/
+-rw-r--r--   0 home       (501) staff       (20)        0 2024-04-09 14:42:37.000000 brainbox-0.0.7/tests/__init__.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2024-05-29 08:09:03.588950 brainbox-0.0.7/tests/physiology/
+-rw-r--r--   0 home       (501) staff       (20)        0 2024-04-09 14:42:37.000000 brainbox-0.0.7/tests/physiology/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)     1557 2024-04-09 14:42:37.000000 brainbox-0.0.7/tests/physiology/test_spiking.py
+-rw-r--r--   0 home       (501) staff       (20)     1439 2024-04-09 14:42:37.000000 brainbox-0.0.7/tests/physiology/test_util.py
```

### Comparing `brainbox-0.0.6/LICENSE.md` & `brainbox-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/datasets/base.py` & `brainbox-0.0.7/brainbox/datasets/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,8 +273,9 @@
 
         if self._transform is not None:
             x = self._transform(x)
 
         if self._target_transform is not None:
             y = self._target_transform(y)
 
-        return x, y
+        # return x, y
+        return x, x
```

### Comparing `brainbox-0.0.6/brainbox/datasets/implementations/singer.py` & `brainbox-0.0.7/brainbox/datasets/implementations/singer.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/datasets/implementations/taylor.py` & `brainbox-0.0.7/brainbox/datasets/implementations/taylor.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/datasets/transforms.py` & `brainbox-0.0.7/brainbox/datasets/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,38 +162,74 @@
     @property
     def hyperparams(self):
         hyperparams = {**super().hyperparams, "frames": self._frames}
 
         return hyperparams
 
 
+class ClipShrink(BBTransform):
+
+    def __init__(self, frames):
+        self._frames = frames
+        self._kernel = torch.ones(1, 1, frames, 1, 1)
+
+    def __call__(self, clip):
+        if self._kernel.device != clip.device:
+            self._kernel = self._kernel.to(clip.device)
+        return F.conv3d(clip, self._kernel, stride=(self._frames, 1, 1))
+
+    @property
+    def hyperparams(self):
+        hyperparams = {**super().hyperparams, "frames": self._frames}
+
+        return hyperparams
+
+
 class ImgToClip(BBTransform):
     def __init__(self, pre_blanks, repeats, post_blanks, c=0):
         self._pre_blanks = pre_blanks
         self._repeats = repeats
         self._post_blanks = post_blanks
         self._c = c
     
     def __call__(self, img):
-        # img: channel x height x width
-        # output: channel x time x height x width
-        assert len(img.shape) == 3
-        channel = img.shape[0]
-        height = img.shape[1]
-        width = img.shape[2]
-
-        clip = self._c * torch.ones(
-            (
-                channel,
-                self._pre_blanks + self._repeats + self._post_blanks,
-                height,
-                width,
+        if len(img.shape) == 3:
+            # img: channel x height x width
+            # output: channel x time x height x width
+            channel = img.shape[0]
+            height = img.shape[1]
+            width = img.shape[2]
+
+            clip = self._c * torch.ones(
+                (
+                    channel,
+                    self._pre_blanks + self._repeats + self._post_blanks,
+                    height,
+                    width,
+                )
             )
-        )
-        clip[:, self._pre_blanks : self._pre_blanks + self._repeats] = img
+            clip[:, self._pre_blanks : self._pre_blanks + self._repeats] = img
+        elif len(img.shape) == 4:
+            # img: batch x channel x height x width
+            # output: batch x channel x time x height x width
+            batch = img.shape[0]
+            channel = img.shape[1]
+            height = img.shape[2]
+            width = img.shape[3]
+
+            clip = self._c * torch.ones(
+                (
+                    batch,
+                    channel,
+                    self._pre_blanks + self._repeats + self._post_blanks,
+                    height,
+                    width,
+                )
+            )
+            clip[:, :, self._pre_blanks : self._pre_blanks + self._repeats] = img.unsqueeze(2)  # Add fake time dim to img
 
         return clip
 
     @property
     def hyperparams(self):
         hyperparams = {
             **super().hyperparams,
@@ -208,15 +244,15 @@
 class GaussianKernel(BBTransform):
     def __init__(self, sigma, width):
         assert width % 2 == 1, "width needs to be an odd number"
         self._sigma = sigma
         self._width = width
 
         self._kernel = self._build_kernel(sigma, width)
-    
+
     def __call__(self, x):
         if len(x.shape) == 3:  # x: channel x time x n_neurons
             x = x.unsqueeze(0)  # add batch dimension
             x = F.pad(x, (0, 0, self._width // 2, self._width // 2))
             x = F.conv2d(x, self._kernel)
 
             return x[0]
```

### Comparing `brainbox-0.0.6/brainbox/models/model.py` & `brainbox-0.0.7/brainbox/models/model.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/models/weight_init.py` & `brainbox-0.0.7/brainbox/models/weight_init.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/neural/correlation.py` & `brainbox-0.0.7/brainbox/physiology/neural/correlation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import torch
 
 
-def r2(output, target):
+def R2(output, target):
+    # output: T
+    # target: T
     assert len(output.shape) == 1
     assert len(target.shape) == 1
     return 1 - torch.pow(target - output, 2).sum() / torch.pow((target - target.mean()), 2).sum()
 
 
 def cc(output, target):
     assert output.shape == target.shape
@@ -45,14 +47,25 @@
     n = target.shape[1]
     sp = (1 / (n - 1)) * (n * target.mean(dim=1).var(unbiased=unbiased) - target.var(dim=0, unbiased=unbiased).mean())
     rp = target.mean(1).var(unbiased=unbiased)
 
     return sp / rp
 
 
+def compute_max_response_reliability(x):
+    # x: clips x time x repeat x neuron
+    n_trials = x.shape[2]
+    mean_response = x.mean(2).unsqueeze(2).repeat(1, 1, n_trials, 1)
+
+    flatten_mean_response = mean_response.flatten(0, 2).permute(1, 0)
+    flatten_trial_response = x.flatten(0, 2).permute(1, 0)
+
+    return cc(flatten_mean_response, flatten_trial_response)
+
+
 def nc(y):
     # y: neurons x repeat x time
     trial_avg = y.mean(1)
     neuron_avg = trial_avg.mean(1)
     total_diff = (y - neuron_avg.view(-1, 1, 1))
     noise_diff = (y - trial_avg.unsqueeze(1))
     N, K, T = y.shape
```

### Comparing `brainbox-0.0.6/brainbox/physiology/rfs/gabor/fit.py` & `brainbox-0.0.7/brainbox/physiology/rfs/gabor/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,16 @@
         self._frequency = nn.Parameter(frequency_init, requires_grad=not freeze)
         self._eps = eps
 
         y, x = torch.meshgrid(
             [
                 torch.arange(rf_size, dtype=torch.float32),
                 torch.arange(rf_size, dtype=torch.float32),
-            ]
+            ],
+            indexing="ij"
         )
         self.y = nn.Parameter(y, requires_grad=False)
         self.x = nn.Parameter(x, requires_grad=False)
 
         self._rf_ghost = nn.Parameter(torch.ones(rf_size, rf_size), requires_grad=False)
 
     @property
```

### Comparing `brainbox-0.0.6/brainbox/physiology/rfs/gabor/query.py` & `brainbox-0.0.7/brainbox/physiology/rfs/gabor/query.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/rfs/gaussian/fit.py` & `brainbox-0.0.7/brainbox/physiology/rfs/gaussian/fit.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import torch
 import torch.fft as fft
 import torch.nn as nn
 import torch.nn.functional as F
 
 import brainbox.physiology.rfs.rfs as rfs_util
 
-logger = logging.getLogger("gabor")
+logger = logging.getLogger("gaussian")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 
 
-class GaborFitter:
+class GaussianFitter:
 
-    GABOR_AMPS = [-1, 1]
-    GABOR_SIGMAS = [0.5, 1, 1.5]
-    GABOR_PS = [-0.5, 0, 0.5]
+    GAUSSIAN_AMPS = [-1, 1]
+    GAUSSIAN_SIGMAS = [0.5, 1, 1.5]
+    GAUSSIAN_PS = [-0.5, 0, 0.5]
 
     def __init__(self):
         pass
 
     def fit_spatial(
             self,
             path,
@@ -38,15 +38,15 @@
     ):
         batch_params = []
 
         iterations = rfs.shape[0] // batch_size
         iterations += 1 if rfs.shape[0] > iterations * batch_size else 0
 
         for b in range(iterations):
-            logger.info(f"Fitting gabors for batch {b}...")
+            logger.info(f"Fitting gaussians for batch {b}...")
             params = self.fit_spatial_single_batch(
                 rfs[b * batch_size : (b + 1) * batch_size],
                 n_spectral_iterations,
                 n_spatial_iterations,
                 spectral_lr,
                 spatial_lr,
                 device,
@@ -75,18 +75,18 @@
             spectral_lr=1e-2,
             spatial_lr=1e-3,
             device="cuda",
             **kwargs,
     ):
         n_rfs = rfs.shape[0]
         rf_size = rfs.shape[-1]
-        initial_gabor_params = GaborFitter._build_initial_gabor_params(
+        initial_gaussian_params = GaussianFitter._build_initial_gaussian_params(
             rf_size, n_rfs, **kwargs
         )
-        n_params = len(initial_gabor_params[0]) // n_rfs
+        n_params = len(initial_gaussian_params[0]) // n_rfs
         normalized_rfs = torch.repeat_interleave(
             rfs_util.normalize_rfs(rfs), n_params, 0
         ).to(device)
 
         # spectral_fitter = SpectralGaussianFitter(
         #     normalized_rfs,
         #     n_spectral_iterations,
@@ -98,19 +98,19 @@
         # spectral_fitter.fit()
         spatial_fitter = SpatialGaussianFitter(
             normalized_rfs,
             n_spatial_iterations,
             spatial_lr,
             device,
             rf_size,
-            *initial_gabor_params,
+            *initial_gaussian_params,
         )
         spatial_fitter.fit()
 
-        return GaborFitter._get_best_fits(
+        return GaussianFitter._get_best_fits(
             normalized_rfs, spatial_fitter.gaussian_model, n_params, n_rfs
         )
 
     # def fit_spatiotemporal(
     #     self,
     #     strfs,
     #     gabor_params,
@@ -132,20 +132,20 @@
     #         *gabor_params,
     #     )
     #     spatial_fitter.fit()
     #
     #     return spatial_fitter.gabor_model.cpu()
 
     @staticmethod
-    def _build_initial_gabor_params(rf_size, repeat, **kwargs):
-        amps_init = kwargs.get("sigmax_init", GaborFitter.GABOR_AMPS)
+    def _build_initial_gaussian_params(rf_size, repeat, **kwargs):
+        amps_init = kwargs.get("sigmax_init", GaussianFitter.GAUSSIAN_AMPS)
         x0_init, y0_init = [rf_size // 2], [rf_size // 2]
-        sigmax_init = kwargs.get("sigmax_init", GaborFitter.GABOR_SIGMAS)
-        sigmay_init = kwargs.get("sigmay_init", GaborFitter.GABOR_SIGMAS)
-        p_init = kwargs.get("p_init", GaborFitter.GABOR_PS)
+        sigmax_init = kwargs.get("sigmax_init", GaussianFitter.GAUSSIAN_SIGMAS)
+        sigmay_init = kwargs.get("sigmay_init", GaussianFitter.GAUSSIAN_SIGMAS)
+        p_init = kwargs.get("p_init", GaussianFitter.GAUSSIAN_PS)
 
         params_product = list(
             itertools.product(
                 amps_init,
                 x0_init,
                 y0_init,
                 sigmax_init,
@@ -166,47 +166,47 @@
             y0_init,
             sigmax_init,
             sigmay_init,
             p_init
         )
 
     @staticmethod
-    def _extract_gabor_params(gabor_model):
-        x0_init = gabor_model.x0.data
-        y0_init = gabor_model.y0.data
-        sigmax_init = gabor_model.sigmax.data
-        sigmay_init = gabor_model.sigmay.data
-        p_init = gabor_model.p.data
+    def _extract_gaussian_params(gaussian_model):
+        x0_init = gaussian_model.x0.data
+        y0_init = gaussian_model.y0.data
+        sigmax_init = gaussian_model.sigmax.data
+        sigmay_init = gaussian_model.sigmay.data
+        p_init = gaussian_model.p.data
 
         return (
             x0_init,
             y0_init,
             sigmax_init,
             sigmay_init,
             p_init,
         )
 
     @staticmethod
-    def _get_best_fits(repeated_rfs, gabor_model, n_params, n_rfs):
-        predictions = gabor_model()
+    def _get_best_fits(repeated_rfs, gaussian_model, n_params, n_rfs):
+        predictions = gaussian_model()
         losses = (
             F.mse_loss(repeated_rfs, predictions, reduction="none")
             .mean(dim=(1, 2))
             .view(n_rfs, n_params)
         )
         best_idxs = torch.argmin(losses, dim=1) + torch.Tensor(
             [n_params * i for i in range(n_rfs)]
         ).int().to(repeated_rfs.device)
 
-        amp = gabor_model.amplitude.data[best_idxs]
-        x0 = gabor_model.x0.data[best_idxs]
-        y0 = gabor_model.y0.data[best_idxs]
-        sigmax = gabor_model.sigmax.data[best_idxs]
-        sigmay = gabor_model.sigmay.data[best_idxs]
-        p = gabor_model.p.data[best_idxs]
+        amp = gaussian_model.amplitude.data[best_idxs]
+        x0 = gaussian_model.x0.data[best_idxs]
+        y0 = gaussian_model.y0.data[best_idxs]
+        sigmax = gaussian_model.sigmax.data[best_idxs]
+        sigmay = gaussian_model.sigmay.data[best_idxs]
+        p = gaussian_model.p.data[best_idxs]
 
         return amp, x0, y0, sigmax, sigmay, p
 
 
 class SpatialGaussianFitter:
     def __init__(
         self,
@@ -302,15 +302,16 @@
         self._p = nn.Parameter(p_init)
         self._eps = eps
 
         y, x = torch.meshgrid(
             [
                 torch.arange(rf_size, dtype=torch.float32),
                 torch.arange(rf_size, dtype=torch.float32),
-            ]
+            ],
+            indexing="ij"
         )
         self.y = nn.Parameter(y, requires_grad=False)
         self.x = nn.Parameter(x, requires_grad=False)
         self._rf_ghost = nn.Parameter(torch.ones(rf_size, rf_size), requires_grad=False)
 
     @property
     def amplitude(self):
```

### Comparing `brainbox-0.0.6/brainbox/physiology/rfs/gaussian/query.py` & `brainbox-0.0.7/brainbox/physiology/rfs/gaussian/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import torch
 import numpy as np
 import pandas as pd
 
 from kornia import geometry
 
 from brainbox.physiology.rfs import rfs
-from brainbox.physiology.rfs.gaussian.fit import GaborFitter, Gaussian2D
+from brainbox.physiology.rfs.gaussian.fit import Gaussian2D
 
-logger = logging.getLogger("gabor")
+logger = logging.getLogger("gaussian")
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 
 
 class GaussianQuery:
 
     SPACE_TIME_SEPARABLE = "separable"
     SPACE_TIME_INSEPARABLE = "inseparable"
 
     def __init__(self, fits_path, strfs):
         self._params_df = pd.read_csv(fits_path)
         self._strfs = strfs.cpu()
 
         self._rf_size = strfs.shape[-1]
         self._spatial_rfs = rfs.get_all_highest_power_spatial_rf(strfs)
-        self._gabors = self._build_gabors()
+        self._gaussians = self._build_gaussians()
         print(len(self._get_correlation()))
         self._params_df["cc"] = self._get_correlation()
 
     def validate(
         self, min_cc, min_env, separability=None, inseperable_thresh=0.5, verbose=True
     ):
         query = self._query_cc(min_cc)
@@ -45,53 +45,18 @@
             )
             logger.info(
                 f"Envelope criteria exclusion {(self._query_envelope(min_env)==False).sum()}"
             )
 
         params_df = self._params_df[query]
         spatial_rfs = self._spatial_rfs[query]
-        gabors = self._gabors[query]
+        gaussians = self._gaussians[query]
         strfs = self._strfs[query]
 
-        return params_df, spatial_rfs, gabors, strfs
-
-    def get_temporal_profile(
-        self,
-        min_cc=0.8,
-        min_env=0.5,
-        separability=None,
-        inseperable_thresh=0.5,
-        verbose=True,
-        n_spatial_iterations=100,
-        spatial_lr=1e-2,
-        device="cuda",
-    ):
-
-        params_df, spatial_rfs, gabors, strfs, rfs2d = self.validate(
-            min_cc,
-            min_env,
-            separability=separability,
-            inseperable_thresh=inseperable_thresh,
-            verbose=verbose,
-        )
-
-        n_dim, t_dim = strfs.shape[0], strfs.shape[1]
-        gabor_params = GaborQuery._df_params_to_gabor_params(params_df)
-        gabor_params = [
-            torch.repeat_interleave(gabor_param, t_dim) for gabor_param in gabor_params
-        ]
-
-        gabor_fitter = GaborFitter()
-        gabor_model = gabor_fitter.fit_spatiotemporal(
-            strfs.to(device), gabor_params, n_spatial_iterations, spatial_lr, device
-        )
-        temporal_profiles = gabor_model.amplitude.view(n_dim, t_dim)
-        rr = [-(tp.min()).item() for tp in temporal_profiles]
-
-        return temporal_profiles, rr
+        return params_df, spatial_rfs, gaussians, strfs
 
     def _query_cc(self, min_cc):
         return self._params_df["cc"] > min_cc
 
     def _query_location(self):
         query = (0 <= self._params_df["x0"]) & (self._params_df["x0"] < self._rf_size)
         query &= (0 <= self._params_df["y0"]) & (self._params_df["y0"] < self._rf_size)
@@ -117,45 +82,45 @@
             if separability == GaussianQuery.SPACE_TIME_INSEPARABLE
             else inseperable_units == False
         )
 
         return query
 
     def _get_correlation(self):
-        def correlation(gabor, rf):
+        def correlation(gaussian, rf):
             return np.corrcoef(
-                gabor.flatten().detach().numpy(), rf.flatten().detach().numpy()
+                gaussian.flatten().detach().numpy(), rf.flatten().detach().numpy()
             )[0, 1]
 
         return [
-            correlation(gabor, rf) for gabor, rf in zip(self._gabors, self._spatial_rfs)
+            correlation(gaussian, rf) for gaussian, rf in zip(self._gaussians, self._spatial_rfs)
         ]
 
-    def _build_gabors(self):
+    def _build_gaussians(self):
         (
             amp,
             x0,
             y0,
             sigmax,
             sigmay,
             p
-        ) = GaussianQuery._df_params_to_gabor_params(self._params_df)
+        ) = GaussianQuery._df_params_to_gaussian_params(self._params_df)
 
         return Gaussian2D(
             rf_size=self._rf_size,
             amp_init=amp,
             x0_init=x0,
             y0_init=y0,
             sigmax_init=sigmax,
             sigmay_init=sigmay,
             p_init=p,
         )()
 
     @staticmethod
-    def _df_params_to_gabor_params(params_df):
+    def _df_params_to_gaussian_params(params_df):
         amp = torch.Tensor(params_df["amp"].to_numpy())
         x0 = torch.Tensor(params_df["x0"].to_numpy())
         y0 = torch.Tensor(params_df["y0"].to_numpy())
         sigmax = torch.Tensor(params_df["sigmax"].to_numpy())
         sigmay = torch.Tensor(params_df["sigmay"].to_numpy())
         p = torch.Tensor(params_df["p"].to_numpy())
```

### Comparing `brainbox-0.0.6/brainbox/physiology/rfs/rfs.py` & `brainbox-0.0.7/brainbox/physiology/rfs/rfs.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/spiking/burst.py` & `brainbox-0.0.7/brainbox/physiology/spiking/burst.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/spiking/isi.py` & `brainbox-0.0.7/brainbox/physiology/spiking/isi.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 def compute_isi_cvs(isis_tensor, n_spikes_thresh):
     mean = util.get_mean(isis_tensor)
     std = util.get_std(isis_tensor, mean=mean)
     cvs = std / mean
 
     invalid_cv_mask = (isis_tensor != 0).sum(dim=2) < n_spikes_thresh
-    cvs[invalid_cv_mask] = 0
+    cvs[invalid_cv_mask] = -1
 
     return cvs
 
 
 def compute_isis_tensor(spike_trains):
     # spike_trains: b x n x t
     spike_trains = spike_trains.type(torch.int16)
```

### Comparing `brainbox-0.0.6/brainbox/physiology/spiking/metric.py` & `brainbox-0.0.7/brainbox/physiology/spiking/metric.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/spiking/rate.py` & `brainbox-0.0.7/brainbox/physiology/spiking/rate.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/tuning/fit.py` & `brainbox-0.0.7/brainbox/physiology/tuning/fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,21 +154,22 @@
     def generate_grating(
         amplitude, rf_w, rf_h, theta, spatial_freq, temporal_freq, duration, dt
     ):
         y, x = torch.meshgrid(
             [
                 torch.arange(rf_h, dtype=torch.float32),
                 torch.arange(rf_w, dtype=torch.float32),
-            ]
+            ],
+            indexing="ij"
         )
         theta = torch.Tensor([theta]).expand_as(y)
         spatial_freq = torch.Tensor([spatial_freq]).expand_as(y)
 
-        fps = int(1000 // dt)
-        n_timesteps = int(duration // dt)
+        fps = int(1000 / dt)
+        n_timesteps = int(duration / dt)
         timesteps = (
             torch.arange(n_timesteps).view(n_timesteps, 1, 1).repeat(1, rf_h, rf_w)
         )
 
         rotx = x * torch.cos(theta) - y * torch.sin(theta)
         grating = amplitude * torch.sin(
             2 * np.pi * (spatial_freq * rotx - temporal_freq * timesteps / fps)
@@ -198,15 +199,15 @@
             batch_response_to_preferred_grating = []
 
             for i in range(
                 self._tuning_query.n_units // batch_size + 1
                 if self._tuning_query.n_units % batch_size > 0
                 else 0
             ):
-                batch_gratings = gratings[i * batch_size : (i + 1) * batch_size]
+                batch_gratings = gratings[i * batch_size: (i + 1) * batch_size]
                 batch_response_to_preferred_grating.append(self.model(batch_gratings))
 
             response_to_preferred_grating = torch.cat(
                 batch_response_to_preferred_grating
             )
             response_to_preferred_grating = torch.stack(
                 [
```

### Comparing `brainbox-0.0.6/brainbox/physiology/tuning/fitters.py` & `brainbox-0.0.7/brainbox/physiology/tuning/fitters.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/physiology/tuning/query.py` & `brainbox-0.0.7/brainbox/physiology/tuning/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
+import warnings
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import pandas as pd
 import numpy as np
 
+warnings.filterwarnings("ignore", category=RuntimeWarning)
+
 
 class TuningQuery:
     def __init__(self, path):
         probe_path = os.path.join(path, "probe.csv")
         spectral_path = (
             os.path.join(path, "spectral.csv")
             if os.path.exists(os.path.join(path, "spectral.csv"))
@@ -104,14 +107,48 @@
         ]
         response_per_theta = response_per_theta.sort_values(by=["theta"])
         theta = response_per_theta[["theta"]].to_numpy().flatten()
         response = response_per_theta[[str(unit_id)]].to_numpy().flatten()
 
         return theta, response
 
+    def orientation_sf_tuning_curve(self, unit_id):
+        preferred_temporal_frequency_query = (
+                 self._probes_df["temporal_frequency"]
+                 == self.preferred_temporal_frequency(unit_id)
+         )
+        response_per_theta = self._probes_df[
+            preferred_temporal_frequency_query
+        ]
+        # return response_per_theta
+        response_per_theta = response_per_theta.sort_values(by=["theta", "spatial_frequency"])
+
+        theta = response_per_theta[["theta"]].to_numpy().flatten()
+        sf = response_per_theta[["spatial_frequency"]].to_numpy().flatten()
+        response = response_per_theta[[str(unit_id)]].to_numpy().flatten()
+
+        return theta, sf, response
+
+    def orientation_tf_tuning_curve(self, unit_id):
+        preferred_temporal_frequency_query = (
+                self._probes_df["spatial_frequency"]
+                == self.preferred_spatial_frequency(unit_id)
+        )
+        response_per_theta = self._probes_df[
+            preferred_temporal_frequency_query
+        ]
+        # return response_per_theta
+        response_per_theta = response_per_theta.sort_values(by=["theta", "temporal_frequency"])
+
+        theta = response_per_theta[["theta"]].to_numpy().flatten()
+        tf = response_per_theta[["temporal_frequency"]].to_numpy().flatten()
+        response = response_per_theta[[str(unit_id)]].to_numpy().flatten()
+
+        return theta, tf, response
+
     def orientation_selectivity_index(self, unit_id):
         thetas = self._probes_df["theta"].unique()
 
         # Absolute orthogonal to preferred
         orthogonal_orientation = (self.preferred_direction(unit_id) + np.pi / 2) % (
             2 * np.pi
         )
```

### Comparing `brainbox-0.0.6/brainbox/physiology/util.py` & `brainbox-0.0.7/brainbox/physiology/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,30 +61,8 @@
     b_dim, n_dim, t_dim = tensor.shape
     mean_repeated = mean.view(b_dim, n_dim, 1).repeat(1, 1, t_dim)
     sqrd_error_with_zero = torch.pow(tensor - mean_repeated, 2).sum(dim=2)
     sqrd_error_from_mask = zero_mask.sum(dim=2) * torch.pow(mean, 2)
 
     return torch.sqrt(
         (sqrd_error_with_zero - sqrd_error_from_mask) / nonzero_mask.sum(dim=2)
-    )
-
-
-def cross_covariance_matrix(x, y, normalize=True):
-    x_min_mean = x - x.mean(0)
-    y_min_mean = y - y.mean(0)
-
-    b_dim = x.shape[0]
-    cross_covariance_matrix_batch = torch.einsum(
-        "bni, bnj -> nij", x_min_mean, y_min_mean
-    )
-    _cross_covariance_matrix = (
-        cross_covariance_matrix_batch / b_dim
-    )  # Average across samples / batch dim
-
-    if normalize:
-        inv_x_std = torch.nan_to_num(1 / x.std(0, unbiased=False))
-        inv_y_std = torch.nan_to_num(1 / y.std(0, unbiased=False))
-        return torch.einsum(
-            "nij, ni, nj -> nij", _cross_covariance_matrix, inv_x_std, inv_y_std
-        )
-
-    return _cross_covariance_matrix
+    )
```

### Comparing `brainbox-0.0.6/brainbox/trainer/__init__.py` & `brainbox-0.0.7/brainbox/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/trainer/crossval.py` & `brainbox-0.0.7/brainbox/trainer/crossval.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,25 +35,26 @@
     @property
     def y(self):
         return self._dataset.y[self._idxs]
 
 
 class BaseValidationTrainer:
 
-    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None):
+    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None, final_epochs=None):
         self._root = root
         self._model = model
         self._train_dataset = train_dataset
         self._trainer_class = trainer_class
         self._trainer_kwargs = trainer_kwargs
         self._lambdas = lambdas
         self._minimise_score = minimise_score
         self._final_repeat = final_repeat
         self._val_loss = val_loss
         self._val_batch_size = val_batch_size
+        self._final_epochs = final_epochs
 
     @property
     def train_path(self):
         path = os.path.join(self._root, "models")
         if not os.path.exists(path):
             os.makedirs(path)
         
@@ -76,25 +77,31 @@
             if val_score_improvement or best_lam is None:
                 best_lam = lam
                 best_val_score = val_score
 
         # Train on all data and save results and model
         logger.info(f"Fitting for best l1={best_lam}...")
         for i in range(self._final_repeat):
-            self._fit_for_fold(best_lam, self._train_dataset, save=True, id=str(i))
+            self._fit_for_fold(best_lam, self._train_dataset, save=True, id=str(i), n_epochs=self._final_epochs)
 
         cv_results = pd.DataFrame(cv_results)
         cv_results.to_csv(os.path.join(self._root, "cv.csv"), index=False)
 
     def _fit_over_folds(self, lam):
         raise NotImplementedError
 
-    def _fit_for_fold(self, lam, train_dataset, val_dataset=None, save=False, id=None):
+    def _fit_for_fold(self, lam, train_dataset, val_dataset=None, save=False, id=None, n_epochs=None):
         model = copy.deepcopy(self._model)
-        trainer = self._trainer_class(self.train_path, model, train_dataset, lam=lam, **self._trainer_kwargs, id=id)
+
+        _trainer_kwargs = self._trainer_kwargs
+        if n_epochs is not None:
+            print("Changing final n_epochs!")
+            _trainer_kwargs["n_epochs"] = n_epochs
+
+        trainer = self._trainer_class(self.train_path, model, train_dataset, lam=lam, **_trainer_kwargs, id=id)
         trainer.train(save)
 
         if val_dataset is None:
             return self._compute_score(model, train_dataset)
         else:
             train_score = self._compute_score(model, train_dataset)
             val_score = self._compute_score(model, val_dataset)
@@ -107,36 +114,40 @@
             val_loss = lambda output, target: trainer.loss(output, target, model)
         else:
             val_loss = self._val_loss
 
         val_batch_size = trainer.batch_size if self._val_batch_size is None else self._val_batch_size
         score = compute_metric(model, dataset, val_loss, val_batch_size, trainer.device, trainer.dtype)
 
+        # Fixes GPU memory clogging up
+        del model
+        torch.cuda.empty_cache()
+
         return torch.Tensor(score).sum().item()
 
 
 class SplitValidationTrainer(BaseValidationTrainer):
 
-    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, train_idxs, val_idxs, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None):
-        super().__init__(root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score, final_repeat, val_loss, val_batch_size)
+    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, train_idxs, val_idxs, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None, final_epochs=None):
+        super().__init__(root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score, final_repeat, val_loss, val_batch_size, final_epochs)
         self._train_idxs = train_idxs
         self._val_idxs = val_idxs
 
     def _fit_over_folds(self, lam):
         train_dataset = FoldDataset(self._train_dataset, self._train_idxs)
         val_dataset = FoldDataset(self._train_dataset, self._val_idxs)
         train_score, val_score = self._fit_for_fold(lam, train_dataset, val_dataset)
 
         return train_score, val_score
 
 
 class KFoldValidationTrainer(BaseValidationTrainer):
 
-    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, k, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None):
-        super().__init__(root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score, final_repeat, val_loss, val_batch_size)
+    def __init__(self, root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, k, minimise_score=True, final_repeat=1, val_loss=None, val_batch_size=None, final_epochs=None):
+        super().__init__(root, model, train_dataset, trainer_class, trainer_kwargs, lambdas, minimise_score, final_repeat, val_loss, val_batch_size, final_epochs)
         self._k = k
 
     def _fit_over_folds(self, lam):
         kf = KFold(n_splits=self._k, shuffle=False)
 
         train_scores_list = []
         val_scores_list = []
```

### Comparing `brainbox-0.0.6/brainbox/trainer/query.py` & `brainbox-0.0.7/brainbox/trainer/query.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/trainer/trainer.py` & `brainbox-0.0.7/brainbox/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox/trainer/validator.py` & `brainbox-0.0.7/brainbox/trainer/validator.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/brainbox.egg-info/SOURCES.txt` & `brainbox-0.0.7/brainbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/setup.cfg` & `brainbox-0.0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = brainbox
-version = 0.0.6
+version = 0.0.7
 author = Luke Taylor
 author_email = webstorms@gmail.com
 description = Simplifying the life of a computational neuroscientist.
 url = https://github.com/webstorms/BrainBox
 project_urls = 
 	Bug Tracker = https://github.com/webstorms/BrainBox/issues
 classifiers = 
@@ -18,12 +18,13 @@
 install_requires = 
 	pandas
 	h5py
 	torch
 	torchvision
 	kornia
 	scipy
+	scikit-learn
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `brainbox-0.0.6/tests/physiology/test_spiking.py` & `brainbox-0.0.7/tests/physiology/test_spiking.py`

 * *Files identical despite different names*

### Comparing `brainbox-0.0.6/tests/physiology/test_util.py` & `brainbox-0.0.7/tests/physiology/test_util.py`

 * *Files identical despite different names*

