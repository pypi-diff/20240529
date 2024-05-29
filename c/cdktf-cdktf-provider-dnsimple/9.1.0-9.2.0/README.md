# Comparing `tmp/cdktf-cdktf-provider-dnsimple-9.1.0.tar.gz` & `tmp/cdktf-cdktf-provider-dnsimple-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dnsimple-9.1.0.tar", last modified: Wed Mar 20 03:13:52 2024, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dnsimple-9.2.0.tar", last modified: Wed May 29 03:38:13 2024, max compression
```

## Comparing `cdktf-cdktf-provider-dnsimple-9.1.0.tar` & `cdktf-cdktf-provider-dnsimple-9.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.018245 cdktf-cdktf-provider-dnsimple-9.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99598 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@9.1.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/contact/
--rw-r--r--   0 runner    (1001) docker     (127)    45341 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)    29576 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/
--rw-r--r--   0 runner    (1001) docker     (127)    40669 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
--rw-r--r--   0 runner    (1001) docker     (127)    17533 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/
--rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/ds_record/
--rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
--rw-r--r--   0 runner    (1001) docker     (127)    21769 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/provider/
--rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/
--rw-r--r--   0 runner    (1001) docker     (127)    64560 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone/
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.026245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
--rw-r--r--   0 runner    (1001) docker     (127)    30413 2024-03-20 03:13:37.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:13:52.022245 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-20 03:13:51.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-20 03:13:51.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:13:51.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-20 03:13:51.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-20 03:13:51.000000 cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.714963 cdktf-cdktf-provider-dnsimple-9.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99597 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@9.2.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/contact/
+-rw-r--r--   0 runner    (1001) docker     (127)    45417 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)    29652 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/
+-rw-r--r--   0 runner    (1001) docker     (127)    40745 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
+-rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/
+-rw-r--r--   0 runner    (1001) docker     (127)    19718 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/ds_record/
+-rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
+-rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)    29042 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    64636 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone/
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.722963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
+-rw-r--r--   0 runner    (1001) docker     (127)    30489 2024-05-29 03:38:02.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:38:13.718963 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-29 03:38:13.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-29 03:38:13.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:38:13.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 03:38:13.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 03:38:13.000000 cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/LICENSE` & `cdktf-cdktf-provider-dnsimple-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 9.1.0
+Version: 9.2.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.5.0
+# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.6.0
 
-This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dnsimple](https://www.npmjs.com/package/@cdktf/provider-dnsimple).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dnsimple provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0)
+* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/README.md` & `cdktf-cdktf-provider-dnsimple-9.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.5.0
+# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.6.0
 
-This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dnsimple](https://www.npmjs.com/package/@cdktf/provider-dnsimple).
 
@@ -58,15 +58,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dnsimple provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0)
+* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/setup.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dnsimple",
-    "version": "9.1.0",
+    "version": "9.2.0",
     "description": "Prebuilt dnsimple Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dnsimple.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -35,25 +35,25 @@
         "cdktf_cdktf_provider_dnsimple.provider",
         "cdktf_cdktf_provider_dnsimple.registered_domain",
         "cdktf_cdktf_provider_dnsimple.zone",
         "cdktf_cdktf_provider_dnsimple.zone_record"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dnsimple._jsii": [
-            "provider-dnsimple@9.1.0.jsii.tgz"
+            "provider-dnsimple@9.2.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dnsimple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "cdktf>=0.20.0, <0.21.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.5.0
+# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.6.0
 
