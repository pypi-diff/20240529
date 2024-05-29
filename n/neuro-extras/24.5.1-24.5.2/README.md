# Comparing `tmp/neuro-extras-24.5.1.tar.gz` & `tmp/neuro-extras-24.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-extras-24.5.1.tar", last modified: Tue May 28 14:44:24 2024, max compression
+gzip compressed data, was "neuro-extras-24.5.2.tar", last modified: Wed May 29 17:12:25 2024, max compression
```

## Comparing `neuro-extras-24.5.1.tar` & `neuro-extras-24.5.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.387762 neuro-extras-24.5.1/neuro_extras/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.387762 neuro-extras-24.5.1/neuro_extras/assets/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1214 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/assets/merge_docker_auths.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.387762 neuro-extras-24.5.1/neuro_extras/assets/seldon.package/
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/assets/seldon.package/seldon.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/assets/seldon.package/seldon_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/neuro_extras/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/data/web.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/seldon.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/neuro_extras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.387762 neuro-extras-24.5.1/neuro_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:44:06.000000 neuro-extras-24.5.1/neuro_extras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 14:44:24.000000 neuro-extras-24.5.1/neuro_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 14:44:24.395762 neuro-extras-24.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/tests/e2e/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/cloud_to_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/cloud_to_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/local_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/local_to_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/platform_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/test_data_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/test_init_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/test_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/e2e/test_seldon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:44:24.391762 neuro-extras-24.5.1/tests/unit/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/image/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/image/test_remote_image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/test_auth_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-28 14:43:53.000000 neuro-extras-24.5.1/tests/unit/test_select_job_preset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.036054 neuro-extras-24.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 17:12:25.036054 neuro-extras-24.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.028054 neuro-extras-24.5.2/neuro_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.028054 neuro-extras-24.5.2/neuro_extras/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1214 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/assets/merge_docker_auths.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.028054 neuro-extras-24.5.2/neuro_extras/assets/seldon.package/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/assets/seldon.package/seldon.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/assets/seldon.package/seldon_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.032054 neuro-extras-24.5.2/neuro_extras/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/data/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/seldon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/neuro_extras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.028054 neuro-extras-24.5.2/neuro_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:12:08.000000 neuro-extras-24.5.2/neuro_extras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 17:12:24.000000 neuro-extras-24.5.2/neuro_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-29 17:12:25.036054 neuro-extras-24.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.032054 neuro-extras-24.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.032054 neuro-extras-24.5.2/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.032054 neuro-extras-24.5.2/tests/e2e/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/cloud_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/cloud_to_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/local_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/local_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/platform_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/test_data_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/test_init_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/test_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/e2e/test_seldon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.036054 neuro-extras-24.5.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:25.036054 neuro-extras-24.5.2/tests/unit/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/image/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/image/test_remote_image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/test_auth_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-29 17:12:00.000000 neuro-extras-24.5.2/tests/unit/test_select_job_preset.py
```

### Comparing `neuro-extras-24.5.1/LICENSE` & `neuro-extras-24.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/README.md` & `neuro-extras-24.5.2/README.md`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/__init__.py` & `neuro-extras-24.5.2/neuro_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/assets/merge_docker_auths.sh` & `neuro-extras-24.5.2/neuro_extras/assets/merge_docker_auths.sh`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/assets/seldon.package/seldon.Dockerfile` & `neuro-extras-24.5.2/neuro_extras/assets/seldon.package/seldon.Dockerfile`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/assets/seldon.package/seldon_model.py` & `neuro-extras-24.5.2/neuro_extras/assets/seldon.package/seldon_model.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/cli.py` & `neuro-extras-24.5.2/neuro_extras/cli.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/common.py` & `neuro-extras-24.5.2/neuro_extras/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/config.py` & `neuro-extras-24.5.2/neuro_extras/config.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/__init__.py` & `neuro-extras-24.5.2/neuro_extras/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/archive.py` & `neuro-extras-24.5.2/neuro_extras/data/archive.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/azure.py` & `neuro-extras-24.5.2/neuro_extras/data/azure.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/common.py` & `neuro-extras-24.5.2/neuro_extras/data/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/fs.py` & `neuro-extras-24.5.2/neuro_extras/data/fs.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/gcs.py` & `neuro-extras-24.5.2/neuro_extras/data/gcs.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/local.py` & `neuro-extras-24.5.2/neuro_extras/data/local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/operations.py` & `neuro-extras-24.5.2/neuro_extras/data/operations.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/remote.py` & `neuro-extras-24.5.2/neuro_extras/data/remote.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/s3.py` & `neuro-extras-24.5.2/neuro_extras/data/s3.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/data/web.py` & `neuro-extras-24.5.2/neuro_extras/data/web.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/image.py` & `neuro-extras-24.5.2/neuro_extras/image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/image_builder.py` & `neuro-extras-24.5.2/neuro_extras/image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
         await self.save_docker_config(docker_config, docker_config_uri)
 
         cache_image = neuro_sdk.RemoteImage(
             name="layer-cache/cache",
             project_name=project_name,
             registry=str(self._client.config.registry_url),
             cluster_name=self._client.cluster_name,
+            org_name=self._client.config.org_name,
         )
         cache_repo = self.parse_image_ref(str(cache_image))
         cache_repo = re.sub(r":.*$", "", cache_repo)  # drop tag
 
         if any(KANIKO_AUTH_PREFIX in env for env in envs):
             # we have extra auth info.
             # in this case we cannot mount registry auth info at the default path
```

