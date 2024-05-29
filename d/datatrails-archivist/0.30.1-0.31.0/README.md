# Comparing `tmp/datatrails_archivist-0.30.1.tar.gz` & `tmp/datatrails_archivist-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrails_archivist-0.30.1.tar", last modified: Tue May 21 09:49:36 2024, max compression
+gzip compressed data, was "datatrails_archivist-0.31.0.tar", last modified: Wed May 29 14:52:29 2024, max compression
```

## Comparing `datatrails_archivist-0.30.1.tar` & `datatrails_archivist-0.31.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-21 09:49:33.000000 datatrails_archivist-0.30.1/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12435 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/confirmation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.496007 datatrails_archivist-0.31.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-29 14:52:29.496007 datatrails_archivist-0.31.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.492007 datatrails_archivist-0.31.0/archivist/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 14:52:26.000000 datatrails_archivist-0.31.0/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12435 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.492007 datatrails_archivist-0.31.0/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.492007 datatrails_archivist-0.31.0/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.492007 datatrails_archivist-0.31.0/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/confirmation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/archivist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:52:29.496007 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 14:52:29.000000 datatrails_archivist-0.31.0/datatrails_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-29 14:50:51.000000 datatrails_archivist-0.31.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-29 14:52:29.496007 datatrails_archivist-0.31.0/setup.cfg
```

### Comparing `datatrails_archivist-0.30.1/LICENSE` & `datatrails_archivist-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/PKG-INFO` & `datatrails_archivist-0.31.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.30.1
+Version: 0.31.0
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
@@ -83,15 +83,14 @@
     The main function would initialize an archivist connection using the url and
     the credentials, called "arch", then call arch.assets.create() and the asset will be created.
     """
 
     from os import getenv
 
     from archivist.archivist import Archivist
-    from archivist.proof_mechanism import ProofMechanism
 
 
     def create_asset(arch):
         """Create an asset using Archivist Connection.
 
         Args:
             arch: archivist connection.
@@ -113,29 +112,21 @@
             # their arc_display_type.
             # So a mistake here can result in asset data being
             # under- or over-shared.
             "some_custom_attribute": "value"  # You can add any custom value as long as
             # it does not start with arc_
         }
         #
-        # Select the mechanism used to prove evidence for the asset.  If the selected proof
-        # mechanism is not enabled for your tenant then an error will occur.
-        # If unspecified then SIMPLE_HASH is used.
-        props = {
-            "proof_mechanism": ProofMechanism.SIMPLE_HASH.name,
-        }
-
-        # The first argument are the properties of the asset
-        # The second argument are the attributes of the asset
-        # The third argument is wait for confirmation:
+        # The first argument are the attributes of the asset
+        # The second argument is wait for confirmation:
         #   If @confirm@ is True then this function will not
-        #   return until the asset is confirmed on the blockchain and ready
+        #   return until the asset is confirmed and ready
         #   to accept events (or an error occurs)
         #
-        return arch.assets.create(props=props, attrs=attrs, confirm=True)
+        return arch.assets.create(attrs=attrs, confirm=True)
         # alternatively if some work can be done whilst the asset is confirmed then this call can be
         # replaced by a two-step alternative:
 
         # asset = arch.assets.create(props=props, attrs=attrs, confirm=False)
 
         # ... do something else here
         # and then wait for confirmation
@@ -159,17 +150,16 @@
         # the client_secret_filename environment variable.
         client_id = getenv("DATATRAILS_APPREG_CLIENT")
         client_secret_file = getenv("DATATRAILS_APPREG_SECRET_FILENAME")
         with open(client_secret_file, mode="r", encoding="utf-8") as tokenfile:
             client_secret = tokenfile.read().strip()
 
         # Initialize connection to Archivist. max_time is the time to wait for confirmation
-        # of an asset or event creation - the default is 1200 seconds but one can optionally
-        # specify a different value here particularly when creating assets on SIMPLE_HASH
-        # as confirmation times are much shorter in this case.
+        # of an asset or event creation - the default is 300 seconds but one can optionally
+        # specify a different value.
         with arch = Archivist(
             "https://app.datatrails.ai",
             (client_id, client_secret),
             max_time=300,
         ) as arch:
             # Create a new asset
             asset = create_asset(arch)
