# Comparing `tmp/wllegal-2023.5.tar.gz` & `tmp/wllegal-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wllegal-2023.5.tar", last modified: Thu Dec  7 15:58:54 2023, max compression
+gzip compressed data, was "wllegal-2024.1.tar", last modified: Wed May 29 11:35:24 2024, max compression
```

## Comparing `wllegal-2023.5.tar` & `wllegal-2024.1.tar`

### file list

```diff
@@ -1,379 +1,382 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-12-07 15:58:40.000000 wllegal-2023.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-07 15:58:40.000000 wllegal-2023.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2023-12-07 15:58:54.255716 wllegal-2023.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-07 15:58:40.000000 wllegal-2023.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-12-07 15:58:40.000000 wllegal-2023.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-07 15:58:40.000000 wllegal-2023.5/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-07 15:58:40.000000 wllegal-2023.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-12-07 15:58:54.255716 wllegal-2023.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1516 2023-12-07 15:58:40.000000 wllegal-2023.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18266 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/af/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43914 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22949 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    51506 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/be_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.231716 wllegal-2023.5/wllegal/locale/be_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23470 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/be_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.203716 wllegal-2023.5/wllegal/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18399 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    24835 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20022 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43488 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42003 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42315 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18371 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    27600 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    44928 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    18130 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    27107 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.235716 wllegal-2023.5/wllegal/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    35264 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.207716 wllegal-2023.5/wllegal/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20927 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43296 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22176 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20014 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    37064 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22554 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    44819 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19069 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/ga/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/ga/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18336 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ga/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42519 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    44531 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18485 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    41050 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    28356 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19639 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.239716 wllegal-2023.5/wllegal/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    41544 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.211716 wllegal-2023.5/wllegal/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ig/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ig/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ig/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    25296 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42728 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43550 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18364 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    28378 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    48302 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23574 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18417 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/kn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/kn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/kn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42878 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18894 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    25392 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18726 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18283 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.215716 wllegal-2023.5/wllegal/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    25685 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.243716 wllegal-2023.5/wllegal/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18868 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42063 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42667 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18104 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18345 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18295 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43062 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43282 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    41384 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    35265 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    37269 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    55547 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.219716 wllegal-2023.5/wllegal/locale/sai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/sai/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sai/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18150 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.247716 wllegal-2023.5/wllegal/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    39581 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19961 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21040 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43738 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23313 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    21122 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42198 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18465 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19222 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18415 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18254 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    43498 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18105 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.223716 wllegal-2023.5/wllegal/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    53453 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18259 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19597 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/yue_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.251716 wllegal-2023.5/wllegal/locale/yue_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18247 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/yue_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18586 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    38694 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    38409 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/settings_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.227716 wllegal-2023.5/wllegal/templates/legal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/templates/legal/documents/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/legal/documents/contracts.html
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/legal/documents/privacy.html
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/legal/documents/summary.html
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/legal/documents/tos.html
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/security.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/weblate_503.html
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templates/weblate_50x.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/templatetags/lawlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2023-12-07 15:58:40.000000 wllegal-2023.5/wllegal/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:58:54.255716 wllegal-2023.5/wllegal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2023-12-07 15:58:54.000000 wllegal-2023.5/wllegal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2023-12-07 15:58:54.000000 wllegal-2023.5/wllegal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 15:58:54.000000 wllegal-2023.5/wllegal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-07 15:58:54.000000 wllegal-2023.5/wllegal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-07 15:58:54.000000 wllegal-2023.5/wllegal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.271919 wllegal-2024.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-29 11:35:10.000000 wllegal-2024.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-29 11:35:10.000000 wllegal-2024.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-29 11:35:24.271919 wllegal-2024.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-29 11:35:10.000000 wllegal-2024.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-29 11:35:10.000000 wllegal-2024.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 11:35:10.000000 wllegal-2024.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 11:35:10.000000 wllegal-2024.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-29 11:35:24.271919 wllegal-2024.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1516 2024-05-29 11:35:10.000000 wllegal-2024.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.215919 wllegal-2024.1/wllegal/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.215919 wllegal-2024.1/wllegal/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/af/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.215919 wllegal-2024.1/wllegal/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.215919 wllegal-2024.1/wllegal/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.243919 wllegal-2024.1/wllegal/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    44407 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    51666 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23470 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18399 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    24835 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18305 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20022 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43488 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/chn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/chn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/chn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42003 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.219919 wllegal-2024.1/wllegal/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.247919 wllegal-2024.1/wllegal/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42315 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18371 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    29757 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    44928 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    18130 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    27294 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    35264 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20927 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43296 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22125 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37064 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22554 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    44819 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19069 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.251919 wllegal-2024.1/wllegal/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.223919 wllegal-2024.1/wllegal/locale/ga/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ga/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18336 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ga/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42963 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18541 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    41037 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19639 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    41544 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ig/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ig/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ig/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    24291 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42686 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43550 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    28378 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    48302 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.255919 wllegal-2024.1/wllegal/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23507 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18417 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/kn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/kn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/kn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.227919 wllegal-2024.1/wllegal/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42893 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18894 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    25392 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18726 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18283 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18868 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42794 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42667 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.259919 wllegal-2024.1/wllegal/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18345 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.231919 wllegal-2024.1/wllegal/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42632 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    35442 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37269 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    55551 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sai/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sai/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18150 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    39581 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21040 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43738 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23313 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.263919 wllegal-2024.1/wllegal/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    21100 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42198 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18465 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    45554 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.235919 wllegal-2024.1/wllegal/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19222 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18254 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    43498 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18105 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    53453 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19597 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18295 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18586 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    38694 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    38409 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/settings_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.267919 wllegal-2024.1/wllegal/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.239919 wllegal-2024.1/wllegal/templates/legal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.271919 wllegal-2024.1/wllegal/templates/legal/documents/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/legal/documents/contracts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/legal/documents/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/legal/documents/summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/legal/documents/tos.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/security.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/weblate_503.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templates/weblate_50x.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.271919 wllegal-2024.1/wllegal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/templatetags/lawlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 11:35:10.000000 wllegal-2024.1/wllegal/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:35:24.271919 wllegal-2024.1/wllegal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-29 11:35:24.000000 wllegal-2024.1/wllegal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-29 11:35:24.000000 wllegal-2024.1/wllegal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:35:24.000000 wllegal-2024.1/wllegal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 11:35:24.000000 wllegal-2024.1/wllegal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 11:35:24.000000 wllegal-2024.1/wllegal.egg-info/top_level.txt
```

### Comparing `wllegal-2023.5/LICENSE` & `wllegal-2024.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/PKG-INFO` & `wllegal-2024.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.5
+Version: 2024.1
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
```

### Comparing `wllegal-2023.5/README.rst` & `wllegal-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/pyproject.toml` & `wllegal-2024.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/setup.cfg` & `wllegal-2024.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wllegal
-version = 2023.5
+version = 2024.1
 description = Hosted Weblate legal stuff
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@cihar.com
 license = GPL-3.0-or-later
```

### Comparing `wllegal-2023.5/setup.py` & `wllegal-2024.1/setup.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ab/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/af/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/af/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/afh/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/afh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ang/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ang/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ar/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ar/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 # mohammadA <mohammadAbdulhadi1@gmail.com>, 2018, 2019.
 # Omar Aglan <omar.aglan91@yahoo.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-09-13 20:56+0000\n"
-"Last-Translator: Shadin <shadin_omari@yahoo.com>\n"
+"PO-Revision-Date: 2024-02-05 16:22+0000\n"
+"Last-Translator: ButterflyOfFire <boffire@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Arabic <https://hosted.weblate.org/projects/weblate/legal/ar/>"
 "\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 ? 4 : 5;\n"
-"X-Generator: Weblate 5.0.1-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "المقاولون من الباطن وفقا للفن. 28 اللائحة العامة لحماية البيانات"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -341,15 +341,15 @@
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "نحن نستخدم ملفات تعريف الارتباط لتقديم خدماتنا."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "نحن لا نستخدم أي ملفات تعريف ارتباط تابعة لجهات خارجية."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "عرض النسخة الإنجليزية"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -615,14 +615,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"بالمعنى المقصود في <a href=\"%(url)s\">المادة 7</a> من اللائحة العامة لحماية "
+"البيانات، يمنح المستخدم بموجب هذا الموافقة على جمع البيانات الشخصية وتخزينها "
+"ومعالجتها وفقًا لـ <a href=\"%(privacy_url)s \">سياسة الخصوصية</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "الترجمات"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
```

### Comparing `wllegal-2023.5/wllegal/locale/ar_LY/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ars/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ars/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ast/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/az/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/be/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/be/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Zmicer Turok <nashtlumach@gmail.com>, 2019, 2020.
 # Alex Ky <esthomolupus@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-12-07 03:06+0000\n"
+"PO-Revision-Date: 2023-12-11 19:23+0000\n"
 "Last-Translator: kopatych <maxklezovich@gmail.com>\n"
 "Language-Team: Belarusian <https://hosted.weblate.org/projects/weblate/legal/"
 "be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -109,14 +109,16 @@
 msgstr "Плацежная інфармацыя"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Калі вы купляеце нашы паслугі, мы збіраем даныя, неабходныя для выстаўлення "
+"рахунку."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Мэта і прававая аснова апрацоўкі асабістых даных"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
```

### Comparing `wllegal-2023.5/wllegal/locale/be_Latn/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ber/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ber/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/bg/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/bn/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/bn_BD/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/bo/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/bo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/br/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ca/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ce/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ce/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ckb/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ckb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/crh/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/crh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/cs/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/cv/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/cv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/cy/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/da/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/lv/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,216 +1,215 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# scootergrisen, 2018.
-# scootergrisen <scootergrisen@gmail.com>, 2018, 2019, 2020.
-# Allan Nordhøy <epost@anotheragency.no>, 2018.
-# anonymous <noreply@weblate.org>, 2019.
-# Henrik Dankvardt <dankvardt@gmail.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate\n"
+"Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-05-31 21:51+0000\n"
-"Last-Translator: Michael Millet <mikevlet@protonmail.com>\n"
-"Language-Team: Danish <https://hosted.weblate.org/projects/weblate/legal/da/>"
-"\n"
-"Language: da\n"
+"PO-Revision-Date: 2022-11-07 19:02+0000\n"
+"Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
+"Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/legal/lv/"
+">\n"
+"Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
+"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
+"X-Generator: Weblate 4.14.2\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Underleverandører i henhold til artikel 28 GDPR"
+msgstr "Apakšuzņēmēji saskaņā ar GDPR 28. pantu"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 #, fuzzy
 #| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Status per oktober 2020."
+msgstr "2020. gada oktobra statuss."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"Vi efterlever regulativ nr. %(law_679_2016)s, General Data Protection "
-"Regulation, også kendt som GDPR. Dette dokument indeholder de nødvendige "
-"specifikationer."
+"Mēs ievērojam regulu Nr. %(law_679_2016)s, Vispārīgo datu aizsardzības "
+"regulu, kas pazīstama arī kā GDPR. Šis dokuments iekļauj nepieciešamās "
+"specifikācijas."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "Personlig datastyring"
+msgstr "Personas datu pārvaldnieks"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, registreringsnummer %(reg_no)s"
+msgstr "%(provider)s, Reģ. Nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate har udpeget en databeskyttelsesansvarlig, der kan kontaktes via "
+"Weblate ir datu aizsardzības speciālists, ar kuru var sazināties, izmantojot "
 "%(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "Personlig data som behandlet af Weblate"
+msgstr "Personas dati, ko apstrādā Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"Weblate behandler kun personlig data som brugerne giver under brug af det:"
+"Weblate vietne apstrādā tikai tos Personas datus, ko Lietotājs pats "
+"iesniedzis, izmantojot mūsu pakalpojumu:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "Navn og e-mailadresse"
+msgstr "Vārds un e-pasta adrese"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 #, fuzzy
 #| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "De bruges til at identificere dig i VCS-indsendelserne"
+msgstr ""
+"Tie tiek izmantoti, lai identificētu jūs VCS iesniegtajās izmaiņās (commits)"
 
 #: wllegal/templates/legal/documents/privacy.html:27
 #, fuzzy
 #| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "E-mail bruges desuden til underretning af overvågede hændelser"
+msgstr ""
+"Turklāt e-pasts tiek izmantots, lai nosūtītu notikumu paziņojumus, kuriem "
+"jūs sekojiet"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Adgangskode er i hashed format"
+msgstr "Parole šifrētā (hashed) formā"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "Bruges til at godkende brugeren, hvis det er konfigureret"
+msgstr "Ja tas ir konfigurēts, izmanto, lai autorizētu lietotāju"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Adgangskoder gemmes hashet ved hjælp af Argon2."
+msgstr "Paroles tiek saglabātas šifrētas, izmantojot Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "IP-adresse og browsernavn"
+msgstr "IP adrese un pārlūkprogrammas nosaukums"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 #, fuzzy
 #| msgid ""
 #| "These are logged in case of important changes to your account (e.g. "
 #| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"De logges i tilfælde af vigtige ændringer på din konto (f.eks. ændring af "
-"adgangskode) så der kan diagnosticeres hvis din konto bliver stjålet"
+"Tie tiek reģistrēti, ja tiek veiktas svarīgas izmaiņas jūsu kontā (piemēram, "
+"paroles maiņa), lai varētu veikt diagnostiku konta nozagšanas gadījumā"
 
 #: wllegal/templates/legal/documents/privacy.html:36
 #, fuzzy
 #| msgid "Billing information"
 msgid "Billing info"
