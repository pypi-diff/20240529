# Comparing `tmp/google-maps-mapsplatformdatasets-0.3.7.tar.gz` & `tmp/google-maps-mapsplatformdatasets-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-maps-mapsplatformdatasets-0.3.7.tar", last modified: Tue Mar  5 19:01:33 2024, max compression
+gzip compressed data, was "google-maps-mapsplatformdatasets-0.4.0.tar", last modified: Wed May 29 16:20:04 2024, max compression
```

## Comparing `google-maps-mapsplatformdatasets-0.3.7.tar` & `google-maps-mapsplatformdatasets-0.4.0.tar`

### file list

```diff
@@ -1,80 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.075641 google-maps-mapsplatformdatasets-0.3.7/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5240 2024-03-05 19:01:33.075641 google-maps-mapsplatformdatasets-0.3.7/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3840 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.055639 google-maps-mapsplatformdatasets-0.3.7/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.055639 google-maps-mapsplatformdatasets-0.3.7/google/maps/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.059640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/
--rw-rw-r--   0 root         (0)     1003     2059 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.059640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/
--rw-rw-r--   0 root         (0)     1003     1530 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2561 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.059640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.063640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/
--rw-rw-r--   0 root         (0)     1003      793 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py
--rw-rw-r--   0 root         (0)     1003    34291 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py
--rw-rw-r--   0 root         (0)     1003    50807 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py
--rw-rw-r--   0 root         (0)     1003     5952 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.063640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/
--rw-rw-r--   0 root         (0)     1003     1492 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8866 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16654 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17004 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    31768 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.063640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/
--rw-rw-r--   0 root         (0)     1003     1195 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2554 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/data_source.py
--rw-rw-r--   0 root         (0)     1003     7560 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     4791 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py
--rw-rw-r--   0 root         (0)     1003      778 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.067640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/
--rw-rw-r--   0 root         (0)     1003     1772 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003     3415 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       93 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.067640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.067640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/
--rw-rw-r--   0 root         (0)     1003      821 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    44257 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/async_client.py
--rw-rw-r--   0 root         (0)     1003    60809 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/client.py
--rw-rw-r--   0 root         (0)     1003    11389 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.067640 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/
--rw-rw-r--   0 root         (0)     1003     1603 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10258 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19404 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19811 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41551 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/maps_platform_datasets_v1_alpha/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     1395 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2754 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/data_source.py
--rw-rw-r--   0 root         (0)     1003     6072 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/dataset.py
--rw-rw-r--   0 root         (0)     1003     8145 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets.py
--rw-rw-r--   0 root         (0)     1003      783 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/types/maps_platform_datasets_alpha_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/
--rw-r--r--   0 root         (0)     1003     5240 2024-03-05 19:01:32.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3699 2024-03-05 19:01:33.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:32.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:32.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-05 19:01:32.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:32.000000 google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:33.075641 google-maps-mapsplatformdatasets-0.3.7/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3217 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.071641 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   185116 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:33.075641 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   235500 2024-03-05 18:46:03.000000 google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1alpha/test_maps_platform_datasets_v1_alpha.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5240 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3840 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.571541 google-maps-mapsplatformdatasets-0.4.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.571541 google-maps-mapsplatformdatasets-0.4.0/google/maps/
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.575541 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/
+-rw-rw-r--   0 root         (0)     1003     1788 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.575541 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/
+-rw-rw-r--   0 root         (0)     1003     1530 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2561 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       93 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.575541 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.579542 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/
+-rw-rw-r--   0 root         (0)     1003      793 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35221 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51434 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py
+-rw-rw-r--   0 root         (0)     1003     5952 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.579542 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/
+-rw-rw-r--   0 root         (0)     1003     1492 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8866 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17205 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19478 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    31682 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.579542 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1195 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2554 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/data_source.py
+-rw-rw-r--   0 root         (0)     1003     7622 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/dataset.py
+-rw-rw-r--   0 root         (0)     1003     5704 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py
+-rw-rw-r--   0 root         (0)     1003      778 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/
+-rw-r--r--   0 root         (0)     1003     5240 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2039 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-05-29 16:20:04.000000 google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3217 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-29 16:20:04.583542 google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/mapsplatformdatasets_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   218723 2024-05-29 16:16:35.000000 google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/LICENSE` & `google-maps-mapsplatformdatasets-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.7/MANIFEST.in` & `google-maps-mapsplatformdatasets-0.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.7/PKG-INFO` & `google-maps-mapsplatformdatasets-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-mapsplatformdatasets
-Version: 0.3.7
+Version: 0.4.0
 Summary: Google Maps Mapsplatformdatasets API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-mapsplatformdatasets
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/README.rst` & `google-maps-mapsplatformdatasets-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,50 +14,44 @@
 # limitations under the License.
 #
 from google.maps.mapsplatformdatasets import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
