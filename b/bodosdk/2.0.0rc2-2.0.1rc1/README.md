# Comparing `tmp/bodosdk-2.0.0rc2.tar.gz` & `tmp/bodosdk-2.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-2.0.0rc2.tar", last modified: Tue May  7 12:10:12 2024, max compression
+gzip compressed data, was "bodosdk-2.0.1rc1.tar", last modified: Wed May 29 21:21:42 2024, max compression
```

## Comparing `bodosdk-2.0.0rc2.tar` & `bodosdk-2.0.1rc1.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    93676 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/job_tpl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/job_tpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/clients/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.833275 bodosdk-2.0.0rc2/bodosdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/deprecation_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37725 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    45991 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    34045 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    93676 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 12:10:12.000000 bodosdk-2.0.0rc2/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 12:10:12.841275 bodosdk-2.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:10:12.837275 bodosdk-2.0.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    80088 2024-05-07 12:09:39.000000 bodosdk-2.0.0rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.562345 bodosdk-2.0.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    95304 2024-05-29 21:21:42.562345 bodosdk-2.0.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.562345 bodosdk-2.0.1rc1/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-29 21:21:42.562345 bodosdk-2.0.1rc1/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.554345 bodosdk-2.0.1rc1/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/job_tpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/bodosdk/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7470 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/bodosdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/job_tpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/clients/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/bodosdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/db/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/db/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/deprecation_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38444 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46839 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34983 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    95304 2024-05-29 21:21:42.000000 bodosdk-2.0.1rc1/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-29 21:21:42.000000 bodosdk-2.0.1rc1/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:21:42.000000 bodosdk-2.0.1rc1/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 21:21:42.000000 bodosdk-2.0.1rc1/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:21:42.000000 bodosdk-2.0.1rc1/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-29 21:21:42.562345 bodosdk-2.0.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:21:42.558345 bodosdk-2.0.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80088 2024-05-29 21:21:10.000000 bodosdk-2.0.1rc1/versioneer.py
```

### Comparing `bodosdk-2.0.0rc2/LICENSE` & `bodosdk-2.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/PKG-INFO` & `bodosdk-2.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 2.0.0rc2
-Summary: Bodo Platform SDK 2.0.0RC2
+Version: 2.0.1rc1
+Summary: Bodo Platform SDK 2.0.1.RC1
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,14 +17,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic~=1.9
 Requires-Dist: requests~=2.27.1
 Requires-Dist: pyjwt~=2.3.0
 Requires-Dist: typing_extensions>=4
 Requires-Dist: callee~=0.3.1
+Requires-Dist: pandas
+Requires-Dist: pyarrow
 
 # Bodo Platform SDK
 
 Bodo Platform SDK is a Python library that provides a simple way to interact with the Bodo Platform API. It allows you
 to create, manage, and monitor resources such as clusters, jobs, and workspaces.
 
 ## Getting Started
@@ -640,27 +642,29 @@
 * **Returns:**
   An instance of ClusterListAPIModel for listing clusters.
 * **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### connect(catalog: str, cluster_id: str)
 
-#### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str = None, auto_stop: int | None = None, auto_pause: int | None = None, image_id: str | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
+#### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str | None = None, auto_stop: int | None = None, auto_pause: int | None = None, auto_upgrade: bool | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
 
 Creates a new cluster with the specified configuration.
 
 * **Parameters:**
   * **name** (*str*) – The name of the cluster.
   * **instance_type** (*str* *,* *optional*) – The type of instance to use for the cluster nodes.
   * **workers_quantity** (*int* *,* *optional*) – The number of worker nodes in the cluster.
   * **description** (*str* *,* *optional*) – A description of the cluster.
   * **bodo_version** (*str* *,* *optional*) – The Bodo version to use for the cluster.
+    If not provided, the latest version is used.
   * **auto_stop** (*int* *,* *optional*) – The auto-stop time in minutes for the cluster.
   * **auto_pause** (*int* *,* *optional*) – The auto-pause time in minutes for the cluster.
-  * **image_id** (*str* *,* *optional*) – The ID of the image to use for the cluster.
+  * **auto_upgrade** (*bool* *,* *optional*) – Should the cluster be automatically upgraded to
+    the latest Bodo version on restart.
   * **accelerated_networking** (*bool* *,* *optional*) – Whether to use accelerated networking.
   * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
   * **use_spot_instance** (*bool* *,* *optional*) – Whether to use spot instances for the cluster.
   * **aws_deployment_subnet_id** (*str* *,* *optional*) – The AWS deployment subnet ID.
   * **availability_zone** (*str* *,* *optional*) – The availability zone for the cluster.
   * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The instance role or a custom role configuration.
   * **custom_tags** (*Dict* *,* *optional*) – Custom tags to assign to the cluster resources.
@@ -859,31 +863,31 @@
 
 #### cancel_jobs(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 #### get(id: str)
 
 #### list(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None, order: Dict | None = None)
 
-#### run(template_id: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run(template_id: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = None)
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = True)
 
 #### wait_for_status(id: str, statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 <a id="module-bodosdk.clients.job_tpl"></a>
 
 ### *class* bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobTemplateClient`
 
 #### *property* JobTemplate *: [JobTemplate](#bodosdk.models.job.JobTemplate)*
 
 #### *property* JobTemplateList *: [JobTemplateList](#bodosdk.models.job.JobTemplateList)*
 
-#### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
+#### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None, store_result: bool = False)
 
 #### get(id: str)
 
 #### list(filters: Dict = None)
 
 #### remove(id: str)
 
@@ -901,14 +905,18 @@
 
 #### *property* CloudConfigList *: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)*
 
 #### *property* Workspace *: [Workspace](#bodosdk.models.workspace.Workspace)*
 
 #### *property* WorkspaceList *: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)*
 
+#### create_aws_cloud_config(name: str, tf_backend_region: str, role_arn: str | None = None, tf_bucket_name: str | None = None, tf_dynamo_db_table_name: str | None = None, account_id: str | None = None, access_key_id: str | None = None, secret_access_key: str | None = None, custom_tags: dict | None = None)
+
+#### create_azure_cloud_config(name: str, tf_backend_region: str, tenant_id: str, subscription_id: str, resource_group: str, custom_tags: dict | None = None)
+
 #### create_workspace(name: str, region: str, storage_endpoint_enabled: bool, cloud_config_id: str = None, vpc_id: str | None = None, public_subnets_ids: List[str] | None = None, private_subnets_ids: List[str] | None = None, custom_tags: dict | None = None)
 
 #### delete_workspace(id)
 
 #### get_cloud_config(id)
 
 #### get_workspace(id)
@@ -994,40 +1002,48 @@
 
 #### username *: str | None*
 
 #### warehouse *: str | None*
 
 <a id="module-bodosdk.models.cloud_config"></a>
 
-### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str = 'AWS', name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAwsCloudConfig`
 
+#### cloud_provider *: str*
+
 #### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None*
 
-### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
+### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None, accessKeyId: str | None = None, secretAccessKey: str | None = None)
 
 Bases: `SDKBaseModel`, `IAwsProviderData`
 
+#### access_key_id *: str | None*
+
 #### account_id *: str | None*
 
 #### external_id *: str | None*
 
 #### role_arn *: str | None*
 
+#### secret_access_key *: str | None*
+
 #### tf_backend_region *: str | None*
 
 #### tf_bucket_name *: str | None*
 
 #### tf_dynamo_db_table_name *: str | None*
 
-### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str = 'AZURE', name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAzureCloudConfig`
 
+#### cloud_provider *: str*
+
 #### data *: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
 ### *class* bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAzureProviderData`
 
 #### application_id *: str | None*
@@ -1115,15 +1131,15 @@
 * **Type:**
   str
 
 #### bodo_version *: str*
 
 #### image_id *: str*
 
-### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
+### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, autoUpgrade: bool | None = None, bodoVersion: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `ICluster`
 
 Represents a cluster in the SDK model, encapsulating various properties and operations
 related to a compute cluster.
 
 #### name
@@ -1180,24 +1196,25 @@
 
 The auto-pause configuration in minutes.
 The cluster automatically pauses when idle for this duration.
 
 * **Type:**
   Optional[int]
 
-#### bodo_version
+#### auto_upgrade
 
-The version of Bodo being used in the cluster.
+Should the cluster be upgraded on restart.
+The cluster is automatically upgraded to the latest Bodo version on restart when True.
 
 * **Type:**
-  Optional[str]
+  Optional[bool]
 
-#### image_id
+#### bodo_version
 
-The ID of the image used for the cluster’s instances.
+The version of Bodo being used in the cluster.
 
 * **Type:**
   Optional[str]
 
 #### cores_per_worker
 
 The number of CPU cores per worker node.
@@ -1349,14 +1366,16 @@
 
 #### auto_az *: bool | None*
 
 #### auto_pause *: int | None*
 
 #### auto_stop *: int | None*
 
+#### auto_upgrade *: bool | None*
+
 #### autoscaling_identifier *: str | None*
 
 #### availability_zone *: str | None*
 
 #### aws_deployment_subnet_id *: str | None*
 
 #### bodo_version *: str | None*
@@ -1411,16 +1430,14 @@
 #### *property* id *: str*
 
 The UUID of the cluster.
 
 * **Returns:**
   The UUID string of the cluster.
 
-#### image_id *: str | None*
-
 #### in_state_since *: datetime | None*
 
 #### instance_role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None*
 
 #### instance_type *: str | None*
 
 #### is_job_dedicated *: bool | None*
@@ -1455,15 +1472,15 @@
 * **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
 * **Returns:**
   The Cluster instance with updated status.
 * **Raises:**
   **ConflictException** – If the cluster cannot be resumed due to its current status.
 
-#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = False)
 
 Submits a batch job for execution using specified configurations and resources.
 
 This method creates and dispatches a job within a computing cluster, allowing for extensive customization of
 execution parameters including source data, runtime environment, and failure handling strategies.
 
 * **Parameters:**
@@ -1477,20 +1494,21 @@
   * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job.
   * **timeout** (*int* *,* *optional*) – Maximum runtime (in seconds) before the job is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
   * **name** (*str* *,* *optional*) – Name of the job.
   * **catalog** (*str* *,* *optional*) – Catalog to log the job under.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object representing the submitted job, capable of providing status and results.
 * **Return type:**
   IJobRun
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = False)
 
 > Submits an SQL query for execution on the cluster, returning a job run object.
 
 > This method handles the execution of an SQL query within a defined cluster environment.
 > It supports customization of execution parameters such as query arguments,
 > job name, execution timeouts, and retry strategies.
 