```

### Comparing `datatrails_archivist-0.30.1/README.rst` & `datatrails_archivist-0.31.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     The main function would initialize an archivist connection using the url and
     the credentials, called "arch", then call arch.assets.create() and the asset will be created.
     """
 
     from os import getenv
 
     from archivist.archivist import Archivist
-    from archivist.proof_mechanism import ProofMechanism
 
 
     def create_asset(arch):
         """Create an asset using Archivist Connection.
 
         Args:
             arch: archivist connection.
@@ -81,29 +80,21 @@
             # their arc_display_type.
             # So a mistake here can result in asset data being
             # under- or over-shared.
             "some_custom_attribute": "value"  # You can add any custom value as long as
             # it does not start with arc_
         }
         #
-        # Select the mechanism used to prove evidence for the asset.  If the selected proof
-        # mechanism is not enabled for your tenant then an error will occur.
-        # If unspecified then SIMPLE_HASH is used.
-        props = {
-            "proof_mechanism": ProofMechanism.SIMPLE_HASH.name,
-        }
-
-        # The first argument are the properties of the asset
-        # The second argument are the attributes of the asset
-        # The third argument is wait for confirmation:
+        # The first argument are the attributes of the asset
+        # The second argument is wait for confirmation:
         #   If @confirm@ is True then this function will not
-        #   return until the asset is confirmed on the blockchain and ready
+        #   return until the asset is confirmed and ready
         #   to accept events (or an error occurs)
         #
-        return arch.assets.create(props=props, attrs=attrs, confirm=True)
+        return arch.assets.create(attrs=attrs, confirm=True)
         # alternatively if some work can be done whilst the asset is confirmed then this call can be
         # replaced by a two-step alternative:
 
         # asset = arch.assets.create(props=props, attrs=attrs, confirm=False)
 
         # ... do something else here
         # and then wait for confirmation
@@ -127,17 +118,16 @@
         # the client_secret_filename environment variable.
         client_id = getenv("DATATRAILS_APPREG_CLIENT")
         client_secret_file = getenv("DATATRAILS_APPREG_SECRET_FILENAME")
         with open(client_secret_file, mode="r", encoding="utf-8") as tokenfile:
             client_secret = tokenfile.read().strip()
 
         # Initialize connection to Archivist. max_time is the time to wait for confirmation
-        # of an asset or event creation - the default is 1200 seconds but one can optionally
-        # specify a different value here particularly when creating assets on SIMPLE_HASH
-        # as confirmation times are much shorter in this case.
+        # of an asset or event creation - the default is 300 seconds but one can optionally
+        # specify a different value.
         with arch = Archivist(
             "https://app.datatrails.ai",
             (client_id, client_secret),
             max_time=300,
         ) as arch:
             # Create a new asset
             asset = create_asset(arch)
```

### Comparing `datatrails_archivist-0.30.1/archivist/access_policies.py` & `datatrails_archivist-0.31.0/archivist/access_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/appidp.py` & `datatrails_archivist-0.31.0/archivist/appidp.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/applications.py` & `datatrails_archivist-0.31.0/archivist/applications.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/archivist.py` & `datatrails_archivist-0.31.0/archivist/archivist.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/archivistpublic.py` & `datatrails_archivist-0.31.0/archivist/archivistpublic.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/asset.py` & `datatrails_archivist-0.31.0/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/assetattachments.py` & `datatrails_archivist-0.31.0/archivist/assetattachments.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/assets.py` & `datatrails_archivist-0.31.0/archivist/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         confirm: bool = True,
     ) -> Asset:
         """Create asset
 
         Creates asset with defined properties and attributes.
 
         Args:
-            props (dict): Properties - usually only the proof_mechanism setting
+            props (dict): Properties
             attrs (dict): attributes of created asset.
             confirm (bool): if True wait for asset to be confirmed.
 
         Returns:
             :class:`Asset` instance
 
         """
