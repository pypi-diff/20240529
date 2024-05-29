# Comparing `tmp/esisdk-0.2.0.tar.gz` & `tmp/esisdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tzumainn/development/esisdk/dist/tmptz0mdm5d/esisdk-0.2.0.tar", last modified: Thu May  9 16:02:08 2024, max compression
+gzip compressed data, was "/home/tzumainn/development/esisdk/dist/tmp146urlvk/esisdk-0.3.0.tar", last modified: Wed May 29 17:04:53 2024, max compression
```

## Comparing `esisdk-0.2.0.tar` & `esisdk-0.3.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      601 2024-04-29 17:59:33.000000 esisdk-0.2.0/.github/workflows/tests.yaml
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/cloud/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/cloud/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2156 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/cloud/_lease.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/lease/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/lease/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/lease/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1680 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/lease/v1/_common.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9925 2024-05-09 16:01:07.000000 esisdk-0.2.0/esi/lease/v1/_proxy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1948 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/lease/v1/event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3184 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/lease/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1675 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/lease/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3330 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/lease/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/lease/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7777 2024-05-09 16:01:07.000000 esisdk-0.2.0/esi/lease/lease_service.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/functional/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/functional/lease/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1105 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/functional/lease/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2521 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1715 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5344 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1391 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5286 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/functional/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/unit/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/unit/cloud/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/unit/cloud/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8132 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/unit/cloud/test_lease.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/unit/lease/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2736 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/test_event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3765 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2220 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3946 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/test_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3189 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/unit/lease/v1/test_proxy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/unit/lease/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/unit/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/tests/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2504 2024-05-09 16:01:07.000000 esisdk-0.2.0/esi/tests/fakes.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2402 2024-04-30 14:18:00.000000 esisdk-0.2.0/esi/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      693 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/_services_mixin.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      896 2024-04-29 17:59:33.000000 esisdk-0.2.0/esi/connection.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3028 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1561 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-04-29 18:02:59.000000 esisdk-0.2.0/esisdk.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      292 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/requires.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        4 2024-05-09 16:02:08.000000 esisdk-0.2.0/esisdk.egg-info/top_level.txt
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/openstack/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/openstack/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/openstack/tests/unit/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/openstack/tests/unit/fixtures/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-09 16:02:08.000000 esisdk-0.2.0/openstack/tests/unit/fixtures/clouds/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      671 2024-04-29 17:59:33.000000 esisdk-0.2.0/openstack/tests/unit/fixtures/clouds/clouds.yaml
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      761 2024-04-29 17:59:33.000000 esisdk-0.2.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1010 2024-04-29 17:59:33.000000 esisdk-0.2.0/openstack/tests/unit/fixtures/discovery.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       48 2024-04-29 17:59:33.000000 esisdk-0.2.0/.stestr.conf
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      151 2024-05-09 16:02:08.000000 esisdk-0.2.0/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      217 2024-05-09 16:02:08.000000 esisdk-0.2.0/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2024-04-29 17:59:33.000000 esisdk-0.2.0/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2088 2024-04-30 14:18:00.000000 esisdk-0.2.0/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.2.0/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       16 2024-04-29 17:59:33.000000 esisdk-0.2.0/babel.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      664 2024-04-29 17:59:33.000000 esisdk-0.2.0/requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      774 2024-05-09 16:02:08.000000 esisdk-0.2.0/setup.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2024-04-29 17:59:33.000000 esisdk-0.2.0/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      665 2024-04-30 14:18:00.000000 esisdk-0.2.0/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1530 2024-04-30 14:18:00.000000 esisdk-0.2.0/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3028 2024-05-09 16:02:08.000000 esisdk-0.2.0/PKG-INFO
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      601 2024-04-29 17:59:33.000000 esisdk-0.3.0/.github/workflows/tests.yaml
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/cloud/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/cloud/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2174 2024-05-29 17:04:02.000000 esisdk-0.3.0/esi/cloud/_lease.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/lease/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/lease/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/lease/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1680 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/lease/v1/_common.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9925 2024-05-09 16:01:07.000000 esisdk-0.3.0/esi/lease/v1/_proxy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1948 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/lease/v1/event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3184 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/lease/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1701 2024-05-29 17:04:02.000000 esisdk-0.3.0/esi/lease/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3330 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/lease/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/lease/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7777 2024-05-09 16:01:07.000000 esisdk-0.3.0/esi/lease/lease_service.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/functional/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/functional/lease/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1105 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/functional/lease/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2521 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1715 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5344 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1391 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5286 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/functional/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/unit/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/unit/cloud/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/unit/cloud/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8132 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/unit/cloud/test_lease.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/unit/lease/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2736 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/test_event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3765 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2220 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3946 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/test_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3189 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/unit/lease/v1/test_proxy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/unit/lease/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/unit/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/tests/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2504 2024-05-09 16:01:07.000000 esisdk-0.3.0/esi/tests/fakes.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2402 2024-04-30 14:18:00.000000 esisdk-0.3.0/esi/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      693 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/_services_mixin.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      896 2024-04-29 17:59:33.000000 esisdk-0.3.0/esi/connection.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3028 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1561 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-04-29 18:02:59.000000 esisdk-0.3.0/esisdk.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      292 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        4 2024-05-29 17:04:53.000000 esisdk-0.3.0/esisdk.egg-info/top_level.txt
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/openstack/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/openstack/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/openstack/tests/unit/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/openstack/tests/unit/fixtures/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-05-29 17:04:53.000000 esisdk-0.3.0/openstack/tests/unit/fixtures/clouds/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      671 2024-04-29 17:59:33.000000 esisdk-0.3.0/openstack/tests/unit/fixtures/clouds/clouds.yaml
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      761 2024-04-29 17:59:33.000000 esisdk-0.3.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1010 2024-04-29 17:59:33.000000 esisdk-0.3.0/openstack/tests/unit/fixtures/discovery.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       48 2024-04-29 17:59:33.000000 esisdk-0.3.0/.stestr.conf
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      151 2024-05-29 17:04:53.000000 esisdk-0.3.0/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      276 2024-05-29 17:04:53.000000 esisdk-0.3.0/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2024-04-29 17:59:33.000000 esisdk-0.3.0/LICENSE
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2088 2024-04-30 14:18:00.000000 esisdk-0.3.0/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-29 17:59:33.000000 esisdk-0.3.0/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       16 2024-04-29 17:59:33.000000 esisdk-0.3.0/babel.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      664 2024-04-29 17:59:33.000000 esisdk-0.3.0/requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      774 2024-05-29 17:04:53.000000 esisdk-0.3.0/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      597 2024-04-29 17:59:33.000000 esisdk-0.3.0/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      665 2024-04-30 14:18:00.000000 esisdk-0.3.0/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1530 2024-04-30 14:18:00.000000 esisdk-0.3.0/tox.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3028 2024-05-29 17:04:53.000000 esisdk-0.3.0/PKG-INFO
```

### Comparing `esisdk-0.2.0/.github/workflows/tests.yaml` & `esisdk-0.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/cloud/_lease.py` & `esisdk-0.3.0/esi/cloud/_lease.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,14 @@
                                        project_id=project_id,
                                        **kwargs)
 
     def delete_lease(self, lease):
         """Delete a lease"""
         return self.lease.delete_lease(lease)
 
