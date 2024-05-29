# Comparing `tmp/fnschool-20240530.80012.827.tar.gz` & `tmp/fnschool-20240530.80026.842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240530.80012.827.tar", last modified: Wed May 29 16:12:32 2024, max compression
+gzip compressed data, was "fnschool-20240530.80026.842.tar", last modified: Wed May 29 16:26:47 2024, max compression
```

## Comparing `fnschool-20240530.80012.827.tar` & `fnschool-20240530.80026.842.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.955913 fnschool-20240530.80012.827/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.80012.827/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 16:12:32.954913 fnschool-20240530.80012.827/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.80012.827/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.80012.827/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-29 16:12:32.955913 fnschool-20240530.80012.827/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.928912 fnschool-20240530.80012.827/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.935913 fnschool-20240530.80012.827/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.80012.827/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.943913 fnschool-20240530.80012.827/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.80012.827/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.80012.827/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.80012.827/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.80012.827/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.944913 fnschool-20240530.80012.827/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255585 2024-05-22 03:00:22.000000 fnschool-20240530.80012.827/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46613 2024-05-29 09:49:05.000000 fnschool-20240530.80012.827/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.80012.827/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.80012.827/src/fnschool/canteen/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.80012.827/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80012.827/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80012.827/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.80012.827/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      601 2024-05-29 13:55:44.000000 fnschool-20240530.80012.827/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.948913 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    18745 2024-05-29 14:28:30.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.80012.827/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80012.827/src/fnschool/canteen/workbook.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.80012.827/src/fnschool/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.949913 fnschool-20240530.80012.827/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240530.80012.827/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.80012.827/src/fnschool/entry.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.951913 fnschool-20240530.80012.827/src/fnschool/exam/
--rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.80012.827/src/fnschool/exam/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.80012.827/src/fnschool/exam/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.80012.827/src/fnschool/exam/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.80012.827/src/fnschool/exam/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.80012.827/src/fnschool/exam/score.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.80012.827/src/fnschool/exam/subject.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.80012.827/src/fnschool/exam/teacher.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.80012.827/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.80012.827/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.931913 fnschool-20240530.80012.827/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.929912 fnschool-20240530.80012.827/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.951913 fnschool-20240530.80012.827/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.930913 fnschool-20240530.80012.827/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.951913 fnschool-20240530.80012.827/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    19437 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.930913 fnschool-20240530.80012.827/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.952913 fnschool-20240530.80012.827/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.931913 fnschool-20240530.80012.827/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.952913 fnschool-20240530.80012.827/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.931913 fnschool-20240530.80012.827/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.952913 fnschool-20240530.80012.827/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:12:27.000000 fnschool-20240530.80012.827/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      898 2024-05-24 05:00:49.000000 fnschool-20240530.80012.827/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.80012.827/src/fnschool/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     5572 2024-05-29 14:01:51.000000 fnschool-20240530.80012.827/src/fnschool/user.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:12:32.953913 fnschool-20240530.80012.827/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2458 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-29 16:12:32.000000 fnschool-20240530.80012.827/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.635922 fnschool-20240530.80026.842/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240530.80026.842/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 16:26:47.635922 fnschool-20240530.80026.842/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240530.80026.842/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240530.80026.842/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-29 16:26:47.635922 fnschool-20240530.80026.842/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.608925 fnschool-20240530.80026.842/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.615924 fnschool-20240530.80026.842/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      522 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5301 2024-05-29 14:52:26.000000 fnschool-20240530.80026.842/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.623923 fnschool-20240530.80026.842/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-29 14:29:30.000000 fnschool-20240530.80026.842/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)      184 2024-05-29 14:01:36.000000 fnschool-20240530.80026.842/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240530.80026.842/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240530.80026.842/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.625923 fnschool-20240530.80026.842/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255585 2024-05-22 03:00:22.000000 fnschool-20240530.80026.842/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46623 2024-05-29 16:15:45.000000 fnschool-20240530.80026.842/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240530.80026.842/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)      616 2024-05-23 14:19:22.000000 fnschool-20240530.80026.842/src/fnschool/canteen/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240530.80026.842/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80026.842/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80026.842/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3803 2024-05-29 14:28:29.000000 fnschool-20240530.80026.842/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      601 2024-05-29 13:55:44.000000 fnschool-20240530.80026.842/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2809 2024-05-29 14:01:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.629922 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4148 2024-05-29 14:01:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10384 2024-05-23 01:03:24.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-29 14:01:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9187 2024-05-29 14:53:23.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10136 2024-05-29 15:24:10.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9164 2024-05-29 14:40:36.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18745 2024-05-29 14:28:30.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4386 2024-05-29 14:01:50.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98394 2024-05-29 14:01:57.000000 fnschool-20240530.80026.842/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240530.80026.842/src/fnschool/canteen/workbook.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1175 2024-05-29 14:01:37.000000 fnschool-20240530.80026.842/src/fnschool/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.629922 fnschool-20240530.80026.842/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240530.80026.842/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)      624 2024-05-24 05:10:01.000000 fnschool-20240530.80026.842/src/fnschool/entry.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.631922 fnschool-20240530.80026.842/src/fnschool/exam/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       78 2024-05-26 16:57:37.000000 fnschool-20240530.80026.842/src/fnschool/exam/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-26 16:57:37.000000 fnschool-20240530.80026.842/src/fnschool/exam/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      614 2024-05-26 15:01:13.000000 fnschool-20240530.80026.842/src/fnschool/exam/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      190 2024-05-26 16:57:37.000000 fnschool-20240530.80026.842/src/fnschool/exam/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      151 2024-05-26 16:57:37.000000 fnschool-20240530.80026.842/src/fnschool/exam/score.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-26 17:04:31.000000 fnschool-20240530.80026.842/src/fnschool/exam/subject.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      258 2024-05-26 17:04:31.000000 fnschool-20240530.80026.842/src/fnschool/exam/teacher.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240530.80026.842/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1883 2024-05-23 14:19:22.000000 fnschool-20240530.80026.842/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.611925 fnschool-20240530.80026.842/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.610925 fnschool-20240530.80026.842/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.632922 fnschool-20240530.80026.842/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.610925 fnschool-20240530.80026.842/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.632922 fnschool-20240530.80026.842/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    19437 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.610925 fnschool-20240530.80026.842/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.633922 fnschool-20240530.80026.842/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.611925 fnschool-20240530.80026.842/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.633922 fnschool-20240530.80026.842/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.611925 fnschool-20240530.80026.842/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.633922 fnschool-20240530.80026.842/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-29 16:26:42.000000 fnschool-20240530.80026.842/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      898 2024-05-24 05:00:49.000000 fnschool-20240530.80026.842/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240530.80026.842/src/fnschool/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5572 2024-05-29 14:01:51.000000 fnschool-20240530.80026.842/src/fnschool/user.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-29 16:26:47.634922 fnschool-20240530.80026.842/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2458 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-29 16:26:47.000000 fnschool-20240530.80026.842/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240530.80012.827/LICENSE` & `fnschool-20240530.80026.842/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/PKG-INFO` & `fnschool-20240530.80026.842/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.80012.827
+Version: 20240530.80026.842
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.80012.827/README.md` & `fnschool-20240530.80026.842/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/pyproject.toml` & `fnschool-20240530.80026.842/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/__init__.py` & `fnschool-20240530.80026.842/src/fnschool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 from fnschool.path import *
 from fnschool.entry import *
 from fnschool.external import *
 from fnschool.user import *
 from fnschool.config import *
 
 