```

### Comparing `datatrails_archivist-0.30.1/archivist/attachments.py` & `datatrails_archivist-0.31.0/archivist/attachments.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/cmds/runner/main.py` & `datatrails_archivist-0.31.0/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/cmds/runner/run.py` & `datatrails_archivist-0.31.0/archivist/cmds/runner/run.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/cmds/template/main.py` & `datatrails_archivist-0.31.0/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/cmds/template/run.py` & `datatrails_archivist-0.31.0/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/compliance.py` & `datatrails_archivist-0.31.0/archivist/compliance.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/compliance_policies.py` & `datatrails_archivist-0.31.0/archivist/compliance_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/compliance_policy_requests.py` & `datatrails_archivist-0.31.0/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/compliance_policy_type.py` & `datatrails_archivist-0.31.0/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/composite.py` & `datatrails_archivist-0.31.0/archivist/composite.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/confirmation_status.py` & `datatrails_archivist-0.31.0/archivist/confirmation_status.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/confirmer.py` & `datatrails_archivist-0.31.0/archivist/confirmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
     status = entity[CONFIRMATION_STATUS]
     if status == ConfirmationStatus.FAILED.name:
         raise ArchivistUnconfirmedError(
             f"confirmation for {identity} FAILED - this is unusable"
         )
 
-    # Simple hash and merkleLog
     if status in (
         ConfirmationStatus.CONFIRMED.name,
         ConfirmationStatus.COMMITTED.name,
         ConfirmationStatus.UNEQUIVOCAL.name,
     ):
         return entity
```

### Comparing `datatrails_archivist-0.30.1/archivist/constants.py` & `datatrails_archivist-0.31.0/archivist/constants.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/dictmerge.py` & `datatrails_archivist-0.31.0/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/errors.py` & `datatrails_archivist-0.31.0/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/events.py` & `datatrails_archivist-0.31.0/archivist/events.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/locations.py` & `datatrails_archivist-0.31.0/archivist/locations.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/logger.py` & `datatrails_archivist-0.31.0/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/parser.py` & `datatrails_archivist-0.31.0/archivist/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from logging import getLogger
 from sys import exit as sys_exit
 from warnings import filterwarnings
 
 from .archivist import Archivist
 from .dictmerge import _deepmerge
 from .logger import set_logger
-from .proof_mechanism import ProofMechanism
 from .utils import get_auth
 
 filterwarnings("ignore", message="Unverified HTTPS request")
 
 
 LOGGER = getLogger(__name__)
 
@@ -78,23 +77,14 @@
         type=str,
         dest="url",
         action="store",
         default="https://app.datatrails.ai",
         help="url of Archivist service",
     )
     parser.add_argument(
-        "-p",
-        "--proof-mechanism",
-        type=ProofMechanism,
-        action=EnumAction,
-        dest="proof_mechanism",
-        default=None,
-        help="mechanism for proving the evidence for events on the Asset",
-    )
-    parser.add_argument(
         "--auth-token",
         type=str,
         dest="auth_token",
         action="store",
         default=None,
         help="API token value",
     )
@@ -148,21 +138,14 @@
         set_logger("DEBUG")
     else:
         set_logger("INFO")
 
     arch = None
     LOGGER.info("Initializing connection to DATATRAILS...")
     fixtures = {}