-from google.maps.mapsplatformdatasets_v1alpha.services.maps_platform_datasets_v1_alpha.async_client import (
-    MapsPlatformDatasetsV1AlphaAsyncClient,
+from google.maps.mapsplatformdatasets_v1.services.maps_platform_datasets.async_client import (
+    MapsPlatformDatasetsAsyncClient,
 )
-from google.maps.mapsplatformdatasets_v1alpha.services.maps_platform_datasets_v1_alpha.client import (
-    MapsPlatformDatasetsV1AlphaClient,
+from google.maps.mapsplatformdatasets_v1.services.maps_platform_datasets.client import (
+    MapsPlatformDatasetsClient,
 )
-from google.maps.mapsplatformdatasets_v1alpha.types.data_source import (
+from google.maps.mapsplatformdatasets_v1.types.data_source import (
     FileFormat,
     GcsSource,
     LocalFileSource,
 )
-from google.maps.mapsplatformdatasets_v1alpha.types.dataset import Dataset, State, Usage
-from google.maps.mapsplatformdatasets_v1alpha.types.maps_platform_datasets import (
+from google.maps.mapsplatformdatasets_v1.types.dataset import Dataset, Status, Usage
+from google.maps.mapsplatformdatasets_v1.types.maps_platform_datasets import (
     CreateDatasetRequest,
     DeleteDatasetRequest,
-    DeleteDatasetVersionRequest,
     GetDatasetRequest,
     ListDatasetsRequest,
     ListDatasetsResponse,
-    ListDatasetVersionsRequest,
-    ListDatasetVersionsResponse,
     UpdateDatasetMetadataRequest,
 )
 
 __all__ = (
-    "MapsPlatformDatasetsV1AlphaClient",
-    "MapsPlatformDatasetsV1AlphaAsyncClient",
+    "MapsPlatformDatasetsClient",
+    "MapsPlatformDatasetsAsyncClient",
     "GcsSource",
     "LocalFileSource",
     "FileFormat",
     "Dataset",
-    "State",
+    "Status",
     "Usage",
     "CreateDatasetRequest",
     "DeleteDatasetRequest",
-    "DeleteDatasetVersionRequest",
     "GetDatasetRequest",
     "ListDatasetsRequest",
     "ListDatasetsResponse",
-    "ListDatasetVersionsRequest",
-    "ListDatasetVersionsResponse",
     "UpdateDatasetMetadataRequest",
 )
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets/gapic_version.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.7"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/gapic_metadata.json` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/gapic_version.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.7"  # {x-release-please-version}
+__version__ = "0.4.0"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/async_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import functools
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -197,29 +198,37 @@
         type(MapsPlatformDatasetsClient),
     )
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Union[str, MapsPlatformDatasetsTransport] = "grpc_asyncio",
+        transport: Optional[
+            Union[
+                str,
+                MapsPlatformDatasetsTransport,
+                Callable[..., MapsPlatformDatasetsTransport],
+            ]
+        ] = "grpc_asyncio",
         client_options: Optional[ClientOptions] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the maps platform datasets async client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, ~.MapsPlatformDatasetsTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,MapsPlatformDatasetsTransport,Callable[..., MapsPlatformDatasetsTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport to use.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the MapsPlatformDatasetsTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -267,15 +276,15 @@
         *,
         parent: Optional[str] = None,
         dataset: Optional[gmm_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gmm_dataset.Dataset:
-        r"""Create a new dataset for the specified project.
+        r"""Creates a new dataset for the specified project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -301,15 +310,15 @@
 
         Args:
             request (Optional[Union[google.maps.mapsplatformdatasets_v1.types.CreateDatasetRequest, dict]]):
                 The request object. Request to create a maps dataset.
             parent (:class:`str`):
                 Required. Parent project that will
                 own the dataset. Format:
-                projects/{$project}
+                projects/{project}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             dataset (:class:`google.maps.mapsplatformdatasets_v1.types.Dataset`):
                 Required. The dataset version to
                 create.
@@ -321,44 +330,45 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, dataset])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = maps_platform_datasets.CreateDatasetRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, maps_platform_datasets.CreateDatasetRequest):
+            request = maps_platform_datasets.CreateDatasetRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
         if dataset is not None:
             request.dataset = dataset
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.create_dataset,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.create_dataset
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -384,15 +394,15 @@
         *,
         dataset: Optional[gmm_dataset.Dataset] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gmm_dataset.Dataset:
-        r"""Update the metadata for the dataset.
+        r"""Updates the metadata for the dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -416,66 +426,67 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.maps.mapsplatformdatasets_v1.types.UpdateDatasetMetadataRequest, dict]]):
                 The request object. Request to update the metadata fields
                 of the dataset.
             dataset (:class:`google.maps.mapsplatformdatasets_v1.types.Dataset`):