-    def list_nodes(self):
+    def list_nodes(self, **kwargs):
         """Return a list of all nodes info"""
-        return list(self.lease.nodes())
+        return list(self.lease.nodes(**kwargs))
 
     def list_events(self, **kwargs):
         """Return a list of events"""
         return list(self.lease.events(**kwargs))
```

### Comparing `esisdk-0.2.0/esi/lease/v1/_common.py` & `esisdk-0.3.0/esi/lease/v1/_common.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/lease/v1/_proxy.py` & `esisdk-0.3.0/esi/lease/v1/_proxy.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/lease/v1/event.py` & `esisdk-0.3.0/esi/lease/v1/event.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/lease/v1/lease.py` & `esisdk-0.3.0/esi/lease/v1/lease.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/lease/v1/node.py` & `esisdk-0.3.0/esi/lease/v1/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     allow_list = True
 
     # client-side query parameter
     _query_mapping = resource.QueryParameters(
         'name',
         'owner',
         'lessee',
+        'resource_class',
         'offer_uuid',
         'lease_uuid'
     )
 
     #: The transaction date and time.
     timestamp = resource.Header("x-timestamp")
     #: The value of the resource. Also available in headers.
```

### Comparing `esisdk-0.2.0/esi/lease/v1/offer.py` & `esisdk-0.3.0/esi/lease/v1/offer.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/lease/lease_service.py` & `esisdk-0.3.0/esi/lease/lease_service.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/README.md` & `esisdk-0.3.0/esi/tests/functional/lease/README.md`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/base.py` & `esisdk-0.3.0/esi/tests/functional/lease/base.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_event.py` & `esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_event.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_lease.py` & `esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_lease.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_node.py` & `esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_node.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/functional/lease/test_esi_leap_offer.py` & `esisdk-0.3.0/esi/tests/functional/lease/test_esi_leap_offer.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/cloud/test_lease.py` & `esisdk-0.3.0/esi/tests/unit/cloud/test_lease.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/lease/v1/test_event.py` & `esisdk-0.3.0/esi/tests/unit/lease/v1/test_event.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/lease/v1/test_lease.py` & `esisdk-0.3.0/esi/tests/unit/lease/v1/test_lease.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/lease/v1/test_node.py` & `esisdk-0.3.0/esi/tests/unit/lease/v1/test_node.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/lease/v1/test_offer.py` & `esisdk-0.3.0/esi/tests/unit/lease/v1/test_offer.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/unit/lease/v1/test_proxy.py` & `esisdk-0.3.0/esi/tests/unit/lease/v1/test_proxy.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/tests/fakes.py` & `esisdk-0.3.0/esi/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/__init__.py` & `esisdk-0.3.0/esi/__init__.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/_services_mixin.py` & `esisdk-0.3.0/esi/_services_mixin.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esi/connection.py` & `esisdk-0.3.0/esi/connection.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/esisdk.egg-info/PKG-INFO` & `esisdk-0.3.0/esisdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esisdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: An SDK for building applications to work with ESI
 Home-page: https://esi.readthedocs.io/en/latest/
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `esisdk-0.2.0/esisdk.egg-info/SOURCES.txt` & `esisdk-0.3.0/esisdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/openstack/tests/unit/fixtures/clouds/clouds.yaml` & `esisdk-0.3.0/openstack/tests/unit/fixtures/clouds/clouds.yaml`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml` & `esisdk-0.3.0/openstack/tests/unit/fixtures/clouds/clouds_cache.yaml`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/openstack/tests/unit/fixtures/discovery.json` & `esisdk-0.3.0/openstack/tests/unit/fixtures/discovery.json`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/LICENSE` & `esisdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/README.md` & `esisdk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/requirements.txt` & `esisdk-0.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/setup.cfg` & `esisdk-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/setup.py` & `esisdk-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/test-requirements.txt` & `esisdk-0.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/tox.ini` & `esisdk-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `esisdk-0.2.0/PKG-INFO` & `esisdk-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esisdk
-Version: 0.2.0
+Version: 0.3.0
 Summary: An SDK for building applications to work with ESI
 Home-page: https://esi.readthedocs.io/en/latest/
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