### Comparing `neuro-extras-24.5.1/neuro_extras/k8s.py` & `neuro-extras-24.5.2/neuro_extras/k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/main.py` & `neuro-extras-24.5.2/neuro_extras/main.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/seldon.py` & `neuro-extras-24.5.2/neuro_extras/seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras/utils.py` & `neuro-extras-24.5.2/neuro_extras/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/neuro_extras.egg-info/SOURCES.txt` & `neuro-extras-24.5.2/neuro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/pyproject.toml` & `neuro-extras-24.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/setup.cfg` & `neuro-extras-24.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/setup.py` & `neuro-extras-24.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/conftest.py` & `neuro-extras-24.5.2/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/cloud_to_local.py` & `neuro-extras-24.5.2/tests/e2e/data/cloud_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/cloud_to_platform.py` & `neuro-extras-24.5.2/tests/e2e/data/cloud_to_platform.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/local_to_cloud.py` & `neuro-extras-24.5.2/tests/e2e/data/local_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/local_to_local.py` & `neuro-extras-24.5.2/tests/e2e/data/local_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/platform_to_cloud.py` & `neuro-extras-24.5.2/tests/e2e/data/platform_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/resources.py` & `neuro-extras-24.5.2/tests/e2e/data/resources.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/test_data_cp.py` & `neuro-extras-24.5.2/tests/e2e/data/test_data_cp.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/data/test_data_transfer.py` & `neuro-extras-24.5.2/tests/e2e/data/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/test_image.py` & `neuro-extras-24.5.2/tests/e2e/test_image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/test_k8s.py` & `neuro-extras-24.5.2/tests/e2e/test_k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/e2e/test_seldon.py` & `neuro-extras-24.5.2/tests/e2e/test_seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/unit/image/conftest.py` & `neuro-extras-24.5.2/tests/unit/image/conftest.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/unit/image/test_remote_image_builder.py` & `neuro-extras-24.5.2/tests/unit/image/test_remote_image_builder.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/unit/test_auth_merge.py` & `neuro-extras-24.5.2/tests/unit/test_auth_merge.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.5.1/tests/unit/test_select_job_preset.py` & `neuro-extras-24.5.2/tests/unit/test_select_job_preset.py`

 * *Files identical despite different names*

