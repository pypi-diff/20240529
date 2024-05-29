# Comparing `tmp/qiskit_alice_bob_provider-0.6.0.tar.gz` & `tmp/qiskit_alice_bob_provider-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_alice_bob_provider-0.6.0.tar", last modified: Wed Apr 24 08:39:32 2024, max compression
+gzip compressed data, was "qiskit_alice_bob_provider-0.7.0.tar", last modified: Wed May 29 12:25:17 2024, max compression
```

## Comparing `qiskit_alice_bob_provider-0.6.0.tar` & `qiskit_alice_bob_provider-0.7.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.449397 qiskit_alice_bob_provider-0.6.0/
--rw-r--r--   0 mdrutel    (501) staff       (20)    11342 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/LICENSE
--rw-r--r--   0 mdrutel    (501) staff       (20)       91 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/MANIFEST.in
--rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-24 08:39:32.449164 qiskit_alice_bob_provider-0.6.0/PKG-INFO
--rw-r--r--   0 mdrutel    (501) staff       (20)     3577 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/README.md
--rw-r--r--   0 mdrutel    (501) staff       (20)     2669 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/pyproject.toml
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.440059 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/
--rw-r--r--   0 mdrutel    (501) staff       (20)      867 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2490 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/custom_instructions.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1039 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/errors.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442420 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/
--rw-r--r--   0 mdrutel    (501) staff       (20)      827 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7765 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/backend.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1905 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/coupling_maps.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7453 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/instruction_durations.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2295 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/job.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442679 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/
--rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7427 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2694 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6679 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/provider.py
--rw-r--r--   0 mdrutel    (501) staff       (20)    11750 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/quantum_errors.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/readout_errors.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.442848 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/
--rw-r--r--   0 mdrutel    (501) staff       (20)   257895 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
--rw-r--r--   0 mdrutel    (501) staff       (20)     4429 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/target.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.444416 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/
--rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6613 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     9375 2024-04-19 10:02:33.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/state_preparation.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.445480 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/
--rw-r--r--   0 mdrutel    (501) staff       (20)     1226 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4840 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/description.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     3112 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/interpolated_cat.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     8903 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/logical_cat.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     9624 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/physical_cat.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.445920 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/
--rw-r--r--   0 mdrutel    (501) staff       (20)     1005 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7780 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4002 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/model.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     7850 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/utils.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.446843 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/
--rw-r--r--   0 mdrutel    (501) staff       (20)      828 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/__init__.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.447506 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/
--rw-r--r--   0 mdrutel    (501) staff       (20)      760 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/__init__.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     3681 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/client.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     4881 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/jobs.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     2261 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/models.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     1286 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/targets.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6806 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/backend.py
--rw-r--r--   0 mdrutel    (501) staff       (20)    10829 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/job.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     3479 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/provider.py
--rw-r--r--   0 mdrutel    (501) staff       (20)     6149 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
--rw-r--r--   0 mdrutel    (501) staff       (20)      408 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/utils.py
-drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-04-24 08:39:32.447689 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/
--rw-r--r--   0 mdrutel    (501) staff       (20)     5650 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/PKG-INFO
--rw-r--r--   0 mdrutel    (501) staff       (20)     2251 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)        1 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/dependency_links.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)      207 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/entry_points.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)      387 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/requires.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)       26 2024-04-24 08:39:32.000000 qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/top_level.txt
--rw-r--r--   0 mdrutel    (501) staff       (20)       38 2024-04-24 08:39:32.449442 qiskit_alice_bob_provider-0.6.0/setup.cfg
--rw-r--r--   0 mdrutel    (501) staff       (20)       69 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.6.0/setup.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.310358 qiskit_alice_bob_provider-0.7.0/
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11342 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/LICENSE
+-rw-r--r--   0 mdrutel    (501) staff       (20)       91 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/MANIFEST.in
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5810 2024-05-29 12:25:17.310076 qiskit_alice_bob_provider-0.7.0/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3524 2024-05-28 14:37:36.000000 qiskit_alice_bob_provider-0.7.0/README.md
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2787 2024-05-29 12:25:08.000000 qiskit_alice_bob_provider-0.7.0/pyproject.toml
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.299413 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      867 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2490 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/custom_instructions.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1039 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.302565 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      827 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7765 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1905 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/coupling_maps.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7453 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/instruction_durations.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2295 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/job.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.302916 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/patch/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/patch/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7427 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2694 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6679 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)    11750 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/quantum_errors.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4375 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/readout_errors.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.303174 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/resources/
+-rw-r--r--   0 mdrutel    (501) staff       (20)   257895 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4429 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/target.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.304595 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/
+-rw-r--r--   0 mdrutel    (501) staff       (20)        0 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6613 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9375 2024-04-19 10:02:33.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/state_preparation.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.305812 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1226 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4840 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/description.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3112 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/interpolated_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     8903 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/logical_cat.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     9624 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/physical_cat.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.306292 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1005 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7780 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4002 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/model.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     7850 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/utils.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.307210 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      828 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/__init__.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.308114 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/
+-rw-r--r--   0 mdrutel    (501) staff       (20)      760 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/__init__.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     3681 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/client.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4881 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/jobs.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2261 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/models.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1286 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/targets.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     1026 2024-05-29 12:25:08.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/version.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6806 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/backend.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)    10829 2024-04-24 08:39:20.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/job.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     4124 2024-05-29 12:25:08.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/provider.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)     6149 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py
+-rw-r--r--   0 mdrutel    (501) staff       (20)      408 2024-05-29 09:49:05.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/utils.py
+drwxr-xr-x   0 mdrutel    (501) staff       (20)        0 2024-05-29 12:25:17.308303 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/
+-rw-r--r--   0 mdrutel    (501) staff       (20)     5810 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/PKG-INFO
+-rw-r--r--   0 mdrutel    (501) staff       (20)     2299 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)        1 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      207 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/entry_points.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)      469 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/requires.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       26 2024-05-29 12:25:17.000000 qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/top_level.txt
+-rw-r--r--   0 mdrutel    (501) staff       (20)       38 2024-05-29 12:25:17.310407 qiskit_alice_bob_provider-0.7.0/setup.cfg
+-rw-r--r--   0 mdrutel    (501) staff       (20)       69 2024-04-15 14:47:24.000000 qiskit_alice_bob_provider-0.7.0/setup.py
```

### Comparing `qiskit_alice_bob_provider-0.6.0/LICENSE` & `qiskit_alice_bob_provider-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/PKG-INFO` & `qiskit_alice_bob_provider-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.6.0
+Version: 0.7.0
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: qiskit<0.45
 Requires-Dist: qiskit-terra<0.45.0,>=0.24.0
 Requires-Dist: qiskit-aer<0.13.0
 Requires-Dist: qiskit-qir-alice-bob-fork==0.3.2rc0