-__version__ = "20240530.80012.827"
+__version__ = "20240530.80026.842"
 
 
 # The end.
```

### Comparing `fnschool-20240530.80012.827/src/fnschool/app.py` & `fnschool-20240530.80026.842/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/bill.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/canteen.toml` & `fnschool-20240530.80026.842/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/consuming.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240530.80026.842/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240530.80026.842/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/entry.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/food.cp.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/food.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/food_classes.toml` & `fnschool-20240530.80026.842/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/operator.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/path.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/profile.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/test.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/canteen/workbook.py` & `fnschool-20240530.80026.842/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/config.py` & `fnschool-20240530.80026.842/src/fnschool/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/entry.py` & `fnschool-20240530.80026.842/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/exam/entry.py` & `fnschool-20240530.80026.842/src/fnschool/exam/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/external.py` & `fnschool-20240530.80026.842/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/fnprint.py` & `fnschool-20240530.80026.842/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/language.py` & `fnschool-20240530.80026.842/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240530.80026.842/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/path.py` & `fnschool-20240530.80026.842/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/test.py` & `fnschool-20240530.80026.842/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool/user.py` & `fnschool-20240530.80026.842/src/fnschool/user.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240530.80012.827/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240530.80026.842/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240530.80012.827
+Version: 20240530.80026.842
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240530.80012.827/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240530.80026.842/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

