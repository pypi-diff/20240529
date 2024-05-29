# Comparing `tmp/spotlight-sdk-0.1.2.tar.gz` & `tmp/spotlight-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-sdk-0.1.2.tar", last modified: Wed May 22 19:07:49 2024, max compression
+gzip compressed data, was "spotlight-sdk-0.1.4.tar", last modified: Wed May 29 02:33:51 2024, max compression
```

## Comparing `spotlight-sdk-0.1.2.tar` & `spotlight-sdk-0.1.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.837814 spotlight-sdk-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-05-22 19:07:49.836814 spotlight-sdk-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 19:07:49.837814 spotlight-sdk-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.822813 spotlight-sdk-0.1.2/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.823813 spotlight-sdk-0.1.2/spotlight/admin/
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/admin/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     7658 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/admin/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     6877 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/admin/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.823813 spotlight-sdk-0.1.2/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.823813 spotlight-sdk-0.1.2/spotlight/api/alert/
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/alert/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/alert/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/alert/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2788 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/alert/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.824813 spotlight-sdk-0.1.2/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.825813 spotlight-sdk-0.1.2/spotlight/api/data/
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4043 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/asynchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.825813 spotlight-sdk-0.1.2/spotlight/api/data/barchart/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/barchart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/barchart/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/barchart/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/barchart/model.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/barchart/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3755 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/data/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.826813 spotlight-sdk-0.1.2/spotlight/api/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/__util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.827813 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2477 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.827813 spotlight-sdk-0.1.2/spotlight/api/dataset/view/
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/dataset/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.828813 spotlight-sdk-0.1.2/spotlight/api/permission/
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3039 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/permission/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.828813 spotlight-sdk-0.1.2/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.829813 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2438 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.830814 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.830814 spotlight-sdk-0.1.2/spotlight/api/sdr_source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/sdr_source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/sdr_source/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/sdr_source/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/api/sdr_source/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.831814 spotlight-sdk-0.1.2/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.832814 spotlight-sdk-0.1.2/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.833814 spotlight-sdk-0.1.2/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2417 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.833814 spotlight-sdk-0.1.2/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.834814 spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.835814 spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.835814 spotlight-sdk-0.1.2/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.835814 spotlight-sdk-0.1.2/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3792 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-05-22 19:07:36.000000 spotlight-sdk-0.1.2/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:07:49.836814 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-05-22 19:07:49.000000 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3577 2024-05-22 19:07:49.000000 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 19:07:49.000000 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-22 19:07:49.000000 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 19:07:49.000000 spotlight-sdk-0.1.2/spotlight_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.099458 spotlight-sdk-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-05-29 02:33:51.098458 spotlight-sdk-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 02:33:51.099458 spotlight-sdk-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.071456 spotlight-sdk-0.1.4/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.072456 spotlight-sdk-0.1.4/spotlight/admin/
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/admin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/admin/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     7658 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/admin/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     6877 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/admin/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.073456 spotlight-sdk-0.1.4/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.074456 spotlight-sdk-0.1.4/spotlight/api/alert/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/alert/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/alert/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/alert/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/alert/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.074456 spotlight-sdk-0.1.4/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.075456 spotlight-sdk-0.1.4/spotlight/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/asynchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.076456 spotlight-sdk-0.1.4/spotlight/api/data/barchart/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/barchart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/barchart/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/barchart/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/barchart/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/barchart/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/data/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.077456 spotlight-sdk-0.1.4/spotlight/api/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/__util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.078456 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.080457 spotlight-sdk-0.1.4/spotlight/api/dataset/view/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/dataset/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.082457 spotlight-sdk-0.1.4/spotlight/api/permission/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/permission/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.083457 spotlight-sdk-0.1.4/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.084457 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.086457 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.088457 spotlight-sdk-0.1.4/spotlight/api/sdr_source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/sdr_source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/sdr_source/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3527 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/sdr_source/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/api/sdr_source/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.088457 spotlight-sdk-0.1.4/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.090458 spotlight-sdk-0.1.4/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2978 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.091458 spotlight-sdk-0.1.4/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.091458 spotlight-sdk-0.1.4/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.093458 spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.094458 spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.094458 spotlight-sdk-0.1.4/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.096458 spotlight-sdk-0.1.4/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3792 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-05-29 02:33:37.000000 spotlight-sdk-0.1.4/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 02:33:51.098458 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-05-29 02:33:50.000000 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-05-29 02:33:51.000000 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 02:33:50.000000 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-29 02:33:50.000000 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 02:33:50.000000 spotlight-sdk-0.1.4/spotlight_sdk.egg-info/top_level.txt
```

### Comparing `spotlight-sdk-0.1.2/PKG-INFO` & `spotlight-sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.1.2
+Version: 0.1.4
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.1.2/README.md` & `spotlight-sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/setup.py` & `spotlight-sdk-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/admin/__init__.py` & `spotlight-sdk-0.1.4/spotlight/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/admin/__util.py` & `spotlight-sdk-0.1.4/spotlight/admin/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/admin/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/admin/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/admin/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/admin/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/alert/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/alert/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/alert/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/alert/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/alert/model.py` & `spotlight-sdk-0.1.4/spotlight/api/alert/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/alert/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/alert/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/auth/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/auth/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/auth/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/data/__util.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 
 
 def _sdr_count_request_info(
     start: Optional[int] = None,
     end: Optional[int] = None,
     repository: Optional[set[Repository]] = None,
     asset_class: Optional[set[AssetClass]] = None,
+    distinct: Optional[bool] = None,
 ) -> dict:
     endpoint = "data/v1.1/sdr/count"
     params = {
         "start": start,
         "end": end,
         "repository": repository,
         "asset_class": asset_class,
+        "distinct": distinct,
     }
 
     filtered_params = {k: v for k, v in params.items() if v is not None}
 
     return {"endpoint": endpoint, "params": filtered_params}