-                Required. The dataset to update. The dataset's name is
-                used to identify the dataset to be updated. The name has
-                the format: projects/{project}/datasets/{dataset_id}
+                Required. Resource name of the dataset to update.
+                Format: projects/{project}/datasets/{dataset_id}
 
                 This corresponds to the ``dataset`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
-                The list of fields to be updated. Support the value "*"
-                for full replacement.
+                The list of fields to be updated.
+
+                The value "*" is used for full replacement (default).
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([dataset, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = maps_platform_datasets.UpdateDatasetMetadataRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, maps_platform_datasets.UpdateDatasetMetadataRequest):
+            request = maps_platform_datasets.UpdateDatasetMetadataRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if dataset is not None:
             request.dataset = dataset
         if update_mask is not None:
             request.update_mask = update_mask
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.update_dataset_metadata,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.update_dataset_metadata
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata(
                 (("dataset.name", request.dataset.name),)
             ),
@@ -500,15 +511,15 @@
         request: Optional[Union[maps_platform_datasets.GetDatasetRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
-        r"""Get the dataset.
+        r"""Gets the dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -532,65 +543,65 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Optional[Union[google.maps.mapsplatformdatasets_v1.types.GetDatasetRequest, dict]]):
                 The request object. Request to get the specified dataset.
             name (:class:`str`):
-                Required. Resource name.
+                Required. Resource name. Format:
                 projects/{project}/datasets/{dataset_id}
 
+                Can also fetch some special versions by appending "@"
+                and a tag. Format:
+                projects/{project}/datasets/{dataset_id}@{tag}
+
+                Tag "active": The info of the latest completed version
+                will be included, and NOT_FOUND if the dataset does not
+                have one.
+
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = maps_platform_datasets.GetDatasetRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, maps_platform_datasets.GetDatasetRequest):
+            request = maps_platform_datasets.GetDatasetRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.get_dataset,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.get_dataset
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
@@ -615,15 +626,15 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsAsyncPager:
-        r"""List all the datasets for the specified project.
+        r"""Lists all the datasets for the specified project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -650,67 +661,60 @@
 
         Args:
             request (Optional[Union[google.maps.mapsplatformdatasets_v1.types.ListDatasetsRequest, dict]]):
                 The request object. Request to list datasets for the
                 project.
             parent (:class:`str`):
                 Required. The name of the project to
-                list all the datasets for.
+                list all the datasets for. Format:
+                projects/{project}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.services.maps_platform_datasets.pagers.ListDatasetsAsyncPager:
-                Response to list datasets for the
-                project.
+                Response object of ListDatasets.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = maps_platform_datasets.ListDatasetsRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, maps_platform_datasets.ListDatasetsRequest):
+            request = maps_platform_datasets.ListDatasetsRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if parent is not None:
             request.parent = parent
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.list_datasets,
-            default_retry=retries.AsyncRetry(
-                initial=1.0,
-                maximum=10.0,
-                multiplier=1.3,
-                predicate=retries.if_exception_type(
-                    core_exceptions.ServiceUnavailable,
-                ),
-                deadline=60.0,
-            ),
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.list_datasets
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("parent", request.parent),)),
         )
 
@@ -744,15 +748,15 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Delete the specified dataset .
+        r"""Deletes the specified dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -772,53 +776,52 @@
 
                 # Make the request
                 await client.delete_dataset(request=request)
 
         Args:
             request (Optional[Union[google.maps.mapsplatformdatasets_v1.types.DeleteDatasetRequest, dict]]):
                 The request object. Request to delete a dataset.
-
-                The dataset to be deleted.
             name (:class:`str`):
-                Required. Format:
-                projects/${project}/datasets/{dataset_id}
+                Required. The name of the dataset to delete. Format:
+                projects/{project}/datasets/{dataset_id}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        request = maps_platform_datasets.DeleteDatasetRequest(request)
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
+        if not isinstance(request, maps_platform_datasets.DeleteDatasetRequest):
+            request = maps_platform_datasets.DeleteDatasetRequest(request)
 
         # If we have keyword arguments corresponding to fields on the
         # request, apply these.
         if name is not None:
             request.name = name
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
-        rpc = gapic_v1.method_async.wrap_method(
-            self._client._transport.delete_dataset,
-            default_timeout=60.0,
-            client_info=DEFAULT_CLIENT_INFO,
-        )
+        rpc = self._client._transport._wrapped_methods[
+            self._client._transport.delete_dataset
+        ]
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 import os
 import re
 from typing import (
+    Callable,
     Dict,
     Mapping,
     MutableMapping,
     MutableSequence,
     Optional,
     Sequence,
     Tuple,
@@ -526,29 +527,37 @@
         """
         return self._universe_domain
 
     def __init__(
         self,
         *,
         credentials: Optional[ga_credentials.Credentials] = None,
-        transport: Optional[Union[str, MapsPlatformDatasetsTransport]] = None,
+        transport: Optional[
+            Union[
+                str,
+                MapsPlatformDatasetsTransport,
+                Callable[..., MapsPlatformDatasetsTransport],
+            ]
+        ] = None,
         client_options: Optional[Union[client_options_lib.ClientOptions, dict]] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
     ) -> None:
         """Instantiates the maps platform datasets client.
 
         Args:
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-            transport (Union[str, MapsPlatformDatasetsTransport]): The
-                transport to use. If set to None, a transport is chosen
-                automatically.
+            transport (Optional[Union[str,MapsPlatformDatasetsTransport,Callable[..., MapsPlatformDatasetsTransport]]]):
+                The transport to use, or a Callable that constructs and returns a new transport.
+                If a Callable is given, it will be called with the same set of initialization
+                arguments as used in the MapsPlatformDatasetsTransport constructor.
+                If set to None, a transport is chosen automatically.
             client_options (Optional[Union[google.api_core.client_options.ClientOptions, dict]]):
                 Custom options for the client.
 
                 1. The ``api_endpoint`` property can be used to override the
                 default endpoint provided by the client when ``transport`` is
                 not explicitly provided. Only if this property is not set and
                 ``transport`` was not explicitly provided, the endpoint is
@@ -649,16 +658,24 @@
             if api_key_value and hasattr(
                 google.auth._default, "get_api_key_credentials"
             ):
                 credentials = google.auth._default.get_api_key_credentials(
                     api_key_value
                 )
 
-            Transport = type(self).get_transport_class(cast(str, transport))
-            self._transport = Transport(
+            transport_init: Union[
+                Type[MapsPlatformDatasetsTransport],
+                Callable[..., MapsPlatformDatasetsTransport],
+            ] = (
+                type(self).get_transport_class(transport)
+                if isinstance(transport, str) or transport is None
+                else cast(Callable[..., MapsPlatformDatasetsTransport], transport)
+            )
+            # initialize with the provided callable or the passed in class
+            self._transport = transport_init(
                 credentials=credentials,
                 credentials_file=self._client_options.credentials_file,
                 host=self._api_endpoint,
                 scopes=self._client_options.scopes,
                 client_cert_source_for_mtls=self._client_cert_source,
                 quota_project_id=self._client_options.quota_project_id,
                 client_info=client_info,
@@ -674,15 +691,15 @@
         *,
         parent: Optional[str] = None,
         dataset: Optional[gmm_dataset.Dataset] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gmm_dataset.Dataset:
-        r"""Create a new dataset for the specified project.
+        r"""Creates a new dataset for the specified project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -708,15 +725,15 @@
 
         Args:
             request (Union[google.maps.mapsplatformdatasets_v1.types.CreateDatasetRequest, dict]):
                 The request object. Request to create a maps dataset.
             parent (str):
                 Required. Parent project that will
                 own the dataset. Format:
-                projects/{$project}
+                projects/{project}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             dataset (google.maps.mapsplatformdatasets_v1.types.Dataset):
                 Required. The dataset version to
                 create.
@@ -728,32 +745,30 @@
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent, dataset])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a maps_platform_datasets.CreateDatasetRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, maps_platform_datasets.CreateDatasetRequest):
             request = maps_platform_datasets.CreateDatasetRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
             if dataset is not None:
@@ -791,15 +806,15 @@
         *,
         dataset: Optional[gmm_dataset.Dataset] = None,
         update_mask: Optional[field_mask_pb2.FieldMask] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> gmm_dataset.Dataset:
-        r"""Update the metadata for the dataset.
+        r"""Updates the metadata for the dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -823,54 +838,52 @@
                 print(response)
 
         Args:
             request (Union[google.maps.mapsplatformdatasets_v1.types.UpdateDatasetMetadataRequest, dict]):
                 The request object. Request to update the metadata fields
                 of the dataset.
             dataset (google.maps.mapsplatformdatasets_v1.types.Dataset):
-                Required. The dataset to update. The dataset's name is
-                used to identify the dataset to be updated. The name has
-                the format: projects/{project}/datasets/{dataset_id}
+                Required. Resource name of the dataset to update.
+                Format: projects/{project}/datasets/{dataset_id}
 
                 This corresponds to the ``dataset`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
-                The list of fields to be updated. Support the value "*"
-                for full replacement.
+                The list of fields to be updated.
+
+                The value "*" is used for full replacement (default).
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([dataset, update_mask])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a maps_platform_datasets.UpdateDatasetMetadataRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, maps_platform_datasets.UpdateDatasetMetadataRequest):
             request = maps_platform_datasets.UpdateDatasetMetadataRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if dataset is not None:
                 request.dataset = dataset
             if update_mask is not None:
@@ -907,15 +920,15 @@
         request: Optional[Union[maps_platform_datasets.GetDatasetRequest, dict]] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> dataset.Dataset:
-        r"""Get the dataset.
+        r"""Gets the dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -939,46 +952,52 @@
                 # Handle the response
                 print(response)
 
         Args:
             request (Union[google.maps.mapsplatformdatasets_v1.types.GetDatasetRequest, dict]):
                 The request object. Request to get the specified dataset.
             name (str):
-                Required. Resource name.
+                Required. Resource name. Format:
                 projects/{project}/datasets/{dataset_id}
 
+                Can also fetch some special versions by appending "@"
+                and a tag. Format:
+                projects/{project}/datasets/{dataset_id}@{tag}
+
+                Tag "active": The info of the latest completed version
+                will be included, and NOT_FOUND if the dataset does not
+                have one.
+
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.types.Dataset:
-                A representation of a Maps Dataset
+                A representation of a dataset
                 resource.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a maps_platform_datasets.GetDatasetRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, maps_platform_datasets.GetDatasetRequest):
             request = maps_platform_datasets.GetDatasetRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
 