-    if args.proof_mechanism is not None:
-        fixtures = {
-            "assets": {
-                "proof_mechanism": args.proof_mechanism.name,
-            },
-        }
-
     if args.namespace is not None:
         fixtures = _deepmerge(
             fixtures,
             {
                 "assets": {
                     "attributes": {
                         "arc_namespace": args.namespace,
```

### Comparing `datatrails_archivist-0.30.1/archivist/proof_mechanism.py` & `datatrails_archivist-0.31.0/archivist/proof_mechanism.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Archivist Proof Mechanism
 
    Enumerated type that allows user to select the proof_mechanism option when
    creating an asset.
 
+   Currently there is only one proof mechanism so this code is here only for
+   compatibility.
 """
 
 # pylint: disable=unused-private-member
 
 from enum import Enum
 
 
 class ProofMechanism(Enum):
     """Enumerate proof mechanism options"""
 
     # previously used but now removed
-    __RESERVED = 1
-    #: Assets and events are proven using a hash of the originator's evidence
-    SIMPLE_HASH = 2
+    __RESERVED1 = 1
+    __RESERVED2 = 2
     #: Assets and events are proven using a merkle log hash of the originator's evidence
     MERKLE_LOG = 3
```

### Comparing `datatrails_archivist-0.30.1/archivist/retry429.py` & `datatrails_archivist-0.31.0/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/runner.py` & `datatrails_archivist-0.31.0/archivist/runner.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/sboms.py` & `datatrails_archivist-0.31.0/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/subjects.py` & `datatrails_archivist-0.31.0/archivist/subjects.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/subjects_confirmer.py` & `datatrails_archivist-0.31.0/archivist/subjects_confirmer.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/tenancies.py` & `datatrails_archivist-0.31.0/archivist/tenancies.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/timestamp.py` & `datatrails_archivist-0.31.0/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/archivist/utils.py` & `datatrails_archivist-0.31.0/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/datatrails_archivist.egg-info/PKG-INFO` & `datatrails_archivist-0.31.0/datatrails_archivist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.30.1
+Version: 0.31.0
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
@@ -83,15 +83,14 @@
     The main function would initialize an archivist connection using the url and
     the credentials, called "arch", then call arch.assets.create() and the asset will be created.
     """
 
     from os import getenv
 
     from archivist.archivist import Archivist
-    from archivist.proof_mechanism import ProofMechanism
 
 
     def create_asset(arch):
         """Create an asset using Archivist Connection.
 
         Args:
             arch: archivist connection.
@@ -113,29 +112,21 @@
             # their arc_display_type.
             # So a mistake here can result in asset data being
             # under- or over-shared.
             "some_custom_attribute": "value"  # You can add any custom value as long as
             # it does not start with arc_
         }
         #
-        # Select the mechanism used to prove evidence for the asset.  If the selected proof
-        # mechanism is not enabled for your tenant then an error will occur.
-        # If unspecified then SIMPLE_HASH is used.
-        props = {
-            "proof_mechanism": ProofMechanism.SIMPLE_HASH.name,
-        }
-
-        # The first argument are the properties of the asset
-        # The second argument are the attributes of the asset
-        # The third argument is wait for confirmation:
+        # The first argument are the attributes of the asset
+        # The second argument is wait for confirmation:
         #   If @confirm@ is True then this function will not
-        #   return until the asset is confirmed on the blockchain and ready
+        #   return until the asset is confirmed and ready
         #   to accept events (or an error occurs)
         #
-        return arch.assets.create(props=props, attrs=attrs, confirm=True)
+        return arch.assets.create(attrs=attrs, confirm=True)
         # alternatively if some work can be done whilst the asset is confirmed then this call can be
         # replaced by a two-step alternative:
 
         # asset = arch.assets.create(props=props, attrs=attrs, confirm=False)
 
         # ... do something else here
         # and then wait for confirmation
@@ -159,17 +150,16 @@
         # the client_secret_filename environment variable.
         client_id = getenv("DATATRAILS_APPREG_CLIENT")
         client_secret_file = getenv("DATATRAILS_APPREG_SECRET_FILENAME")
         with open(client_secret_file, mode="r", encoding="utf-8") as tokenfile:
             client_secret = tokenfile.read().strip()
 
         # Initialize connection to Archivist. max_time is the time to wait for confirmation
-        # of an asset or event creation - the default is 1200 seconds but one can optionally
-        # specify a different value here particularly when creating assets on SIMPLE_HASH
-        # as confirmation times are much shorter in this case.
+        # of an asset or event creation - the default is 300 seconds but one can optionally
+        # specify a different value.
         with arch = Archivist(
             "https://app.datatrails.ai",
             (client_id, client_secret),
             max_time=300,
         ) as arch:
             # Create a new asset
             asset = create_asset(arch)
```

### Comparing `datatrails_archivist-0.30.1/datatrails_archivist.egg-info/SOURCES.txt` & `datatrails_archivist-0.31.0/datatrails_archivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/pyproject.toml` & `datatrails_archivist-0.31.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datatrails_archivist-0.30.1/setup.cfg` & `datatrails_archivist-0.31.0/setup.cfg`

 * *Files identical despite different names*

