# Comparing `tmp/apn-validators-0.2.tar.gz` & `tmp/apn-validators-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apn-validators-0.2.tar", last modified: Wed May  8 07:01:14 2024, max compression
+gzip compressed data, was "apn-validators-0.3.tar", last modified: Wed May 29 10:08:14 2024, max compression
```

## Comparing `apn-validators-0.2.tar` & `apn-validators-0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-08 07:01:14.251352 apn-validators-0.2/
--rw-r--r--   0 linux     (1000) linux     (1000)       56 2024-05-08 07:01:14.251352 apn-validators-0.2/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)        0 2024-05-08 05:24:51.000000 apn-validators-0.2/README.md
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-08 07:01:14.251352 apn-validators-0.2/apn_validators/
--rw-rw-r--   0 linux     (1000) linux     (1000)      192 2024-05-07 10:59:30.000000 apn-validators-0.2/apn_validators/__init__.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     4024 2024-05-08 06:04:25.000000 apn-validators-0.2/apn_validators/base_validator.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     3722 2024-05-08 05:25:12.000000 apn-validators-0.2/apn_validators/date_validators.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     1055 2024-05-07 11:29:37.000000 apn-validators-0.2/apn_validators/file_validators.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     4484 2024-05-07 21:03:15.000000 apn-validators-0.2/apn_validators/number_validators.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     4602 2024-05-08 05:25:19.000000 apn-validators-0.2/apn_validators/pattern_validators.py
--rw-rw-r--   0 linux     (1000) linux     (1000)     9970 2024-05-08 05:25:23.000000 apn-validators-0.2/apn_validators/string_validators.py
-drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-08 07:01:14.251352 apn-validators-0.2/apn_validators.egg-info/
--rw-r--r--   0 linux     (1000) linux     (1000)       56 2024-05-08 07:01:14.000000 apn-validators-0.2/apn_validators.egg-info/PKG-INFO
--rw-rw-r--   0 linux     (1000) linux     (1000)      407 2024-05-08 07:01:14.000000 apn-validators-0.2/apn_validators.egg-info/SOURCES.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)        1 2024-05-08 07:01:14.000000 apn-validators-0.2/apn_validators.egg-info/dependency_links.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       15 2024-05-08 07:01:14.000000 apn-validators-0.2/apn_validators.egg-info/top_level.txt
--rw-rw-r--   0 linux     (1000) linux     (1000)       38 2024-05-08 07:01:14.251352 apn-validators-0.2/setup.cfg
--rw-rw-r--   0 linux     (1000) linux     (1000)      202 2024-05-08 07:00:52.000000 apn-validators-0.2/setup.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-29 10:08:14.633171 apn-validators-0.3/
+-rw-r--r--   0 linux     (1000) linux     (1000)       56 2024-05-29 10:08:14.633171 apn-validators-0.3/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)     3614 2024-05-24 01:17:53.000000 apn-validators-0.3/README.md
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-29 10:08:14.633171 apn-validators-0.3/apn_validators/
+-rw-rw-r--   0 linux     (1000) linux     (1000)       29 2024-05-21 17:07:52.000000 apn-validators-0.3/apn_validators/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)     2744 2024-05-26 06:21:17.000000 apn-validators-0.3/apn_validators/base_validator.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-29 10:08:14.633171 apn-validators-0.3/apn_validators/rules/
+-rw-rw-r--   0 linux     (1000) linux     (1000)      161 2024-05-21 17:07:42.000000 apn-validators-0.3/apn_validators/rules/__init__.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)     3811 2024-05-26 08:30:35.000000 apn-validators-0.3/apn_validators/rules/date_validators.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)     1616 2024-05-27 18:53:04.000000 apn-validators-0.3/apn_validators/rules/file_validators.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)     8930 2024-05-26 03:53:56.000000 apn-validators-0.3/apn_validators/rules/number_validators.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)     5929 2024-05-24 01:50:53.000000 apn-validators-0.3/apn_validators/rules/pattern_validators.py
+-rw-rw-r--   0 linux     (1000) linux     (1000)    13453 2024-05-25 18:56:48.000000 apn-validators-0.3/apn_validators/rules/string_validators.py
+drwxrwxr-x   0 linux     (1000) linux     (1000)        0 2024-05-29 10:08:14.633171 apn-validators-0.3/apn_validators.egg-info/
+-rw-r--r--   0 linux     (1000) linux     (1000)       56 2024-05-29 10:08:14.000000 apn-validators-0.3/apn_validators.egg-info/PKG-INFO
+-rw-rw-r--   0 linux     (1000) linux     (1000)      470 2024-05-29 10:08:14.000000 apn-validators-0.3/apn_validators.egg-info/SOURCES.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)        1 2024-05-29 10:08:14.000000 apn-validators-0.3/apn_validators.egg-info/dependency_links.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       15 2024-05-29 10:08:14.000000 apn-validators-0.3/apn_validators.egg-info/top_level.txt
+-rw-rw-r--   0 linux     (1000) linux     (1000)       38 2024-05-29 10:08:14.633171 apn-validators-0.3/setup.cfg
+-rw-rw-r--   0 linux     (1000) linux     (1000)      202 2024-05-29 10:07:55.000000 apn-validators-0.3/setup.py
```