@@ -1013,15 +1032,15 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListDatasetsPager:
-        r"""List all the datasets for the specified project.
+        r"""Lists all the datasets for the specified project.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1048,48 +1067,47 @@
 
         Args:
             request (Union[google.maps.mapsplatformdatasets_v1.types.ListDatasetsRequest, dict]):
                 The request object. Request to list datasets for the
                 project.
             parent (str):
                 Required. The name of the project to
-                list all the datasets for.
+                list all the datasets for. Format:
+                projects/{project}
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
             google.maps.mapsplatformdatasets_v1.services.maps_platform_datasets.pagers.ListDatasetsPager:
-                Response to list datasets for the
-                project.
+                Response object of ListDatasets.
+
                 Iterating over this object will yield
                 results and resolve additional pages
                 automatically.
 
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([parent])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a maps_platform_datasets.ListDatasetsRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, maps_platform_datasets.ListDatasetsRequest):
             request = maps_platform_datasets.ListDatasetsRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if parent is not None:
                 request.parent = parent
 
@@ -1133,15 +1151,15 @@
         ] = None,
         *,
         name: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> None:
-        r"""Delete the specified dataset .
+        r"""Deletes the specified dataset.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1161,43 +1179,39 @@
 
                 # Make the request
                 client.delete_dataset(request=request)
 
         Args:
             request (Union[google.maps.mapsplatformdatasets_v1.types.DeleteDatasetRequest, dict]):
                 The request object. Request to delete a dataset.
-
-                The dataset to be deleted.
             name (str):
-                Required. Format:
-                projects/${project}/datasets/{dataset_id}
+                Required. The name of the dataset to delete. Format:
+                projects/{project}/datasets/{dataset_id}
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
         """
         # Create or coerce a protobuf request object.
-        # Quick check: If we got a request object, we should *not* have
-        # gotten any keyword arguments that map to the request.
+        # - Quick check: If we got a request object, we should *not* have
+        #   gotten any keyword arguments that map to the request.
         has_flattened_params = any([name])
         if request is not None and has_flattened_params:
             raise ValueError(
                 "If the `request` argument is set, then none of "
                 "the individual field arguments should be set."
             )
 
-        # Minor optimization to avoid making a copy if the user passes
-        # in a maps_platform_datasets.DeleteDatasetRequest.
-        # There's no risk of modifying the input as we've already verified
-        # there are no flattened fields.
+        # - Use the request object if provided (there's no risk of modifying the input as
+        #   there are no flattened fields), or create one.
         if not isinstance(request, maps_platform_datasets.DeleteDatasetRequest):
             request = maps_platform_datasets.DeleteDatasetRequest(request)
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if name is not None:
                 request.name = name
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -48,15 +48,15 @@
     def __init__(
         self,
         *,
         host: str = "mapsplatformdatasets.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -68,36 +68,39 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'mapsplatformdatasets.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
-                which to make calls.
+                ignored if a ``channel`` instance is provided.
+            channel (Optional[Union[grpc.Channel, Callable[..., grpc.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -115,15 +118,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, grpc.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
 
         else:
@@ -156,15 +159,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -233,15 +238,15 @@
 
     @property
     def create_dataset(
         self,
     ) -> Callable[[maps_platform_datasets.CreateDatasetRequest], gmm_dataset.Dataset]:
         r"""Return a callable for the create dataset method over gRPC.
 
-        Create a new dataset for the specified project.
+        Creates a new dataset for the specified project.
 
         Returns:
             Callable[[~.CreateDatasetRequest],
                     ~.Dataset]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -261,15 +266,15 @@
     def update_dataset_metadata(
         self,
     ) -> Callable[
         [maps_platform_datasets.UpdateDatasetMetadataRequest], gmm_dataset.Dataset
     ]:
         r"""Return a callable for the update dataset metadata method over gRPC.
 
-        Update the metadata for the dataset.
+        Updates the metadata for the dataset.
 
         Returns:
             Callable[[~.UpdateDatasetMetadataRequest],
                     ~.Dataset]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -287,15 +292,15 @@
 
     @property
     def get_dataset(
         self,
     ) -> Callable[[maps_platform_datasets.GetDatasetRequest], dataset.Dataset]:
         r"""Return a callable for the get dataset method over gRPC.
 
-        Get the dataset.
+        Gets the dataset.
 
         Returns:
             Callable[[~.GetDatasetRequest],
                     ~.Dataset]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -316,15 +321,15 @@
         self,
     ) -> Callable[
         [maps_platform_datasets.ListDatasetsRequest],
         maps_platform_datasets.ListDatasetsResponse,
     ]:
         r"""Return a callable for the list datasets method over gRPC.
 
-        List all the datasets for the specified project.
+        Lists all the datasets for the specified project.
 
         Returns:
             Callable[[~.ListDatasetsRequest],
                     ~.ListDatasetsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -342,15 +347,15 @@
 
     @property
     def delete_dataset(
         self,
     ) -> Callable[[maps_platform_datasets.DeleteDatasetRequest], empty_pb2.Empty]:
         r"""Return a callable for the delete dataset method over gRPC.
 
-        Delete the specified dataset .
+        Deletes the specified dataset.
 
         Returns:
             Callable[[~.DeleteDatasetRequest],
                     ~.Empty]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/grpc_asyncio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
+from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, grpc_helpers_async
+from google.api_core import retry_async as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.protobuf import empty_pb2  # type: ignore
 import grpc  # type: ignore
 from grpc.experimental import aio  # type: ignore
 
 from google.maps.mapsplatformdatasets_v1.types import dataset