-msgstr "Faktureringsinformation"
+msgstr "Rēķinu informācija"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "Formålet og det lovgrundlaget for behandling af personlige data"
+msgstr "Personas datu apstrādes mērķis un juridiskais pamats"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Dine personlige data vil blive brugt til tjenestens formål:"
+msgstr "Jūsu personas dati tiks izmantoti pakalpojuma vajadzībām:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"til at levere vores tjenester på tjenesten, til at kontakte dig i spørgsmål "
-"vedrørende vores tjenester (også ved hjælp af e-mails og beskeder) og til at "
-"sikre den tekniske funktionalitet af vores tjenester opfyldelse af "
-"kontraktlige eller førkontraktlige forpligtelser (<a href=\"%(url)s"
-"\">Artikel 6 (1) b. GDPR</a>)"
+"nodrošināt mūsu pakalpojumus, kas saistīti ar pakalpojumu, un sazināties ar "
+"jums jautājumos par mūsu pakalpojumiem (tostarp izmantojot e-pastu un "
+"ziņojumapmaiņu) un būt pārliecinātiem par mūsu pakalpojumu tehnisko "
+"funkcionalitāti, pildot līgumsaistības vai pirmslīguma saistības (<a href="
+"\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"at analysere din brug af vores tjenester og forbedre vores tjenester (<a "
-"href=\"%(url)s\">Artikel 6 (1) b. og f. GDPR</a>)"
+"lai analizētu mūsu pakalpojumu izmantošanu un uzlabotu mūsu pakalpojumus (<a "
+"href=\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) un f) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"med dit udtrykkelige samtykke eller instruktion om at udføre vores "
-"forretningsaktiviteter eller sende dig nyhedsbreve (<a href=\"%(url)s"
-"\">Artikel 6, stk. 1, litra a. GDPR</a>)"
+"ar jūsu nepārprotamu piekrišanu vai norādījumiem, lai veiktu mūsu "
+"uzņēmējdarbību vai nosūtītu jums informatīvos izdevumus (<a href=\"%(url)s"
+"\">VDAR(GDPR) 6. panta 1. punkts a.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Adgang til den personlige data"
+msgstr "Piekļuve personas datiem"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
-"Den registeransvarlige har gjort alle rimelige tekniske midler til at "
-"beskytte personoplysningerne. Kun autoriserede personer kan få adgang til "
-"personoplysningerne."
+"Pārvaldnieks ir veicis visus saprātīgos tehniskos pasākumus personas datu "
+"aizsardzībai. Personas datiem var piekļūt tikai pilnvarotas personas."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
 msgstr ""
-"Tredjeparter, der kan få adgang til de personlige data, når det er "
-"nødvendigt, er:"
+"Trešās personas, kuras vajadzības gadījumā var piekļūt personas datiem:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr ""
-"Personer, der har indgået kontrakt for teknisk forsikring af tjenesten."
+msgstr "Personas, ar kurām noslēgts līgums par pakalpojuma tehnisko drošību."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Alle personlige data er lagret i den Europæiske Union."
+msgstr "Visi personas dati tiek glabāti Eiropas Savienībā."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
 msgid "Disclosure of the Personal Data"
-msgstr "Adgang til den personlige data"
+msgstr "Piekļuve personas datiem"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
@@ -223,340 +222,333 @@
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
-msgstr "Opbevaring af personoplysninger"
+msgstr "Tiesības uz personas datu glabāšanu"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"De personlige data gemmes i tjenesten, indtil brugeren sletter deres konto i "
-"tjenesten."
+"Personas datus pakalpojums uzglabā līdz brīdim, kad lietotājs izdzēš savu "
+"kontu."
 
 #: wllegal/templates/legal/documents/privacy.html:75
 #, fuzzy
 #| msgid ""
 #| "Access log information might be collected for a longer period for the "
 #| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Adgangslogoplysninger kan indsamles i en længere periode med henblik på at "
-"etablere, udøve eller forsvare juridiske krav."
+"Piekļuves žurnāla informācija var tikt vākta ilgāku laika periodu, lai "
+"celtu, izskatītu vai aizstāvētu juridiskās prasības tiesvedībā."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
-msgstr "Dine rettigheder"
+msgstr "Jūsu tiesības"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"Brugeren stiller frivilligt personoplysninger til rådighed for os. Uden "
-"disse personoplysninger er Weblate ikke i stand til at levere vores "
-"tjenester."
+"Lietotājs savus personas datu sniedz brīvprātīgi. Weblate nevar sniegt "
+"pakalpojumus bez šiem personas datiem."
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Vi ønsker, at du altid skal have kontrol over dine personlige oplysninger. "
-"Med henblik herpå har du visse rettigheder, der giver dig mulighed for det. "
-"Under visse betingelser kan du:"
+"Mēs vēlamies, lai jūs vienmēr varētu kontrolēt savu personisko informāciju. "
+"Šajā nolūkā jums ir atbilstošas tiesības, kas to atļauj. Noteiktos apstākļos "
+"jūs varat:"
 
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Få adgang til alle dine personlige data, som Weblate bruger eller behandler, "
-"og endda få en kopi af dem alle (<a href=\"%(url)s\">Artikel 15 GDPR</a>)"
+"Iegūt piekļuvi visiem saviem personas datiem, kurus Weblate izmanto vai "
+"apstrādā, kā arī iegūt to pilno kopiju (<a href=\"%(url)s\">VDAR(GDPR) 15. "
+"pants</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"Korrigere de personlige data, som Weblate behandler, hvis du mener, at der "
-"er fejl"
+"Labot personas datus, kurus Weblate apstrādā, ja domājat, ka tie satur kļūdas"
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid "Order us to delete your Personal Data"
-msgstr "Få os til at slette dine personlige oplysninger"
+msgstr "Pieprasīt mūs dzēst jūsu personas datus"
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
-msgstr "Begræns behandlingen af personoplysninger"
+msgstr "Ierobežot personas datu apstrādi"
 
 #: wllegal/templates/legal/documents/privacy.html:89
 msgid "Object to processing"
-msgstr "Indsigelse mod behandling"
+msgstr "Iebilst pret apstrādi"
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Modtag dine personoplysninger i et almindeligt anvendt og maskinlæsbart "
-"format eller for at overføre disse personoplysninger til en anden udbyder."
+"Iegūt savus personas datus parastā un mašīnlasāmā formātā vai pārsūtīt šos "
+"personas datus citam pakalpojuma sniedzējam."
 
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
+"Jūsu personas datu dzēšanu, labošanu vai ieguvi var veikt no kontu "
+"pārvaldības, un tā ir pilnībā automatizēta."
 
 #: wllegal/templates/legal/documents/summary.html:4
 #, fuzzy
 #| msgid ""
 #| "We process private data (such as your e-mail address), those will be "
 #| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Vi behandler private data (såsom din e-mailadresse). Disse vil blive slettet "
-"fra databasen, så snart kontoen fjernes."
+"Mēs apstrādājam privātos datus (piemēram, jūsu e-pasta adresi), tie tiks "
+"izdzēsti no mūsu datu bāzes, tiklīdz izdzēsīsit savu kontu."
 
 #: wllegal/templates/legal/documents/summary.html:5
 #, fuzzy
 #| msgid ""
 #| "Your translations are made under license which is specified by each "
 #| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Oversættelser er foretaget i henhold til licensen, som er angivet ved hver "
-"enkelt oversættelse."
+"Jūsu veiktie tulkojumi tiek izdoti saskaņā ar licenci, kas norādīta katram "
+"tulkošanas projektam."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
-msgstr "Navn og e-mail bruges i VCS-indsendelser, der bliver de for evigt."
+msgstr ""
+"Jūsu vārds un e-pasta adrese tiks izmantota versiju kontroles (VCS) "
+"iesniegtajās izmaiņās (commits), un tie paliek tur uz visiem laikiem."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
-msgstr "Vi bruger cookies til at levere vores tjenester."
+msgstr "Mēs izmantojam sīkfailus, lai nodrošinātu mūsu pakalpojumus."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Vis engelsk udgave"
+msgstr "Skatīt angļu valodas versiju"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Dokumentet Tjenestevilkår er autoritativt på engelsk, oversættelser leveres "
-"for din bekvemmelighed."
+"Pakalpojuma oficiālie lietošanas noteikumi ir dokumentēti angļu valodā, jūsu "
+"ērtībai tiek sniegti tulkojumi."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"Brugerens og udbyderens rettigheder og forpligtelser som følge af brugen af "
-"tjenesten er reguleret af disse vilkår for tjenesten."
+"Šie pakalpojuma noteikumi regulē lietotāja un pakalpojuma sniedzēja tiesības "
+"un pienākumus, kas rodas pakalpojuma izmantošanas rezultātā."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
-msgstr "Definitioner"
+msgstr "Definīcijas"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "I disse vilkår for tjeneste:"
+msgstr "Šajos pakalpojumu sniegšanas noteikumos:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "Aftale"
+msgstr "Līgums"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
-"betyder licensaftale som omhandlet i artikel 2358 ff. i den civillovbog, der "
-"er indgået af og mellem brugeren og udbyderen ved samtykket"
+"licences līgums (tādā nozīmē, kādā to interpretē ar Civilkodeksa 2358. "
+"pantu), kas noslēgts starp lietotāju un pakalpojuma sniedzēju ar viņu "
+"piekrišanu"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr "Civillovbog"
+msgstr "Civilkodekss"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
-msgstr "lov nr. %(law_89_2012)s Coll., den civile lovbog, som ændret"
+msgstr "likums Nr. %(law_89_2012)s Coll., Čehijas Civilkodekss ar grozījumiem"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr "Samtykke"
+msgstr "Vienošanās"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
-"betyder brugerens samtykke til disse servicevilkår og andre juridiske "
-"dokumenter, som kommer til udtryk ved at afkrydse afkrydsningsfeltet under "
-"registreringen"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Cookies"
+msgstr "Sīkdatnes"
 
 #: wllegal/templates/legal/documents/tos.html:36
-#, fuzzy
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
-"betyder enhver datafil, der sendes af tjenestens webserver til brugerens "
-"computer eller anden enhed, der er tilsluttet internettet, og som gør det "
-"muligt at opnå entydig identifikation af brugerens webbrowser"
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "GDPR"
+msgstr "VDAR(GDPR)"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
-"betyder EU-forordning nr. %(law_679_2016)s, den generelle "
-"databeskyttelsesforordning"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Licens"
+msgstr "Licence"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
-"betyder ikke-eksklusiv licens, som udbyderen har givet brugeren til brug af "
-"tjenesten"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "Udbyder"
+msgstr "Pakalpojumu sniedzējs"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr "betyder %(provider)s, Reg. nr. %(reg_no)s"
+msgstr "%(provider)s ar reģ. Nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Personlige Data"
+msgstr "Personas dati, Personiskie dati"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
-"betyder personoplysninger i henhold til EU-forordning nr. %(law_679_2016)s, "
-"som brugeren har indsat i tjenesten og/eller cookies"
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Ejer"
+msgstr "Īpašnieks"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "betyder den bruger, der kan administrere projektet"
+msgstr "lietotājs, kurš var pārvaldīt projektu"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekt"
+msgstr "Projekts"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "betyder oversættelsesprojekt som opererer på tjenesten"
+msgstr "tulkošanas projekts, kas tiek realizēts, izmantojot Pakalpojumu"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Tjeneste"
+msgstr "Pakalpojums"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"betyder hjemmesiden og tjenester baseret på Weblate, der drives af udbyderen"
+"uz Weblate balstīta tīmekļa vietne un pakalpojumi, ko nodrošina Pakalpojumu "
+"sniedzējs"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
-msgstr "Oversættelseshukommelse"
+msgstr "Tulkojumu atmiņa"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
-msgstr "den valgfrie oversættelseshukommelsestjeneste, der leveres i Weblate"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Bruger"
+msgstr "Lietotājs"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr "Versiju kontroles sistēma (VCS)"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
+"projektā izmantotā versiju kontroles sistēma, piemēram, Git vai Mercurial"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr ""
+msgstr "Licences līguma noslēgšana"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr ""
+msgstr "Licences līgums"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
 
@@ -616,15 +608,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "Oversættelser"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -692,110 +684,25 @@
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
-#~ "Dersom du køber en tjeneste fra os, så vil vi indsamle yderligere "
-#~ "nødvendige faktureringsoplysninger til udstedelse af faktura"
+#~ "Ja iegādājaties pakalpojumu no mums, mēs ievācam papildus informāciju, "
+#~ "kas nepieciešama rēķina izrakstīšanai"
 
 #~ msgid "Payment processors."
-#~ msgstr "Betalingsprocesser."
+#~ msgstr "Maksājumu apstrādātāji."
 
 #~ msgid ""
 #~ "The services are provided “as is”, at your own risk, without any warranty."
 #~ msgstr ""
-#~ "Tjenesterne leveres, \"som de er\", på egen risiko, uden nogen form for "
-#~ "garanti."
+#~ "Pakalpojumi tiek sniegti “tādi, kādi tie ir”, uz jūsu risku un "
+#~ "atbildības, bez jebkādas garantijas."
 
 #~ msgid ""
 #~ "Additional guarantees might apply to commercial customers, those are "
 #~ "expressed in corresponding contracts."
 #~ msgstr ""
-#~ "Yderligere garantier kan anvendes til kommercielle kunder, de er udtrykt "
-#~ "i de respektive kontrakter."
-
-#~ msgid "Reset all changes in the local repository"
-#~ msgstr "Nulstil alle ændringer i det lokale arkiv"
-
-#~ msgid "Billing"
-#~ msgstr "Fakturering"
-
-#~ msgid "Create new billing plan"
-#~ msgstr "Opret ny betalingsplan"
-
-#~ msgid "Create billing plan"
-#~ msgstr "Opret betalingsplan"
-
-#~ msgid "New billing plan"
-#~ msgstr "Ny betalingsplan"
-
-#~ msgid "Please choose a hosting plan that fits the size of your project."
-#~ msgstr ""
-#~ "Vælg venligst den hostingplan der bedst passer størrelsen af dit projekt."
-
-#~ msgid "Current billing status"
-#~ msgstr "Nuværende betalingsstatus"
-
-#~ msgid "Too small for your project."
-#~ msgstr "For lille til dit projekt."
-
-#~ msgid "Too small"
-#~ msgstr "For lille"
-
-#~ msgid "Selected plan"
-#~ msgstr "Valgte plan"
-
-#~ msgid "Current plan"
-#~ msgstr "Nuværende plan"
-
-#~ msgid "Strings limit"
-#~ msgstr "Begrænsning for strenge"
-
-#~ msgid "Unlimited"
-#~ msgstr "Ubegrænset"
-
-#~ msgid "Languages limit"
-#~ msgstr "Sproggrænse"
-
-#~ msgid "Component limit"
-#~ msgstr "Komponents grænse"
-
-#~ msgid "Projects limit"
-#~ msgstr "Projektets grænse"
-
-#~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR / måned"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s EUR / år"
-
-#~ msgid ""
-#~ "Pricing is based on the number of source strings and target languages. "
-#~ "The source string is a text unit defined in a translation format, it can "
-#~ "be a word, sentence or paragraph."
-#~ msgstr ""
-#~ "Prissætningen er baseret på antallet af kildestrenge og målsprog. "
-#~ "Kildestrengen er en tekstenhed defineret i et oversættelsesformat, kan "
-#~ "være et ord, sætning eller afsnit."
-
-#~ msgid "The payment was rejected: {}"
-#~ msgstr "Betalingen blev afvist: {}"
-
-#~ msgid "Unknown reason"
-#~ msgstr "Ukendt årsag"
-
-#~ msgid "Payments are temporarily inactive."
-#~ msgstr "Betalinger er midlertidigt inaktive."
-
-#~ msgid "Payment card"
-#~ msgstr "Betalingskort"
-
-#~ msgid "Payment error"
-#~ msgstr "Fejl ved betaling"
-
-#~ msgid "Monthly"
-#~ msgstr "Månedlig"
-
-#~ msgid "Repositories limit"
-#~ msgstr "Begrænsning for arkiv"
+#~ "Papildu garantijas var būt spēkā maksas (komerciāliem) klientiem, tās ir "
+#~ "aprakstītas attiecīgajos līgumos."
```

### Comparing `wllegal-2023.5/wllegal/locale/de/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/django.pot` & `wllegal-2024.1/wllegal/locale/django.pot`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/dv/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/dv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/el/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/el/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # THANOS SIOURDAKIS <siourdakisthanos@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2021-12-16 08:54+0000\n"
-"Last-Translator: george kitsoukakis <norhorn@gmail.com>\n"
-"Language-Team: Greek <https://hosted.weblate.org/projects/weblate/legal/el/"
-">\n"
+"PO-Revision-Date: 2023-12-31 09:01+0000\n"
+"Last-Translator: Michalis <michalisntovas@yahoo.gr>\n"
+"Language-Team: Greek <https://hosted.weblate.org/projects/weblate/legal/el/>"
+"\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Υπεργολάβοι σύμφωνα με το άρθρο. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 #, fuzzy
@@ -327,14 +327,16 @@
 msgstr "Προβολή αγγλικής έκδοσης"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
+"Το έγγραφο των Όρων χρήσης είναι έγκυρο στα αγγλικά, οι μεταφράσεις "
+"παρέχονται για τη διευκόλυνσή σας."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/en_GB/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/enm/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/enm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/eo/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/es/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/et/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/et/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,39 +2,37 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 # Janar Leas <janar.leas@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-03-10 11:02+0000\n"
-"Last-Translator: Priit Jõerüüt <hwlate@joeruut.com>\n"
+"PO-Revision-Date: 2024-02-26 17:31+0000\n"
+"Last-Translator: Lauri Linnamäe <de0g7o8f@duck.com>\n"
 "Language-Team: Estonian <https://hosted.weblate.org/projects/weblate/legal/"
 "et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 "Alltöövõtjate tegevus toimub vastavalt Isikuandmete Kaitse Üldmääruse "
 "artiklile 28"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "2020. aasta oktoobri seisuga."
+msgstr "2023. aasta märtsi seisuga."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -410,15 +408,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Isiklik teave"
+msgstr "Isiklikud andmed"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/eu/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/eu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Osoitz <oelkoro@gmail.com>, 2018.
 # Michal Čihař <michal@cihar.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 # S <sendoasojo@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2020-04-08 03:31+0000\n"
-"Last-Translator: BiziA <adrianpena.hf@gmail.com>\n"
-"Language-Team: Basque <https://hosted.weblate.org/projects/weblate/legal/eu/"
-">\n"
+"PO-Revision-Date: 2024-01-16 22:06+0000\n"
+"Last-Translator: Alexander Gabilondo <alexgabi@openmailbox.org>\n"
+"Language-Team: Basque <https://hosted.weblate.org/projects/weblate/legal/eu/>"
+"\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.0-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -386,15 +386,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Datu pertsonalak"
+msgstr "Informazio pertsonala"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/fa/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/fi/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/fil/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fil/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/fr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/fur/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fur/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/fy/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/fy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ga/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ga/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/gl/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/gl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,754 +5,743 @@
 # Iván Seoane <ivanrsm1997@gmail.com>, 2018, 2019.
 # Iváns <ivanrsm1997@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-06-30 17:49+0000\n"
-"Last-Translator: Xosé Calvo <xosecalvo@gmail.com>\n"
+"PO-Revision-Date: 2024-04-13 08:01+0000\n"
+"Last-Translator: \"Miguel A. Bouzada\" <mbouzada@gmail.com>\n"
 "Language-Team: Galician <https://hosted.weblate.org/projects/weblate/legal/"
 "gl/>\n"
 "Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Subcontratistas de acordo co art. 28 GDPR"
+msgstr "Subcontratistas en conformidade co art. 28 do RXPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
-msgstr "Estado a outubro de 2023."
+msgstr "Estado en marzo de 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"Cumprimos ca lei número %(law_679_2016)s, a normativa xeral da protección de "
-"datos, tamén coñecida coma a RGPD. Este documento inclúe as especificacións "
-"precisadas."
+"Cumprimos co Regulamento %(law_679_2016)s, o Regulamento Xeral de Protección "
+"de Datos, tamén coñecido coma a RXPD. Este documento inclúe as "
+"especificacións precisas."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "Control dos datos persoais"
+msgstr "Delegado de Protección de Datos"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, número do rexistro %(reg_no)s"
+msgstr "%(provider)s, núm. de rexistro %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"O Weblate definiu un responsábel de protección de datos que pode ser "
-"contactado a través de %(privacy_contact)s."
+"Weblate designou un delegado de protección de datos co que pode contactar a "
+"través de %(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "Datos persoais procesados polo Weblate"
+msgstr "Datos persoais procesados por Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"O Weblate procesa de xeito único os datos persoais que o usuario fornece ó "
-"empregalo:"
+"Weblate só procesa os datos persoais que o «Usuario» fornece ao empregalo:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "Nome e enderezo do correo electrónico"
+msgstr "Nome e enderezo de correo-e"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Estes empréganse para identificarlle nas confirmacións VCS"
+msgstr "Empréganse para identificalo (a Vde.) nos «commits» no SCV."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Ademais, o correo electrónico emprégase para a notificación dos "
-"acontecementos observados"
+"Alén diso, emprégase o correo-e para notificar os eventos monitorizados."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Contrasinal en forma de 'hash'"
+msgstr "Contrasinal en forma de resumo criptográfico"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "Emprégase para autenticar ó usuario se está configurado"
+msgstr "Emprégase para autenticar ao «Usuario», se está configurado"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Os contrasinais almacénanse con hash usando Argon2."
+msgstr ""
+"Os contrasinais almacénanse como resumo criptográfico empregando Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "Enderezo IP e nome do navigador"
+msgstr "Enderezo IP e nome do navegador"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Estes rexístranse no caso de mudanzas importantes na súa conta (por exemplo, "
-"mudado do contrasinal) para permiti-lo diagnóstico no caso de que a súa "
-"conta sexa roubada"
+"Rexístranse no caso de cambios importantes na súa conta (p. ex., cambio do "
+"contrasinal) para permitir o diagnóstico no caso de que a súa conta sexa "
+"roubada."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Informacións de pagamentos"
+msgstr "Información de facturación"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Os datos necesarios para emitir unha factura recóllense ao mercar un servizo "
+"con nós."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "Obxectivo e bases legais para o procesamento dos datos personais"
+msgstr "Finalidade e base xurídica do tratamento de datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Os seus datos persoais só serán empregados con obxectivos do servizo:"
+msgstr "Os seus datos persoais só serán empregados para os fins do «Servizo»:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"por dar os nosos servizos no \"Servizo\", para contactar con problemas dos "
-"nosos servizos (tamén coma método de correos elec. e mensaxes) e para "
-"asegura-las funcionalidades técnicas do noso servizo cumpren cas obrigas "
-"contractuais e precontractuais (<a href=\"%(url)s\">Artigo 6 (1) b. RGPD</a>)"
+"para prestar os nosos servizos no «Servizo», contactar con Vde. en asuntos "
+"relacionados cos nosos servizos (tamén por medio de correos-e e mensaxes) e "
+"garantir a funcionalidade técnica do noso servizo e o cumprimento das "
+"obrigacións contratuais ou precontratuais (<a href=\"%(url)s\">Artigo 6 (1) "
+"b. RXPD</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"para analizar o teu emprego dos servizos e mellorar os nosos servizos (<a "
+"para analizar o emprego dos nosos servizos pola súa parte e melloralos (<a "
 "href=\"%(url)s\">Artigo 6 (1) b. e f. RGPD</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"co teu consentemento expreso ou indicación de facer as nosas actividades de "
-"negocio ou enviar boletíns de novas (<a href=\"%(url)s\">Artigo 6 (1) a. "
-"RGPD</a>)"
+"co seu consentimento explícito ou autorización para desenvolver as nosas "
+"actividades comerciais ou enviarlle boletíns informativos (<a href=\"%(url)"
+"s\">Artigo 6 (1) a. RXPD</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Acceso ós datos persoais"
+msgstr "Acceso aos datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
-"A empresa fixo os esforzos precisados para protexer os datos persoais. Só "
-"persoas autorizadas teñen o acceso ós datos persoais."
+"O Delegado de Protección de Datos (DPD) empregou todos os medios técnicos "
+"razoables para protexer os datos persoais. Só persoas autorizadas poden "
+"acceder aos datos persoais."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
 msgstr ""
-"Os terceiros que poden conseguer acceso ós datos persoais necesariamente son:"
+"Os terceiros que poden acceder aos datos persoais cando sexa necesario son:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr "Persoas que son contratadas para a seguranza técnica do servizo."
+msgstr "Persoas contratadas para a seguranza técnica do servizo."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Procesadores de pagamentos ao mercar un servizo noso."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Tódolos datos persoais son almacenados na Unión Europea."
+msgstr "Todos os datos persoais están almacenados na Unión Europea."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
 msgid "Disclosure of the Personal Data"
-msgstr "Acceso ós datos persoais"
+msgstr "Divulgación dos datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Os datos persoais poden ser revelados a terceiros en circunstancias "
+"limitadas cando o Delegado de Protección de Datos (DPD) crea de boa fe que "
+"así o esixe a lei, como por virtude dunha citación ou outra orden xudicial "
+"ou administrativa."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"No caso de que o Delegado de Protección de Datos (DPD) estea obrigado por "
+"lei a revelar os datos persoais, realizarase un intento de notificar "
+"previamente ao «Usuario» por correo-e (a menos que o DPD o teña prohibido ou "
+"sexa inútil) de que foi feita unha solicitude dos seus datos persoais para "
+"permitirlle ao «Usuario» oporse á revelación. Se o «Usuario» non impugna a "
+"solicitude de revelación, o DPD pode estar legalmente obrigado a entregar os "
+"datos persoais."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
-msgstr "A conservación dos datos persoais"
+msgstr "A retención de datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"Os datos persoais son almacenados no servizo até que o usuario elimine a súa "
-"conta no servizo."
+"Os datos persoais son almacenados no «Servizo» ata que o «Usuario» elimine a "
+"súa conta no servizo."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"A información dos accesos á cuenta serán almacenados por máis tempo co "
-"obxectivo do estabelecemento, exercitamento ou defensa das demandas "
-"xudiciais."
+"Pódese recoller información do rexistro de acceso durante un período máis "
+"longo coa finalidade de estabelecer, exercer ou defender reclamacións legais."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Os seus dereitos"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"O usuario fornece de xeito voluntario acceso ós seus datos persoais. Sen "
-"estes datos, o Weblate non podería ofrecer os seus servizos."
+"O «Usuario» fornece o uso dos seus datos persoais voluntariamente. Sen estes "
+"datos persoais, Weblate non pode prestar os servizos."
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Nós desexamos que sempre manteña o control dos seus datos persoais. Por iso "
-"vostede ten certos dereitos que lle amparan. Baixo o abeiro de certas "
-"circunstancias, vostede pode:"
+"Queremos que teña sempre o control dos seus datos persoais. Para iso, Vde, "
+"ten certos dereitos que o permiten. En determinadas condicións, pode:"
 
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Para conseguir o acceso a tódolos teus datos persoais que estamos a empregar "
-"ou a procesar, e incluso conseguir unha copia de todo iso (<a href=\"%(url)s"
-"\">Artigo 15 da RGPD</a>)"
+"Obter acceso a todos os seus datos persoais que Weblate utiliza ou procesa e "
+"incluso obter unha copia completa dos mesmos (<a href=\"%(url)s\">Artigo 15 "
+"do RXPD</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"Corrixir dos datos persoais procesados polo Weblate se cres que teñen erros"
+"Corrixa os datos persoais procesados por Weblate se considera que hai erros"
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid "Order us to delete your Personal Data"
-msgstr "Pregar que eliminemos os seus datos persoais"
+msgstr "Indíquenos que eliminemos os seus datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
-msgstr "Restrinxi-lo proceso dos datos persoais"
+msgstr "Restrinxir o tratamento de datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:89
 msgid "Object to processing"
-msgstr "Obxecto do procesamento"
+msgstr "Oporse ao procesamento"
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Recibi-los seus datos persoais nun formato de emprego corrente e lexíbel por "
-"calquera computador ou para transmitir estes datos persoais cara un "
-"fornecedor diferente."
+"Reciba os seus datos persoais nun formato de uso habitual e lexíbel por "
+"máquinas ou para transmitírllelos a un provedor diferente."
 
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "A eliminación, corrección e recuperación dos seus datos persoais pódese "
-"facer desde a xestión da conta e estopase enteira automatizada."
+"facer dende a xestión da conta e está totalmente automatizada."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Procesamos datos privados (coma o enderezo do correo electrónico), estes "
-"desbotaranse da nosa base de datos ó elimina-la súa cuenta."
+"Procesamos os datos persoais (como o seu enderezo de correo-e); desbotaranse "
+"da nosa base de datos se elimina a súa conta."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "As súas traducións fanse baixo licenza especifica de cada tradución."
+msgstr ""
+"As súas traducións fainas baixo a licenza que se especifica de cada "
+"tradución."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
-"O su nome e mailo seu enderezo do correo electrónico empréganse en envíos do "
-"VCS, e ficarán alí de xeito indefinido."
+"O seu nome e mailo seu enderezo do correo-e empréganse en «commits» do SCV, "
+"e permanecerán alí de xeito indefinido."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"O nome escollido depende de Vde. e o enderezo de correo-e utilizado para as "
+"confirmacións pódese enmascarar polo sistema Weblate para protexer a súa "
+"privacidade."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
-msgstr "Empregamos cookies para fornece-los nosos servizos."
+msgstr "Empregamos cookies para ofrecer os nosos servizos."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Non empregamos cookies de terceiros."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Ollar versión en inglés"
+msgstr "Ver a versión en inglés"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"O documento dos Termos do Servizo autorizado está en inglés, as traducións "
-"fornécense para a súa conveniencia."
+"O documento vinculante das Condicións do Servizo está en inglés, as "
+"traducións fornécense para a súa comodidade."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"Os dereitos e obligacións do usuario e do fornecedor coma resultado do uso "
-"do servizo ríxense por estes Termos do Servizo."
+"Os dereitos e obrigas do «Usuario» e do«Fornecedor» como resultado do uso do "
+"«Servizo» determínanse por estas Condicións do Servizo."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
 msgstr "Definicións"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "Nestes Termos do Servizo:"
+msgstr "Nestas Condicións do Servizo:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
 msgstr "Acordo"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
-"significa Acordo de Licenza segundo o artigo 2358 do Código Civil conclúe "
-"por e entre o usuario e o fornecedor co consentemento"
+"refírese ao Acordo de Licenza no sentido dos artigos 2358 e ss. do Código "
+"Civil celebrado por e entre o «Usuario» e o «Fornecedor» mediante "
+"consentimento"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
 msgstr "Código civil"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
 msgstr ""
-"significa o número de lei %(law_89_2012)s, do Código Civil, tal e coma "
-"enmendouse"
+"refírese á Lei núm. %(law_89_2012)s Coll., do Código Civil, segundo a súa "
+"modificación"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr "Consentemento"
+msgstr "Consentimento"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
-"significa o consentemento do Usuario con estes Termos do Servizo e outros "
-"documentos legais expresados marcando a cela de verificación mentres "
-"transcorre o rexistro"
+"refírese ao consentimento do «Usuario» con esas Condicións do Servizo e "
+"outros documentos legais expresados marcando a caixa de verificación durante "
+"o rexistro"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
 msgstr "Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
-"refírese a calquera ficheiro de datos enviado polo servidor web do Servizo ó "
-"computador do Usuario ou cara outro dispositivo conectado á Internet, que "
-"permita obter unha identificación única do navegador web do Usuario"
+"refírese a calquera ficheiro de datos enviado polo servidor web do «Servizo» "
+"ao computador do «Usuario» ou cara a outro dispositivo conectado á Internet, "
+"que permita obter unha identificación única do navegador web do «Usuario»"
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "RGPD"
+msgstr "RXPD"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
-"significa o Regulamento da UE No.%(law_679_2016)s, o Regulamento Xeral de "
+"refírese ao Regulamento da UE núm. %(law_679_2016)s, o Regulamento Xeral de "
 "Protección de Datos"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
 msgstr "Licenza"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
-"refírese á licenza non exclusiva outorgada polo Fornecedor ó Usuario para o "
-"seu uso do Servizo"
+"refírese á licenza non exclusiva outorgada polo «Fornecedor» ao «Usuario» "
+"para o uso do «Servizo»"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
 msgstr "Fornecedor"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr "significa %(provider)s, Número de Rexistro %(reg_no)s"
+msgstr "refírese a %(provider)s, núm. de rexistro %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
 msgstr "Datos persoais"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
-"significa que os datos persoais no senso do Regulamento da UE No. "
-"%(law_679_2016)s inseridos polo Usuario no Servizo e/ou Cookies"
+"refírese aos datos persoais no senso do Regulamento da UE No. %(law_679_2016)"
+"s inseridos polo «Usuario» no «Servizo» e/ou nas cookies"
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Dono"
+msgstr "Propietario"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "significa o usuario que pode xestiona-lo Proxecto"
+msgstr "refírese ao «Usuario» que pode xestionar o proxecto"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
 msgstr "Proxecto"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "significa proxecto de tradución xestionado no Servizo"
+msgstr "refírese ao proxecto de tradución xestionado no «Servizo»"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
 msgstr "Servizo"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"significa que a páxina web e os servizos baseados no Weblate son xestionados "
-"polo fornecedor"
+"refírese a que a páxina web e os servizos baseados en Weblate son operados "
+"polo «Fornecedor»"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
 msgstr "Memoria de tradución"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
-"refírese ó servizo opcional da memoria de tradución fornecido polo Weblate"
+"refírese ao servizo opcional de memoria de tradución fornecido por Weblate"
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
 msgstr "Usuario"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
-"significa calquera entidade legal ou individual diferente ó Proveedor, que "
-"estea a emprega-lo Servizo"
+"refírese a calquera entidade legal ou individual diferente ao «Fornecedor», "
+"que estea a empregar o «Servizo»"
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
 msgstr "Sistema do Control de Versións (VCS)"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
-"o sistema de control das versións distribuído empregado polo proxecto, coma "
-"o Git ou o Mercurial"
+"refírese ao sistema de control de versións distribuído empregado polo "
+"proxecto, como Git ou o Mercurial"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr "Remate do Acordo da Licenza"
+msgstr "Conclusión do Acordo de Licenza"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
-"Conclúese co Acordo da Licenza ca aceptación do usuario dunha proposta do "
-"fornecedor."
+"O Acordo de Licenza conclúese coa aceptación por parte do «Usuario» da "
+"oferta do «Fornecedor»."
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr "Acordo da Licenza"
+msgstr "Acordo de Licenza"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
-"Ó remata-lo Acordo de conformidade co artigo 2.1 deste Acordo, as seguintes "
-"disposicións deste artigo 3 dos Termos do Servizo entran en vigor."
+"Ao concluír o acordo en virtude do artigo 2.1 deste acordo, terán efecto as "
+"seguintes disposicións deste artigo 3 das Condicións do Servizo."
 
 #: wllegal/templates/legal/documents/tos.html:80
 msgid ""
 "The Provider presents the User with a License Agreement and the User accepts "
 "this License Agreement, all this under the terms and conditions stated in "
 "these Terms of Service."
 msgstr ""
-"O Fornecedor presenta ó Usuario un Contrato de Licenza e o Usuario acepta "
-"este Contrato de Licenza, todo iso baixo os termos e condicións "
-"estabelecidos nestes Termos de Servizo."
+"O «Fornecedor» presenta ao «Usuario» un Acordo de Licenza e o «Usuario» "
+"acepta este Acordo de Licenza, todo iso baixo os termos e condicións "
+"estabelecidos nestas Condicións do Servizo."
 
 #: wllegal/templates/legal/documents/tos.html:82
 msgid ""
 "The Provider shall have the right to shut down, adjust, modify or make the "
 "Service unavailable on the web address at any time."
 msgstr ""
-"O Fornecedor terá dereito a pechar, axustar, modificar ou facer que o "
-"Servizo non esté dispoñíbel no enderezo web en calquera intre."
+"O «Fornecedor» terá dereito a pechar, axustar, modificar ou facer que o "
+"«Servizo» non estea dispoñíbel no enderezo web en calquera momento."
 
 #: wllegal/templates/legal/documents/tos.html:84
 msgid ""
 "The User agrees to use the Service only in a manner not jeopardizing "
 "technical software and/or hardware means of the Provider and/or such means "
 "in the Provider’s use."
 msgstr ""
-"O Usuario comprométese a emprega-lo Servizo soamente de xeito que non poña "
-"en perigo os medios técnicos de software e/ou hardware do Fornecedor e/ou "
-"devanditos medios no uso do Fornecedor."
+"O «Usuario» comprométese a empregar o «Servizo» soamente de xeito que non "
+"poña en perigo os medios técnicos de software e/ou hardware do «Fornecedor» "
+"e/ou devanditos medios no uso do «Fornecedor»."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
 msgstr ""
-"O Usuario comprométese a absterse de emprega-lo Servizo de má fe e/ou de "
-"causar de xeito deliberado calquera dano ó Servizo."
+"O «Usuario» comprométese a absterse de empregar o «Servizo» de mala fe e/ou "
+"de causar de xeito deliberado calquera dano ao «Servizo»."
 
 #: wllegal/templates/legal/documents/tos.html:88
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
-"O Usuario comprométese a absterse de eludi-los medios de software e/ou "
-"hardware técnico do Servizo, de xeito particular os sistemas de seguranza."
+"O «Usuario» comprométese a absterse de eludir os medios técnicos de software "
+"e/ou hardware do «Servizo», de xeito particular os sistemas de seguranza."
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
-msgstr "Responsabilidade polos danos e prexuízos"
+msgstr "Responsabilidade por danos e prexuízos"
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
 "The User hereby renders it undisputed that the Provider shall not be liable "
 "for any damage caused to the User resulting from the use of the Service."
 msgstr ""
-"O Usuario deixa craro que o Fornecedor non será responsábel de ningún dano "
-"feito ó Usuario coma resultado do emprego do Servizo."
+"O «Usuario» declara por este medio que o «Fornecedor» non será responsable "
+"por calquera dano causado ao «Usuario» como resultado do uso do «Servizo»."
 
 #: wllegal/templates/legal/documents/tos.html:95
 msgid ""
 "If the User is an entrepreneur, it hereby expressly waives its right to "
 "compensation from the Provider for damage unintentionally caused by the "
 "Provider to the User through a breach of any obligation contained in these "
 "Terms of Service and/or resulting from the use of the Service."
 msgstr ""
-"Se o Usuario é un empresario, desta maneira renuncia de xeito expreso ó seu "
-"dereito de compensación por parte do Fornecedor por danos feitos de xeito "
-"inintencionado polo Fornecedor ó Usuario a través do rompemento de calquera "
-"obligación contida nestes Termos do Servizo e/ou resultantes polo emprego do "
-"Servizo."
+"Se o «Usuario» é un empresario, renuncia expresamente ao seu dereito a unha "
+"indemnización por parte do «Fornecedor» polos danos causados non "
+"intencionalmente polo «Fornecedor» ao «Usuario» polo incumprimento de "
+"calquera obriga contida nas presentes Condicións do Servizo e/ou derivados "
+"do uso do «Servizo»."
 
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"No senso do <a href=\"%(url)s\">Artigo 7</a> do RXPD, o «Usuario» outorga o "
+"seu consentimento para a recollida, almacenamento e tratamento dos seus "
+"datos persoais segundo a <a href=\"%(privacy_url)s \">Directiva de "
+"privacidade</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Traducións"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
-"O Servizo organiza as traducións en Proxectos individuais, onde o Dono é "
-"responsábel na xestión deles e para cumprir con precisión a licenza do "
-"Proxecto."
+"O «Servizo» organiza as traducións en proxectos individuais, nos que o "
+"propietario é responsábel de xestionalos e de especificar con precisión a "
+"licenza do proxecto."
 
 #: wllegal/templates/legal/documents/tos.html:107
 msgid ""
 "Not specifying translation license means that the translations are available "
 "under same license as the given Project itself."
 msgstr ""
-"Se non se precisa licenza de tradución significa que as traducións están "
-"dispoñíbeis baixo a mesma licenza do proxecto."
+"Non especificar a licenza de tradución significa que as traducións están "
+"dispoñíbeis baixo a mesma licenza que o propio proxecto."
 
 #: wllegal/templates/legal/documents/tos.html:109
 msgid ""
 "Should the Project opt in for the Translation Memory, license to use the "
 "translation is granted to all Translation Memory users."
 msgstr ""
-"Se o Proxecto opta pola Memoria de tradución, a licenza de emprego da "
-"tradución outórgase a tódolos usuarios da Memoria de tradución."
+"Se o proxecto opta pola memoria de tradución, a licenza de uso da tradución "
+"outórgase a todos os usuarios da memoria de tradución."
 
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
-"O usuario concorda, ó contribuír para un proxecto, ca licenza que o proxecto "
-"especificou."
+"O Usuario acepta, ao facer achegas a un proxecto, a licenza especificada "
+"polo proxecto."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"O Usuario acepta o emprego do seu nome e email coma autoría nas "
-"consolidacións no Sistema de Control das Versións (SCV). O usuario entende "
-"que esta aceptación non é revogábel pola natureza do SCV."
+"O «Usuario» acepta o emprego do seu nome e correo-e como autoría nos "
+"«commits» ao SCV. O «Usuario» entende que esta aceptación non é revogábel "
+"por mor da natureza do SCV."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
-"No sentido do artigo 89 da Lei núm. %(law_480_2004)s Coll., das "
-"comunicacións electrónicas, na súa versión modificada, infórmase ao Usuario "
-"de que o Servizo utiliza Cookies."
+"No senso do artigo 89 da Lei núm. %(law_480_2004)s Coll., das comunicacións "
+"electrónicas, na súa versión modificada, infórmase ao «Usuario» de que o "
+"«Servizo» utiliza cookies."
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid "The Service uses Cookies to personalise content."
-msgstr "O Servizo utiliza cookies para persoalizar o contido."
+msgstr "O «Servizo» utiliza cookies para personalizar o contido."
 
 #: wllegal/templates/legal/documents/tos.html:123
 msgid "Governing Law"
 msgstr "Lei aplicábel"
 
 #: wllegal/templates/legal/documents/tos.html:125
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
-"Estas Condicións do Servizo rexeranse polas leis da República Checa con "
+"Estas Condicións do Servizo rexeranse polas leis da República Checa coa "
 "exclusión das regras de conflito."
 
 #: wllegal/templates/legal/documents/tos.html:127
 msgid ""
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
 msgstr ""
-"Calquera liorta que xorda sobre a base do Acordo e/ou destes Termos do "
+"Calquera disputa que xurda en base ao acordo e/ou a estas Condicións do "
 "Servizo será resolta polo tribunal da República Checa que teña xurisdición "
-"ou potestade sustantiva e local."
+"substantiva e local."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Efecto"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Estes Termos do Servizo entrarán en vixenza o 1 de setembro do 2017."
+msgstr ""
+"Estas Condicións do Servizo terán efecto a partir do 15 de maio de 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "No caso de que merques o noso servizo, colleitamos informacións "
 #~ "adicionais de pagamento necesarias para a emisión dun pagamento"
```

### Comparing `wllegal-2023.5/wllegal/locale/he/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/hi/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/hi/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2022-10-17 00:57+0000\n"
-"Last-Translator: Ritwik <ritwikraghav14@gmail.com>\n"
-"Language-Team: Hindi <https://hosted.weblate.org/projects/weblate/legal/hi/"
-">\n"
+"PO-Revision-Date: 2024-02-29 10:01+0000\n"
+"Last-Translator: Scrambled777 <weblate.scrambled777@simplelogin.com>\n"
+"Language-Team: Hindi <https://hosted.weblate.org/projects/weblate/legal/hi/>"
+"\n"
 "Language: hi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "जीडीपीआर अनुच्छेद 28 GDPR के अनुसार उपठेकेदार"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 #, fuzzy
@@ -382,15 +382,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "व्यक्तिगत डेटा"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/hr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/hr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Milo Ivir <mail@milotype.de>, 2019, 2020.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-11-05 13:34+0000\n"
+"PO-Revision-Date: 2024-01-26 18:43+0000\n"
 "Last-Translator: Milo Ivir <mail@milotype.de>\n"
 "Language-Team: Croatian <https://hosted.weblate.org/projects/weblate/legal/"
 "hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Podugovarači sukladno čl. 28 GDPR-a"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -55,31 +55,31 @@
 "%(privacy_contact)s."
 msgstr ""
 "Weblate je imenovao službenu osobu za zaštitu podataka, a može je se "
 "kontaktirati putem %(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr "Osobni podaci koje Weblate obrađuje"
+msgstr "Osobni podatci koje Weblate obrađuje"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 "Weblate obrađuje samo osobne podatke koje korisnik pruža pri upotrebi "
 "Weblatea:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Ime i e-adresa"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
-"Ovi se podaci koriste kako bi te se identificiralo u promjenama u sustavu za "
-"kontrolu verzija."
+"Ovi se podatci koriste kako bi te se identificiralo u promjenama u sustavu "
+"za kontrolu verzija."
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr "Dodatno tome se koristi e-mail za obavijesti praćenih događaja."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
@@ -98,36 +98,36 @@
 msgstr "IP adresa i ime preglednika"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Ovi se podaci bilježe u slučaju značajnih promjena u tvom računu (npr. "
+"Ovi se podatci bilježe u slučaju značajnih promjena u tvom računu (npr. "
 "promjena lozinke) i služe za dijagnozu u slučaju da se tvoj račun ukrade."
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing info"
-msgstr "Podaci naplate"
+msgstr "Podatci naplate"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
-"Potrebni podaci za izdavanje računa prikupljaju se prilikom kupnje jedne od "
+"Potrebni podatci za izdavanje računa prikupljaju se prilikom kupnje jedne od "
 "naših usluga."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Svrha i pravna osnova za obradu osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "U svrhu pružanja usluge, tvoji osobni podaci koristit će se za:"
+msgstr "U svrhu pružanja usluge, tvoji će se osobni podatci koristiti za:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
@@ -158,89 +158,89 @@
 msgstr ""
 "uz tvoj izričiti pristanak ili nalog, za obavljanje naših poslovnih "
 "aktivnosti ili slanje biltena <a href=\"%(url)s\">Članak 6 (1) a. Opće "
 "uredbe o zaštiti podataka </a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Pristup osobnim podacima"
+msgstr "Pristup osobnim podatcima"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
 "Kontrolor je poduzeo sve odgovarajuće tehničke mjere za zaštitu osobnih "
-"podataka. Samo ovlaštene osobe imaju pristup osobnim podacima."
+"podataka. Samo ovlaštene osobe imaju pristup osobnim podatcima."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
-msgstr "Treće strane koje po potrebi mogu dobiti pristup osobnim podacima su:"
+msgstr "Treće strane koje po potrebi mogu dobiti pristup osobnim podatcima su:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Osobe s kojima je zaključen ugovor za tehničko osiguravanje usluge."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
 msgstr "Procesori plaćanja prilikom kupnje jedne od naših usluga."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Svi osobni podaci spremaju se u Europskoj uniji."
+msgstr "Svi osobni podatci se spremaju u Europskoj uniji."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 msgid "Disclosure of the Personal Data"
 msgstr "Otkrivanje osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
-"Osobni podaci se mogu otkriti trećim stranama u ograničenim okolnostima kada "
-"kontrolor u dobroj vjeri vjeruje da to zahtijeva zakon, kao što je sudski "
-"poziv ili jedan drugi sudski ili administrativni nalog."
+"Osobni podatci se mogu otkriti trećim stranama u ograničenim okolnostima "
+"kada kontrolor u dobroj vjeri vjeruje da to zahtijeva zakon, kao što je "
+"sudski poziv ili jedan drugi sudski ili administrativni nalog."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
 "U slučaju da kontrolor na osnovi zakona mora otkriti osobne podatke, pokušat "
 "će se prethodno obavijestiti korisnika putem e-maila (osim ako je to "
 "kontroloru zabranjeno ili ako bi bilo uzaludno) da je zahtjev za osobnim "
-"podacima napravljeno kako bi se korisniku omogućilo ulaganje prigovora na "
+"podatcima napravljeno kako bi se korisniku omogućilo ulaganje prigovora na "
 "otkrivanje. Ako korisnik ne ospori zahtjev za otkrivanje, kontrolor može "
 "biti zakonski obvezan predati osobne podatke."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Zadržavanje osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"Osobni podaci se spremaju u usluzi sve dok korisnik ne izbriše svoj račun na "
-"usluzi."
+"Osobni podatci se spremaju u usluzi sve dok korisnik ne izbriše svoj račun "
+"na usluzi."
 
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Podaci o pristupanjima mogu se prikupljati na duže vremensko razdoblje u "
+"Podatci o pristupanjima mogu se prikupljati na duže vremensko razdoblje u "
 "svrhu utvrđivanja, ostvarivanja ili zaštite pravnih zahtjeva."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Tvoja prava"
 
 #: wllegal/templates/legal/documents/privacy.html:79
@@ -252,52 +252,51 @@
 "ne može pružiti naše usluge."
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Želimo da uvijek imaš kontrolu nad svojim osobnim podacima. U tu svrhu imaš "
+"Želimo da uvijek upravljaš tvojim osobnim podatcima. U tu svrhu imaš "
 "određena prava koja to dopuštaju. Pod određenim uvjetima, možeš:"
 
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Dobiti pristup svim tvojim osobnim podacima koje Weblate koristi ili "
-"obrađuje, pa čak i dobiti kopiju svih podataka <a href=\"%(url)s\">Članak 15 "
-"Opće uredbe o zaštiti podataka </a>)"
+"Dobij pristup svim tvojim osobnim podatcima koje Weblate koristi ili "
+"obrađuje i dobij kopiju svih podataka <a href=\"%(url)s\">Članak 15 Opće "
+"uredbe o zaštiti podataka </a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
-msgstr ""
-"Ispraviti osobne podatke koje Weblate obrađuje, ako smatraš da ima grešaka"
+msgstr "Ispravi osobne podatke koje Weblate obrađuje ako smatraš da ima grešaka"
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid "Order us to delete your Personal Data"
-msgstr "Naručiti brisanje tvojih osobnih podataka"
+msgstr "Naruči brisanje tvojih osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
-msgstr "Ograničiti obradu osobnih podataka"
+msgstr "Ograniči obradu osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:89
 msgid "Object to processing"
-msgstr "Prigovoriti obradi podataka"
+msgstr "Prigovori obradi podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Primati svoje osobne podatke u uobičajenom i strojno čitljivom obliku ili "
+"Primi svoje osobne podatke u uobičajenom i strojno čitljivom obliku ili "
 "proslijediti te osobne podatke drugom pružatelju usluga."
 
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
@@ -305,15 +304,15 @@
 "izvršiti na stranici za upravljanje računom i potpuno je automatizirano."
 
 #: wllegal/templates/legal/documents/summary.html:4
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Obrađujemo osobne podatke (kao što je tvoja e-adresa). Ti se podaci "
+"Obrađujemo osobne podatke (kao što je tvoja e-adresa). Ti se podatci "
 "uklanjaju iz naše baze podataka ako ukloniš račun."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
@@ -453,24 +452,24 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr "znači %(provider)s, reg. br. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Osobni podaci"
+msgstr "Osobni podatci"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
-"znači osobni podaci u smislu EU uredbe br. %(law_679_2016)s koje je korisnik "
-"upisao u uslugu i/ili kolačiće"
+"znači osobni podatci u smislu EU uredbe br. %(law_679_2016)s koje je "
+"korisnik upisao u uslugu i/ili kolačiće"
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
 msgstr "Vlasnik"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
```

### Comparing `wllegal-2023.5/wllegal/locale/hu/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/hy/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/hy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ia/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ia/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/id/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ie/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ie/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ig/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ig/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/is/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/is/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-01-31 21:41+0000\n"
+"PO-Revision-Date: 2024-03-14 13:36+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
 "Language-Team: Icelandic <https://hosted.weblate.org/projects/weblate/legal/"
 "is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n % 10 != 1 || n % 100 == 11;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Undirverktakar í samræmi við grein nr. 28 í GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Staða miðað við október 2020."
+msgstr "Staða miðað við mars 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -69,26 +67,22 @@
 "að:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nafn og vefpóstfang"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Þetta er notað til þess að auðkenna þig í VCS-innleggjum"
+msgstr "Þetta er notað til þess að auðkenna þig í VCS-innleggjum."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
 "Auk þess er tölvupóstfangið notað til þess að senda út umbeðin tíðindi og "
-"fréttir"
+"fréttir."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Aðgangsorð með tætigildi (hash)"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -99,31 +93,25 @@
 msgstr "Lykilorð eru geymd dulrituð með Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-númer og heiti vafra"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Þetta er skráð til að nota ef mikilvægar breytingar verða á notandaaðgangnum "
 "þínum (t.d. breytingar á lykilorði) svo hægt sé að greina hvort aðgangnum "
-"þínum hafi verið stolið"
+"þínum hafi verið stolið."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Upplýsingar um greiðanda"
+msgstr "Greiðsluupplýsingar"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
 
@@ -197,16 +185,14 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Öll persónuleg gögn eru vistuð í Evrópusambandinu."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
 msgid "Disclosure of the Personal Data"
 msgstr "Aðgangur að persónulegum gögnum"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
@@ -232,18 +218,14 @@
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Persónulegar upplýsingar eru geymdar í þjónustunni þar til notandinn eyðir "
 "notandaaðgangi sínum úr þjónustunni."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Upplýsingum um innskráningu og aðgang gæti verið safnað yfir lengri tímabil "
 "í þeim tilgangi að styðja, framfylgja eða verjast lagalegum kröfum."
 
@@ -309,31 +291,23 @@
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Við vinnum með persónuleg gögn (eins og t.d. tölvupóstfangið þitt), þeim "
+"Við vinnum með persónuleg gögn (eins og t.d. tölvupóstfangið þitt); þeim "
 "verður eytt úr gagnagrunninum okkar um leið og þú eyðir notandaaðgangnum "
 "þínum."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Þýðingarnar þínar eru aðgengilegar með því notkunarleyfi sem tilgreint er "
 "fyrir hverja þýðingaskrá."
 
@@ -353,15 +327,15 @@
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Við notum vefkökur til að veita þjónustuna okkar."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Við notum engar vefkökur frá utanaðkomandi aðilum."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Skoða enska útgáfu textans"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -646,22 +620,16 @@
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:120
-#, fuzzy
-#| msgid ""
-#| "The Service uses Cookies to personalise content, and to analyse our "
-#| "traffic."
 msgid "The Service uses Cookies to personalise content."
-msgstr ""
-"Þjónustan notar vefkökur til að persónuaðlaga efni og til að greina "
-"netumferðina okkar."
+msgstr "Þjónustan notar vefkökur til að persónuaðlaga efni."
 
 #: wllegal/templates/legal/documents/tos.html:123
 msgid "Governing Law"
 msgstr "Gildandi lög"
 
 #: wllegal/templates/legal/documents/tos.html:125
 msgid ""
```

### Comparing `wllegal-2023.5/wllegal/locale/it/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # Valter Mura <valtermura@gmail.com>, 2019.
 # Valentina Grassi <vale.grassi11@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-11-09 17:57+0000\n"
-"Last-Translator: Massimo Pissarello <mapi68@gmail.com>\n"
+"PO-Revision-Date: 2024-01-15 10:06+0000\n"
+"Last-Translator: bovirus <roberto.boriotti@canon.it>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/weblate/legal/it/"
 ">\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 "X-Poedit-SourceCharset: UTF-8\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subappaltatori in conformità con l'Art. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
@@ -123,15 +123,15 @@
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Scopo e base giuridica del trattamento dei dati personali"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "I tuoi dati personali saranno utilizzati per gli scopi del servizio:"
+msgstr "I dati personali saranno usati per gli scopi del servizio:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
@@ -146,25 +146,25 @@
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"per analizzare il tuo utilizzo dei nostri servizi e migliorarli (<a href="
-"\"%(url)s\">Articolo 6 (1) b. e f. GDPR</a>)"
+"per analizzare l'uso dei nostri servizi e migliorarli (<a href=\"%(url)s\""
+">Articolo 6 (1) b. e f. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"con il tuo esplicito consenso od istruzioni per svolgere le nostre attività "
+"con il tuo consenso esplicito od istruzioni per svolgere le nostre attività "
 "commerciali od inviando newsletter (<a href=\"%(url)s\">Articolo 6 (1) a. "
 "del GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
 msgstr "Accesso ai dati personali"
 
@@ -368,16 +368,16 @@
 "fornite per comodità dell'utente."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"I diritti e gli obblighi dell'Utente e del Fornitore derivanti dall'utilizzo "
-"del Servizio sono regolati dai presenti Termini del servizio."
+"I diritti e gli obblighi dell'Utente e del Fornitore derivanti dall'uso del "
+"Servizio sono regolati dai presenti Termini del servizio."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
 msgstr "Definizioni"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
@@ -453,16 +453,16 @@
 msgstr "Licenza"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
-"indica una licenza non esclusiva concessa dal fornitore all'utente per "
-"l'utilizzo del servizio"
+"indica una licenza non esclusiva concessa dal fornitore all'utente per l'uso "
+"del servizio"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
 msgstr "Fornitore"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
@@ -587,15 +587,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:84
 msgid ""
 "The User agrees to use the Service only in a manner not jeopardizing "
 "technical software and/or hardware means of the Provider and/or such means "
 "in the Provider’s use."
 msgstr ""
-"L'Utente accetta di utilizzare il Servizio solo in modo da non mettere a "
+"L'Utente accetta di usare il Servizio solo in modo da non mettere a "
 "repentaglio il software e/o l'hardware del Fornitore e/o tali mezzi nell'uso "
 "del Fornitore."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
@@ -671,15 +671,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:109
 msgid ""
 "Should the Project opt in for the Translation Memory, license to use the "
 "translation is granted to all Translation Memory users."
 msgstr ""
 "Nel caso in cui il progetto opti per la memoria di traduzione, la licenza di "
-"utilizzo della traduzione viene concessa a tutti gli utenti della memoria di "
+"uso della traduzione viene concessa a tutti gli utenti della memoria di "
 "traduzione."
 
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/ja/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ka/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/kab/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/kab/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/kk/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/kk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/km/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/km/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Michal Čihař <michal@cihar.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-11-08 09:38+0000\n"
-"Last-Translator: កុសិនារា <kursinarapok@gmail.com>\n"
+"PO-Revision-Date: 2024-05-14 12:01+0000\n"
+"Last-Translator: សិទ្ធិការ្យ <setthikarpok@gmail.com>\n"
 "Language-Team: Khmer (Central) <https://hosted.weblate.org/projects/weblate/"
 "legal/km/>\n"
 "Language: km\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.6-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -30,26 +30,26 @@
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"យើងអនុវត្តតាមបទប្បញ្ញត្តិលេខ %(law_679_2016)s "
-"បទប្បញ្ញត្តិការពារទិន្នន័យទូទៅដែលត្រូវបានគេស្គាល់ថា GDPR ។ "
-"ឯកសារនេះរួមបញ្ចូលទាំងការបញ្ជាក់ចាំបាច់មួយចំនួន។"
+"យើងគោរពតាមបទប្បញ្ញត្តិលេខ %(law_679_2016)s នៃច្បាប់ការពារទិន្នន័យទូទៅ "
+"ក៏ត្រូវបានគេស្គាល់ថាជា GDPR ។ "
+"ឯកសារគោលនេះរួមបញ្ចូលទាំងព័ត៌មានលម្អិតចាំបាច់មួយចំនួន។"
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "ឧបករណ៍គ្រប់គ្រងទិន្នន័យផ្ទាល់ខ្លួន"
+msgstr "ការីត្រួតពិនិត្យទិន្នន័យផ្ទាល់ខ្លួន"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s លេខចុះបញ្ជាការ %(reg_no)s"
+msgstr "%(provider)s ចុះបញ្ជីលេខ %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -62,27 +62,25 @@
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr "Weblate គ្រាន់តែដំណើការទិន្នន័យឯកជនដែលអ្នកប្រើប្រាស់ផ្ដល់ជូនដោយប្រើវា៖"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr ""
+msgstr "ឈ្មោះ និងអាសយដ្ឋានអ៊ីម៉ែល"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "ទាំងនេះត្រូវបានប្រើ ដើម្បីកំណត់អត្តសញ្ញាណអ្នកនៅក្នុងការប្តេជ្ញាចិត្ត VCS"
+msgstr ""
+"ទាំងនេះត្រូវបានប្រើ ដើម្បីកំណត់អត្តសញ្ញាណអ្នកនៅក្នុងការប្តេជ្ញាចិត្ត VCS។"
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "លើសពីនេះទៀតអ៊ីមែលត្រូវបានប្រើសម្រាប់ការជូនដំណឹងអំពីព្រឹត្តិការណ៍ដែលបានមើល"
+msgstr ""
+"លើសពីនេះទៀត អ៊ីម៉ែលត្រូវបានប្រើសម្រាប់ការជូនដំណឹងពីព្រឹត្តិការណ៍ដែលបានមើល។"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "ពាក្យសម្ងាត់នៅក្នុងសំណុំបែបបទរួមផ្សំ"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
```

### Comparing `wllegal-2023.5/wllegal/locale/kmr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/kmr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/kn/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/kn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ko/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ko/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 # Jun Hyung Shin <shmishmi79@gmail.com>, 2019.
 # Lee Yunseok <ironyunseok@protonmail.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-06-04 10:49+0000\n"
-"Last-Translator: Hoseok Seo <ddinghoya@gmail.com>\n"
+"PO-Revision-Date: 2024-01-10 04:06+0000\n"
+"Last-Translator: 이정희 <daemul72@gmail.com>\n"
 "Language-Team: Korean <https://hosted.weblate.org/projects/weblate/legal/ko/>"
 "\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "GDPR Art. 28에 따른 협력업체"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -313,16 +313,16 @@
 "귀하의 이름과 전자우편 주소는 VCS 커밋에 사용되며 무한정 머무를 것입니다."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
-"커밋에 사용되는 이메일 주소는 개인 정보 보호를 위해 웨블레이트 시스템에서 "
-"마스킹할 수 있으며, 선택한 이름은 귀하에게 달려 있습니다."
+"선택한 이름은 사용자에게 달려 있으며 커밋에 사용되는 이메일 주소는 사용자의 "
+"개인 정보를 보호하기 위해 웹레이트시스템에 의해 가려질 수 있습니다."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "우리는 우리의 서비스를 제공하기 위해 쿠키를 사용합니다."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
```

### Comparing `wllegal-2023.5/wllegal/locale/ksh/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ksh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ln/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ln/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/lt/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/mk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# anonymous <noreply@weblate.org>, 2019.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-07-22 07:40+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
-"Language-Team: Lithuanian <https://hosted.weblate.org/projects/weblate/"
-"hosted/lt/>\n"
-"Language: lt\n"
+"Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
+"hosted/mk/>\n"
+"Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 0 : n%10>=2 && (n%100<10 || n"
-"%100>=20) ? 1 : n%10==0 || (n%100>10 && n%100<20) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=n==1 || n%10==1 ? 0 : 1;\n"
 "X-Generator: Weblate 3.8-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
@@ -33,60 +31,54 @@
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
-#, fuzzy
-#| msgid "Versions"
 msgid "Personal Data Controller"
-msgstr "Versijos"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:17
-#, fuzzy
-#| msgid "Translation status"
 msgid "Personal Data processed by Weblate"
-msgstr "Vertimų būsena"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 #, fuzzy
 #| msgid "Username or email"
 msgid "Name and e-mail address"
-msgstr "Naudotojo vardas arba el. p. adresas"
+msgstr "Корисничко име или е-пошта"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:29
-#, fuzzy
-#| msgid "Password has been changed."
 msgid "Password in hashed form"
-msgstr "Slaptažodis pakeistas."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
@@ -206,18 +198,16 @@
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:77
-#, fuzzy
-#| msgid "Your profile"
 msgid "Your rights"
-msgstr "Jūsų profilis"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -309,18 +299,16 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
-#, fuzzy
-#| msgid "Description"
 msgid "Definitions"
-msgstr "Aprašas"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
@@ -351,15 +339,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Slapukai"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -373,15 +361,15 @@
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Licencija"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -395,15 +383,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 #, fuzzy
 #| msgid "Personal info"
 msgid "Personal Data"
-msgstr "Asmeninė informacija"
+msgstr "Лични податоци"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -414,42 +402,42 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projektas"
+msgstr "Проект"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Paslauga"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
 #, fuzzy
-#| msgid "Translation status"
+#| msgid "Translation notifications"
 msgid "Translation Memory"
-msgstr "Vertimų būsena"
+msgstr "Преведувачки известувања"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Naudotojas"
+msgstr "Корисник"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
@@ -540,15 +528,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "Vertimai"
+msgstr "Превод"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -612,25 +600,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
 
-#~ msgid "Current plan"
-#~ msgstr "Dabartinis planas"
-
 #, fuzzy
-#~| msgid "Project"
+#~| msgid "Subject"
 #~ msgid "Component limit"
-#~ msgstr "Projektas"
+#~ msgstr "Предмет"
 
 #, fuzzy
-#~| msgid "Project"
+#~| msgid "Subject"
 #~ msgid "Projects limit"
-#~ msgstr "Projektas"
-
-#~ msgid "%(price)s EUR / month"
-#~ msgstr "%(price)s EUR / mėnesiui"
-
-#~ msgid "%(price)s EUR / year"
-#~ msgstr "%(price)s EUR / metus"
+#~ msgstr "Предмет"
```

### Comparing `wllegal-2023.5/wllegal/locale/lv/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/th/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,215 +1,178 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2022-11-07 19:02+0000\n"
-"Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
-"Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/legal/lv/"
-">\n"
-"Language: lv\n"
+"PO-Revision-Date: 2023-05-27 08:16+0000\n"
+"Last-Translator: สุริยา ชอบชอยยิกๆๆ <kkbaatlove@gmail.com>\n"
+"Language-Team: Thai <https://hosted.weblate.org/projects/weblate/legal/th/>\n"
+"Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n % 10 == 0 || n % 100 >= 11 && n % 100 <= "
-"19) ? 0 : ((n % 10 == 1 && n % 100 != 11) ? 1 : 2);\n"
-"X-Generator: Weblate 4.14.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Apakšuzņēmēji saskaņā ar GDPR 28. pantu"
+msgstr "ผู้ทำสัญญาช่วงตามที่บัญญัติในมาตรา 28 แห่ง GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "2020. gada oktobra statuss."
+msgstr "kkbaatlove1"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"Mēs ievērojam regulu Nr. %(law_679_2016)s, Vispārīgo datu aizsardzības "
-"regulu, kas pazīstama arī kā GDPR. Šis dokuments iekļauj nepieciešamās "
-"specifikācijas."
 
 #: wllegal/templates/legal/documents/privacy.html:9
+#, fuzzy
+#| msgid "Versions"
 msgid "Personal Data Controller"
-msgstr "Personas datu pārvaldnieks"
+msgstr "รุ่น"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, Reģ. Nr. %(reg_no)s"
+msgstr "%(provider)s, เลขจดทะเบียน %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate ir datu aizsardzības speciālists, ar kuru var sazināties, izmantojot "
-"%(privacy_contact)s."
+"Weblate ได้แต่งตั้งเจ้าหน้าที่คุ้มครองข้อมูล โดยสามารถติดต่อได้ผ่าน %(privacy_contact)s"
 
 #: wllegal/templates/legal/documents/privacy.html:17
+#, fuzzy
+#| msgid "Administration"
 msgid "Personal Data processed by Weblate"
-msgstr "Personas dati, ko apstrādā Weblate"
+msgstr "การดูแลระบบ"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"Weblate vietne apstrādā tikai tos Personas datus, ko Lietotājs pats "
-"iesniedzis, izmantojot mūsu pakalpojumu:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "Vārds un e-pasta adrese"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
-"Tie tiek izmantoti, lai identificētu jūs VCS iesniegtajās izmaiņās (commits)"
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Turklāt e-pasts tiek izmantots, lai nosūtītu notikumu paziņojumus, kuriem "
-"jūs sekojiet"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Parole šifrētā (hashed) formā"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "Ja tas ir konfigurēts, izmanto, lai autorizētu lietotāju"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Paroles tiek saglabātas šifrētas, izmantojot Argon2."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "IP adrese un pārlūkprogrammas nosaukums"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Tie tiek reģistrēti, ja tiek veiktas svarīgas izmaiņas jūsu kontā (piemēram, "
-"paroles maiņa), lai varētu veikt diagnostiku konta nozagšanas gadījumā"
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Rēķinu informācija"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "Personas datu apstrādes mērķis un juridiskais pamats"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Jūsu personas dati tiks izmantoti pakalpojuma vajadzībām:"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"nodrošināt mūsu pakalpojumus, kas saistīti ar pakalpojumu, un sazināties ar "
-"jums jautājumos par mūsu pakalpojumiem (tostarp izmantojot e-pastu un "
-"ziņojumapmaiņu) un būt pārliecinātiem par mūsu pakalpojumu tehnisko "
-"funkcionalitāti, pildot līgumsaistības vai pirmslīguma saistības (<a href="
-"\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"lai analizētu mūsu pakalpojumu izmantošanu un uzlabotu mūsu pakalpojumus (<a "
-"href=\"%(url)s\">VDAR(GDPR) 6. panta 1. punkta b) un f) apakšpunkts</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"ar jūsu nepārprotamu piekrišanu vai norādījumiem, lai veiktu mūsu "
-"uzņēmējdarbību vai nosūtītu jums informatīvos izdevumus (<a href=\"%(url)s"
-"\">VDAR(GDPR) 6. panta 1. punkts a.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Piekļuve personas datiem"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
-"Pārvaldnieks ir veicis visus saprātīgos tehniskos pasākumus personas datu "
-"aizsardzībai. Personas datiem var piekļūt tikai pilnvarotas personas."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
 msgstr ""
-"Trešās personas, kuras vajadzības gadījumā var piekļūt personas datiem:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr "Personas, ar kurām noslēgts līgums par pakalpojuma tehnisko drošību."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
-msgstr "Visi personas dati tiek glabāti Eiropas Savienībā."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
 msgid "Disclosure of the Personal Data"
-msgstr "Piekļuve personas datiem"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
@@ -222,333 +185,296 @@
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
-msgstr "Tiesības uz personas datu glabāšanu"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"Personas datus pakalpojums uzglabā līdz brīdim, kad lietotājs izdzēš savu "
-"kontu."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Piekļuves žurnāla informācija var tikt vākta ilgāku laika periodu, lai "
-"celtu, izskatītu vai aizstāvētu juridiskās prasības tiesvedībā."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
-msgstr "Jūsu tiesības"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"Lietotājs savus personas datu sniedz brīvprātīgi. Weblate nevar sniegt "
-"pakalpojumus bez šiem personas datiem."
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Mēs vēlamies, lai jūs vienmēr varētu kontrolēt savu personisko informāciju. "
-"Šajā nolūkā jums ir atbilstošas tiesības, kas to atļauj. Noteiktos apstākļos "
-"jūs varat:"
 
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Iegūt piekļuvi visiem saviem personas datiem, kurus Weblate izmanto vai "
-"apstrādā, kā arī iegūt to pilno kopiju (<a href=\"%(url)s\">VDAR(GDPR) 15. "
-"pants</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"Labot personas datus, kurus Weblate apstrādā, ja domājat, ka tie satur kļūdas"
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid "Order us to delete your Personal Data"
-msgstr "Pieprasīt mūs dzēst jūsu personas datus"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
-msgstr "Ierobežot personas datu apstrādi"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:89
+#, fuzzy
+#| msgid "Language"
 msgid "Object to processing"
-msgstr "Iebilst pret apstrādi"
+msgstr "ภาษา"
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Iegūt savus personas datus parastā un mašīnlasāmā formātā vai pārsūtīt šos "
-"personas datus citam pakalpojuma sniedzējam."
 
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
-"Jūsu personas datu dzēšanu, labošanu vai ieguvi var veikt no kontu "
-"pārvaldības, un tā ir pilnībā automatizēta."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Mēs apstrādājam privātos datus (piemēram, jūsu e-pasta adresi), tie tiks "
-"izdzēsti no mūsu datu bāzes, tiklīdz izdzēsīsit savu kontu."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Jūsu veiktie tulkojumi tiek izdoti saskaņā ar licenci, kas norādīta katram "
-"tulkošanas projektam."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
-"Jūsu vārds un e-pasta adrese tiks izmantota versiju kontroles (VCS) "
-"iesniegtajās izmaiņās (commits), un tie paliek tur uz visiem laikiem."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
-msgstr "Mēs izmantojam sīkfailus, lai nodrošinātu mūsu pakalpojumus."
+msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Skatīt angļu valodas versiju"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Pakalpojuma oficiālie lietošanas noteikumi ir dokumentēti angļu valodā, jūsu "
-"ērtībai tiek sniegti tulkojumi."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"Šie pakalpojuma noteikumi regulē lietotāja un pakalpojuma sniedzēja tiesības "
-"un pienākumus, kas rodas pakalpojuma izmantošanas rezultātā."
 
 #: wllegal/templates/legal/documents/tos.html:20
+#, fuzzy
+#| msgid "Description"
 msgid "Definitions"
-msgstr "Definīcijas"
+msgstr "คำอธิบาย"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "Šajos pakalpojumu sniegšanas noteikumos:"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "Līgums"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
-"licences līgums (tādā nozīmē, kādā to interpretē ar Civilkodeksa 2358. "
-"pantu), kas noslēgts starp lietotāju un pakalpojuma sniedzēju ar viņu "
-"piekrišanu"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr "Civilkodekss"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
-msgstr "likums Nr. %(law_89_2012)s Coll., Čehijas Civilkodekss ar grozījumiem"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
-msgstr "Vienošanās"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Sīkdatnes"
+msgstr "คุกกี้"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "VDAR(GDPR)"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Licence"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "Pakalpojumu sniedzējs"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s ar reģ. Nr. %(reg_no)s"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
+#, fuzzy
+#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "Personas dati, Personiskie dati"
+msgstr "ข้อมูลส่วนบุคคล"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Īpašnieks"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
-msgstr "lietotājs, kurš var pārvaldīt projektu"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Projekts"
+msgstr "โครงการ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "tulkošanas projekts, kas tiek realizēts, izmantojot Pakalpojumu"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Pakalpojums"
+msgstr "บริการ"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"uz Weblate balstīta tīmekļa vietne un pakalpojumi, ko nodrošina Pakalpojumu "
-"sniedzējs"
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "Administration"
 msgid "Translation Memory"
-msgstr "Tulkojumu atmiņa"
+msgstr "การดูแลระบบ"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Lietotājs"
+msgstr "ผู้ใช้"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "Versiju kontroles sistēma (VCS)"
+msgstr "VCS"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
-"projektā izmantotā versiju kontroles sistēma, piemēram, Git vai Mercurial"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr "Licences līguma noslēgšana"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr "Licences līgums"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
 
@@ -608,15 +534,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr ""
+msgstr "การแปล"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -680,29 +606,11 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
 
-#~ msgid ""
-#~ "In case you purchase service from us, we collect additional billing "
-#~ "information necessary for issuing an invoice"
-#~ msgstr ""
-#~ "Ja iegādājaties pakalpojumu no mums, mēs ievācam papildus informāciju, "
-#~ "kas nepieciešama rēķina izrakstīšanai"
-
-#~ msgid "Payment processors."
-#~ msgstr "Maksājumu apstrādātāji."
-
-#~ msgid ""
-#~ "The services are provided “as is”, at your own risk, without any warranty."
-#~ msgstr ""
-#~ "Pakalpojumi tiek sniegti “tādi, kādi tie ir”, uz jūsu risku un "
-#~ "atbildības, bez jebkādas garantijas."
-
-#~ msgid ""
-#~ "Additional guarantees might apply to commercial customers, those are "
-#~ "expressed in corresponding contracts."
-#~ msgstr ""
-#~ "Papildu garantijas var būt spēkā maksas (komerciāliem) klientiem, tās ir "
-#~ "aprakstītas attiecīgajos līgumos."
+#, fuzzy
+#~| msgid "Language"
+#~ msgid "Languages limit"
+#~ msgstr "ภาษา"
```

### Comparing `wllegal-2023.5/wllegal/locale/lzh/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/lzh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/mk/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ml/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2019-07-22 07:40+0000\n"
-"Last-Translator: Michal Čihař <michal@cihar.com>\n"
-"Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
-"hosted/mk/>\n"
-"Language: mk\n"
+"PO-Revision-Date: 2020-12-22 00:29+0000\n"
+"Last-Translator: vachan-maker <vachan2014carmel@gmail.com>\n"
+"Language-Team: Malayalam <https://hosted.weblate.org/projects/weblate/legal/"
+"ml/>\n"
+"Language: ml\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n==1 || n%10==1 ? 0 : 1;\n"
-"X-Generator: Weblate 3.8-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -55,18 +56,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
-#, fuzzy
-#| msgid "Username or email"
 msgid "Name and e-mail address"
-msgstr "Корисничко име или е-пошта"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events."
@@ -371,27 +370,25 @@
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr ""
+msgstr "ദാതാവ്"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
-#, fuzzy
-#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "Лични податоци"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -402,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Проект"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -418,26 +415,24 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "Translation notifications"
 msgid "Translation Memory"
-msgstr "Преведувачки известувања"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Корисник"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
@@ -528,15 +523,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "Превод"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -599,17 +594,7 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-
-#, fuzzy
-#~| msgid "Subject"
-#~ msgid "Component limit"
-#~ msgstr "Предмет"
-
-#, fuzzy
-#~| msgid "Subject"
-#~ msgid "Projects limit"
-#~ msgstr "Предмет"
```

### Comparing `wllegal-2023.5/wllegal/locale/ml/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2020-12-22 00:29+0000\n"
-"Last-Translator: vachan-maker <vachan2014carmel@gmail.com>\n"
-"Language-Team: Malayalam <https://hosted.weblate.org/projects/weblate/legal/"
-"ml/>\n"
-"Language: ml\n"
+"PO-Revision-Date: 2022-10-24 16:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
+"weblate/legal/pa_PK/>\n"
+"Language: pa_PK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.4-dev\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.14.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -338,15 +338,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr ""
+msgstr "کوکیاں"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -370,25 +370,25 @@
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "ദാതാവ്"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "نِجی ڈیٹا"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -399,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "پروجیکٹ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -435,15 +435,15 @@
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr ""
+msgstr "ورژن کنترول سسٹم"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/mr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/mr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ms/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/my/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/nb/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/nb/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 # Kurt Eilertsen <kurt@kheds.com>, 2018.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-11-03 17:40+0000\n"
+"PO-Revision-Date: 2024-05-26 23:23+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/weblate/"
 "legal/nb_NO/>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.6-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Underleverandører i samsvar med artikkel nr. 28 av GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -40,15 +40,15 @@
 msgstr ""
 "Vi overholding regulering nr. %(law_679_2016)s, General Data Protection "
 "Regulation, også kjent som GDPR. Dette dokumentet inneholder nødvendige "
 "spesifikasjoner."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "Personlig datakontrollør"
+msgstr "Kontrolløren av personlig data"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
 msgstr "%(provider)s, Reg. nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
@@ -194,16 +194,17 @@
 "nødvendig er:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Personer som har blitt innleid for teknisk betjening av tjenesten."
 
 #: wllegal/templates/legal/documents/privacy.html:60
+#, fuzzy
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Betalingsformidlere ved kjøp av tjenester fra oss."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "All personlig data er lagret i den europeiske unionen."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
@@ -213,24 +214,33 @@
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Personlig data kan oppgis til tredjeparter i begrensede fall der "
+"kontrolløren i god tro mener det er påkrevd av lov, som ved "
+"ransakelsesordre, eller annen rettslig/administrativ beslutning."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"I fall det kreves av kontrolløren å oppgi data gitt av lov vil det bli gjort "
+"et forsøk på å la dette komme brukeren til kjenne via e-post (med mindre "
+"kontrolløren forhindres fra dette, eller det er fånyttes) at det har kommet "
+"en forespørsel om personlig data, slik at brukeren kan motsi seg "
+"overlevering. Hvis brukeren ikke motsetter seg overlevering kan det hende "
+"kontrolløren er lovmessig bundet til å gi fra seg den personlige dataen."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Oppbevaring av personlig data"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
```

### Comparing `wllegal-2023.5/wllegal/locale/nl/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/nn/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/nn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/oc/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/oc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/or/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/or/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/pa/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/pa_PK/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/tlh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2022-10-24 16:14+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
-"weblate/legal/pa_PK/>\n"
-"Language: pa_PK\n"
+"PO-Revision-Date: 2019-07-22 07:41+0000\n"
+"Last-Translator: Michal Čihař <michal@cihar.com>\n"
+"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/hosted/"
+"tlh/>\n"
+"Language: tlh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.14.2-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 3.8-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -338,15 +337,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "کوکیاں"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -380,15 +379,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "نِجی ڈیٹا"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -399,15 +398,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "پروجیکٹ"
+msgstr "jInmol"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -415,16 +414,18 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "New password (again)"
 msgid "Translation Memory"
-msgstr ""
+msgstr "mu'wIj chu' (jatlhqa')"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
@@ -435,15 +436,15 @@
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "ورژن کنترول سسٹم"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -523,15 +524,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr ""
+msgstr "mughmeH"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -594,7 +595,12 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
+
+#, fuzzy
+#~| msgid "Last name"
+#~ msgid "Repositories limit"
+#~ msgstr "pong Qav"
```

### Comparing `wllegal-2023.5/wllegal/locale/peo/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/peo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/pl/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ps/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ps/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/pt/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pt/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 # Pedro Albuquerque <pmra@gmx.com>, 2019.
 # Manuela Silva <mmsrs@sky.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-08-07 14:12+0000\n"
-"Last-Translator: Hugo Carvalho <hugokarvalho@hotmail.com>\n"
+"PO-Revision-Date: 2024-04-22 01:07+0000\n"
+"Last-Translator: Francielle Souza <fransoonerorlater@gmail.com>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/weblate/legal/"
 "pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0-dev\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subcontratados de acordo com o art. 28 RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -215,38 +215,40 @@
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Caso o Controlador seja obrigado por lei a divulgar os Dados Pessoais, será "
+"feita uma tentativa de fornecer ao Utilizador um aviso por e-mail (a menos "
+"que o Controlador seja proibido, ou seja, inútil) de que uma solicitação de "
+"Dados Pessoais foi feita para permitir que o utilizador se oponha à "
+"divulgação. Se o Utilizador não contestar a solicitação de divulgação, o "
+"Controlador poderá ser legalmente obrigado a entregar os Dados Pessoais."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "A retenção de \"Dados Pessoais\""
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Os \"Dados Pessoais\" são guardados no \"Serviço\" até que o \"Utilizador\" "
 "elimine a sua conta no serviço."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"A informação do registo dos acessos pode ser obtida mais tempo para o "
-"propósito de estabelecer, exercer ou defender reclamações legais."
+"As informações de registro de acesso podem ser coletadas por um período mais "
+"longo com a finalidade de estabelecer, exercer ou defender ações judiciais."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Os seus direitos"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -310,24 +312,21 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "A remoção, correção e recuperação dos seus dados pessoais pode ser feita a "
 "partir da gestão da conta e é totalmente automatizada."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "Nós processamos os dados privados (tal como o seu endereço de ''e-mail''), "
-"que serão removidos da nossa base de dados assim que remover a sua conta."
+"que serão removidos da nossa base de dados assim que você remover a sua "
+"conta."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "As suas traduções são feitas sob a licença especificada por cada tradução."
```

### Comparing `wllegal-2023.5/wllegal/locale/pt_BR/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Luiz Fernando Ranghetti <elchevive@opensuse.org>, 2018.
 # Rafael Fontenelle <rafaelff@gnome.org>, 2018, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-10-18 19:52+0000\n"
-"Last-Translator: Luiz Fernando Ranghetti <elchevive@opensuse.org>\n"
+"PO-Revision-Date: 2023-12-15 20:37+0000\n"
+"Last-Translator: Claudio Filho F Filho <filhocf@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "weblate/legal/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.3\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Sub-contratantes de Acordo com o Artigo 28 do RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -106,14 +106,16 @@
 msgstr "Informações de cobrança"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Os dados necessários para emitir uma fatura são coletados no momento da "
+"compra de um serviço nosso."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Proposta e base legal de processamento de Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -174,42 +176,49 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Pessoas que são contratadas para garantia técnica do serviço."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Processadores de pagamento ao adquirir um serviço nosso."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Todos os Dados Pessoais são armazenados na União Europeia."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
 msgid "Disclosure of the Personal Data"
-msgstr "Acesso aos Dados Pessoais"
+msgstr "Divulgação dos Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Os Dados Pessoais poderão ser divulgados a terceiros em circunstâncias "
+"limitadas quando o Controlador acreditar, de boa fé, que isso é exigido por "
+"lei, como sob uma intimação ou outra ordem judicial ou administrativa."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Caso o Controlador seja obrigado por lei a divulgar os Dados Pessoais, será "
+"feita uma tentativa de fornecer ao Usuário um aviso prévio por e-mail (a "
+"menos que o Controlador seja proibido ou seja inútil) de que uma solicitação "
+"de Dados Pessoais foi feita para permitir que o usuário se oponha à "
+"divulgação. Se o Usuário não contestar a solicitação de divulgação, o "
+"Controlador poderá ser legalmente obrigado a entregar os Dados Pessoais."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "A retenção de Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
@@ -317,22 +326,25 @@
 "para sempre."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"O nome escolhido fica a seu critério e o endereço de e-mail usado para "
+"commits pode ser mascarado pelo sistema Weblate para proteger sua "
+"privacidade."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Usamos cookies para entregar nossos serviços."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Não usamos cookies de terceiros."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Ver a versão em inglês"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -613,14 +625,18 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Na acepção do <a href=\"%(url)s\">Artigo 7</a> da GDPR, o Usuário dá "
+"consentimento para a coleta, armazenamento e processamento dos Dados "
+"Pessoais de acordo com a <a href=\"%(privacy_url)s\">Política de "
+"Privacidade</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Traduções"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
```

### Comparing `wllegal-2023.5/wllegal/locale/pt_PT/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-08-22 05:09+0000\n"
-"Last-Translator: ssantos <ssantos@web.de>\n"
+"PO-Revision-Date: 2024-04-28 18:28+0000\n"
+"Last-Translator: Manuela Silva <mmsrs@sky.com>\n"
 "Language-Team: Portuguese (Portugal) <https://hosted.weblate.org/projects/"
 "weblate/legal/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.0-dev\n"
+"X-Generator: Weblate 5.5.1\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subcontratados de acordo com o art. 28 RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -72,27 +72,28 @@
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits."
 msgstr "Estes são utilizados para identificá-lo nas submissões de VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Além disso, o email é usado para a notificação de eventos observados."
+msgstr ""
+"Além disso, o ''email'' é utilizado para a notificação dos eventos vigiados."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Palavra-passe em formato \"hash\""
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr "Utilizado para autenticar o \"Utilizador\", se configurado"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Palavras-passe são armazenadas em hash a usar Argon2."
+msgstr "As palavras-passe são guardadas em \"hash\" utilizando Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Endereço de IP e nome do navegador"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
@@ -213,38 +214,41 @@
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Caso o Controlador seja obrigado por lei a divulgar os Dados Pessoais, será "
+"feita uma tentativa de fornecer ao Utilizador um aviso por e-mail (a menos "
+"que o Controlador seja proibido, ou seja, inútil) de que uma solicitação de "
+"Dados Pessoais foi feita para permitir que o utilizador se oponha à "
+"divulgação. Se o Utilizador não contestar a solicitação de divulgação, o "
+"Controlador poderá ser legalmente obrigado a entregar os Dados Pessoais."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "A retenção de \"Dados Pessoais\""
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Os \"Dados Pessoais\" são guardados no \"Serviço\" até que o \"Utilizador\" "
 "elimine a sua conta no serviço."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"A informação do registo dos acessos pode ser obtida mais tempo para o "
-"propósito de estabelecer, exercer ou defender reclamações legais."
+"A informação do registo de acesso poderá ser obtida para um período mais "
+"longo para o propósito de estabelecer, exercer ou defender reclamações "
+"legais."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Os seus direitos"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -308,24 +312,20 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "A remoção, correção e recuperação dos seus dados pessoais pode ser feita a "
 "partir da gestão da conta e é totalmente automatizada."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Nós processamos os dados privados (tal como o seu endereço de ''e-mail''), "
-"que serão removidos da nossa base de dados assim que remover a sua conta."
+"Nós processamos os dados pessoais (tal como o seu endereço de ''e-mail''), "
+"que serão removidos da nossa base de dados se remover a sua conta."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "As suas traduções são feitas sob a licença especificada por cada tradução."
```

### Comparing `wllegal-2023.5/wllegal/locale/ro/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # Automatically generated, 2014.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-10-27 09:26+0000\n"
+"PO-Revision-Date: 2024-01-25 13:31+0000\n"
 "Last-Translator: Vlăduț Ilie <vladilie94@gmail.com>\n"
 "Language-Team: Romanian <https://hosted.weblate.org/projects/weblate/legal/"
 "ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2;\n"
-"X-Generator: Weblate 5.2-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 "Subcontractanți în conformitate cu art. 28 GDPR (Regulamentul general "
 "privind protecția datelor)"
```

### Comparing `wllegal-2023.5/wllegal/locale/ro_MD/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ru/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # Vadim Nekhai <vadimnekhai@gmail.com>, 2019.
 # Golubev Alexander <fatzer2@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-10-11 20:22+0000\n"
-"Last-Translator: Victor K <ktrace@yandex.ru>\n"
+"PO-Revision-Date: 2023-12-23 11:55+0000\n"
+"Last-Translator: Blueberry <igory.ygr200@gmail.com>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/weblate/legal/ru/"
 ">\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.1-dev\n"
+"X-Generator: Weblate 5.4-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Субподрядчики в соответствии со ст. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -89,15 +89,15 @@
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Пароль в хэшированном виде"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "Если настроено, используется для аутентификации Пользователя"
+msgstr "Если настроено, используется для авторизации пользователя"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
 msgstr "Пароли хранятся хэшированными с помощью Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
@@ -220,15 +220,15 @@
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
 "В случае, если Контролер обязан по закону раскрыть Персональные данные, "
 "будет предпринята попытка предоставить Пользователю предварительное "
-"уведомление по электронной почте (если только Контролер не запрещен или это "
+"уведомление по электронной почте (если только Контролер не запрещён или это "
 "было бы бесполезно) о том, что был сделан запрос на Персональные данные, "
 "чтобы позволить Пользователю возразить против раскрытия. Если Пользователь "
 "не оспаривает запрос на раскрытие информации, Контролер может быть "
 "юридически обязан передать Персональные данные."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
@@ -320,15 +320,15 @@
 
 #: wllegal/templates/legal/documents/summary.html:4
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "Мы обрабатываем персональные данные (например, ваш адрес электронной почты); "
-"Они будут удалены из нашей базы данных, если вы удалите свою учетную запись."
+"Они будут удалены из нашей базы данных, если вы удалите свою учётную запись."
 
 #: wllegal/templates/legal/documents/summary.html:5
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Ваши переводы выполняются в соответствии с лицензией, которая указана в "
@@ -353,15 +353,15 @@
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Мы используем файлы «куки», чтобы предоставлять наши услуги."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr "Мы не используем сторонние файлы cookie."
+msgstr "Мы не используем сторонние файлы куки."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Посмотреть английскую версию"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -644,17 +644,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
-"По смыслу <a href=\"%(url)s\">Статьи 7</a> GDPR Пользователь настоящим дает "
+"По смыслу <a href=\"%(url)s\">статьи 7</a> GDPR Пользователь настоящим даёт "
 "согласие на сбор, хранение и обработку Персональных данных в соответствии с "
-"<a href=\"%(privacy_url)s\">Политикой конфиденциальности</a>."
+"<a href=\"%(privacy_url)s\">«Политикой конфиденциальности»</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Переводы"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -693,15 +693,15 @@
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
 "Пользователь соглашается на использование имени и адреса электронной почты в "
 "качестве авторства в обязательствах VCS. Пользователь понимает, что это "
-"предоставление не может быть отозвано из-за характера СКВ."
+"предоставление не может быть отозвано из-за характера VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
```

### Comparing `wllegal-2023.5/wllegal/locale/sai/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sai/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sc/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sc/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/si/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sk/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/skr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/skr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sl/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sq/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sr_Latn/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Nikola Perović <nikolaperovicccc@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2021-02-09 02:02+0000\n"
-"Last-Translator: Слободан Симић(Slobodan Simić) <slsimic@gmail.com>\n"
+"PO-Revision-Date: 2024-04-10 07:58+0000\n"
+"Last-Translator: Vladan Ristić <info@vlaristic.rs>\n"
 "Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
 "legal/sr_Latn/>\n"
 "Language: sr_Latn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.5-dev\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Podizvođači u skladu sa članom 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 #, fuzzy
@@ -383,15 +383,15 @@
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr ""
+msgstr "Provajder"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
```

### Comparing `wllegal-2023.5/wllegal/locale/sv/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/sw/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/ta/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/lt/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,137 +1,145 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# anonymous <noreply@weblate.org>, 2019.
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2022-01-13 15:57+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Tamil <https://hosted.weblate.org/projects/weblate/legal/ta/"
-">\n"
-"Language: ta\n"
+"PO-Revision-Date: 2024-04-18 04:31+0000\n"
+"Last-Translator: Vaclovas Intas <vaclovas1999@gmail.com>\n"
+"Language-Team: Lithuanian <https://hosted.weblate.org/projects/weblate/legal/"
+"lt/>\n"
+"Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10.1\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 0 : n%10>=2 && (n%100<10 || "
+"n%100>=20) ? 1 : n%10==0 || (n%100>10 && n%100<20) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "கலைக்கு ஏற்ப துணை ஒப்பந்தக்காரர்கள். 28 GDPR"
+msgstr "Subrangovai pagal CK 6.1 str. 28 BDAR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "அக்டோபர் 2020 நிலவரப்படி."
+msgstr "Statusas 2023 m. kovo mėn."
 
 #: wllegal/templates/legal/documents/privacy.html:6
-#, fuzzy, python-format
+#, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
-"GDPR எனப்படும் பொதுத் தரவுப் பாதுகாப்பு ஒழுங்குமுறை விதி எண் %(சட்டம் 679 2016)க்கு "
-"நாங்கள் இணங்குகிறோம். இந்த ஆவணத்தில் தேவையான விவரக்குறிப்புகள் உள்ளன."
+"Mes laikomės Reglamento nr. %(law_679_2016)s, Bendrojo duomenų apsaugos "
+"reglamento, dar vadinamo BDAR. Šiame dokumente pateikiamos būtinos "
+"specifikacijos."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "தனிப்பட்ட தரவுக் கட்டுப்பாட்டாளர்"
+msgstr "Asmens duomenų valdytojas"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, பதிவு எண்.%(reg_no)s"
+msgstr "%(provider)s, Reg. nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"%(privacy_contact)s வழியாக அணுகக்கூடிய தரவு பாதுகாப்பு அதிகாரியை Weblate "
-"நியமித்துள்ளது."
+"„Weblate“ paskyrė duomenų apsaugos pareigūną, su kuriuo galima susisiekti "
+"per %(privacy_contact)s."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
-msgstr ""
+msgstr "„Weblate“ apdorojami asmens duomenys"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
+"„Weblate“ apdoroja tik tuos asmens duomenis, kuriuos naudotojas pateikia "
+"naudodamasis ja:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "பெயர் மற்றும் மின்னஞ்சல் முகவரி"
+msgstr "Vardas ir el. pašto adresas"
 
 #: wllegal/templates/legal/documents/privacy.html:26
 msgid "These are used to identify you in the VCS commits."
-msgstr ""
+msgstr "Jie naudojami jūsų tapatybei VCS įsipareigojimuose identifikuoti."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "கூடுதலாக, பார்த்த நிகழ்வுகளின் அறிவிப்பிற்காக மின்னஞ்சல் பயன்படுத்தப்படுகிறது"
+msgstr "Be to, el. paštas naudojamas parnešti apie stebimus įvykius."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "ஹாஷ் வடிவத்தில் கடவுச்சொல்"
+msgstr "Slaptažodis maišos formoje"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
-msgstr "கட்டமைக்கப்பட்டிருந்தால், பயனரை அங்கீகரிக்கப் பயன்படுகிறது"
+msgstr "Naudojamas nustatyti tapatybę naudotojui, jei sukonfigūruota"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "கடவுச்சொற்கள் ஆர்கான் 2 ஐப் பயன்படுத்தி ஹாஷ் முறையில் சேமிக்கப்படுகின்றன."
+msgstr "Slaptažodžiai saugomi užmaišuoti naudojant „Argon2“."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
-msgstr "ஐபி முகவரி மற்றும் உலாவி பெயர்"
+msgstr "IP adresas ir naršyklės pavadinimas"
 
 #: wllegal/templates/legal/documents/privacy.html:34
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
+"Jie įrašomi svarbių jūsų paskyros pakeitimų (pvz., slaptažodžio pakeitimo) "
+"atveju, kad būtų galima diagnozuoti, jei jūsų paskyra būtų pavogta."
 
 #: wllegal/templates/legal/documents/privacy.html:36
 msgid "Billing info"
-msgstr ""
+msgstr "Atsiskaitymo informacija"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Būtini duomenys sąskaitai faktūrai išrašyti renkami perkant iš mūsų paslaugą."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr ""
+msgstr "Asmens duomenų apdorojimo tikslas ir teisinis pagrindas"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr ""
+msgstr "Jūsų asmens duomenys bus naudojami paslaugos teikimo tikslais:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
+"teikiant mūsų paslaugas paslaugoje, siekiant susisiekti su jumis mūsų "
+"paslaugų klausimais (taip pat el. laiškais ir žinutėmis) ir siekiant "
+"užtikrinti mūsų paslaugų techninį funkcionalumą, sutartinių ar ikisutartinių "
+"įsipareigojimų laikymąsi (<a href=\"%(url)s\">BDAR 6 straipsnio 1 dalies b "
+"punktas</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
@@ -205,16 +213,18 @@
 #: wllegal/templates/legal/documents/privacy.html:75
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:77
+#, fuzzy
+#| msgid "Your profile"
 msgid "Your rights"
-msgstr ""
+msgstr "Jūsų profilis"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
 
@@ -306,16 +316,18 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
+#, fuzzy
+#| msgid "Description"
 msgid "Definitions"
-msgstr ""
+msgstr "Aprašas"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
@@ -346,15 +358,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr ""
+msgstr "Slapukai"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -368,15 +380,15 @@
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr ""
+msgstr "Licencija"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -387,16 +399,18 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
+#, fuzzy
+#| msgid "Personal info"
 msgid "Personal Data"
-msgstr ""
+msgstr "Asmeninė informacija"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -407,51 +421,53 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "Projektas"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "சேவை"
+msgstr "Paslauga"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "Translation status"
 msgid "Translation Memory"
-msgstr ""
+msgstr "Vertimų būsena"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr ""
+msgstr "Naudotojas/Vartotojas"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "வி.சி.எஸ்"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -531,15 +547,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr ""
+msgstr "Vertimai"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -602,7 +618,26 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
+
+#~ msgid "Current plan"
+#~ msgstr "Dabartinis planas"
+
+#, fuzzy
+#~| msgid "Project"
+#~ msgid "Component limit"
+#~ msgstr "Projektas"
+
+#, fuzzy
+#~| msgid "Project"
+#~ msgid "Projects limit"
+#~ msgstr "Projektas"
+
+#~ msgid "%(price)s EUR / month"
+#~ msgstr "%(price)s EUR / mėnesiui"
+
+#~ msgid "%(price)s EUR / year"
+#~ msgstr "%(price)s EUR / metus"
```

### Comparing `wllegal-2023.5/wllegal/locale/te/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/te/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/th/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/tzm/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate\n"
+"Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-05-27 08:16+0000\n"
-"Last-Translator: สุริยา ชอบชอยยิกๆๆ <kkbaatlove@gmail.com>\n"
-"Language-Team: Thai <https://hosted.weblate.org/projects/weblate/legal/th/>\n"
-"Language: th\n"
+"PO-Revision-Date: 2021-01-28 08:55+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
+"projects/weblate/legal/tzm/>\n"
+"Language: tzm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Plural-Forms: nplurals=2; plural=n >= 2 && (n < 11 || n > 99);\n"
+"X-Generator: Weblate 4.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "ผู้ทำสัญญาช่วงตามที่บัญญัติในมาตรา 28 แห่ง GDPR"
+msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
-msgstr "kkbaatlove1"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
-#, fuzzy
-#| msgid "Versions"
 msgid "Personal Data Controller"
-msgstr "รุ่น"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, เลขจดทะเบียน %(reg_no)s"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate ได้แต่งตั้งเจ้าหน้าที่คุ้มครองข้อมูล โดยสามารถติดต่อได้ผ่าน %(privacy_contact)s"
 
 #: wllegal/templates/legal/documents/privacy.html:17
-#, fuzzy
-#| msgid "Administration"
 msgid "Personal Data processed by Weblate"
-msgstr "การดูแลระบบ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
@@ -237,18 +234,16 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:89
-#, fuzzy
-#| msgid "Language"
 msgid "Object to processing"
-msgstr "ภาษา"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
 
@@ -303,18 +298,16 @@
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:20
-#, fuzzy
-#| msgid "Description"
 msgid "Definitions"
-msgstr "คำอธิบาย"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
@@ -345,37 +338,37 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "คุกกี้"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr ""
+msgstr "GDPR"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr ""
+msgstr "Turagt"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -386,64 +379,60 @@
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
-#, fuzzy
-#| msgid "Personal info"
 msgid "Personal Data"
-msgstr "ข้อมูลส่วนบุคคล"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr ""
+msgstr "Bab"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "โครงการ"
+msgstr "Asefaṛ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "บริการ"
+msgstr "Tanafut"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "Administration"
 msgid "Translation Memory"
-msgstr "การดูแลระบบ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "ผู้ใช้"
+msgstr "Anessemres"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
@@ -534,15 +523,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "การแปล"
+msgstr "Tisuɣal"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -605,12 +594,7 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-
-#, fuzzy
-#~| msgid "Language"
-#~ msgid "Languages limit"
-#~ msgstr "ภาษา"
```

### Comparing `wllegal-2023.5/wllegal/locale/tlh/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/tok/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2019-07-22 07:41+0000\n"
-"Last-Translator: Michal Čihař <michal@cihar.com>\n"
-"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/hosted/"
-"tlh/>\n"
-"Language: tlh\n"
+"PO-Revision-Date: 2023-04-28 16:51+0000\n"
+"Last-Translator: Sena <jn-sena@proton.me>\n"
+"Language-Team: Toki Pona <https://hosted.weblate.org/projects/weblate/legal/"
+"tok/>\n"
+"Language: tok\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.8-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -379,15 +380,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "sona jan"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -398,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "jInmol"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -414,18 +415,16 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "New password (again)"
 msgid "Translation Memory"
-msgstr "mu'wIj chu' (jatlhqa')"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
@@ -524,15 +523,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "mughmeH"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -595,12 +594,7 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-
-#, fuzzy
-#~| msgid "Last name"
-#~ msgid "Repositories limit"
-#~ msgstr "pong Qav"
```

### Comparing `wllegal-2023.5/wllegal/locale/tok/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/uz/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-04-28 16:51+0000\n"
-"Last-Translator: Sena <jn-sena@proton.me>\n"
-"Language-Team: Toki Pona <https://hosted.weblate.org/projects/weblate/legal/"
-"tok/>\n"
-"Language: tok\n"
+"PO-Revision-Date: 2023-02-12 16:39+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/"
+">\n"
+"Language: uz\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -338,15 +338,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr ""
+msgstr "Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -380,15 +380,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "sona jan"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/tr/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/tt/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/tt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/tzm/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/zgh/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,49 +4,51 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2021-01-28 08:55+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
-"projects/weblate/legal/tzm/>\n"
-"Language: tzm\n"
+"PO-Revision-Date: 2023-04-02 01:08+0000\n"
+"Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
+"Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
+"projects/weblate/legal/zgh/>\n"
+"Language: zgh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n >= 2 && (n < 11 || n > 99);\n"
-"X-Generator: Weblate 4.5-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
+#, fuzzy
+#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr ""
+msgstr "ⴰⵙⵓⵔⵙ ⵙⴳ ⴽⵟⵓⴱⵕ 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr ""
+msgstr "ⵜⵉⴹⴰⴼ ⵏ ⵜⵎⵓⵛⴰ ⵜⵉⵏⵉⵎⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s,ⵓⵟⵟⵓⵏ ⵏ ⵓⵣⵎⵎⴻⵎ. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -349,26 +351,26 @@
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "GDPR"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
-msgstr "Turagt"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
@@ -380,42 +382,42 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "ⵜⵉⵎⵓⵛⴰ ⵜⵓⴷⵎⴰⵡⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Bab"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "Asefaṛ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
-msgstr "Tanafut"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
@@ -424,26 +426,26 @@
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr "Anessemres"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 
@@ -523,15 +525,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "Tisuɣal"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/ug/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/ug/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/uk/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/uz/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2023-02-12 16:39+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/"
-">\n"
-"Language: uz\n"
+"PO-Revision-Date: 2024-03-07 15:01+0000\n"
+"Last-Translator: Ray <ray@users.noreply.hosted.weblate.org>\n"
+"Language-Team: Yue (Traditional) <https://hosted.weblate.org/projects/"
+"weblate/legal/yue_Hant/>\n"
+"Language: yue_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -338,15 +338,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Cookies"
+msgstr "Cookie"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -424,15 +424,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
-msgstr ""
+msgstr "使用者"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/vi/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/yue_Hant/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/chn/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
 "POT-Creation-Date: 2023-05-17 14:12+0000\n"
-"PO-Revision-Date: 2022-08-21 08:34+0000\n"
-"Last-Translator: Ray <ray.cfu@protonmail.com>\n"
-"Language-Team: Yue <https://hosted.weblate.org/projects/weblate/legal/yue/>\n"
-"Language: yue\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: chn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.14-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -337,15 +335,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Cookie"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
```

### Comparing `wllegal-2023.5/wllegal/locale/zh_Hans/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/locale/zh_Hant/LC_MESSAGES/django.po` & `wllegal-2024.1/wllegal/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/legal/documents/privacy.html` & `wllegal-2024.1/wllegal/templates/legal/documents/privacy.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/legal/documents/summary.html` & `wllegal-2024.1/wllegal/templates/legal/documents/summary.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/legal/documents/tos.html` & `wllegal-2024.1/wllegal/templates/legal/documents/tos.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/security.txt` & `wllegal-2024.1/wllegal/templates/security.txt`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/weblate_503.html` & `wllegal-2024.1/wllegal/templates/weblate_503.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templates/weblate_50x.html` & `wllegal-2024.1/wllegal/templates/weblate_50x.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/templatetags/lawlinks.py` & `wllegal-2024.1/wllegal/templatetags/lawlinks.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal/tests.py` & `wllegal-2024.1/wllegal/tests.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.5/wllegal.egg-info/PKG-INFO` & `wllegal-2024.1/wllegal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.5
+Version: 2024.1
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
```

### Comparing `wllegal-2023.5/wllegal.egg-info/SOURCES.txt` & `wllegal-2024.1/wllegal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 wllegal/locale/bg/LC_MESSAGES/django.po
 wllegal/locale/bn/LC_MESSAGES/django.po
 wllegal/locale/bn_BD/LC_MESSAGES/django.po
 wllegal/locale/bo/LC_MESSAGES/django.po
 wllegal/locale/br/LC_MESSAGES/django.po
 wllegal/locale/ca/LC_MESSAGES/django.po
 wllegal/locale/ce/LC_MESSAGES/django.po
+wllegal/locale/chn/LC_MESSAGES/django.po
 wllegal/locale/ckb/LC_MESSAGES/django.po
 wllegal/locale/crh/LC_MESSAGES/django.po
 wllegal/locale/cs/LC_MESSAGES/django.po
 wllegal/locale/cv/LC_MESSAGES/django.po
 wllegal/locale/cy/LC_MESSAGES/django.po
 wllegal/locale/da/LC_MESSAGES/django.po
 wllegal/locale/de/LC_MESSAGES/django.po
```