-This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dnsimple](https://www.npmjs.com/package/@cdktf/provider-dnsimple).
 
@@ -59,15 +59,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dnsimple provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0)
+* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
@@ -89,14 +89,17 @@
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [CDKTF Repository Manager](https://github.com/cdktf/cdktf-repository-manager/).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/contact/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_contact`
 
-Refer to the Terraform Registry for docs: [`dnsimple_contact`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact).
+Refer to the Terraform Registry for docs: [`dnsimple_contact`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Contact(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.contact.Contact",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact dnsimple_contact}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact dnsimple_contact}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         address1: builtins.str,
@@ -51,32 +54,32 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact dnsimple_contact} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact dnsimple_contact} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param address1: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address1 Contact#address1}.
-        :param city: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#city Contact#city}.
-        :param country: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#country Contact#country}.
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#email Contact#email}.
-        :param first_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#first_name Contact#first_name}.
-        :param last_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#last_name Contact#last_name}.
-        :param phone: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#phone Contact#phone}.
-        :param postal_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#postal_code Contact#postal_code}.
-        :param state_province: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#state_province Contact#state_province}.
-        :param address2: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address2 Contact#address2}.
-        :param fax: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#fax Contact#fax}.
-        :param job_title: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#job_title Contact#job_title}.
-        :param label: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#label Contact#label}.
-        :param organization_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#organization_name Contact#organization_name}.
+        :param address1: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address1 Contact#address1}.
+        :param city: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#city Contact#city}.
+        :param country: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#country Contact#country}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#email Contact#email}.
+        :param first_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#first_name Contact#first_name}.
+        :param last_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#last_name Contact#last_name}.
+        :param phone: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#phone Contact#phone}.
+        :param postal_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#postal_code Contact#postal_code}.
+        :param state_province: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#state_province Contact#state_province}.
+        :param address2: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address2 Contact#address2}.
+        :param fax: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#fax Contact#fax}.
+        :param job_title: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#job_title Contact#job_title}.
+        :param label: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#label Contact#label}.
+        :param organization_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#organization_name Contact#organization_name}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -120,15 +123,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Contact resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Contact to import.
-        :param import_from_id: The id of the existing Contact that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Contact that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Contact to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e854be2adc7b729c6034b72b50557089e5c581ae7859aa78ba01b62b6850171)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -494,28 +497,28 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param address1: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address1 Contact#address1}.
-        :param city: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#city Contact#city}.
-        :param country: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#country Contact#country}.
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#email Contact#email}.
-        :param first_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#first_name Contact#first_name}.
-        :param last_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#last_name Contact#last_name}.
-        :param phone: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#phone Contact#phone}.
-        :param postal_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#postal_code Contact#postal_code}.
-        :param state_province: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#state_province Contact#state_province}.
-        :param address2: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address2 Contact#address2}.
-        :param fax: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#fax Contact#fax}.
-        :param job_title: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#job_title Contact#job_title}.
-        :param label: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#label Contact#label}.
-        :param organization_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#organization_name Contact#organization_name}.
+        :param address1: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address1 Contact#address1}.
+        :param city: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#city Contact#city}.
+        :param country: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#country Contact#country}.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#email Contact#email}.
+        :param first_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#first_name Contact#first_name}.
+        :param last_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#last_name Contact#last_name}.
+        :param phone: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#phone Contact#phone}.
+        :param postal_code: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#postal_code Contact#postal_code}.
+        :param state_province: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#state_province Contact#state_province}.
+        :param address2: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address2 Contact#address2}.
+        :param fax: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#fax Contact#fax}.
+        :param job_title: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#job_title Contact#job_title}.
+        :param label: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#label Contact#label}.
+        :param organization_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#organization_name Contact#organization_name}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__39980be67df6955084a3514dd46c0503ebb589fb08097912147d00aa617ab6bd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -636,102 +639,102 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def address1(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address1 Contact#address1}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address1 Contact#address1}.'''
         result = self._values.get("address1")
         assert result is not None, "Required property 'address1' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def city(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#city Contact#city}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#city Contact#city}.'''
         result = self._values.get("city")
         assert result is not None, "Required property 'city' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def country(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#country Contact#country}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#country Contact#country}.'''
         result = self._values.get("country")
         assert result is not None, "Required property 'country' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#email Contact#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#email Contact#email}.'''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def first_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#first_name Contact#first_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#first_name Contact#first_name}.'''
         result = self._values.get("first_name")
         assert result is not None, "Required property 'first_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def last_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#last_name Contact#last_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#last_name Contact#last_name}.'''
         result = self._values.get("last_name")
         assert result is not None, "Required property 'last_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def phone(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#phone Contact#phone}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#phone Contact#phone}.'''
         result = self._values.get("phone")
         assert result is not None, "Required property 'phone' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def postal_code(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#postal_code Contact#postal_code}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#postal_code Contact#postal_code}.'''
         result = self._values.get("postal_code")
         assert result is not None, "Required property 'postal_code' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def state_province(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#state_province Contact#state_province}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#state_province Contact#state_province}.'''
         result = self._values.get("state_province")
         assert result is not None, "Required property 'state_province' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address2(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#address2 Contact#address2}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#address2 Contact#address2}.'''
         result = self._values.get("address2")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def fax(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#fax Contact#fax}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#fax Contact#fax}.'''
         result = self._values.get("fax")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_title(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#job_title Contact#job_title}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#job_title Contact#job_title}.'''
         result = self._values.get("job_title")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def label(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#label Contact#label}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#label Contact#label}.'''
         result = self._values.get("label")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def organization_name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/contact#organization_name Contact#organization_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/contact#organization_name Contact#organization_name}.'''
         result = self._values.get("organization_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dnsimple_certificate`
 
-Refer to the Terraform Registry for docs: [`data_dnsimple_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate).
+Refer to the Terraform Registry for docs: [`data_dnsimple_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsimpleCertificate(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate dnsimple_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate dnsimple_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         certificate_id: jsii.Number,
@@ -40,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate dnsimple_certificate} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate dnsimple_certificate} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,29 +90,29 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsimpleCertificate resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsimpleCertificate to import.
-        :param import_from_id: The id of the existing DataDnsimpleCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsimpleCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsimpleCertificate to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f32f02dcceea8df22bd175d9b6ea615cb7e1ad61d3aecf1b878be7b0f65bdf5d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
         return typing.cast(_cdktf_9a9027ec.ImportableResource, jsii.sinvoke(cls, "generateConfigForImport", [scope, import_to_id, import_from_id, provider]))
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: A string that can be `parsed as a duration <https://pkg.go.dev/time#ParseDuration>`_ consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
+        :param read: A string that can be `parsed as a duration <https://pkg.go.dev/time#ParseDuration>`_ consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
         '''
         value = DataDnsimpleCertificateTimeouts(read=read)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetTimeouts")
     def reset_timeouts(self) -> None:
@@ -235,17 +238,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataDnsimpleCertificateTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da)
@@ -344,35 +347,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def certificate_id(self) -> jsii.Number:
         '''Certificate ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
         '''
         result = self._values.get("certificate_id")
         assert result is not None, "Required property 'certificate_id' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
         '''Domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         '''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataDnsimpleCertificateTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#timeouts DataDnsimpleCertificate#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataDnsimpleCertificateTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -389,28 +392,28 @@
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificateTimeouts",
     jsii_struct_bases=[],
     name_mapping={"read": "read"},
 )
 class DataDnsimpleCertificateTimeouts:
     def __init__(self, *, read: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param read: A string that can be `parsed as a duration <https://pkg.go.dev/time#ParseDuration>`_ consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
+        :param read: A string that can be `parsed as a duration <https://pkg.go.dev/time#ParseDuration>`_ consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c57c25169f7fc6d2a154fdacc39b2464da6dbb169d2b7f877cf8deb70d21afaf)
             check_type(argname="argument read", value=read, expected_type=type_hints["read"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if read is not None:
             self._values["read"] = read
 
     @builtins.property
     def read(self) -> typing.Optional[builtins.str]:
         '''A string that can be `parsed as a duration <https://pkg.go.dev/time#ParseDuration>`_ consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/certificate#read DataDnsimpleCertificate#read}
         '''
         result = self._values.get("read")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dnsimple_registrant_change_check`
 
-Refer to the Terraform Registry for docs: [`data_dnsimple_registrant_change_check`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check).
+Refer to the Terraform Registry for docs: [`data_dnsimple_registrant_change_check`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsimpleRegistrantChangeCheck(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleRegistrantChangeCheck.DataDnsimpleRegistrantChangeCheck",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check dnsimple_registrant_change_check}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check dnsimple_registrant_change_check}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         contact_id: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check dnsimple_registrant_change_check} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check dnsimple_registrant_change_check} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param contact_id: DNSimple contact ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
-        :param domain_id: DNSimple domain ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
+        :param contact_id: DNSimple contact ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
+        :param domain_id: DNSimple domain ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsimpleRegistrantChangeCheck resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsimpleRegistrantChangeCheck to import.
-        :param import_from_id: The id of the existing DataDnsimpleRegistrantChangeCheck that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsimpleRegistrantChangeCheck that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsimpleRegistrantChangeCheck to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__696d5e0c0f46e0e3cee8a06d1e9be84fe7e50238720c63f986e59a4ae26c16e1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -197,16 +200,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param contact_id: DNSimple contact ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
-        :param domain_id: DNSimple domain ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
+        :param contact_id: DNSimple contact ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
+        :param domain_id: DNSimple domain ID for which the registrant change check is being performed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bdb9b20b62fef803e7bae7931a4da88dacee2e41c0df63448407bbe062398e80)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -300,25 +303,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def contact_id(self) -> builtins.str:
         '''DNSimple contact ID for which the registrant change check is being performed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#contact_id DataDnsimpleRegistrantChangeCheck#contact_id}
         '''
         result = self._values.get("contact_id")
         assert result is not None, "Required property 'contact_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def domain_id(self) -> builtins.str:
         '''DNSimple domain ID for which the registrant change check is being performed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/registrant_change_check#domain_id DataDnsimpleRegistrantChangeCheck#domain_id}
         '''
         result = self._values.get("domain_id")
         assert result is not None, "Required property 'domain_id' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_dnsimple_zone`
 
-Refer to the Terraform Registry for docs: [`data_dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone).
+Refer to the Terraform Registry for docs: [`data_dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataDnsimpleZone(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleZone.DataDnsimpleZone",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone dnsimple_zone}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone dnsimple_zone}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone dnsimple_zone} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone dnsimple_zone} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataDnsimpleZone resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataDnsimpleZone to import.
-        :param import_from_id: The id of the existing DataDnsimpleZone that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataDnsimpleZone that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataDnsimpleZone to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7cd769e5e47e497ab39411249b317bd8d619662c52fc90c8f37c10d934edda4a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -173,15 +176,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9051fabefb514091998aee3b06ffda795da4195d413ca0bc91120a12dc8cf592)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -273,15 +276,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Zone Name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/data-sources/zone#name DataDnsimpleZone#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_domain`
 
-Refer to the Terraform Registry for docs: [`dnsimple_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain).
+Refer to the Terraform Registry for docs: [`dnsimple_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Domain(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.domain.Domain",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain dnsimple_domain}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain dnsimple_domain}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -38,19 +41,19 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain dnsimple_domain} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain dnsimple_domain} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain#name Domain#name}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -81,15 +84,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Domain resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Domain to import.
-        :param import_from_id: The id of the existing Domain that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Domain that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Domain to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__920aa8720c40d9e1dde6c773717175196857430861eecca64aac7aad4cc2b7e9)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -193,15 +196,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain#name Domain#name}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -291,15 +294,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain#name Domain#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain#name Domain#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_domain_delegation`
 
-Refer to the Terraform Registry for docs: [`dnsimple_domain_delegation`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation).
+Refer to the Terraform Registry for docs: [`dnsimple_domain_delegation`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DomainDelegation(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.domainDelegation.DomainDelegation",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation dnsimple_domain_delegation}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation dnsimple_domain_delegation}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         domain: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation dnsimple_domain_delegation} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation dnsimple_domain_delegation} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.
-        :param name_servers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.
+        :param name_servers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DomainDelegation resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DomainDelegation to import.
-        :param import_from_id: The id of the existing DomainDelegation that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DomainDelegation that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DomainDelegation to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3d383bf5d6e223e98ae0d87fc73a6dbe55f531f8d38d3a49a1d577938ff02099)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -185,16 +188,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.
-        :param name_servers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.
+        :param name_servers: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8161bccbe3c7a1544f8ed1fe59557f74cf289edd6978daf40109625ed2572d42)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -286,22 +289,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#domain DomainDelegation#domain}.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name_servers(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/domain_delegation#name_servers DomainDelegation#name_servers}.'''
         result = self._values.get("name_servers")
         assert result is not None, "Required property 'name_servers' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_ds_record`
 
-Refer to the Terraform Registry for docs: [`dnsimple_ds_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record).
+Refer to the Terraform Registry for docs: [`dnsimple_ds_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DsRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dsRecord.DsRecord",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record dnsimple_ds_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record dnsimple_ds_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         algorithm: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record dnsimple_ds_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record dnsimple_ds_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#domain DsRecord#domain}.
-        :param digest: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest DsRecord#digest}.
-        :param digest_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.
-        :param keytag: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#keytag DsRecord#keytag}.
-        :param public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#public_key DsRecord#public_key}.
+        :param algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#domain DsRecord#domain}.
+        :param digest: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest DsRecord#digest}.
+        :param digest_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.
+        :param keytag: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#keytag DsRecord#keytag}.
+        :param public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#public_key DsRecord#public_key}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DsRecord resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DsRecord to import.
-        :param import_from_id: The id of the existing DsRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DsRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DsRecord to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d2b0d2d146e303f9a124423d6970ff4ead65152e43c438bfdd6b49be41eaf2a1)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -299,20 +302,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#domain DsRecord#domain}.
-        :param digest: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest DsRecord#digest}.
-        :param digest_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.
-        :param keytag: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#keytag DsRecord#keytag}.
-        :param public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#public_key DsRecord#public_key}.
+        :param algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#domain DsRecord#domain}.
+        :param digest: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest DsRecord#digest}.
+        :param digest_type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.
+        :param keytag: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#keytag DsRecord#keytag}.
+        :param public_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#public_key DsRecord#public_key}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0ce18a877d9588c06ea5cfd06eab9a3dcb78d0c9500244b54773ad2c628ee40d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -416,47 +419,47 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def algorithm(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#algorithm DsRecord#algorithm}.'''
         result = self._values.get("algorithm")
         assert result is not None, "Required property 'algorithm' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#domain DsRecord#domain}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#domain DsRecord#domain}.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def digest(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest DsRecord#digest}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest DsRecord#digest}.'''
         result = self._values.get("digest")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def digest_type(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#digest_type DsRecord#digest_type}.'''
         result = self._values.get("digest_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def keytag(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#keytag DsRecord#keytag}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#keytag DsRecord#keytag}.'''
         result = self._values.get("keytag")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def public_key(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/ds_record#public_key DsRecord#public_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/ds_record#public_key DsRecord#public_key}.'''
         result = self._values.get("public_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_email_forward`
 
-Refer to the Terraform Registry for docs: [`dnsimple_email_forward`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward).
+Refer to the Terraform Registry for docs: [`dnsimple_email_forward`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class EmailForward(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForward",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward dnsimple_email_forward}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward dnsimple_email_forward}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias_name: builtins.str,
@@ -40,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward dnsimple_email_forward} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward dnsimple_email_forward} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#domain EmailForward#domain}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a EmailForward resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the EmailForward to import.
-        :param import_from_id: The id of the existing EmailForward that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing EmailForward that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the EmailForward to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f63ccc6704a50ffde144d4cd964836f1bc757131d905b11020f5d730b90ced8f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -212,17 +215,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#domain EmailForward#domain}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -316,29 +319,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def alias_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.'''
         result = self._values.get("alias_name")
         assert result is not None, "Required property 'alias_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def destination_email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.'''
         result = self._values.get("destination_email")
         assert result is not None, "Required property 'destination_email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/email_forward#domain EmailForward#domain}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/email_forward#domain EmailForward#domain}.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_lets_encrypt_certificate`
 
-Refer to the Terraform Registry for docs: [`dnsimple_lets_encrypt_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate).
+Refer to the Terraform Registry for docs: [`dnsimple_lets_encrypt_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class LetsEncryptCertificate(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.letsEncryptCertificate.LetsEncryptCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a LetsEncryptCertificate resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the LetsEncryptCertificate to import.
-        :param import_from_id: The id of the existing LetsEncryptCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing LetsEncryptCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the LetsEncryptCertificate to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7b680792b6b16d335e61b2a427875ce8e01d6a1174ff13ee73c8e5f1d96def94)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -299,19 +302,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param alternate_names: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -411,42 +414,42 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
         result = self._values.get("auto_renew")
         assert result is not None, "Required property 'auto_renew' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def domain_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
         result = self._values.get("domain_id")
         assert result is not None, "Required property 'domain_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def alternate_names(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#alternate_names LetsEncryptCertificate#alternate_names}.'''
         result = self._values.get("alternate_names")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def signature_algorithm(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
         result = self._values.get("signature_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `provider`
 
-Refer to the Terraform Registry for docs: [`dnsimple`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs).
+Refer to the Terraform Registry for docs: [`dnsimple`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,38 +25,38 @@
 
 
 class DnsimpleProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.provider.DnsimpleProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs dnsimple}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs dnsimple}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         account: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs dnsimple} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs dnsimple} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7ef56b7728822c45a23750e2602fff787208bfb71fa54a96467397e10a6e47c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DnsimpleProviderConfig(
             account=account,
@@ -75,15 +78,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DnsimpleProvider resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DnsimpleProvider to import.
-        :param import_from_id: The id of the existing DnsimpleProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DnsimpleProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DnsimpleProvider to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a4edfc9e8a657653d4fcd97200d4c0bf459f5954ee5b33da4ca414163f4b238e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -264,20 +267,20 @@
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38b8bc1cdf1e0a8d7a730ac02381391ddfa090074fe8470d004c65b043c59d30)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument prefetch", value=prefetch, expected_type=type_hints["prefetch"])
             check_type(argname="argument sandbox", value=sandbox, expected_type=type_hints["sandbox"])
@@ -297,64 +300,64 @@
         if user_agent is not None:
             self._values["user_agent"] = user_agent
 
     @builtins.property
     def account(self) -> typing.Optional[builtins.str]:
         '''The account for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#account DnsimpleProvider#account}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#account DnsimpleProvider#account}
         '''
         result = self._values.get("account")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#alias DnsimpleProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#alias DnsimpleProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefetch(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the prefetch of zone records.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#prefetch DnsimpleProvider#prefetch}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#prefetch DnsimpleProvider#prefetch}
         '''
         result = self._values.get("prefetch")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def sandbox(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the sandbox API.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#sandbox DnsimpleProvider#sandbox}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#sandbox DnsimpleProvider#sandbox}
         '''
         result = self._values.get("sandbox")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The API v2 token for API operations.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#token DnsimpleProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#token DnsimpleProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_agent(self) -> typing.Optional[builtins.str]:
         '''Custom string to append to the user agent used for sending HTTP requests to the API.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs#user_agent DnsimpleProvider#user_agent}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         result = self._values.get("user_agent")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/registered_domain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_registered_domain`
 
-Refer to the Terraform Registry for docs: [`dnsimple_registered_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain).
+Refer to the Terraform Registry for docs: [`dnsimple_registered_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class RegisteredDomain(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.registeredDomain.RegisteredDomain",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain dnsimple_registered_domain}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain dnsimple_registered_domain}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         contact_id: jsii.Number,
@@ -46,27 +49,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain dnsimple_registered_domain} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain dnsimple_registered_domain} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param contact_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#name RegisteredDomain#name}.
-        :param auto_renew_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.
-        :param dnssec_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.
-        :param extended_attributes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.
-        :param premium_price: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.
-        :param timeouts: Timeouts for operations, given as a parsable string as in ``10m`` or ``30s``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
-        :param transfer_lock_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.
-        :param whois_privacy_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.
+        :param contact_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#name RegisteredDomain#name}.
+        :param auto_renew_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.
+        :param dnssec_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.
+        :param extended_attributes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.
+        :param premium_price: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.
+        :param timeouts: Timeouts for operations, given as a parsable string as in ``10m`` or ``30s``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
+        :param transfer_lock_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.
+        :param whois_privacy_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -105,15 +108,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a RegisteredDomain resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the RegisteredDomain to import.
-        :param import_from_id: The id of the existing RegisteredDomain that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing RegisteredDomain that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the RegisteredDomain to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6feddb1eb699d20b1684b6e0638d9c20ed59ea492b231b01304b5beba8d23705)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -125,17 +128,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Create timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#create RegisteredDomain#create}
-        :param delete: Delete timeout (currently unused). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
-        :param update: Update timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#update RegisteredDomain#update}
+        :param create: Create timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#create RegisteredDomain#create}
+        :param delete: Delete timeout (currently unused). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
+        :param update: Update timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#update RegisteredDomain#update}
         '''
         value = RegisteredDomainTimeouts(create=create, delete=delete, update=update)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetAutoRenewEnabled")
     def reset_auto_renew_enabled(self) -> None:
@@ -444,23 +447,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param contact_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#name RegisteredDomain#name}.
-        :param auto_renew_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.
-        :param dnssec_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.
-        :param extended_attributes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.
-        :param premium_price: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.
-        :param timeouts: Timeouts for operations, given as a parsable string as in ``10m`` or ``30s``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
-        :param transfer_lock_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.
-        :param whois_privacy_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.
+        :param contact_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#name RegisteredDomain#name}.
+        :param auto_renew_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.
+        :param dnssec_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.
+        :param extended_attributes: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.
+        :param premium_price: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.
+        :param timeouts: Timeouts for operations, given as a parsable string as in ``10m`` or ``30s``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
+        :param transfer_lock_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.
+        :param whois_privacy_enabled: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = RegisteredDomainTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b2f6046a173166f9a95fbe5fe60474c69a14e222062e454a32cda2fafc3fd7b4)
@@ -575,78 +578,78 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def contact_id(self) -> jsii.Number:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#contact_id RegisteredDomain#contact_id}.'''
         result = self._values.get("contact_id")
         assert result is not None, "Required property 'contact_id' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#name RegisteredDomain#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#name RegisteredDomain#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def auto_renew_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#auto_renew_enabled RegisteredDomain#auto_renew_enabled}.'''
         result = self._values.get("auto_renew_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def dnssec_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#dnssec_enabled RegisteredDomain#dnssec_enabled}.'''
         result = self._values.get("dnssec_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def extended_attributes(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#extended_attributes RegisteredDomain#extended_attributes}.'''
         result = self._values.get("extended_attributes")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def premium_price(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#premium_price RegisteredDomain#premium_price}.'''
         result = self._values.get("premium_price")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["RegisteredDomainTimeouts"]:
         '''Timeouts for operations, given as a parsable string as in ``10m`` or ``30s``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#timeouts RegisteredDomain#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["RegisteredDomainTimeouts"], result)
 
     @builtins.property
     def transfer_lock_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#transfer_lock_enabled RegisteredDomain#transfer_lock_enabled}.'''
         result = self._values.get("transfer_lock_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def whois_privacy_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#whois_privacy_enabled RegisteredDomain#whois_privacy_enabled}.'''
         result = self._values.get("whois_privacy_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -662,26 +665,26 @@
     jsii_type="@cdktf/provider-dnsimple.registeredDomain.RegisteredDomainDomainRegistration",
     jsii_struct_bases=[],
     name_mapping={"state": "state"},
 )
 class RegisteredDomainDomainRegistration:
     def __init__(self, *, state: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#state RegisteredDomain#state}.
+        :param state: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#state RegisteredDomain#state}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0f69574b1f60aacf3b528afb57c264f579c89ad8ec6c8cf637860ec9984d65b0)
             check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if state is not None:
             self._values["state"] = state
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#state RegisteredDomain#state}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#state RegisteredDomain#state}.'''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -764,28 +767,28 @@
     jsii_type="@cdktf/provider-dnsimple.registeredDomain.RegisteredDomainRegistrantChange",
     jsii_struct_bases=[],
     name_mapping={"state": "state"},
 )
 class RegisteredDomainRegistrantChange:
     def __init__(self, *, state: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param state: State of the registrant change. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#state RegisteredDomain#state}
+        :param state: State of the registrant change. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#state RegisteredDomain#state}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__28b5b154681bf35f2869ff0a92b661c0a829dc1cb798e1ebaa73d23814b81692)
             check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if state is not None:
             self._values["state"] = state
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
         '''State of the registrant change.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#state RegisteredDomain#state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#state RegisteredDomain#state}
         '''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -900,17 +903,17 @@
         self,
         *,
         create: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Create timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#create RegisteredDomain#create}
-        :param delete: Delete timeout (currently unused). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
-        :param update: Update timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#update RegisteredDomain#update}
+        :param create: Create timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#create RegisteredDomain#create}
+        :param delete: Delete timeout (currently unused). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
+        :param update: Update timeout. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#update RegisteredDomain#update}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fcdee2d25c1f0e15a45a3d141748657e972c27e6c2a62521062527b391036c0f)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -921,33 +924,33 @@
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
         '''Create timeout.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#create RegisteredDomain#create}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#create RegisteredDomain#create}
         '''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
         '''Delete timeout (currently unused).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#delete RegisteredDomain#delete}
         '''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
         '''Update timeout.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/registered_domain#update RegisteredDomain#update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/registered_domain#update RegisteredDomain#update}
         '''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_zone`
 
-Refer to the Terraform Registry for docs: [`dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone).
+Refer to the Terraform Registry for docs: [`dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Zone(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.zone.Zone",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone dnsimple_zone}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone dnsimple_zone}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone dnsimple_zone} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone dnsimple_zone} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#name Zone#name}.
-        :param active: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#active Zone#active}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#name Zone#name}.
+        :param active: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#active Zone#active}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Zone resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Zone to import.
-        :param import_from_id: The id of the existing Zone that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Zone that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Zone to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__487e98040ed54bad4e09340d234cc5720a000ae781ba9c8bfbfc4300523b0899)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -214,16 +217,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#name Zone#name}.
-        :param active: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#active Zone#active}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#name Zone#name}.
+        :param active: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#active Zone#active}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5fb06cfd899a4694c0a5cc1959582bd9228cd329e0933c9d30d3b6c3cf8c9785)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -316,24 +319,24 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#name Zone#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#name Zone#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def active(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone#active Zone#active}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone#active Zone#active}.'''
         result = self._values.get("active")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `dnsimple_zone_record`
 
-Refer to the Terraform Registry for docs: [`dnsimple_zone_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record).
+Refer to the Terraform Registry for docs: [`dnsimple_zone_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class ZoneRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.zoneRecord.ZoneRecord",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record dnsimple_zone_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record dnsimple_zone_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -44,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record dnsimple_zone_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record dnsimple_zone_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#priority ZoneRecord#priority}.
-        :param regions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#regions ZoneRecord#regions}.
-        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param regions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#regions ZoneRecord#regions}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a ZoneRecord resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the ZoneRecord to import.
-        :param import_from_id: The id of the existing ZoneRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing ZoneRecord that should be imported. Refer to the {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the ZoneRecord to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fe4d917237d3b5835a6fba89179488fbe6cae79508d7d427815b5af55a11db50)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -327,21 +330,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#priority ZoneRecord#priority}.
-        :param regions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#regions ZoneRecord#regions}.
-        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param regions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#regions ZoneRecord#regions}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -446,55 +449,55 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#name ZoneRecord#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#name ZoneRecord#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#type ZoneRecord#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#type ZoneRecord#type}.'''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#value ZoneRecord#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#value ZoneRecord#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.'''
         result = self._values.get("zone_name")
         assert result is not None, "Required property 'zone_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def priority(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#priority ZoneRecord#priority}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#priority ZoneRecord#priority}.'''
         result = self._values.get("priority")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def regions(self) -> typing.Optional[typing.List[builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#regions ZoneRecord#regions}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#regions ZoneRecord#regions}.'''
         result = self._values.get("regions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.'''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 9.1.0
+Version: 9.2.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.5.0
+# CDKTF prebuilt bindings for dnsimple/dnsimple provider version 1.6.0
 
-This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-dnsimple](https://www.npmjs.com/package/@cdktf/provider-dnsimple).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform dnsimple provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.5.0)
+* [Terraform dnsimple provider](https://registry.terraform.io/providers/dnsimple/dnsimple/1.6.0)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-dnsimple-9.1.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dnsimple-9.2.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dnsimple/py.typed
 src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
-src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@9.1.0.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@9.2.0.jsii.tgz
 src/cdktf_cdktf_provider_dnsimple/contact/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_registrant_change_check/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain_delegation/__init__.py
 src/cdktf_cdktf_provider_dnsimple/ds_record/__init__.py
```