@@ -63,15 +65,14 @@
             credentials (Optional[~.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify this application to the service. If
                 none are specified, the client will attempt to ascertain
                 the credentials from the environment.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             kwargs (Optional[dict]): Keyword arguments, which are passed to the
                 channel creation.
@@ -93,15 +94,15 @@
     def __init__(
         self,
         *,
         host: str = "mapsplatformdatasets.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[Union[aio.Channel, Callable[..., aio.Channel]]] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -113,37 +114,40 @@
             host (Optional[str]):
                  The hostname to connect to (default: 'mapsplatformdatasets.googleapis.com').
             credentials (Optional[google.auth.credentials.Credentials]): The
                 authorization credentials to attach to requests. These
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
+                This argument is ignored if a ``channel`` instance is provided.
             scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
                 service. These are only used when credentials are not specified and
                 are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
-                which to make calls.
+            channel (Optional[Union[aio.Channel, Callable[..., aio.Channel]]]):
+                A ``Channel`` instance through which to make calls, or a Callable
+                that constructs and returns one. If set to None, ``self.create_channel``
+                is used to create the channel. If a Callable is given, it will be called
+                with the same arguments as used in ``self.create_channel``.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
                 private key bytes, both in PEM format. It is ignored if
                 ``api_mtls_endpoint`` is None.
             ssl_channel_credentials (grpc.ChannelCredentials): SSL credentials
-                for the grpc channel. It is ignored if ``channel`` is provided.
+                for the grpc channel. It is ignored if a ``channel`` instance is provided.
             client_cert_source_for_mtls (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 A callback to provide client certificate bytes and private key bytes,
                 both in PEM format. It is used to configure a mutual TLS channel. It is
-                ignored if ``channel`` or ``ssl_channel_credentials`` is provided.
+                ignored if a ``channel`` instance or ``ssl_channel_credentials`` is provided.
             quota_project_id (Optional[str]): An optional project to use for billing
                 and quota.
             client_info (google.api_core.gapic_v1.client_info.ClientInfo):
                 The client info used to send a user-agent string along with
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
@@ -161,15 +165,15 @@
         self._stubs: Dict[str, Callable] = {}
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
-        if channel:
+        if isinstance(channel, aio.Channel):
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
         else:
             if api_mtls_endpoint:
@@ -201,15 +205,17 @@
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
             api_audience=api_audience,
         )
 
         if not self._grpc_channel:
-            self._grpc_channel = type(self).create_channel(
+            # initialize with the provided callable or the default channel
+            channel_init = channel or type(self).create_channel
+            self._grpc_channel = channel_init(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
                 # Set ``credentials_file`` to ``None`` here as
                 # the credentials that we saved earlier should be used.
                 credentials_file=None,
                 scopes=self._scopes,
@@ -238,15 +244,15 @@
     def create_dataset(
         self,
     ) -> Callable[
         [maps_platform_datasets.CreateDatasetRequest], Awaitable[gmm_dataset.Dataset]
     ]:
         r"""Return a callable for the create dataset method over gRPC.
 
-        Create a new dataset for the specified project.
+        Creates a new dataset for the specified project.
 
         Returns:
             Callable[[~.CreateDatasetRequest],
                     Awaitable[~.Dataset]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -267,15 +273,15 @@
         self,
     ) -> Callable[
         [maps_platform_datasets.UpdateDatasetMetadataRequest],
         Awaitable[gmm_dataset.Dataset],
     ]:
         r"""Return a callable for the update dataset metadata method over gRPC.
 
-        Update the metadata for the dataset.
+        Updates the metadata for the dataset.
 
         Returns:
             Callable[[~.UpdateDatasetMetadataRequest],
                     Awaitable[~.Dataset]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -295,15 +301,15 @@
     def get_dataset(
         self,
     ) -> Callable[
         [maps_platform_datasets.GetDatasetRequest], Awaitable[dataset.Dataset]
     ]:
         r"""Return a callable for the get dataset method over gRPC.
 
-        Get the dataset.
+        Gets the dataset.
 
         Returns:
             Callable[[~.GetDatasetRequest],
                     Awaitable[~.Dataset]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -324,15 +330,15 @@
         self,
     ) -> Callable[
         [maps_platform_datasets.ListDatasetsRequest],
         Awaitable[maps_platform_datasets.ListDatasetsResponse],
     ]:
         r"""Return a callable for the list datasets method over gRPC.
 
-        List all the datasets for the specified project.
+        Lists all the datasets for the specified project.
 
         Returns:
             Callable[[~.ListDatasetsRequest],
                     Awaitable[~.ListDatasetsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -352,15 +358,15 @@
     def delete_dataset(
         self,
     ) -> Callable[
         [maps_platform_datasets.DeleteDatasetRequest], Awaitable[empty_pb2.Empty]
     ]:
         r"""Return a callable for the delete dataset method over gRPC.
 
-        Delete the specified dataset .
+        Deletes the specified dataset.
 
         Returns:
             Callable[[~.DeleteDatasetRequest],
                     Awaitable[~.Empty]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -372,12 +378,60 @@
             self._stubs["delete_dataset"] = self.grpc_channel.unary_unary(
                 "/google.maps.mapsplatformdatasets.v1.MapsPlatformDatasets/DeleteDataset",
                 request_serializer=maps_platform_datasets.DeleteDatasetRequest.serialize,
                 response_deserializer=empty_pb2.Empty.FromString,
             )
         return self._stubs["delete_dataset"]
 
+    def _prep_wrapped_messages(self, client_info):
+        """Precompute the wrapped methods, overriding the base class method to use async wrappers."""
+        self._wrapped_methods = {
+            self.create_dataset: gapic_v1.method_async.wrap_method(
+                self.create_dataset,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.update_dataset_metadata: gapic_v1.method_async.wrap_method(
+                self.update_dataset_metadata,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.get_dataset: gapic_v1.method_async.wrap_method(
+                self.get_dataset,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_datasets: gapic_v1.method_async.wrap_method(
+                self.list_datasets,
+                default_retry=retries.AsyncRetry(
+                    initial=1.0,
+                    maximum=10.0,
+                    multiplier=1.3,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.ServiceUnavailable,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.delete_dataset: gapic_v1.method_async.wrap_method(
+                self.delete_dataset,
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+        }
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("MapsPlatformDatasetsGrpcAsyncIOTransport",)
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/services/maps_platform_datasets/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -339,15 +339,15 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gmm_dataset.Dataset:
-                    A representation of a Maps Dataset
+                    A representation of a dataset
                 resource.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
@@ -425,16 +425,14 @@
             metadata: Sequence[Tuple[str, str]] = (),
         ):
             r"""Call the delete dataset method over HTTP.
 
             Args:
                 request (~.maps_platform_datasets.DeleteDatasetRequest):
                     The request object. Request to delete a dataset.
-
-                The dataset to be deleted.
                 retry (google.api_core.retry.Retry): Designation of what errors, if any,
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
             """
 
@@ -508,15 +506,15 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.dataset.Dataset:
-                    A representation of a Maps Dataset
+                    A representation of a dataset
                 resource.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
@@ -596,17 +594,15 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.maps_platform_datasets.ListDatasetsResponse:
-                    Response to list datasets for the
-                project.
-
+                    Response object of ListDatasets.
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
                     "uri": "/v1/{parent=projects/*}/datasets",
                 },
@@ -684,15 +680,15 @@
                     should be retried.
                 timeout (float): The timeout for this request.
                 metadata (Sequence[Tuple[str, str]]): Strings which should be
                     sent along with the request as metadata.
 
             Returns:
                 ~.gmm_dataset.Dataset:
-                    A representation of a Maps Dataset
+                    A representation of a dataset
                 resource.
 
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/data_source.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/dataset.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -44,31 +44,33 @@
             styling.
     """
     USAGE_UNSPECIFIED = 0
     USAGE_DATA_DRIVEN_STYLING = 1
 
 
 class Dataset(proto.Message):
-    r"""A representation of a Maps Dataset resource.
+    r"""A representation of a dataset resource.
 
     This message has `oneof`_ fields (mutually exclusive fields).
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
         name (str):
-            Resource name, projects/{project}/datasets/{dataset_id}
+            Resource name. Format:
+            projects/{project}/datasets/{dataset_id}
         display_name (str):
-            Human readable name, shown in the console UI
-            .
+            Human readable name, shown in the console UI.
+
+            Must be unique within a project.
         description (str):
-            A description of this dataset .
+            A description of this dataset.
         version_id (str):
             The version ID of the dataset.
         usage (MutableSequence[google.maps.mapsplatformdatasets_v1.types.Usage]):
             Specified use case for this dataset.
         local_file_source (google.maps.mapsplatformdatasets_v1.types.LocalFileSource):
             A local file source for the dataset for a
             single upload.
@@ -85,15 +87,16 @@
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the dataset was first
             created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when the dataset metadata
             was last updated.
         version_create_time (google.protobuf.timestamp_pb2.Timestamp):
-            Output only. Time when the data was uploaded.
+            Output only. Time when this version was
+            created.
         version_description (str):
             Output only. The description for this version
             of dataset. It is provided when importing data
             to the dataset.
     """
 
     name: str = proto.Field(
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,15 +37,15 @@
 
 class CreateDatasetRequest(proto.Message):
     r"""Request to create a maps dataset.
 
     Attributes:
         parent (str):
             Required. Parent project that will own the
-            dataset. Format: projects/{$project}
+            dataset. Format: projects/{project}
         dataset (google.maps.mapsplatformdatasets_v1.types.Dataset):
             Required. The dataset version to create.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
@@ -58,20 +58,20 @@
 
 
 class UpdateDatasetMetadataRequest(proto.Message):
     r"""Request to update the metadata fields of the dataset.
 
     Attributes:
         dataset (google.maps.mapsplatformdatasets_v1.types.Dataset):
-            Required. The dataset to update. The dataset's name is used
-            to identify the dataset to be updated. The name has the
-            format: projects/{project}/datasets/{dataset_id}
+            Required. Resource name of the dataset to update. Format:
+            projects/{project}/datasets/{dataset_id}
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
-            The list of fields to be updated. Support the value "*" for
-            full replacement.
+            The list of fields to be updated.
+
+            The value "*" is used for full replacement (default).
     """
 
     dataset: gmm_dataset.Dataset = proto.Field(
         proto.MESSAGE,
         number=1,
         message=gmm_dataset.Dataset,
     )
@@ -83,65 +83,90 @@
 
 
 class GetDatasetRequest(proto.Message):
     r"""Request to get the specified dataset.
 
     Attributes:
         name (str):
-            Required. Resource name.
+            Required. Resource name. Format:
             projects/{project}/datasets/{dataset_id}
+
+            Can also fetch some special versions by appending "@" and a
+            tag. Format: projects/{project}/datasets/{dataset_id}@{tag}
+
+            Tag "active": The info of the latest completed version will
+            be included, and NOT_FOUND if the dataset does not have one.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
 
 
 class ListDatasetsRequest(proto.Message):
     r"""Request to list datasets for the project.
 
     Attributes:
         parent (str):
             Required. The name of the project to list all
-            the datasets for.
+            the datasets for. Format: projects/{project}
         page_size (int):
-            The maximum number of versions to return per
-            page. If unspecified (or zero), all datasets
-            will be returned.
+            The maximum number of datasets to return per
+            page.
+            If unspecified (or zero), all datasets will be
+            returned.
         page_token (str):
             The page token, received from a previous
             ListDatasets call. Provide this to retrieve the
             subsequent page.
+        tag (str):
+            The tag that specifies the desired version
+            for each dataset.
+            Note that when pagination is also specified,
+            some filtering can happen after pagination,
+            which may cause the response to contain fewer
+            datasets than the page size, even if it's not
+            the last page.
+
+            Tag "active": Each dataset in the response will
+            include the info of its latest completed
+            version, and the dataset will be skipped if it
+            does not have one.
     """
 
     parent: str = proto.Field(
         proto.STRING,
         number=1,
     )
     page_size: int = proto.Field(
         proto.INT32,
         number=2,
     )
     page_token: str = proto.Field(
         proto.STRING,
         number=3,
     )
+    tag: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
 
 
 class ListDatasetsResponse(proto.Message):
-    r"""Response to list datasets for the project.
+    r"""Response object of ListDatasets.
 
     Attributes:
         datasets (MutableSequence[google.maps.mapsplatformdatasets_v1.types.Dataset]):
             All the datasets for the project.
         next_page_token (str):
             A token that can be sent as ``page_token`` to retrieve the
-            next page. If this field is omitted, there are no subsequent
-            pages.
+            next page.
+
+            If this field is omitted, there are no subsequent pages.
     """
 
     @property
     def raw_page(self):
         return self
 
     datasets: MutableSequence[gmm_dataset.Dataset] = proto.RepeatedField(
@@ -154,19 +179,18 @@
         number=2,
     )
 
 
 class DeleteDatasetRequest(proto.Message):
     r"""Request to delete a dataset.
 
-    The dataset to be deleted.
-
     Attributes:
         name (str):
-            Required. Format: projects/${project}/datasets/{dataset_id}
+            Required. The name of the dataset to delete. Format:
+            projects/{project}/datasets/{dataset_id}
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py` & `google-maps-mapsplatformdatasets-0.4.0/google/maps/mapsplatformdatasets_v1/types/maps_platform_datasets_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/gapic_version.py` & `google-maps-mapsplatformdatasets-0.4.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.7"  # {x-release-please-version}
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google/maps/mapsplatformdatasets_v1alpha/services/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/google_maps_mapsplatformdatasets.egg-info/PKG-INFO` & `google-maps-mapsplatformdatasets-0.4.0/google_maps_mapsplatformdatasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-maps-mapsplatformdatasets
-Version: 0.3.7
+Version: 0.4.0
 Summary: Google Maps Mapsplatformdatasets API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-maps-mapsplatformdatasets
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/setup.py` & `google-maps-mapsplatformdatasets-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/tests/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/tests/unit/__init__.py` & `google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/mapsplatformdatasets_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-maps-mapsplatformdatasets-0.3.7/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py` & `google-maps-mapsplatformdatasets-0.4.0/tests/unit/gapic/mapsplatformdatasets_v1/test_maps_platform_datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1218,15 +1218,16 @@
             version_description="version_description_value",
         )
         response = client.create_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.CreateDatasetRequest()
+        request = maps_platform_datasets.CreateDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gmm_dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1240,20 +1241,160 @@
     client = MapsPlatformDatasetsClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.create_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.create_dataset()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.CreateDatasetRequest()
 
 
+def test_create_dataset_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = MapsPlatformDatasetsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = maps_platform_datasets.CreateDatasetRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.create_dataset(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.CreateDatasetRequest(
+            parent="parent_value",
+        )
+
+
+def test_create_dataset_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_dataset] = mock_rpc
+        request = {}
+        client.create_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_create_dataset_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = MapsPlatformDatasetsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_dataset), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gmm_dataset.Dataset(
+                name="name_value",
+                display_name="display_name_value",
+                description="description_value",
+                version_id="version_id_value",
+                usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
+                version_description="version_description_value",
+            )
+        )
+        response = await client.create_dataset()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.CreateDatasetRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_dataset_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.create_dataset
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.create_dataset
+        ] = mock_object
+
+        request = {}
+        await client.create_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.create_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_create_dataset_async(
     transport: str = "grpc_asyncio",
     request_type=maps_platform_datasets.CreateDatasetRequest,
 ):
     client = MapsPlatformDatasetsAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1278,15 +1419,16 @@
             )
         )
         response = await client.create_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.CreateDatasetRequest()
+        request = maps_platform_datasets.CreateDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gmm_dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1479,15 +1621,16 @@
             version_description="version_description_value",
         )
         response = client.update_dataset_metadata(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
+        request = maps_platform_datasets.UpdateDatasetMetadataRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gmm_dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1503,20 +1646,165 @@
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(
         type(client.transport.update_dataset_metadata), "__call__"
     ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.update_dataset_metadata()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
 
 
+def test_update_dataset_metadata_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = MapsPlatformDatasetsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = maps_platform_datasets.UpdateDatasetMetadataRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_dataset_metadata), "__call__"
+    ) as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.update_dataset_metadata(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
+
+
+def test_update_dataset_metadata_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_dataset_metadata
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_dataset_metadata
+        ] = mock_rpc
+        request = {}
+        client.update_dataset_metadata(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_dataset_metadata(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_update_dataset_metadata_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = MapsPlatformDatasetsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_dataset_metadata), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            gmm_dataset.Dataset(
+                name="name_value",
+                display_name="display_name_value",
+                description="description_value",
+                version_id="version_id_value",
+                usage=[gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
+                version_description="version_description_value",
+            )
+        )
+        response = await client.update_dataset_metadata()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_dataset_metadata_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.update_dataset_metadata
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.update_dataset_metadata
+        ] = mock_object
+
+        request = {}
+        await client.update_dataset_metadata(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.update_dataset_metadata(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_update_dataset_metadata_async(
     transport: str = "grpc_asyncio",
     request_type=maps_platform_datasets.UpdateDatasetMetadataRequest,
 ):
     client = MapsPlatformDatasetsAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1543,15 +1831,16 @@
             )
         )
         response = await client.update_dataset_metadata(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.UpdateDatasetMetadataRequest()
+        request = maps_platform_datasets.UpdateDatasetMetadataRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, gmm_dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1750,15 +2039,16 @@
             version_description="version_description_value",
         )
         response = client.get_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.GetDatasetRequest()
+        request = maps_platform_datasets.GetDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1772,20 +2062,160 @@
     client = MapsPlatformDatasetsClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.get_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.get_dataset()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.GetDatasetRequest()
 
 
+def test_get_dataset_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = MapsPlatformDatasetsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = maps_platform_datasets.GetDatasetRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.get_dataset(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.GetDatasetRequest(
+            name="name_value",
+        )
+
+
+def test_get_dataset_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_dataset] = mock_rpc
+        request = {}
+        client.get_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_get_dataset_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = MapsPlatformDatasetsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_dataset), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            dataset.Dataset(
+                name="name_value",
+                display_name="display_name_value",
+                description="description_value",
+                version_id="version_id_value",
+                usage=[dataset.Usage.USAGE_DATA_DRIVEN_STYLING],
+                version_description="version_description_value",
+            )
+        )
+        response = await client.get_dataset()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.GetDatasetRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_dataset_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.get_dataset
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.get_dataset
+        ] = mock_object
+
+        request = {}
+        await client.get_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.get_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_get_dataset_async(
     transport: str = "grpc_asyncio",
     request_type=maps_platform_datasets.GetDatasetRequest,
 ):
     client = MapsPlatformDatasetsAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1810,15 +2240,16 @@
             )
         )
         response = await client.get_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.GetDatasetRequest()
+        request = maps_platform_datasets.GetDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, dataset.Dataset)
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
@@ -1994,15 +2425,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.list_datasets(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.ListDatasetsRequest()
+        request = maps_platform_datasets.ListDatasetsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDatasetsPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_datasets_empty_call():
@@ -2011,20 +2443,159 @@
     client = MapsPlatformDatasetsClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.list_datasets), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.list_datasets()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.ListDatasetsRequest()
 
 
+def test_list_datasets_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = MapsPlatformDatasetsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = maps_platform_datasets.ListDatasetsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        tag="tag_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_datasets), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.list_datasets(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.ListDatasetsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            tag="tag_value",
+        )
+
+
+def test_list_datasets_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_datasets in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_datasets] = mock_rpc
+        request = {}
+        client.list_datasets(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_datasets(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_list_datasets_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = MapsPlatformDatasetsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_datasets), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            maps_platform_datasets.ListDatasetsResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_datasets()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.ListDatasetsRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_datasets_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.list_datasets
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.list_datasets
+        ] = mock_object
+
+        request = {}
+        await client.list_datasets(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.list_datasets(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_list_datasets_async(
     transport: str = "grpc_asyncio",
     request_type=maps_platform_datasets.ListDatasetsRequest,
 ):
     client = MapsPlatformDatasetsAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2044,15 +2615,16 @@
             )
         )
         response = await client.list_datasets(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.ListDatasetsRequest()
+        request = maps_platform_datasets.ListDatasetsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDatasetsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -2415,15 +2987,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.DeleteDatasetRequest()
+        request = maps_platform_datasets.DeleteDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_dataset_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2431,20 +3004,151 @@
     client = MapsPlatformDatasetsClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport="grpc",
     )
 
     # Mock the actual call within the gRPC stub, and fake the request.
     with mock.patch.object(type(client.transport.delete_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
         client.delete_dataset()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == maps_platform_datasets.DeleteDatasetRequest()
 
 
+def test_delete_dataset_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = MapsPlatformDatasetsClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = maps_platform_datasets.DeleteDatasetRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_dataset), "__call__") as call:
+        call.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client.delete_dataset(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.DeleteDatasetRequest(
+            name="name_value",
+        )
+
+
+def test_delete_dataset_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="grpc",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_dataset] = mock_rpc
+        request = {}
+        client.delete_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
+@pytest.mark.asyncio
+async def test_delete_dataset_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = MapsPlatformDatasetsAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_dataset), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_dataset()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == maps_platform_datasets.DeleteDatasetRequest()
+
+
+@pytest.mark.asyncio
+async def test_delete_dataset_async_use_cached_wrapped_rpc(
+    transport: str = "grpc_asyncio",
+):
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method_async.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsAsyncClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport=transport,
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._client._transport.delete_dataset
+            in client._client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        class AwaitableMock(mock.AsyncMock):
+            def __await__(self):
+                self.await_count += 1
+                return iter([])
+
+        mock_object = AwaitableMock()
+        client._client._transport._wrapped_methods[
+            client._client._transport.delete_dataset
+        ] = mock_object
+
+        request = {}
+        await client.delete_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_object.call_count == 1
+
+        await client.delete_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_object.call_count == 2
+
+
 @pytest.mark.asyncio
 async def test_delete_dataset_async(
     transport: str = "grpc_asyncio",
     request_type=maps_platform_datasets.DeleteDatasetRequest,
 ):
     client = MapsPlatformDatasetsAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -2460,15 +3164,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_dataset(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == maps_platform_datasets.DeleteDatasetRequest()
+        request = maps_platform_datasets.DeleteDatasetRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_dataset_async_from_dict():
@@ -2741,14 +3446,50 @@
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
     assert response.usage == [gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING]
     assert response.version_description == "version_description_value"
 
 
+def test_create_dataset_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.create_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.create_dataset] = mock_rpc
+
+        request = {}
+        client.create_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.create_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_create_dataset_rest_required_fields(
     request_type=maps_platform_datasets.CreateDatasetRequest,
 ):
     transport_class = transports.MapsPlatformDatasetsRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3108,14 +3849,55 @@
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
     assert response.usage == [gmm_dataset.Usage.USAGE_DATA_DRIVEN_STYLING]
     assert response.version_description == "version_description_value"
 
 
+def test_update_dataset_metadata_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert (
+            client._transport.update_dataset_metadata
+            in client._transport._wrapped_methods
+        )
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[
+            client._transport.update_dataset_metadata
+        ] = mock_rpc
+
+        request = {}
+        client.update_dataset_metadata(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.update_dataset_metadata(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_update_dataset_metadata_rest_required_fields(
     request_type=maps_platform_datasets.UpdateDatasetMetadataRequest,
 ):
     transport_class = transports.MapsPlatformDatasetsRestTransport
 
     request_init = {}
     request = request_type(**request_init)
@@ -3383,14 +4165,50 @@
     assert response.display_name == "display_name_value"
     assert response.description == "description_value"
     assert response.version_id == "version_id_value"
     assert response.usage == [dataset.Usage.USAGE_DATA_DRIVEN_STYLING]
     assert response.version_description == "version_description_value"
 
 
+def test_get_dataset_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.get_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.get_dataset] = mock_rpc
+
+        request = {}
+        client.get_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.get_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_get_dataset_rest_required_fields(
     request_type=maps_platform_datasets.GetDatasetRequest,
 ):
     transport_class = transports.MapsPlatformDatasetsRestTransport
 
     request_init = {}
     request_init["name"] = ""
@@ -3646,14 +4464,50 @@
         response = client.list_datasets(request)
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDatasetsPager)
     assert response.next_page_token == "next_page_token_value"
 
 
+def test_list_datasets_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.list_datasets in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.list_datasets] = mock_rpc
+
+        request = {}
+        client.list_datasets(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.list_datasets(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_list_datasets_rest_required_fields(
     request_type=maps_platform_datasets.ListDatasetsRequest,
 ):
     transport_class = transports.MapsPlatformDatasetsRestTransport
 
     request_init = {}
     request_init["parent"] = ""
@@ -3678,14 +4532,15 @@
         credentials=ga_credentials.AnonymousCredentials()
     ).list_datasets._get_unset_required_fields(jsonified_request)
     # Check that path parameters and body parameters are not mixing in.
     assert not set(unset_fields) - set(
         (
             "page_size",
             "page_token",
+            "tag",
         )
     )
     jsonified_request.update(unset_fields)
 
     # verify required fields with non-default values are left alone
     assert "parent" in jsonified_request
     assert jsonified_request["parent"] == "parent_value"
@@ -3738,14 +4593,15 @@
 
     unset_fields = transport.list_datasets._get_unset_required_fields({})
     assert set(unset_fields) == (
         set(
             (
                 "pageSize",
                 "pageToken",
+                "tag",
             )
         )
         & set(("parent",))
     )
 
 
 @pytest.mark.parametrize("null_interceptor", [True, False])
@@ -3978,14 +4834,50 @@
         req.return_value = response_value
         response = client.delete_dataset(request)
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
+def test_delete_dataset_rest_use_cached_wrapped_rpc():
+    # Clients should use _prep_wrapped_messages to create cached wrapped rpcs,
+    # instead of constructing them on each call
+    with mock.patch("google.api_core.gapic_v1.method.wrap_method") as wrapper_fn:
+        client = MapsPlatformDatasetsClient(
+            credentials=ga_credentials.AnonymousCredentials(),
+            transport="rest",
+        )
+
+        # Should wrap all calls on client creation
+        assert wrapper_fn.call_count > 0
+        wrapper_fn.reset_mock()
+
+        # Ensure method has been cached
+        assert client._transport.delete_dataset in client._transport._wrapped_methods
+
+        # Replace cached wrapped function with mock
+        mock_rpc = mock.Mock()
+        mock_rpc.return_value.name = (
+            "foo"  # operation_request.operation in compute client(s) expect a string.
+        )
+        client._transport._wrapped_methods[client._transport.delete_dataset] = mock_rpc
+
+        request = {}
+        client.delete_dataset(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert mock_rpc.call_count == 1
+
+        client.delete_dataset(request)
+
+        # Establish that a new wrapper was not created for this call
+        assert wrapper_fn.call_count == 0
+        assert mock_rpc.call_count == 2
+
+
 def test_delete_dataset_rest_required_fields(
     request_type=maps_platform_datasets.DeleteDatasetRequest,
 ):
     transport_class = transports.MapsPlatformDatasetsRestTransport
 
     request_init = {}
     request_init["name"] = ""
```