```

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/data/asynchronous.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,22 +107,26 @@
 
 @async_data_request
 def async_sdr_count(
     start: Optional[int] = None,
     end: Optional[int] = None,
     repository: Optional[set[Repository]] = None,
     asset_class: Optional[set[AssetClass]] = None,
+    distinct: Optional[bool] = None,
 ) -> int:
     """
     Get SDR Data count.
 
     Args:
         start (Optional[int]): Unix timestamp for the start of the time window. If None, the beginning of time is used
         end (Optional[int]): Unix timestamp for the end of the time window. If None, the current time is used
         repository (Optional[set[Repository]]): Repository. If None, all repositories are included
         asset_class (Optional[set[AssetClass]]): Asset class. If None, all asset classes are included
+        distinct (Optional[bool]): Flag to determine whether distinct values should be counted
 
     Returns:
         int: Number of records
     """
-    request_info = _sdr_count_request_info(start, end, repository, asset_class)
+    request_info = _sdr_count_request_info(
+        start, end, repository, asset_class, distinct
+    )
     return __async_get_request(**request_info)
```

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/barchart/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/data/barchart/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/barchart/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/data/barchart/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/model.py` & `spotlight-sdk-0.1.4/spotlight/api/data/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/data/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/data/synchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,22 +107,26 @@
 
 @data_request
 def sdr_count(
     start: Optional[int] = None,
     end: Optional[int] = None,
     repository: Optional[set[Repository]] = None,
     asset_class: Optional[set[AssetClass]] = None,
+    distinct: Optional[bool] = None,
 ) -> int:
     """
     Get SDR Data count.
 
     Args:
         start (Optional[int]): Unix timestamp for the start of the time window. If None, the beginning of time is used
         end (Optional[int]): Unix timestamp for the end of the time window. If None, the current time is used
         repository (Optional[set[Repository]]): Repository. If None, all repositories are included
         asset_class (Optional[set[AssetClass]]): Asset class. If None, all asset classes are included
+        distinct (Optional[bool]): Flag to determine whether to return distinct records
 
     Returns:
         int: Number of records
     """
-    request_info = _sdr_count_request_info(start, end, repository, asset_class)
+    request_info = _sdr_count_request_info(
+        start, end, repository, asset_class, distinct
+    )
     return __get_request(**request_info)
```

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/model.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/abstract/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/abstract/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/model.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/view/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/view/model.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/view/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/dataset/view/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/dataset/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/permission/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/permission/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/permission/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/permission/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/permission/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/permission/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/model.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/rule/data_rule_result/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/rule/data_rule_result/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/sdr_source/__util.py` & `spotlight-sdk-0.1.4/spotlight/api/sdr_source/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/sdr_source/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/sdr_source/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/api/sdr_source/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/api/sdr_source/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/base.py` & `spotlight-sdk-0.1.4/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/config.py` & `spotlight-sdk-0.1.4/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/date/function.py` & `spotlight-sdk-0.1.4/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/__util.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/decorators/timeit.py` & `spotlight-sdk-0.1.4/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/enum.py` & `spotlight-sdk-0.1.4/spotlight/core/common/enum.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/errors.py` & `spotlight-sdk-0.1.4/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/function.py` & `spotlight-sdk-0.1.4/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/metaclass/singleton.py` & `spotlight-sdk-0.1.4/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/requests/asynchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight/core/common/requests/synchronous.py` & `spotlight-sdk-0.1.4/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.1.2/spotlight_sdk.egg-info/PKG-INFO` & `spotlight-sdk-0.1.4/spotlight_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.1.2
+Version: 0.1.4
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.1.2/spotlight_sdk.egg-info/SOURCES.txt` & `spotlight-sdk-0.1.4/spotlight_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