@@ -1500,14 +1518,15 @@
 >   sql_query (str, optional): The SQL query string to be executed.
 >   name (str, optional): Descriptive name for the SQL job.
 >   args (dict, optional): Dictionary of arguments that are passed to the SQL query.
 >   timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
 >   num_retries (int, optional): Number of times the job will be retried on failure.
 >   delay_between_retries (int, optional): Interval in seconds between job retries.
 >   retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+>   store_result (bool, optional): Whether to store on S3 job results or not.
 
 > Returns:
 > : IJobRun: An object representing the status and result of the executed SQL job.
 
 ```
 `
 ```
@@ -1528,21 +1547,22 @@
 Stops the cluster.
 
 * **Parameters:**
   **wait** – If True, waits till cluster will be STOPPED.
 * **Returns:**
   The Cluster instance with updated status.
 
-#### update(auto_stop: int | None = None, auto_pause: int | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
+#### update(auto_stop: int | None = None, auto_pause: int | None = None, auto_upgrade: bool | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the cluster’s configuration with the provided values.
 
 * **Parameters:**
   * **auto_stop** – Optional; configures auto-stop feature.
   * **auto_pause** – Optional; configures auto-pause feature.
+  * **auto_upgrade** – Optional; enables/disables auto-upgrade on restart.
   * **description** – Optional; updates the cluster’s description.
   * **name** – Optional; updates the cluster’s name.
   * **workers_quantity** – Optional; updates the number of workers.
   * **instance_role** – Optional; updates the instance role.
   * **instance_type** – Optional; updates the instance type.
   * **bodo_version** – Optional; updates the Bodo version.
   * **auto_az** – Optional; enables/disables automatic availability zone selection.
@@ -1758,15 +1778,15 @@
 
 * **Returns:**
   The current instance of ClusterList after attempting to resume
   : all clusters.
 * **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = None)
 
 Executes a job across all clusters managed by the instance.
 
 This method supports multiple source types and configurations for executing jobs,
 including retries and custom environment variables.
 
 * **Parameters:**
@@ -1780,23 +1800,24 @@
   * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job execution.
   * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
   * **name** (*str* *,* *optional*) – A name for the job run.
   * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the job.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object listing the UUIDs of jobs that were successfully initiated.
 * **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = None)
 
 Executes an SQL job across all clusters managed by the instance.
 
 This method submits an SQL query for execution, allowing for additional configurations such as retries
 and setting execution timeouts.
 
 * **Parameters:**
@@ -1805,14 +1826,15 @@
   * **sql_query** (*str* *,* *optional*) – The SQL query to execute.
   * **name** (*str* *,* *optional*) – A name for the job run.
   * **args** (*dict* *,* *optional*) – Additional arguments specific to the SQL job.
   * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object listing the UUIDs of SQL jobs that were successfully initiated.
 * **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
@@ -1935,31 +1957,31 @@
 
 ### *class* bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
 
 Bases: `object`
 
 #### cursor()
 
-### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
+### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int = 3600)
 
 Bases: `object`
 
 #### execute(query: str, \*\*kwargs)
 
 #### execute_async(query: str, \*\*kwargs)
 
 #### fetchall()
 
 #### fetchmany(size)
 
 #### fetchone()
 
-### *exception* bodosdk.db.connection.QueryError
+#### *property* rowcount
 
-Bases: `Exception`
+#### *property* rownumber
 
 <a id="module-bodosdk.models.job"></a>
 
 ### *class* bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
 
 Bases: `SDKBaseModel`
 
@@ -2001,15 +2023,15 @@
 
 #### token *: str*
 
 #### type *: str*
 
 #### username *: str*
 
-### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
+### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None, storeResult: bool | None = False)
 
 Bases: `SDKBaseModel`, `IJobConfig`
 
 Configures details for executing a job, including the execution source, file location, and execution parameters.
 
 #### type
 
@@ -2095,14 +2117,16 @@
 
 #### retry_strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None*
 
 #### source *: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None*
 
 #### sql_query_parameters *: dict | None*
 
+#### store_result *: bool | None*
+
 #### timeout *: int | None*
 
 #### type *: str | None*
 
 ### *class* bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
 
 Bases: `SDKBaseModel`
@@ -2329,14 +2353,16 @@
 
 #### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
 #### finished_at *: datetime | None*
 
 #### get_logs_urls()
 
+#### get_result_urls()
+
 #### get_stderr()
 
 #### get_stdout()
 
 #### *property* id *: str*
 
 #### job_template_id *: str | None*
@@ -2614,15 +2640,15 @@
 
 #### *property* id
 
 #### job_runs *: List[[JobRun](#bodosdk.models.job.JobRun)]*
 
 #### name *: str | None*
 
-#### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
+#### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None, store_result: bool = False)
 
 #### uuid *: str | None*
 
 ### *class* bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplateFilter`
 
@@ -2866,34 +2892,27 @@
 
 #### path *: str*
 
 #### type *: str*
 
 <a id="module-bodosdk.models.common"></a>
 
-### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
+### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
 
 Bases: [`NetworkData`](#bodosdk.models.common.NetworkData)
 
 Extends the NetworkData class to include specific properties for AWS networking.
 
 #### vpc_id
 
 The ID of the AWS Virtual Private Cloud (VPC) where workspace should be created.
 
 * **Type:**
   Optional[str]
 
-#### fetched_vpc_id
-
-The ID of the fetched AWS VPC - if no vpc_id provided.
-
-* **Type:**
-  Optional[str]
-
 #### public_subnets_ids
 
 List of IDs for the public subnets within the AWS VPC.
 
 * **Type:**
   Optional[List[str]]
 
@@ -2907,16 +2926,14 @@
 #### policies_arn
 
 List of AWS Resource Names (ARNs) for the policies applied to the network.
 
 * **Type:**
   Optional[List[str]]
 
-#### fetched_vpc_id *: str | None*
-
 #### policies_arn *: List[str] | None*
 
 #### private_subnets_ids *: List[str] | None*
 
 #### public_subnets_ids *: List[str] | None*
 
 #### vpc_id *: str | None*
@@ -3076,21 +3093,21 @@
 
 #### page_size *: int | None*
 
 #### total *: int | None*
 
 <a id="module-bodosdk.models.workspace"></a>
 
-### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
+### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase) | [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspace`
 
 #### assigned_at *: datetime | None*
 
-#### cloud_config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
+#### cloud_config *: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase) | [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
 
 #### created_by *: str | None*
 
 #### custom_tags *: Dict[str, Any] | None*
 
 #### delete()
```

### Comparing `bodosdk-2.0.0rc2/README.md` & `bodosdk-2.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/auth.py` & `bodosdk-2.0.1rc1/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/base.py` & `bodosdk-2.0.1rc1/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/billing.py` & `bodosdk-2.0.1rc1/bodosdk/api/billing.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/catalog.py` & `bodosdk-2.0.1rc1/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/cloud_config.py` & `bodosdk-2.0.1rc1/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/cluster.py` & `bodosdk-2.0.1rc1/bodosdk/api/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return ClusterListAPIModel(**response.json())
 
     def create_cluster(self, cluster_definition: ClusterDefinition) -> ClusterResponse:
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
         resp = self._requests.post(
             f"{self.get_resource_url('v1')}",
-            data=cluster_definition.json(by_alias=True),
+            data=cluster_definition.json(by_alias=True, exclude_none=True),
             headers=headers,
         )
         self.handle_error(resp)
         return ClusterResponse(**resp.json())
 
     def remove_cluster(self, uuid, force_remove, mark_as_terminated):
         params = {
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/instance_role.py` & `bodosdk-2.0.1rc1/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/job.py` & `bodosdk-2.0.1rc1/bodosdk/api/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -65,34 +65,14 @@
         try:
             headers = self.get_auth_header()
             url = f"{self.get_resource_url('v1')}/{uuid}/logs?forceRefresh={str(force_refresh).lower()}"
             resp = self._requests.get(url, headers=headers)
             self.handle_error(resp)
             json_data = resp.json()
             job_run_logs_response = JobRunLogsResponseApiModel(**json_data)
-
-            def fetch_and_write_file(url: str, file_name: str) -> None:
-                try:
-                    response = self._requests.get(url)
-                    if response.status_code == 200:
-                        with open(file_name, "wb") as file:
-                            file.write(response.content)
-                    else:
-                        logging.error(
-                            f"File {file_name} fetch failed: {response.status_code}"
-                        )
-                except Exception as e:
-                    logging.error(f"Bad File fetch Response: {e}")
-
-            fetch_and_write_file(
-                job_run_logs_response.stdout_location_url, f"stdout_{uuid}.txt"
-            )
-            fetch_and_write_file(
-                job_run_logs_response.stderr_location_url, f"stderr_{uuid}.txt"
-            )
             return job_run_logs_response
         except Exception as e:
             logging.error(f"Bad Response: {e}")
 
     def create_job_run(self, job_run: IJobRun):
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
@@ -126,7 +106,17 @@
         headers.update(self.get_auth_header())
         resp = self._requests.delete(
             f"{self.get_resource_url('v1')}/{uuid}",
             headers=headers,
         )
         self.handle_error(resp)
         return resp.json()
+
+    def get_result_links(self, uuid) -> dict:
+        headers = {"Content-type": "application/json"}
+        headers.update(self.get_auth_header())
+        resp = self._requests.get(
+            f"{self.get_resource_url('v1')}/{uuid}/result",
+            headers=headers,
+        )
+        self.handle_error(resp)
+        return resp.json()
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/job_tpl.py` & `bodosdk-2.0.1rc1/bodosdk/api/job_tpl.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/__init__.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/catalog.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/cloud_config.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/cloud_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 from bodosdk.base import APIBaseModel
 
 
 class CreateAwsProviderDataAPIModel(APIBaseModel):
     tf_backend_region: str = Field(..., alias="tfBackendRegion")
     secret_access_key: Optional[str] = Field(None, alias="secretAccessKey")
     access_key_id: Optional[str] = Field(None, alias="accessKeyId")
+    role_arn: Optional[str] = Field(None, alias="roleArn")
+    tf_bucket_name: Optional[str] = Field(None, alias="tfBucketName")
+    tf_dynamo_db_table_name: Optional[str] = Field(None, alias="tfDynamoDbTableName")
+    external_id: Optional[str] = Field(None, alias="externalId")
+    account_id: Optional[str] = Field(None, alias="accountId")
 
 
 class CreateAzureProviderDataAPIModel(APIBaseModel):
     tf_backend_region: Optional[str] = Field(None, alias="tfBackendRegion")
     subscription_id: str = Field(..., alias="subscriptionId")
     tenant_id: str = Field(..., alias="tenantId")
     resource_group: str = Field(..., alias="resourceGroup")
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/cluster.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 class ClusterDefinition(APIBaseModel):
     name: Optional[str]
     instance_type: Optional[str] = Field(None, alias="instanceType")
     workers_quantity: Optional[int] = Field(None, alias="workersQuantity")
     auto_stop: Optional[int] = Field(None, alias="autoStop")  # in minutes
     auto_pause: Optional[int] = Field(None, alias="autoPause")  # in minutes
-    image_id: Optional[str] = Field(None, alias="imageId")
+    auto_upgrade: Optional[bool] = Field(None, alias="autoUpgrade")
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
     description: Optional[str] = None
     accelerated_networking: Optional[bool] = Field(False, alias="acceleratedNetworking")
     is_job_dedicated: Optional[bool] = Field(False, alias="isJobDedicated")
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
     aws_deployment_subnet_id: Optional[str] = Field(None, alias="awsDeploymentSubnetId")
     instance_role_uuid: Optional[str] = Field(None, alias="instanceRoleUUID")
@@ -70,14 +70,15 @@
     uuid: Union[str, UUID]
     status: Optional[str]
     description: Optional[str] = ""
     instance_type: Optional[str] = Field(None, alias="instanceType")
     workers_quantity: Optional[int] = Field(None, alias="workersQuantity")
     auto_stop: Optional[int] = Field(None, alias="autoStop")
     auto_pause: Optional[int] = Field(None, alias="autoPause")
+    auto_upgrade: Optional[bool] = Field(None, alias="autoUpgrade")
     # TODO: Should be removed in version +2.x.x node metadata have the same information
     nodes_ip: Optional[List[str]] = Field(None, alias="nodesIp")
     # TODO: In ClusterDefinition when cluster is creating that field is required
     #  but here is optional
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
     # TODO: In ClusterDefinition when cluster is creating that field is optional
     #  but here is required
@@ -101,14 +102,15 @@
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
 
 
 class ModifyCluster(APIBaseModel):
     uuid: Union[str, UUID]
     auto_stop: Optional[int] = Field(None, alias="autoStop")
     auto_pause: Optional[int] = Field(None, alias="autoPause")
+    auto_upgrade: Optional[bool] = Field(None, alias="autoUpgrade")
     description: Optional[str] = Field(None, alias="description")
     name: Optional[str] = Field(None, alias="name")
     workers_quantity: Optional[int] = Field(None, alias="workersQuantity")
     instance_role_uuid: Optional[str] = Field(None, alias="instanceRoleUUID")
     instance_type: Optional[str] = Field(None, alias="instanceType")
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
     auto_az: Optional[bool] = Field(True, alias="autoAZ")
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/instance_role.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/job.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from bodosdk.base import APIBaseModel, PaginationOrder
 
 
 class JobClusterDefinition(APIBaseModel):
     instance_type: str = Field(..., alias="instanceType")
     workers_quantity: int = Field(..., alias="workersQuantity")
     accelerated_networking: bool = Field(..., alias="acceleratedNetworking")
-    image_id: Optional[str] = Field(None, alias="imageId")
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
     instance_role_uuid: Optional[str] = Field(None, alias="instanceRoleUUID")
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
     aws_deployment_subnet_id: Optional[str] = Field(None, alias="awsDeploymentSubnetId")
     custom_tags: Optional[Dict[str, str]] = Field(None, alias="customTags")
     auto_pause: Optional[int] = Field(60, alias="autoPause")
     auto_stop: Optional[int] = Field(0, alias="autoStop")
@@ -221,14 +220,15 @@
     exec_text: Optional[str] = Field(None, alias="sqlQueryText")
     sql_query_parameters: Optional[dict] = Field(None, alias="sqlQueryParameters")
     args: Optional[Union[dict, str]]
     retry_strategy: Optional[RetryStrategy] = Field(None, alias="retryStrategy")
     timeout: Optional[int]
     env_vars: Optional[dict] = Field(None, alias="envVars")
     catalog: Optional[str]
+    store_result: Optional[bool] = Field(False, alias="storeResult")
 
     def __repr__(self):
         repr_str = ""
         for k, v in self.dict().items():
             if v is not None:
                 repr_str += f"{k}: {v}\n"
             else:
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/models/workspace.py` & `bodosdk-2.0.1rc1/bodosdk/api/models/workspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 class NetworkData(APIBaseModel):
     region: str
     storage_endpoint: bool = Field(..., alias="storageEndpoint")
 
 
 class AWSNetworkData(NetworkData):
     vpc_id: Optional[str] = Field(None, alias="vpcId")
-    fetched_vpc_id: Optional[str] = Field(None, alias="fetchedVpcId")
     public_subnets_ids: Optional[List[str]] = Field(None, alias="publicSubnetsIds")
     private_subnets_ids: Optional[List[str]] = Field(None, alias="privateSubnetsIds")
     policies_arn: Optional[List[str]] = Field(None, alias="policyArns")
 
 
 class Relation(APIBaseModel):
     uuid: Union[UUID, str]
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/request_wrapper.py` & `bodosdk-2.0.1rc1/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/secret_group.py` & `bodosdk-2.0.1rc1/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/secrets.py` & `bodosdk-2.0.1rc1/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/api/workspace.py` & `bodosdk-2.0.1rc1/bodosdk/api/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self._resource_url = "workspaces"
 
     def create(self, workspace_definition: WorkspaceAPIModel):
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
         resp = self._requests.post(
             f"{self.get_resource_url('v1')}",
-            data=workspace_definition.json(by_alias=True),
+            data=workspace_definition.json(by_alias=True, exclude_none=True),
             headers=headers,
         )
         self.handle_error(resp)
         return WorkspaceAPIModel(**resp.json())
 
     def get(self, uuid) -> WorkspaceAPIModel:
         resp = self._requests.get(
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/base.py` & `bodosdk-2.0.1rc1/bodosdk/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/catalog.py` & `bodosdk-2.0.1rc1/bodosdk/clients/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/cluster.py` & `bodosdk-2.0.1rc1/bodosdk/clients/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,18 +69,18 @@
     @check_deprecation
     def create(
         self,
         name: str,
         instance_type: str = None,
         workers_quantity: int = None,
         description: Optional[str] = None,
-        bodo_version: str = None,
+        bodo_version: Optional[str] = None,
         auto_stop: Optional[int] = None,
         auto_pause: Optional[int] = None,
-        image_id: Optional[str] = None,
+        auto_upgrade: Optional[bool] = None,
         accelerated_networking: Optional[bool] = None,
         auto_az: Optional[bool] = None,
         use_spot_instance: Optional[bool] = None,
         aws_deployment_subnet_id: Optional[str] = None,
         availability_zone: Optional[str] = None,
         instance_role: Optional[Union[InstanceRole, Dict]] = None,
         custom_tags: Optional[Dict] = None,
@@ -90,17 +90,19 @@
 
         Args:
             name (str): The name of the cluster.
             instance_type (str, optional): The type of instance to use for the cluster nodes.
             workers_quantity (int, optional): The number of worker nodes in the cluster.
             description (str, optional): A description of the cluster.
             bodo_version (str, optional): The Bodo version to use for the cluster.
+                If not provided, the latest version is used.
             auto_stop (int, optional): The auto-stop time in minutes for the cluster.
             auto_pause (int, optional): The auto-pause time in minutes for the cluster.
-            image_id (str, optional): The ID of the image to use for the cluster.
+            auto_upgrade (bool, optional): Should the cluster be automatically upgraded to
+                the latest Bodo version on restart.
             accelerated_networking (bool, optional): Whether to use accelerated networking.
             auto_az (bool, optional): Whether to automatically select the availability zone.
             use_spot_instance (bool, optional): Whether to use spot instances for the cluster.
             aws_deployment_subnet_id (str, optional): The AWS deployment subnet ID.
             availability_zone (str, optional): The availability zone for the cluster.
             instance_role (InstanceRole | Dict, optional): The instance role or a custom role configuration.
             custom_tags (Dict, optional): Custom tags to assign to the cluster resources.
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/instance_role.py` & `bodosdk-2.0.1rc1/bodosdk/clients/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/job.py` & `bodosdk-2.0.1rc1/bodosdk/clients/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,27 +54,31 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = None,
     ) -> bodosdk.models.job.JobRun:
         if isinstance(cluster, dict):
             cluster = self._workspace_client.ClusterClient.Cluster(**cluster)
         data = {
             "name": name,
             "job_template_id": template_id,
             "config": {
                 "type": code_type,
                 "source": source,
                 "exec_file": exec_file,
                 "exec_text": exec_text,
                 "args": args if code_type != "SQL" else None,
                 "sql_query_parameters": args if code_type == "SQL" else None,
+                "store_result": store_result
+                if store_result is not None
+                else code_type == "SQL",
                 "env_vars": env_vars,
                 "timeout": timeout,
                 "catalog": catalog,
             },
         }
         if (
             num_retries is not None
@@ -102,27 +106,29 @@
         cluster: Union[dict, ICluster] = None,
         name: str = None,
         args: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
+        store_result: bool = True,
     ) -> bodosdk.models.job.JobRun:
         if isinstance(cluster, dict):
             cluster = self._workspace_client.ClusterClient.Cluster(**cluster)
         data = {
             "name": name,
             "job_template_id": template_id,
             "config": {
                 "type": "SQL",
                 "source": TextSource(),
                 "exec_text": sql_query,
                 "catalog": catalog,
                 "sql_query_parameters": args,
                 "timeout": timeout,
+                "store_result": store_result,
             },
         }
         if (
             num_retries is not None
             or delay_between_retries is not None
             or retry_on_timeout is not None
         ):
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/job_tpl.py` & `bodosdk-2.0.1rc1/bodosdk/clients/job_tpl.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,25 +48,29 @@
         args: Union[dict, str] = None,
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> JobTemplate:
         if isinstance(cluster, dict):
             cluster = self._workspace_client.ClusterClient.Cluster(**cluster)
         data = {
             "name": name,
             "description": description,
             "config": {
                 "type": code_type,
                 "source": {"type": "SQL"}
                 if code_type == "SQL" and exec_text
                 else source,
+                "store_result": store_result
+                if store_result is not None
+                else code_type == "SQL",
                 "exec_file": exec_file,
                 "exec_text": exec_text,
                 "args": args if code_type != "SQL" else None,
                 "sql_query_parameters": args if code_type == "SQL" else None,
                 "env_vars": env_vars,
                 "timeout": timeout,
                 "catalog": catalog,
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/organization.py` & `bodosdk-2.0.1rc1/bodosdk/clients/organization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from time import sleep
 from typing import Optional, List, Union
 from unittest.mock import MagicMock
 
 from bodosdk import _version
 from bodosdk.api.auth import AuthApi
 from bodosdk.api.cloud_config import CloudConfigApi
 from bodosdk.api.request_wrapper import RequestWrapper
@@ -16,14 +17,16 @@
     IAzureCloudConfig,
 )
 from bodosdk.models.cloud_config import (
     CloudConfigList,
     AwsCloudConfig,
     AzureCloudConfig,
     CloudConfigBase,
+    AwsProviderData,
+    AzureProviderData,
 )
 from bodosdk.models.common import AWSNetworkData, NetworkData
 from bodosdk.models.workspace import Workspace, WorkspaceList, WorkspaceFilter
 
 
 class BodoOrganizationClient(IBodoOrganizationClient):
     def __init__(
@@ -145,9 +148,66 @@
     @check_deprecation
     def list_cloud_configs(
         self, filters: Optional[Union[dict]] = None
     ) -> CloudConfigList:
         return self.CloudConfigList(filters=filters)
 
     @check_deprecation
+    def create_aws_cloud_config(
+        self,
+        name: str,
+        tf_backend_region: str,
+        role_arn: Optional[str] = None,
+        tf_bucket_name: Optional[str] = None,
+        tf_dynamo_db_table_name: Optional[str] = None,
+        account_id: Optional[str] = None,
+        access_key_id: Optional[str] = None,
+        secret_access_key: Optional[str] = None,
+        custom_tags: Optional[dict] = None,
+    ) -> AwsCloudConfig:
+        cloud_config = self.AwsCloudConfig(
+            name=name,
+            custom_tags=custom_tags,
+            data=AwsProviderData(
+                tf_backend_region=tf_backend_region,
+                role_arn=role_arn,
+                tf_bucket_name=tf_bucket_name,
+                tf_dynamo_db_table_name=tf_dynamo_db_table_name,
+                account_id=account_id,
+                access_key_id=access_key_id,
+                secret_access_key=secret_access_key,
+            ),
+        )
+        cloud_config._save()
+        cloud_config._load()
+        # need to wait till AWS / AZURE resource be ready
+        sleep(10)
+        return cloud_config
+
+    @check_deprecation
+    def create_azure_cloud_config(
+        self,
+        name: str,
+        tf_backend_region: str,
+        tenant_id: str,
+        subscription_id: str,
+        resource_group: str,
+        custom_tags: Optional[dict] = None,
+    ) -> AzureCloudConfig:
+        cloud_config = self.AzureCloudConfig(
+            name=name,
+            custom_tags=custom_tags,
+            data=AzureProviderData(
+                tf_backend_region=tf_backend_region,
+                resource_group=resource_group,
+                tenant_id=tenant_id,
+                subscription_id=subscription_id,
+            ),
+        )
+        cloud_config._save()
+        # need to wait till AWS / AZURE resource be ready
+        sleep(20)
+        return cloud_config
+
+    @check_deprecation
     def get_cloud_config(self, id) -> Union[IAwsCloudConfig, IAzureCloudConfig]:
         return self.CloudConfig(uuid=id)._load()
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/secret.py` & `bodosdk-2.0.1rc1/bodosdk/clients/secret.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/clients/workspace.py` & `bodosdk-2.0.1rc1/bodosdk/clients/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/deprecation_decorator.py` & `bodosdk-2.0.1rc1/bodosdk/deprecation_decorator.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/interfaces.py` & `bodosdk-2.0.1rc1/bodosdk/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,17 @@
         finished_at: Union[datetime, None] = None,
         page: int = None,
         size: int = None,
         order: str = None,
     ) -> dict:
         raise NotImplementedError
 
+    def get_result_links(self, uuid):
+        raise NotImplementedError
+
 
 class IJobTplApi(ABC):
     @abstractmethod
     def list_job_tpl(
         self,
         page: int = None,
         size: int = None,
@@ -431,14 +434,15 @@
     exec_text: Optional[str]
     sql_query_parameters: Optional[dict]
     args: Optional[Union[dict, str]]
     retry_strategy: Optional[IRetryStrategy]
     timeout: Optional[int]
     env_vars: Optional[dict]
     catalog: Optional[str]
+    store_result: Optional[bool]
 
 
 class IJobRun(ABC):
     def dict(self):
         super().dict()
 
     def __call__(self, **kwargs) -> "IJobRun":
@@ -461,15 +465,17 @@
     cluster_config: Optional[ICluster]
     config: Optional[Union[dict, IJobConfig]]
     job_template_id: Optional[str]
     submitter: Optional[str]
     stats: Optional[dict]
 
     @abstractmethod
-    def wait_for_status(self, statuses, timeout, tick) -> "IJobRun":
+    def wait_for_status(
+        self, statuses: List[str], timeout: int = 3600, tick: int = 30
+    ) -> "IJobRun":
         raise NotImplementedError
 
     @abstractmethod
     def _save(self) -> IJobRun:
         raise NotImplementedError
 
     @property
@@ -492,14 +498,18 @@
     def get_stdout(self) -> str:
         raise NotImplementedError
 
     @abstractmethod
     def get_stderr(self) -> str:
         raise NotImplementedError
 
+    @abstractmethod
+    def get_result_urls(self) -> list:
+        raise NotImplementedError
+
 
 class IJobTemplate(ABC):
     uuid: Optional[str]
     name: Optional[str]
     job_runs: List[IJobRun]
     description: Optional[str]
     created_by: Optional[str]
@@ -531,14 +541,15 @@
         args: Union[dict, str] = None,
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> IJobRun:
         raise NotImplementedError
 
     @abstractmethod
     def delete(self):
         raise NotImplementedError
 
@@ -579,15 +590,17 @@
         raise NotImplementedError
 
     @abstractmethod
     def refresh(self) -> "IClusterList":
         raise NotImplementedError
 
     @abstractmethod
-    def wait_for_status(self, statuses, timeout, tick) -> "IClusterList":
+    def wait_for_status(
+        self, statuses: List[str], timeout: int = 300, tick: int = 30
+    ) -> "IClusterList":
         raise NotImplementedError
 
     @abstractmethod
     def run_job(
         self,
         template_id: str = None,
         code_type: str = None,
@@ -599,14 +612,15 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> IJobRunList:
         raise NotImplementedError
 
     @abstractmethod
     def run_sql_query(
         self,
         template_id: str = None,
@@ -663,15 +677,17 @@
         raise NotImplementedError
 
     @abstractmethod
     def _load_next_page(self) -> IJobRunList:
         raise NotImplementedError
 
     @abstractmethod
-    def wait_for_status(self, statuses, timeout, tick) -> IJobRunList:
+    def wait_for_status(
+        self, statuses: List[str], timeout: int = 3600, tick: int = 30
+    ) -> IJobRunList:
         raise NotImplementedError
 
     @property
     def clusters(self) -> IClusterList:
         raise NotImplementedError
 
 
@@ -720,16 +736,16 @@
     id: Optional[str]
     status: Optional[str]
     description: Optional[str]
     instance_type: Optional[str]
     workers_quantity: Optional[int]
     auto_stop: Optional[int]
     auto_pause: Optional[int]
+    auto_upgrade: Optional[bool]
     bodo_version: Optional[str]
-    image_id: Optional[str]
     cores_per_worker: Optional[int]
     accelerated_networking: Optional[bool]
     created_at: Optional[str]
     updated_at: Optional[str]
     is_job_dedicated: Optional[bool]
     auto_az: Optional[bool]
     use_spot_instance: Optional[bool]
@@ -767,14 +783,15 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> IJobRun:  # TODO: add other fields and attribute typing
         raise NotImplementedError
 
     @abstractmethod
     def run_sql_query(
         self,
         template_id: str = None,
@@ -782,14 +799,15 @@
         sql_query: str = None,
         name: str = None,
         args: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
+        store_result: bool = False,
     ) -> IJobRun:  # TODO: add other fields and attribute typing
         raise NotImplementedError
 
     @abstractmethod
     def cancel_jobs(self) -> "ICluster":
         raise NotImplementedError
 
@@ -818,22 +836,25 @@
         raise NotImplementedError
 
     @abstractmethod
     def delete(self, force=False, mark_as_terminated=False, wait=False):
         raise NotImplementedError
 
     @abstractmethod
-    def wait_for_status(self, statuses, timeout=600, tick=30) -> "ICluster":
+    def wait_for_status(
+        self, statuses: List[str], timeout: int = 600, tick: int = 30
+    ) -> "ICluster":
         raise NotImplementedError
 
     @abstractmethod
     def update(
         self,
         auto_stop: Optional[int] = None,
         auto_pause: Optional[int] = None,
+        auto_upgrade: Optional[bool] = None,
         description: Optional[str] = None,
         name: Optional[str] = None,
         workers_quantity: Optional[int] = None,
         instance_role: Optional[IInstanceRole] = None,
         instance_type: Optional[str] = None,
         bodo_version: Optional[str] = None,
         auto_az: Optional[bool] = None,
@@ -864,14 +885,16 @@
     def fetchmany(self, size):
         raise NotImplementedError
 
     @abstractmethod
     def fetchall(self):
         raise NotImplementedError
 
+    rowcount: int
+
 
 class IConnection:
     @abstractmethod
     def cursor(self) -> ICursor:
         raise NotImplementedError
 
 
@@ -901,15 +924,15 @@
         name: str,
         instance_type: str = None,
         workers_quantity: int = None,
         description: Optional[str] = None,
         bodo_version: str = None,
         auto_stop: Optional[int] = None,
         auto_pause: Optional[int] = None,
-        image_id: Optional[str] = None,
+        auto_upgrade: Optional[bool] = None,
         accelerated_networking: Optional[bool] = None,
         auto_az: Optional[bool] = None,
         use_spot_instance: Optional[bool] = None,
         aws_deployment_subnet_id: Optional[str] = None,
         availability_zone: Optional[str] = None,
         instance_role: Optional[Union[IInstanceRole, Dict]] = None,
         custom_tags: Optional[Dict] = None,
@@ -952,14 +975,15 @@
     def update(
         self,
         id: str,
         name: Optional[str] = None,
         description: Optional[str] = None,
         auto_stop: Optional[int] = None,
         auto_pause: Optional[int] = None,
+        auto_upgrade: Optional[bool] = None,
         workers_quantity: Optional[int] = None,
         instance_role: Optional[Union[IInstanceRole, Dict]] = None,
         instance_type: Optional[str] = None,
         bodo_version: Optional[str] = None,
         auto_az: Optional[bool] = None,
         availability_zone: Optional[str] = None,
         custom_tags: Optional[Dict] = None,
@@ -1037,14 +1061,15 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> "IJobRun":
         raise NotImplementedError
 
     @abstractmethod
     def run_sql_query(
         self,
         template_id: str = None,
@@ -1053,14 +1078,15 @@
         cluster: Union[dict, ICluster] = None,
         name: str = None,
         args: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
+        store_result: bool = False,
     ) -> "IJobRun":
         raise NotImplementedError
 
     @abstractmethod
     def get(self, id: str) -> "IJobRun":
         raise NotImplementedError
 
@@ -1078,15 +1104,15 @@
 
     @abstractmethod
     def cancel_jobs(self, filters: Optional[Union[Dict, IJobFilter]] = None) -> IJobRun:
         raise NotImplementedError
 
     @abstractmethod
     def wait_for_status(
-        self, id: str, statuses: List, timeout: int = 3600, tick: int = 30
+        self, id: str, statuses: List[str], timeout: int = 3600, tick: int = 30
     ) -> abstractmethod:
         raise NotImplementedError
 
 
 class IJobTemplateClient(ABC):
     _workspace_client: IBodoWorkspaceClient
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/__init__.py` & `bodosdk-2.0.1rc1/bodosdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/catalog.py` & `bodosdk-2.0.1rc1/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/cloud_config.py` & `bodosdk-2.0.1rc1/bodosdk/models/cloud_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 class AwsProviderData(SDKBaseModel, IAwsProviderData):
     role_arn: Optional[str] = Field(None, alias="roleArn")
     tf_bucket_name: Optional[str] = Field(None, alias="tfBucketName")
     tf_dynamo_db_table_name: Optional[str] = Field(None, alias="tfDynamoDbTableName")
     tf_backend_region: Optional[str] = Field(None, alias="tfBackendRegion")
     external_id: Optional[str] = Field(None, alias="externalId")
     account_id: Optional[str] = Field(None, alias="accountId")
+    access_key_id: Optional[str] = Field(None, alias="accessKeyId")
+    secret_access_key: Optional[str] = Field(None, alias="secretAccessKey")
 
 
 class CloudConfigBase(SDKBaseModel, ICloudConfig):
     cloud_provider: Optional[str] = Field(None, alias="cloudProvider")
     name: Optional[str]
     status: Optional[str]
     organization_uuid: Optional[str] = Field(None, alias="organizationUUID")
@@ -111,14 +113,15 @@
             except ValidationError as e:
                 raise ValueError(f"Invalid data for data: {e}")
         else:
             super().__setattr__(key, value)
 
 
 class AzureCloudConfig(CloudConfigBase, IAzureCloudConfig):
+    cloud_provider: str = Field("AZURE", alias="cloudProvider", const=True)
     data: Optional[AzureProviderData] = Field(None, alias="azureProviderData")
 
     def __call__(self, **data) -> CloudConfigBase:
         return AzureCloudConfig(self._org_client, **data)
 
     def __setattr__(self, key: str, value: Any):
         if key == "data" and isinstance(value, dict):
@@ -127,14 +130,15 @@
             except ValidationError as e:
                 raise ValueError(f"Invalid data for data: {e}")
         else:
             super().__setattr__(key, value)
 
 
 class AwsCloudConfig(CloudConfigBase, IAwsCloudConfig):
+    cloud_provider: str = Field("AWS", alias="cloudProvider", const=True)
     data: Optional[AwsProviderData] = Field(None, alias="awsProviderData")
 
     def __call__(self, **data) -> CloudConfigBase:
         return AwsCloudConfig(self._org_client, **data)
 
     def __setattr__(self, key: str, value: Any):
         if key == "data" and isinstance(value, dict):
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/cluster.py` & `bodosdk-2.0.1rc1/bodosdk/models/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         description (Optional[str]): A description of the cluster.
         instance_type (Optional[str]): The type of instances used in the cluster (e.g., 'c5.large').
         workers_quantity (Optional[int]): The number of worker nodes in the cluster.
         auto_stop (Optional[int]): The auto-stop configuration in minutes.
             The cluster automatically stops when idle for this duration.
         auto_pause (Optional[int]): The auto-pause configuration in minutes.
             The cluster automatically pauses when idle for this duration.
+        auto_upgrade (Optional[bool]): Should the cluster be upgraded on restart.
+            The cluster is automatically upgraded to the latest Bodo version on restart when True.
         bodo_version (Optional[str]): The version of Bodo being used in the cluster.
-        image_id (Optional[str]): The ID of the image used for the cluster's instances.
         cores_per_worker (Optional[int]): The number of CPU cores per worker node.
         accelerated_networking (Optional[bool]): Whether accelerated networking is enabled.
         created_at (Optional[str]): The creation timestamp of the cluster.
         updated_at (Optional[str]): The last update timestamp of the cluster.
         is_job_dedicated (Optional[bool]): Whether the cluster is dedicated to a specific job.
         auto_az (Optional[bool]): Whether automatic availability zone selection is enabled.
         use_spot_instance (Optional[bool]): Whether spot instances are used for the cluster.
@@ -79,16 +80,16 @@
     uuid: Optional[str] = Field(None, alias="uuid")
     status: Optional[str] = Field(None, alias="status")
     description: Optional[str] = Field(None, alias="description")
     instance_type: Optional[str] = Field(None, alias="instanceType")
     workers_quantity: Optional[int] = Field(None, alias="workersQuantity")
     auto_stop: Optional[int] = Field(None, alias="autoStop")
     auto_pause: Optional[int] = Field(None, alias="autoPause")
+    auto_upgrade: Optional[bool] = Field(None, alias="autoUpgrade")
     bodo_version: Optional[str] = Field(None, alias="bodoVersion")
-    image_id: Optional[str] = Field(None, alias="imageId")
     cores_per_worker: Optional[int] = Field(None, alias="coresPerWorker")
     accelerated_networking: Optional[bool] = Field(None, alias="acceleratedNetworking")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
     is_job_dedicated: Optional[bool] = Field(None, alias="isJobDedicated")
     auto_az: Optional[bool] = Field(None, alias="autoAZ")
     use_spot_instance: Optional[bool] = Field(None, alias="useSpotInstance")
@@ -102,15 +103,15 @@
     node_metadata: Optional[List[NodeMetadata]] = Field(None, alias="nodeMetadata")
     availability_zone: Optional[str] = Field(None, alias="availabilityZone")
     instance_role: Optional[InstanceRole] = Field(None, alias="instanceRole")
     workspace: Optional[dict] = Field(None, alias="workspace")
     autoscaling_identifier: Optional[str] = Field(None, alias="autoscalingIdentifier")
     last_asg_activity_id: Optional[str] = Field(None, alias="lastAsgActivityId")
     nodes_ip: Optional[List[str]] = Field(None, alias="nodesIp")
-    custom_tags: Optional[Dict] = Field(default_factory=dict, alias="customTags")
+    custom_tags: Optional[Dict] = Field(None, alias="customTags")
 
     def __setattr__(self, key: str, value: Any):
         """
         Sets the value of an attribute using custom logic for 'node_metadata' and 'instance_role',
         ensuring they are correctly instantiated.
 
         Args:
@@ -153,15 +154,15 @@
         Args:
             **data: Arbitrary keyword arguments representing cluster properties.
 
         Returns:
             A new instance of Cluster.
         """
         c = Cluster(self._workspace_client, **data)
-        if not c.bodo_version and not c.image_id:
+        if not c.bodo_version:
             c._update(
                 {
                     "bodo_version": self._workspace_client.ClusterClient.latest_bodo_version
                 }
             )
         if c.instance_role:
             c.instance_role._workspace_client = self._workspace_client
@@ -263,14 +264,15 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = False,
     ) -> IJobRun:
         """
         Submits a batch job for execution using specified configurations and resources.
 
         This method creates and dispatches a job within a computing cluster, allowing for extensive customization of
         execution parameters including source data, runtime environment, and failure handling strategies.
 
@@ -286,14 +288,15 @@
             env_vars (dict, optional): Environment variables to set for the job.
             timeout (int, optional): Maximum runtime (in seconds) before the job is terminated.
             num_retries (int, optional): Number of times to retry the job on failure.
             delay_between_retries (int, optional): Time to wait between retries.
             retry_on_timeout (bool, optional): Whether to retry the job if it times out.
             name (str, optional): Name of the job.
             catalog (str, optional): Catalog to log the job under.
+            store_result (bool, optional): Whether to store on S3 job results or not.
 
         Returns:
             IJobRun: An object representing the submitted job, capable of providing status and results.
 
         """
         return self._workspace_client.JobClient.run(
             cluster=self,
@@ -305,28 +308,30 @@
             env_vars=env_vars,
             timeout=timeout,
             num_retries=num_retries,
             delay_between_retries=delay_between_retries,
             retry_on_timeout=retry_on_timeout,
             name=name,
             catalog=catalog,
+            store_result=store_result,
         )
 
     @check_deprecation
     def run_sql_query(
         self,
         template_id: str = None,
         catalog: str = None,
         sql_query: str = None,
         name: str = None,
         args: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
+        store_result: bool = False,
     ) -> IJobRun:
         """
                 Submits an SQL query for execution on the cluster, returning a job run object.
 
                 This method handles the execution of an SQL query within a defined cluster environment.
                 It supports customization of execution parameters such as query arguments,
                 job name, execution timeouts, and retry strategies.
@@ -337,14 +342,15 @@
                     sql_query (str, optional): The SQL query string to be executed.
                     name (str, optional): Descriptive name for the SQL job.
                     args (dict, optional): Dictionary of arguments that are passed to the SQL query.
                     timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
                     num_retries (int, optional): Number of times the job will be retried on failure.
                     delay_between_retries (int, optional): Interval in seconds between job retries.
                     retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+                    store_result (bool, optional): Whether to store on S3 job results or not.
 
                 Returns:
                     IJobRun: An object representing the status and result of the executed SQL job.
         `
         """
         return self._workspace_client.JobClient.run_sql_query(
             cluster=self,
@@ -353,14 +359,15 @@
             sql_query=sql_query,
             name=name,
             args=args,
             timeout=timeout,
             num_retries=num_retries,
             delay_between_retries=delay_between_retries,
             retry_on_timeout=retry_on_timeout,
+            store_result=store_result,
         )
 
     @check_deprecation
     def cancel_jobs(self) -> Cluster:
         """
         Cancels all jobs associated with the cluster.
 
@@ -547,14 +554,15 @@
         return self
 
     @check_deprecation
     def update(
         self,
         auto_stop: Optional[int] = None,
         auto_pause: Optional[int] = None,
+        auto_upgrade: Optional[bool] = None,
         description: Optional[str] = None,
         name: Optional[str] = None,
         workers_quantity: Optional[int] = None,
         instance_role: Optional[InstanceRole] = None,
         instance_type: Optional[str] = None,
         bodo_version: Optional[str] = None,
         auto_az: Optional[bool] = None,
@@ -563,14 +571,15 @@
     ) -> Cluster:
         """
         Updates the cluster's configuration with the provided values.
 
         Args:
             auto_stop: Optional; configures auto-stop feature.
             auto_pause: Optional; configures auto-pause feature.
+            auto_upgrade: Optional; enables/disables auto-upgrade on restart.
             description: Optional; updates the cluster's description.
             name: Optional; updates the cluster's name.
             workers_quantity: Optional; updates the number of workers.
             instance_role: Optional; updates the instance role.
             instance_type: Optional; updates the instance type.
             bodo_version: Optional; updates the Bodo version.
             auto_az: Optional; enables/disables automatic availability zone selection.
@@ -964,14 +973,15 @@
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         name: str = None,
         catalog: str = None,
+        store_result: bool = None,
     ) -> IJobRunList:
         """
         Executes a job across all clusters managed by the instance.
 
         This method supports multiple source types and configurations for executing jobs,
         including retries and custom environment variables.
 
@@ -986,14 +996,15 @@
             env_vars (dict, optional): Environment variables to set for the job execution.
             timeout (int, optional): Maximum time in seconds for the job to run before it is terminated.
             num_retries (int, optional): Number of times to retry the job on failure.
             delay_between_retries (int, optional): Time in seconds to wait between retries.
             retry_on_timeout (bool, optional): Whether to retry the job if it times out.
             name (str, optional): A name for the job run.
             catalog (str, optional): Catalog identifier to specify a data catalog for the job.
+            store_result (bool, optional): Whether to store on S3 job results or not.
 
         Returns:
             IJobRunList: An object listing the UUIDs of jobs that were successfully initiated.
 
         Decorators:
             @check_deprecation: Checks if the method or its parameters are deprecated.
 
@@ -1009,14 +1020,15 @@
                 env_vars=env_vars,
                 timeout=timeout,
                 num_retries=num_retries,
                 delay_between_retries=delay_between_retries,
                 retry_on_timeout=retry_on_timeout,
                 name=name,
                 catalog=catalog,
+                store_result=store_result,
             )
             job_uuids.append(job.uuid)
         return self._workspace_client.JobClient.JobRunList(filters={"ids": job_uuids})
 
     @check_deprecation
     def run_sql_query(
         self,
@@ -1025,14 +1037,15 @@
         sql_query: str = None,
         name: str = None,
         args: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
+        store_result: bool = None,
     ) -> IJobRunList:
         """
         Executes an SQL job across all clusters managed by the instance.
 
         This method submits an SQL query for execution, allowing for additional configurations such as retries
         and setting execution timeouts.
 
@@ -1042,14 +1055,15 @@
             sql_query (str, optional): The SQL query to execute.
             name (str, optional): A name for the job run.
             args (dict, optional): Additional arguments specific to the SQL job.
             timeout (int, optional): Maximum time in seconds for the job to run before it is terminated.
             num_retries (int, optional): Number of times to retry the job on failure.
             delay_between_retries (int, optional): Time in seconds to wait between retries.
             retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+            store_result (bool, optional): Whether to store on S3 job results or not.
 
         Returns:
             IJobRunList: An object listing the UUIDs of SQL jobs that were successfully initiated.
 
         Decorators:
             @check_deprecation: Checks if the method or its parameters are deprecated.
 
@@ -1062,14 +1076,15 @@
                 sql_query=sql_query,
                 name=name,
                 args=args,
                 timeout=timeout,
                 num_retries=num_retries,
                 delay_between_retries=delay_between_retries,
                 retry_on_timeout=retry_on_timeout,
+                store_result=store_result,
             )
             job_uuids.append(job.uuid)
         return self._workspace_client.JobClient.JobRunList(filters={"ids": job_uuids})
 
     @check_deprecation
     def cancel_jobs(self) -> ClusterList:
         """
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/common.py` & `bodosdk-2.0.1rc1/bodosdk/models/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,16 @@
 
 class AWSNetworkData(NetworkData):
     """
     Extends the NetworkData class to include specific properties for AWS networking.
 
     Attributes:
         vpc_id (Optional[str]): The ID of the AWS Virtual Private Cloud (VPC) where workspace should be created.
-        fetched_vpc_id (Optional[str]): The ID of the fetched AWS VPC - if no vpc_id provided.
         public_subnets_ids (Optional[List[str]]): List of IDs for the public subnets within the AWS VPC.
         private_subnets_ids (Optional[List[str]]): List of IDs for the private subnets within the AWS VPC.
         policies_arn (Optional[List[str]]): List of AWS Resource Names (ARNs) for the policies applied to the network.
     """
 
     vpc_id: Optional[str] = Field(None, alias="vpcId")
-    fetched_vpc_id: Optional[str] = Field(None, alias="fetchedVpcId")
     public_subnets_ids: Optional[List[str]] = Field(None, alias="publicSubnetsIds")
     private_subnets_ids: Optional[List[str]] = Field(None, alias="privateSubnetsIds")
     policies_arn: Optional[List[str]] = Field(None, alias="policyArns")
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/instance_role.py` & `bodosdk-2.0.1rc1/bodosdk/models/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/job.py` & `bodosdk-2.0.1rc1/bodosdk/models/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     exec_text: Optional[str] = Field(None, alias="sqlQueryText")
     sql_query_parameters: Optional[dict] = Field(None, alias="sqlQueryParameters")
     args: Optional[Union[dict, str]]
     retry_strategy: Optional[RetryStrategy] = Field(None, alias="retryStrategy")
     timeout: Optional[int]
     env_vars: Optional[dict] = Field(None, alias="envVars")
     catalog: Optional[str]
+    store_result: Optional[bool] = Field(False, alias="storeResult")
 
 
 class JobRun(SDKBaseModel, IJobRun):
     """
     Details a specific instance of a job run, including status and configuration details.
 
     Attributes:
@@ -362,14 +363,20 @@
         logs = self.get_logs_urls()
         if logs and logs.stdout_location_url:
             response = requests.get(logs.stderr_location_url)
             if response.status_code == 200:
                 return response.text
         return ""
 
+    @check_deprecation
+    def get_result_urls(self) -> list:
+        if self.id and self.status in ("FAILED", "CANCELLED", "SUCCEEDED"):
+            resp = self._workspace_client._job_api.get_result_links(self.id)
+            return resp
+
 
 class JobRunLogsResponse(SDKBaseModel, IJobRunLogsResponse):
     """
     Represents the response object containing URLs for accessing logs related to a job run.
 
     Attributes:
         stderr_location_url (str): The URL to access the standard error logs of the job run.
@@ -776,14 +783,24 @@
     def __init__(self, workspace_client: IBodoWorkspaceClient = None, **data):
         super().__init__(**data)
         self._workspace_client = workspace_client
 
     def __call__(self, **data) -> JobTemplate:
         return JobTemplate(self._workspace_client, **data)
 
+    def __setattr__(self, key: str, value: Any):
+        if key == "config" and isinstance(value, dict):
+            processed_value = JobConfig(**value)
+            super().__setattr__(key, processed_value)
+        elif key == "cluster_config" and isinstance(value, dict):
+            processed_value = self._workspace_client.ClusterClient.Cluster(**value)
+            super().__setattr__(key, processed_value)
+        else:
+            super().__setattr__(key, value)
+
     @check_deprecation
     def run(
         self,
         name: str = None,
         cluster: Union[dict, ICluster] = None,
         code_type: str = None,
         source: Union[
@@ -794,14 +811,15 @@
         args: Union[dict, str] = None,
         env_vars: dict = None,
         timeout: int = None,
         num_retries: int = None,
         delay_between_retries: int = None,
         retry_on_timeout: bool = None,
         catalog: str = None,
+        store_result: bool = False,
     ):
         return self._workspace_client.JobClient.run(
             template_id=self.uuid,
             cluster=cluster,
             name=name,
             code_type=code_type,
             source=source,
@@ -810,14 +828,17 @@
             args=args,
             env_vars=env_vars,
             timeout=timeout,
             num_retries=num_retries,
             delay_between_retries=delay_between_retries,
             retry_on_timeout=retry_on_timeout,
             catalog=catalog,
+            store_result=store_result
+            if store_result is not None
+            else self.config.type == "SQL",
         )
 
     @check_deprecation
     def delete(self):
         self._workspace_client._job_tpl_api.delete_job_tpl(self.uuid)
 
     @check_deprecation
```

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/secret.py` & `bodosdk-2.0.1rc1/bodosdk/models/secret.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/bodosdk/models/workspace.py` & `bodosdk-2.0.1rc1/bodosdk/models/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from bodosdk.exceptions import TimeoutException, ResourceNotFound, ValidationError
 from bodosdk.interfaces import (
     IWorkspace,
     IWorkspaceList,
     IWorkspaceFilter,
     IBodoOrganizationClient,
 )
-from bodosdk.models import AwsCloudConfig, AzureCloudConfig
+from bodosdk.models import AwsCloudConfig, AzureCloudConfig, CloudConfigBase
 from bodosdk.models.common import NetworkData, AWSNetworkData
 
 
 class Workspace(SDKBaseModel, IWorkspace):
     name: Optional[str]
     uuid: Optional[Union[str, UUID]]
     status: Optional[str]
@@ -39,17 +39,17 @@
     )
     assigned_at: Optional[datetime] = Field(None, alias="assignedAt")
     custom_tags: Optional[Dict[str, Any]] = Field(
         default_factory=dict, alias="customTags"
     )
     jupyter_last_activity: Optional[datetime] = Field(None, alias="jupyterLastActivity")
     jupyter_is_active: Optional[bool] = Field(False, alias="jupyterIsActive")
-    cloud_config: Optional[Union[AwsCloudConfig, AzureCloudConfig]] = Field(
-        None, alias="cloudConfig"
-    )
+    cloud_config: Optional[
+        Union[CloudConfigBase, AwsCloudConfig, AzureCloudConfig]
+    ] = Field(None, alias="cloudConfig")
 
     @property
     def id(self):
         return self.uuid
 
     def __init__(self, org_client: IBodoOrganizationClient = None, **data):
         """
@@ -175,16 +175,24 @@
                 self._mutable = False
                 return self
             raise
         start_time = time.time()  # Record the start time
         while self.status not in statuses:
             current_time = time.time()
             elapsed_time = current_time - start_time
-            self._load()
-
+            try:
+                self._load()
+            except ResourceNotFound:
+                if "TERMINATED" in statuses:
+                    self._mutable = True
+                    self.status = "TERMINATED"
+                    self._mutable = False
+                    return self
+                else:
+                    raise
             # Check if timeout is reached
             if elapsed_time > timeout:
                 raise TimeoutException(
                     f"workspace {self.uuid} wait for states {statuses} timeout! Current state: {self.status}"
                 )
             time.sleep(tick)
         return self
```

### Comparing `bodosdk-2.0.0rc2/bodosdk.egg-info/PKG-INFO` & `bodosdk-2.0.1rc1/bodosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 2.0.0rc2
-Summary: Bodo Platform SDK 2.0.0RC2
+Version: 2.0.1rc1
+Summary: Bodo Platform SDK 2.0.1.RC1
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,14 +17,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic~=1.9
 Requires-Dist: requests~=2.27.1
 Requires-Dist: pyjwt~=2.3.0
 Requires-Dist: typing_extensions>=4
 Requires-Dist: callee~=0.3.1
+Requires-Dist: pandas
+Requires-Dist: pyarrow
 
 # Bodo Platform SDK
 
 Bodo Platform SDK is a Python library that provides a simple way to interact with the Bodo Platform API. It allows you
 to create, manage, and monitor resources such as clusters, jobs, and workspaces.
 
 ## Getting Started
@@ -640,27 +642,29 @@
 * **Returns:**
   An instance of ClusterListAPIModel for listing clusters.
 * **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
 #### connect(catalog: str, cluster_id: str)
 
-#### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str = None, auto_stop: int | None = None, auto_pause: int | None = None, image_id: str | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
+#### create(name: str, instance_type: str = None, workers_quantity: int = None, description: str | None = None, bodo_version: str | None = None, auto_stop: int | None = None, auto_pause: int | None = None, auto_upgrade: bool | None = None, accelerated_networking: bool | None = None, auto_az: bool | None = None, use_spot_instance: bool | None = None, aws_deployment_subnet_id: str | None = None, availability_zone: str | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | Dict | None = None, custom_tags: Dict | None = None)
 
 Creates a new cluster with the specified configuration.
 
 * **Parameters:**
   * **name** (*str*) – The name of the cluster.
   * **instance_type** (*str* *,* *optional*) – The type of instance to use for the cluster nodes.
   * **workers_quantity** (*int* *,* *optional*) – The number of worker nodes in the cluster.
   * **description** (*str* *,* *optional*) – A description of the cluster.
   * **bodo_version** (*str* *,* *optional*) – The Bodo version to use for the cluster.
+    If not provided, the latest version is used.
   * **auto_stop** (*int* *,* *optional*) – The auto-stop time in minutes for the cluster.
   * **auto_pause** (*int* *,* *optional*) – The auto-pause time in minutes for the cluster.
-  * **image_id** (*str* *,* *optional*) – The ID of the image to use for the cluster.
+  * **auto_upgrade** (*bool* *,* *optional*) – Should the cluster be automatically upgraded to
+    the latest Bodo version on restart.
   * **accelerated_networking** (*bool* *,* *optional*) – Whether to use accelerated networking.
   * **auto_az** (*bool* *,* *optional*) – Whether to automatically select the availability zone.
   * **use_spot_instance** (*bool* *,* *optional*) – Whether to use spot instances for the cluster.
   * **aws_deployment_subnet_id** (*str* *,* *optional*) – The AWS deployment subnet ID.
   * **availability_zone** (*str* *,* *optional*) – The availability zone for the cluster.
   * **instance_role** ([*InstanceRole*](#bodosdk.models.instance_role.InstanceRole) *|* *Dict* *,* *optional*) – The instance role or a custom role configuration.
   * **custom_tags** (*Dict* *,* *optional*) – Custom tags to assign to the cluster resources.
@@ -859,31 +863,31 @@
 
 #### cancel_jobs(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None)
 
 #### get(id: str)
 
 #### list(filters: Dict | [JobFilter](#bodosdk.models.job.JobFilter) | None = None, order: Dict | None = None)
 
-#### run(template_id: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run(template_id: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = None)
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, cluster: dict | ICluster = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = True)
 
 #### wait_for_status(id: str, statuses: List[str], timeout: int = 3600, tick: int = 30)
 
 <a id="module-bodosdk.clients.job_tpl"></a>
 
 ### *class* bodosdk.clients.job_tpl.JobTemplateClient(workspace_client: IBodoWorkspaceClient)
 
 Bases: `IJobTemplateClient`
 
 #### *property* JobTemplate *: [JobTemplate](#bodosdk.models.job.JobTemplate)*
 
 #### *property* JobTemplateList *: [JobTemplateList](#bodosdk.models.job.JobTemplateList)*
 
-#### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
+#### create(name: str = None, description: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None, store_result: bool = False)
 
 #### get(id: str)
 
 #### list(filters: Dict = None)
 
 #### remove(id: str)
 
@@ -901,14 +905,18 @@
 
 #### *property* CloudConfigList *: [CloudConfigList](#bodosdk.models.cloud_config.CloudConfigList)*
 
 #### *property* Workspace *: [Workspace](#bodosdk.models.workspace.Workspace)*
 
 #### *property* WorkspaceList *: [WorkspaceList](#bodosdk.models.workspace.WorkspaceList)*
 
+#### create_aws_cloud_config(name: str, tf_backend_region: str, role_arn: str | None = None, tf_bucket_name: str | None = None, tf_dynamo_db_table_name: str | None = None, account_id: str | None = None, access_key_id: str | None = None, secret_access_key: str | None = None, custom_tags: dict | None = None)
+
+#### create_azure_cloud_config(name: str, tf_backend_region: str, tenant_id: str, subscription_id: str, resource_group: str, custom_tags: dict | None = None)
+
 #### create_workspace(name: str, region: str, storage_endpoint_enabled: bool, cloud_config_id: str = None, vpc_id: str | None = None, public_subnets_ids: List[str] | None = None, private_subnets_ids: List[str] | None = None, custom_tags: dict | None = None)
 
 #### delete_workspace(id)
 
 #### get_cloud_config(id)
 
 #### get_workspace(id)
@@ -994,40 +1002,48 @@
 
 #### username *: str | None*
 
 #### warehouse *: str | None*
 
 <a id="module-bodosdk.models.cloud_config"></a>
 
-### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AwsCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str = 'AWS', name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, awsProviderData: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAwsCloudConfig`
 
+#### cloud_provider *: str*
+
 #### data *: [AwsProviderData](#bodosdk.models.cloud_config.AwsProviderData) | None*
 
-### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None)
+### *class* bodosdk.models.cloud_config.AwsProviderData(\*, roleArn: str | None = None, tfBucketName: str | None = None, tfDynamoDbTableName: str | None = None, tfBackendRegion: str | None = None, externalId: str | None = None, accountId: str | None = None, accessKeyId: str | None = None, secretAccessKey: str | None = None)
 
 Bases: `SDKBaseModel`, `IAwsProviderData`
 
+#### access_key_id *: str | None*
+
 #### account_id *: str | None*
 
 #### external_id *: str | None*
 
 #### role_arn *: str | None*
 
+#### secret_access_key *: str | None*
+
 #### tf_backend_region *: str | None*
 
 #### tf_bucket_name *: str | None*
 
 #### tf_dynamo_db_table_name *: str | None*
 
-### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str | None = None, name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
+### *class* bodosdk.models.cloud_config.AzureCloudConfig(org_client: IBodoOrganizationClient = None, \*, cloudProvider: str = 'AZURE', name: str | None = None, status: str | None = None, organizationUUID: str | None = None, customTags: dict | None = None, uuid: str | UUID | None = None, azureProviderData: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None = None)
 
 Bases: [`CloudConfigBase`](#bodosdk.models.cloud_config.CloudConfigBase), `IAzureCloudConfig`
 
+#### cloud_provider *: str*
+
 #### data *: [AzureProviderData](#bodosdk.models.cloud_config.AzureProviderData) | None*
 
 ### *class* bodosdk.models.cloud_config.AzureProviderData(\*, tfBackendRegion: str | None = None, resourceGroup: str | None = None, subscriptionId: str | None = None, tenantId: str | None = None, tfStorageAccountName: str | None = None, applicationId: str | None = None)
 
 Bases: `SDKBaseModel`, `IAzureProviderData`
 
 #### application_id *: str | None*
@@ -1115,15 +1131,15 @@
 * **Type:**
   str
 
 #### bodo_version *: str*
 
 #### image_id *: str*
 
-### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, bodoVersion: str | None = None, imageId: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
+### *class* bodosdk.models.cluster.Cluster(workspace_client: IBodoWorkspaceClient = None, \*, name: str | None = None, uuid: str | None = None, status: str | None = None, description: str | None = None, instanceType: str | None = None, workersQuantity: int | None = None, autoStop: int | None = None, autoPause: int | None = None, autoUpgrade: bool | None = None, bodoVersion: str | None = None, coresPerWorker: int | None = None, acceleratedNetworking: bool | None = None, createdAt: datetime | None = None, updatedAt: datetime | None = None, isJobDedicated: bool | None = None, autoAZ: bool | None = None, useSpotInstance: bool | None = None, lastKnownActivity: datetime | None = None, inStateSince: datetime | None = None, clusterAgentVersion: str | None = None, clusterInitStatus: str | None = None, clusterHealthStatus: str | None = None, primaryAgentIP: str | None = None, awsDeploymentSubnetId: str | None = None, nodeMetadata: List[[NodeMetadata](#bodosdk.models.cluster.NodeMetadata)] | None = None, availabilityZone: str | None = None, instanceRole: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, workspace: dict | None = None, autoscalingIdentifier: str | None = None, lastAsgActivityId: str | None = None, nodesIp: List[str] | None = None, customTags: Dict | None = None)
 
 Bases: `SDKBaseModel`, `ICluster`
 
 Represents a cluster in the SDK model, encapsulating various properties and operations
 related to a compute cluster.
 
 #### name
@@ -1180,24 +1196,25 @@
 
 The auto-pause configuration in minutes.
 The cluster automatically pauses when idle for this duration.
 
 * **Type:**
   Optional[int]
 
-#### bodo_version
+#### auto_upgrade
 
-The version of Bodo being used in the cluster.
+Should the cluster be upgraded on restart.
+The cluster is automatically upgraded to the latest Bodo version on restart when True.
 
 * **Type:**
-  Optional[str]
+  Optional[bool]
 
-#### image_id
+#### bodo_version
 
-The ID of the image used for the cluster’s instances.
+The version of Bodo being used in the cluster.
 
 * **Type:**
   Optional[str]
 
 #### cores_per_worker
 
 The number of CPU cores per worker node.
@@ -1349,14 +1366,16 @@
 
 #### auto_az *: bool | None*
 
 #### auto_pause *: int | None*
 
 #### auto_stop *: int | None*
 
+#### auto_upgrade *: bool | None*
+
 #### autoscaling_identifier *: str | None*
 
 #### availability_zone *: str | None*
 
 #### aws_deployment_subnet_id *: str | None*
 
 #### bodo_version *: str | None*
@@ -1411,16 +1430,14 @@
 #### *property* id *: str*
 
 The UUID of the cluster.
 
 * **Returns:**
   The UUID string of the cluster.
 
-#### image_id *: str | None*
-
 #### in_state_since *: datetime | None*
 
 #### instance_role *: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None*
 
 #### instance_type *: str | None*
 
 #### is_job_dedicated *: bool | None*
@@ -1455,15 +1472,15 @@
 * **Parameters:**
   **wait** – If True, waits till cluster will be RUNNING.
 * **Returns:**
   The Cluster instance with updated status.
 * **Raises:**
   **ConflictException** – If the cluster cannot be resumed due to its current status.
 
-#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = False)
 
 Submits a batch job for execution using specified configurations and resources.
 
 This method creates and dispatches a job within a computing cluster, allowing for extensive customization of
 execution parameters including source data, runtime environment, and failure handling strategies.
 
 * **Parameters:**
@@ -1477,20 +1494,21 @@
   * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job.
   * **timeout** (*int* *,* *optional*) – Maximum runtime (in seconds) before the job is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
   * **name** (*str* *,* *optional*) – Name of the job.
   * **catalog** (*str* *,* *optional*) – Catalog to log the job under.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object representing the submitted job, capable of providing status and results.
 * **Return type:**
   IJobRun
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = False)
 
 > Submits an SQL query for execution on the cluster, returning a job run object.
 
 > This method handles the execution of an SQL query within a defined cluster environment.
 > It supports customization of execution parameters such as query arguments,
 > job name, execution timeouts, and retry strategies.
 
@@ -1500,14 +1518,15 @@
 >   sql_query (str, optional): The SQL query string to be executed.
 >   name (str, optional): Descriptive name for the SQL job.
 >   args (dict, optional): Dictionary of arguments that are passed to the SQL query.
 >   timeout (int, optional): Maximum allowable runtime in seconds before the job is terminated.
 >   num_retries (int, optional): Number of times the job will be retried on failure.
 >   delay_between_retries (int, optional): Interval in seconds between job retries.
 >   retry_on_timeout (bool, optional): Whether to retry the job if it times out.
+>   store_result (bool, optional): Whether to store on S3 job results or not.
 
 > Returns:
 > : IJobRun: An object representing the status and result of the executed SQL job.
 
 ```
 `
 ```
@@ -1528,21 +1547,22 @@
 Stops the cluster.
 
 * **Parameters:**
   **wait** – If True, waits till cluster will be STOPPED.
 * **Returns:**
   The Cluster instance with updated status.
 
-#### update(auto_stop: int | None = None, auto_pause: int | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
+#### update(auto_stop: int | None = None, auto_pause: int | None = None, auto_upgrade: bool | None = None, description: str | None = None, name: str | None = None, workers_quantity: int | None = None, instance_role: [InstanceRole](#bodosdk.models.instance_role.InstanceRole) | None = None, instance_type: str | None = None, bodo_version: str | None = None, auto_az: bool | None = None, availability_zone: str | None = None, custom_tags: Dict | None = None)
 
 Updates the cluster’s configuration with the provided values.
 
 * **Parameters:**
   * **auto_stop** – Optional; configures auto-stop feature.
   * **auto_pause** – Optional; configures auto-pause feature.
+  * **auto_upgrade** – Optional; enables/disables auto-upgrade on restart.
   * **description** – Optional; updates the cluster’s description.
   * **name** – Optional; updates the cluster’s name.
   * **workers_quantity** – Optional; updates the number of workers.
   * **instance_role** – Optional; updates the instance role.
   * **instance_type** – Optional; updates the instance type.
   * **bodo_version** – Optional; updates the Bodo version.
   * **auto_az** – Optional; enables/disables automatic availability zone selection.
@@ -1758,15 +1778,15 @@
 
 * **Returns:**
   The current instance of ClusterList after attempting to resume
   : all clusters.
 * **Return type:**
   [ClusterList](#bodosdk.models.cluster.ClusterList)
 
-#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None)
+#### run_job(template_id: str = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, name: str = None, catalog: str = None, store_result: bool = None)
 
 Executes a job across all clusters managed by the instance.
 
 This method supports multiple source types and configurations for executing jobs,
 including retries and custom environment variables.
 
 * **Parameters:**
@@ -1780,23 +1800,24 @@
   * **env_vars** (*dict* *,* *optional*) – Environment variables to set for the job execution.
   * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
   * **name** (*str* *,* *optional*) – A name for the job run.
   * **catalog** (*str* *,* *optional*) – Catalog identifier to specify a data catalog for the job.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object listing the UUIDs of jobs that were successfully initiated.
 * **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
 
-#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None)
+#### run_sql_query(template_id: str = None, catalog: str = None, sql_query: str = None, name: str = None, args: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, store_result: bool = None)
 
 Executes an SQL job across all clusters managed by the instance.
 
 This method submits an SQL query for execution, allowing for additional configurations such as retries
 and setting execution timeouts.
 
 * **Parameters:**
@@ -1805,14 +1826,15 @@
   * **sql_query** (*str* *,* *optional*) – The SQL query to execute.
   * **name** (*str* *,* *optional*) – A name for the job run.
   * **args** (*dict* *,* *optional*) – Additional arguments specific to the SQL job.
   * **timeout** (*int* *,* *optional*) – Maximum time in seconds for the job to run before it is terminated.
   * **num_retries** (*int* *,* *optional*) – Number of times to retry the job on failure.
   * **delay_between_retries** (*int* *,* *optional*) – Time in seconds to wait between retries.
   * **retry_on_timeout** (*bool* *,* *optional*) – Whether to retry the job if it times out.
+  * **store_result** (*bool* *,* *optional*) – Whether to store on S3 job results or not.
 * **Returns:**
   An object listing the UUIDs of SQL jobs that were successfully initiated.
 * **Return type:**
   IJobRunList
 
 Decorators:
 : @check_deprecation: Checks if the method or its parameters are deprecated.
@@ -1935,31 +1957,31 @@
 
 ### *class* bodosdk.db.connection.Connection(catalog: str, cluster: ICluster, timeout=3600)
 
 Bases: `object`
 
 #### cursor()
 
-### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int)
+### *class* bodosdk.db.connection.Cursor(catalog: str, cluster: ICluster, timeout: int = 3600)
 
 Bases: `object`
 
 #### execute(query: str, \*\*kwargs)
 
 #### execute_async(query: str, \*\*kwargs)
 
 #### fetchall()
 
 #### fetchmany(size)
 
 #### fetchone()
 
-### *exception* bodosdk.db.connection.QueryError
+#### *property* rowcount
 
-Bases: `Exception`
+#### *property* rownumber
 
 <a id="module-bodosdk.models.job"></a>
 
 ### *class* bodosdk.models.job.GitRepoSource(\*, type: str = 'GIT', repoUrl: str, reference: str | None = '', username: str, token: str)
 
 Bases: `SDKBaseModel`
 
@@ -2001,15 +2023,15 @@
 
 #### token *: str*
 
 #### type *: str*
 
 #### username *: str*
 
-### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None)
+### *class* bodosdk.models.job.JobConfig(\*, type: str | None = None, source: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None = None, sourceLocation: str | None = None, sqlQueryText: str | None = None, sqlQueryParameters: dict | None = None, args: dict | str | None = None, retryStrategy: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None = None, timeout: int | None = None, envVars: dict | None = None, catalog: str | None = None, storeResult: bool | None = False)
 
 Bases: `SDKBaseModel`, `IJobConfig`
 
 Configures details for executing a job, including the execution source, file location, and execution parameters.
 
 #### type
 
@@ -2095,14 +2117,16 @@
 
 #### retry_strategy *: [RetryStrategy](#bodosdk.models.job.RetryStrategy) | None*
 
 #### source *: [GitRepoSource](#bodosdk.models.job.GitRepoSource) | [WorkspaceSource](#bodosdk.models.job.WorkspaceSource) | [S3Source](#bodosdk.models.job.S3Source) | [TextSource](#bodosdk.models.job.TextSource) | None*
 
 #### sql_query_parameters *: dict | None*
 
+#### store_result *: bool | None*
+
 #### timeout *: int | None*
 
 #### type *: str | None*
 
 ### *class* bodosdk.models.job.JobFilter(\*, ids: List[str | UUID] | None = None, template_ids: List[str | UUID] | None = None, cluster_ids: List[str | UUID] | None = None, types: List[str] | None = None, statuses: List[str] | None = None, started_at: datetime | None = None, finished_at: datetime | None = None)
 
 Bases: `SDKBaseModel`
@@ -2329,14 +2353,16 @@
 
 #### config *: [JobConfig](#bodosdk.models.job.JobConfig) | None*
 
 #### finished_at *: datetime | None*
 
 #### get_logs_urls()
 
+#### get_result_urls()
+
 #### get_stderr()
 
 #### get_stdout()
 
 #### *property* id *: str*
 
 #### job_template_id *: str | None*
@@ -2614,15 +2640,15 @@
 
 #### *property* id
 
 #### job_runs *: List[[JobRun](#bodosdk.models.job.JobRun)]*
 
 #### name *: str | None*
 
-#### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None)
+#### run(name: str = None, cluster: dict | ICluster = None, code_type: str = None, source: dict | IS3Source | IGitRepoSource | IWorkspaceSource | ITextSource = None, exec_file: str = None, exec_text: str = None, args: dict | str = None, env_vars: dict = None, timeout: int = None, num_retries: int = None, delay_between_retries: int = None, retry_on_timeout: bool = None, catalog: str = None, store_result: bool = False)
 
 #### uuid *: str | None*
 
 ### *class* bodosdk.models.job.JobTemplateFilter(\*, ids: List[str] | None = None, names: List[str] | None = None, tags: dict | None = None)
 
 Bases: `SDKBaseModel`, `IJobTemplateFilter`
 
@@ -2866,34 +2892,27 @@
 
 #### path *: str*
 
 #### type *: str*
 
 <a id="module-bodosdk.models.common"></a>
 
-### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, fetchedVpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
+### *class* bodosdk.models.common.AWSNetworkData(\*, region: str | None = None, storageEndpoint: bool | None = None, vpcId: str | None = None, publicSubnetsIds: List[str] | None = None, privateSubnetsIds: List[str] | None = None, policyArns: List[str] | None = None)
 
 Bases: [`NetworkData`](#bodosdk.models.common.NetworkData)
 
 Extends the NetworkData class to include specific properties for AWS networking.
 
 #### vpc_id
 
 The ID of the AWS Virtual Private Cloud (VPC) where workspace should be created.
 
 * **Type:**
   Optional[str]
 
-#### fetched_vpc_id
-
-The ID of the fetched AWS VPC - if no vpc_id provided.
-
-* **Type:**
-  Optional[str]
-
 #### public_subnets_ids
 
 List of IDs for the public subnets within the AWS VPC.
 
 * **Type:**
   Optional[List[str]]
 
@@ -2907,16 +2926,14 @@
 #### policies_arn
 
 List of AWS Resource Names (ARNs) for the policies applied to the network.
 
 * **Type:**
   Optional[List[str]]
 
-#### fetched_vpc_id *: str | None*
-
 #### policies_arn *: List[str] | None*
 
 #### private_subnets_ids *: List[str] | None*
 
 #### public_subnets_ids *: List[str] | None*
 
 #### vpc_id *: str | None*
@@ -3076,21 +3093,21 @@
 
 #### page_size *: int | None*
 
 #### total *: int | None*
 
 <a id="module-bodosdk.models.workspace"></a>
 
-### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
+### *class* bodosdk.models.workspace.Workspace(org_client: IBodoOrganizationClient = None, \*, name: str | None = None, uuid: str | UUID | None = None, status: str | None = None, organizationUUID: str | UUID | None = None, networkData: [NetworkData](#bodosdk.models.common.NetworkData) | [AWSNetworkData](#bodosdk.models.common.AWSNetworkData) | None = None, createdBy: str | None = None, notebookAutoDeployEnabled: bool | None = None, assignedAt: datetime | None = None, customTags: Dict[str, Any] | None = None, jupyterLastActivity: datetime | None = None, jupyterIsActive: bool | None = False, cloudConfig: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase) | [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None = None)
 
 Bases: `SDKBaseModel`, `IWorkspace`
 
 #### assigned_at *: datetime | None*
 
-#### cloud_config *: [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
+#### cloud_config *: [CloudConfigBase](#bodosdk.models.cloud_config.CloudConfigBase) | [AwsCloudConfig](#bodosdk.models.cloud_config.AwsCloudConfig) | [AzureCloudConfig](#bodosdk.models.cloud_config.AzureCloudConfig) | None*
 
 #### created_by *: str | None*
 
 #### custom_tags *: Dict[str, Any] | None*
 
 #### delete()
```

### Comparing `bodosdk-2.0.0rc2/bodosdk.egg-info/SOURCES.txt` & `bodosdk-2.0.1rc1/bodosdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 bodosdk/clients/job.py
 bodosdk/clients/job_tpl.py
 bodosdk/clients/organization.py
 bodosdk/clients/secret.py
 bodosdk/clients/workspace.py
 bodosdk/db/__init__.py
 bodosdk/db/connection.py
+bodosdk/db/downloader.py
+bodosdk/db/exc.py
 bodosdk/models/__init__.py
 bodosdk/models/catalog.py
 bodosdk/models/cloud_config.py
 bodosdk/models/cluster.py
 bodosdk/models/common.py
 bodosdk/models/instance_role.py
 bodosdk/models/job.py
```

### Comparing `bodosdk-2.0.0rc2/setup.py` & `bodosdk-2.0.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/tests/test_base.py` & `bodosdk-2.0.1rc1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-2.0.0rc2/versioneer.py` & `bodosdk-2.0.1rc1/versioneer.py`

 * *Files identical despite different names*