@@ -33,34 +33,38 @@
 Provides-Extra: dev
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: codespell==2.2.2; extra == "dev"
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: flake8-quotes==3.3.2; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
+Requires-Dist: mock==5.1.0; extra == "dev"
 Requires-Dist: mypy==1.0.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.21.0; extra == "dev"
 Requires-Dist: pylint==2.16.1; extra == "dev"
 Requires-Dist: pytest==7.2.1; extra == "dev"
 Requires-Dist: requests-mock==1.10.0; extra == "dev"
-Requires-Dist: types-requests==2.30.0.0; extra == "dev"
+Requires-Dist: traitlets==5.14.3; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: types-mock==5.1.0; extra == "dev"
+Requires-Dist: types-setuptools==70.0.0.20240524; extra == "dev"
+Requires-Dist: types-requests==2.30.0.0; extra == "dev"
 Requires-Dist: build==0.10.0; extra == "dev"
 
 # Alice & Bob Qiskit provider
 
 This project contains a provider that allows access to
 [Alice & Bob](https://alice-bob.com/) QPUs and emulators using
 the Qiskit framework.
 
 Full documentation
-[is available here](https://alice-bob.notion.site/Alice-Bob-Felis-documentation-52e554ccbea54e34831761f083883e49)
+[is available here](https://felis.alice-bob.com/docs/)
 and sample notebooks using the provider
-[are available here](https://github.com/Alice-Bob-SW/emulation-examples).
+[are available here](https://github.com/Alice-Bob-SW/felis/tree/main/samples).
 
 ## Installation
 
 You can install the provider using `pip`:
 
 ```bash
 pip install qiskit-alice-bob-provider
@@ -98,15 +102,15 @@
 c.measure_x(0, 0)
 c.measure(0, 1)
 job = execute(c, backend)
 res = job.result()
 print(res.get_counts())
 ```
 
-## Local emulation of cat quit processors
+## Local emulation of cat qubit processors
 
 This project contains multiple emulators of multi cat qubit processors.
 
 ```python
 from qiskit_alice_bob_provider import AliceBobLocalProvider
 from qiskit import QuantumCircuit, execute, transpile
```

### Comparing `qiskit_alice_bob_provider-0.6.0/README.md` & `qiskit_alice_bob_provider-0.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Alice & Bob Qiskit provider
 
 This project contains a provider that allows access to
 [Alice & Bob](https://alice-bob.com/) QPUs and emulators using
 the Qiskit framework.
 
 Full documentation
-[is available here](https://alice-bob.notion.site/Alice-Bob-Felis-documentation-52e554ccbea54e34831761f083883e49)
+[is available here](https://felis.alice-bob.com/docs/)
 and sample notebooks using the provider
-[are available here](https://github.com/Alice-Bob-SW/emulation-examples).
+[are available here](https://github.com/Alice-Bob-SW/felis/tree/main/samples).
 
 ## Installation
 
 You can install the provider using `pip`:
 
 ```bash
 pip install qiskit-alice-bob-provider
@@ -49,15 +49,15 @@
 c.measure_x(0, 0)
 c.measure(0, 1)
 job = execute(c, backend)
 res = job.result()
 print(res.get_counts())
 ```
 
-## Local emulation of cat quit processors
+## Local emulation of cat qubit processors
 
 This project contains multiple emulators of multi cat qubit processors.
 
 ```python
 from qiskit_alice_bob_provider import AliceBobLocalProvider
 from qiskit import QuantumCircuit, execute, transpile
```

### Comparing `qiskit_alice_bob_provider-0.6.0/pyproject.toml` & `qiskit_alice_bob_provider-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qiskit_alice_bob_provider"
 authors = [
     {name = "Alice & Bob Software Team"},
 ]
-version = "0.6.0"
+version = "0.7.0"
 description = "Provider for running Qiskit circuits on Alice & Bob QPUs and simulators"
 readme = "README.md"
 license = {text = "Apache 2.0"}
 keywords = ["Qiskit", "Alice & Bob", "Quantum", "SDK"]
 classifiers=[
     "Environment :: Console",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 urls = {Homepage = "https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider", "Alice & Bob" = "https://alice-bob.com/"}
-requires-python = ">=3.7"
+requires-python = ">=3.8, <3.12"
 dependencies = [
     "requests",
     "qiskit<0.45",
     # >=0.24.0: required for correct handling of durations
     # <0.45.0: this version introduces many API changes that we need to integrate
     "qiskit-terra>=0.24.0,<0.45.0",
     # <0.13.0: qiskit-aer has become irritatingly slow in this release.
@@ -47,22 +47,26 @@
 dev = [
     "black==23.1.0",
     "codespell==2.2.2",
     "coverage==7.2.2",
     "flake8>=5.0.4",
     "flake8-quotes==3.3.2",
     "isort>=5.11.5",
+    "mock==5.1.0",
     "mypy==1.0.0",
     "mypy-extensions==1.0.0",
     "pre-commit>=2.21.0",
     "pylint==2.16.1",
     "pytest==7.2.1",
     "requests-mock==1.10.0",
-    "types-requests==2.30.0.0",
+    "traitlets==5.14.3",
     "twine==4.0.2",
+    "types-mock==5.1.0",
+    "types-setuptools==70.0.0.20240524",
+    "types-requests==2.30.0.0",
     "build==0.10.0"
 ]
 
 [project.entry-points."qiskit.transpiler.translation"]
 state_preparation = "qiskit_alice_bob_provider.plugins.state_preparation:StatePreparationPlugin"
 sk_synthesis = "qiskit_alice_bob_provider.plugins.sk_synthesis:SKSynthesisPlugin"
```

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/custom_instructions.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/custom_instructions.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/errors.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/backend.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/coupling_maps.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/coupling_maps.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/instruction_durations.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/instruction_durations.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/job.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/patch/local_noise_pass.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/proc_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/provider.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/quantum_errors.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/quantum_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/readout_errors.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/readout_errors.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/resources/lescanne_2020.json`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/local/target.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/local/target.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/sk_synthesis.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/plugins/state_preparation.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/plugins/state_preparation.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/description.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/description.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/interpolated_cat.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/interpolated_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/logical_cat.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/logical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/physical_cat.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/physical_cat.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/interpolate.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/serialization/model.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/serialization/model.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/processor/utils.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/processor/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/__init__.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/client.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/jobs.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/jobs.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/models.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/models.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/api/targets.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/api/targets.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/backend.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/job.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/job.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/provider.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,52 +10,70 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 
+import logging
 from typing import List, Optional
 
 from qiskit.providers import BackendV2, ProviderV1
 from qiskit.providers.providerutils import filter_backends
 
+from qiskit_alice_bob_provider.remote.api.version import (
+    ProviderStatus,
+    get_provider_status,
+)
+
 from .api.client import ApiClient
 from .api.targets import list_targets
 from .backend import AliceBobRemoteBackend
 
 
 class AliceBobRemoteProvider(ProviderV1):
     """
     Class listing and providing access to all Alice & Bob remote backends.
     """
 
     def __init__(
         self,
         api_key: str,
-        url: str = 'https://api.alice-bob.com/',
+        url: str = 'https://api-gcp.alice-bob.com/',
         retries: int = 5,
         wait_between_retries_seconds: int = 1,
     ):
         """
         Args:
             api_key (str): an API key for the Alice & Bob API
             url (str): Base URL of the Alice & Bob API.
-                Defaults to 'https://api.alice-bob.com/'.
+                Defaults to 'https://api-gcp.alice-bob.com/'.
         """
         client = ApiClient(
             api_key=api_key,
             url=url,
             retries=retries,
             wait_between_retries_seconds=wait_between_retries_seconds,
         )
         self._backends = []
         for ab_target in list_targets(client):
             self._backends.append(AliceBobRemoteBackend(client, ab_target))
 
+        provider_status = get_provider_status()
+        if provider_status == ProviderStatus.UNKNOWN:
+            logging.warning(
+                'Could not determine the latest version of the provider. '
+                'Your installation may be outdated.'
+            )
+        elif provider_status == ProviderStatus.OUTDATED:
+            logging.warning(
+                'A new version of the provider is available. Install it with '
+                '"pip install -U qiskit-alice-bob-provider".'
+            )
+
     def get_backend(
         self, name=None, verbose=True, **kwargs
     ) -> AliceBobRemoteBackend:
         """Return a single backend matching by its name.
 
         Args:
             name (str): name of the backend
```

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider/remote/qir_to_qiskit.py`

 * *Files identical despite different names*

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/PKG-INFO` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: qiskit_alice_bob_provider
-Version: 0.6.0
+Version: 0.7.0
 Summary: Provider for running Qiskit circuits on Alice & Bob QPUs and simulators
 Author: Alice & Bob Software Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
 Project-URL: Alice & Bob, https://alice-bob.com/
 Keywords: Qiskit,Alice & Bob,Quantum,SDK
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: qiskit<0.45
 Requires-Dist: qiskit-terra<0.45.0,>=0.24.0
 Requires-Dist: qiskit-aer<0.13.0
 Requires-Dist: qiskit-qir-alice-bob-fork==0.3.2rc0
@@ -33,34 +33,38 @@
 Provides-Extra: dev
 Requires-Dist: black==23.1.0; extra == "dev"
 Requires-Dist: codespell==2.2.2; extra == "dev"
 Requires-Dist: coverage==7.2.2; extra == "dev"
 Requires-Dist: flake8>=5.0.4; extra == "dev"
 Requires-Dist: flake8-quotes==3.3.2; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
+Requires-Dist: mock==5.1.0; extra == "dev"
 Requires-Dist: mypy==1.0.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=2.21.0; extra == "dev"
 Requires-Dist: pylint==2.16.1; extra == "dev"
 Requires-Dist: pytest==7.2.1; extra == "dev"
 Requires-Dist: requests-mock==1.10.0; extra == "dev"
-Requires-Dist: types-requests==2.30.0.0; extra == "dev"
+Requires-Dist: traitlets==5.14.3; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
+Requires-Dist: types-mock==5.1.0; extra == "dev"
+Requires-Dist: types-setuptools==70.0.0.20240524; extra == "dev"
+Requires-Dist: types-requests==2.30.0.0; extra == "dev"
 Requires-Dist: build==0.10.0; extra == "dev"
 
 # Alice & Bob Qiskit provider
 
 This project contains a provider that allows access to
 [Alice & Bob](https://alice-bob.com/) QPUs and emulators using
 the Qiskit framework.
 
 Full documentation
-[is available here](https://alice-bob.notion.site/Alice-Bob-Felis-documentation-52e554ccbea54e34831761f083883e49)
+[is available here](https://felis.alice-bob.com/docs/)
 and sample notebooks using the provider
-[are available here](https://github.com/Alice-Bob-SW/emulation-examples).
+[are available here](https://github.com/Alice-Bob-SW/felis/tree/main/samples).
 
 ## Installation
 
 You can install the provider using `pip`:
 
 ```bash
 pip install qiskit-alice-bob-provider
@@ -98,15 +102,15 @@
 c.measure_x(0, 0)
 c.measure(0, 1)
 job = execute(c, backend)
 res = job.result()
 print(res.get_counts())
 ```
 
-## Local emulation of cat quit processors
+## Local emulation of cat qubit processors
 
 This project contains multiple emulators of multi cat qubit processors.
 
 ```python
 from qiskit_alice_bob_provider import AliceBobLocalProvider
 from qiskit import QuantumCircuit, execute, transpile
```

### Comparing `qiskit_alice_bob_provider-0.6.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt` & `qiskit_alice_bob_provider-0.7.0/qiskit_alice_bob_provider.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,9 @@
 qiskit_alice_bob_provider/remote/provider.py
 qiskit_alice_bob_provider/remote/qir_to_qiskit.py
 qiskit_alice_bob_provider/remote/utils.py
 qiskit_alice_bob_provider/remote/api/__init__.py
 qiskit_alice_bob_provider/remote/api/client.py
 qiskit_alice_bob_provider/remote/api/jobs.py
 qiskit_alice_bob_provider/remote/api/models.py
-qiskit_alice_bob_provider/remote/api/targets.py
+qiskit_alice_bob_provider/remote/api/targets.py
+qiskit_alice_bob_provider/remote/api/version.py
```

