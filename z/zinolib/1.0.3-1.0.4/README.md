# Comparing `tmp/zinolib-1.0.3.tar.gz` & `tmp/zinolib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zinolib-1.0.3.tar", last modified: Thu Apr  4 12:57:16 2024, max compression
+gzip compressed data, was "zinolib-1.0.4.tar", last modified: Wed May 29 08:05:02 2024, max compression
```

## Comparing `zinolib-1.0.3.tar` & `zinolib-1.0.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.296699 zinolib-1.0.3/
--rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.0.3/.git-blame-ignore-revs
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.288699 zinolib-1.0.3/.github/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/.github/workflows/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-03-18 06:51:15.000000 zinolib-1.0.3/.github/workflows/linter.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.0.3/.github/workflows/publish-test-results.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)     1406 2024-03-18 06:51:15.000000 zinolib-1.0.3/.github/workflows/test.yml
--rw-rw-r--   0 hm        (1000) hm        (1000)      192 2024-03-18 06:51:15.000000 zinolib-1.0.3/.gitignore
--rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.0.3/.pre-commit-config.yaml
--rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.0.3/LICENSE
--rw-rw-r--   0 hm        (1000) hm        (1000)      484 2024-03-18 06:51:15.000000 zinolib-1.0.3/Makefile
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-04-04 12:57:16.292698 zinolib-1.0.3/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.0.3/README.rst
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/examples/
--rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/auth.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.0.3/examples/host_up_cleanup.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/monitor.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-add.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/pm-test2.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.0.3/examples/reboot.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.0.3/examples/schedule_reboot_host.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/test-with.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.0.3/examples/test.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2024-03-18 06:51:15.000000 zinolib-1.0.3/pyproject.toml
--rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-04-04 12:57:16.296699 zinolib-1.0.3/setup.cfg
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.288699 zinolib-1.0.3/src/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.0.3/src/zinolib/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      689 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/compat.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      373 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/models.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      917 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2545 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/config/zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib/controllers/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/controllers/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2015 2024-04-04 12:53:35.000000 zinolib-1.0.3/src/zinolib/controllers/base.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    19002 2024-04-04 12:53:52.000000 zinolib-1.0.3/src/zinolib/controllers/zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7072 2024-03-20 09:16:53.000000 zinolib-1.0.3/src/zinolib/event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)    38357 2024-03-20 09:16:58.000000 zinolib-1.0.3/src/zinolib/ritz.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-03-18 06:51:15.000000 zinolib-1.0.3/src/zinolib/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib/version.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.0.3/src/zinolib/zino_emu.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/src/zinolib.egg-info/
--rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/SOURCES.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/dependency_links.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-11-27 12:05:48.000000 zinolib-1.0.3/src/zinolib.egg-info/not-zip-safe
--rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/requires.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-04-04 12:57:16.000000 zinolib-1.0.3/src/zinolib.egg-info/top_level.txt
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.0.3/tests/__init__.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/config/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_tcl.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_toml.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     2280 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/config/test_zino1.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-04 12:57:16.292698 zinolib-1.0.3/tests/ritz/
--rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/test_default.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/ritz/test_slow.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9314 2024-04-04 12:53:35.000000 zinolib-1.0.3/tests/test_zinolib_controllers_zino1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     9189 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/test_zinolib_event_types.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.0.3/tests/test_zinolib_utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2024-03-18 06:51:15.000000 zinolib-1.0.3/tests/utils.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-03-18 06:51:15.000000 zinolib-1.0.3/tox.ini
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      114 2023-08-23 12:45:06.000000 zinolib-1.0.4/.git-blame-ignore-revs
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/.github/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/.github/workflows/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1654 2024-05-22 06:40:42.000000 zinolib-1.0.4/.github/workflows/linter.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1049 2023-10-17 13:10:05.000000 zinolib-1.0.4/.github/workflows/publish-test-results.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1406 2024-05-29 08:04:50.000000 zinolib-1.0.4/.github/workflows/test.yml
+-rw-rw-r--   0 hm        (1000) hm        (1000)      192 2024-05-22 06:40:42.000000 zinolib-1.0.4/.gitignore
+-rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-08-23 12:43:58.000000 zinolib-1.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-08-23 12:43:58.000000 zinolib-1.0.4/LICENSE
+-rw-rw-r--   0 hm        (1000) hm        (1000)      484 2024-05-22 06:40:42.000000 zinolib-1.0.4/Makefile
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-29 08:05:02.399951 zinolib-1.0.4/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)      955 2023-08-23 12:45:06.000000 zinolib-1.0.4/README.rst
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/examples/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      771 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/auth.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2993 2023-08-15 12:56:17.000000 zinolib-1.0.4/examples/host_up_cleanup.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2598 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/monitor.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2261 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-add.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1932 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1930 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/pm-test2.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2199 2023-08-17 12:47:05.000000 zinolib-1.0.4/examples/reboot.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1902 2023-08-17 12:47:05.000000 zinolib-1.0.4/examples/schedule_reboot_host.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2465 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/test-with.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2576 2023-08-23 12:43:58.000000 zinolib-1.0.4/examples/test.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1172 2024-05-29 08:02:49.000000 zinolib-1.0.4/pyproject.toml
+-rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-05-29 08:05:02.399951 zinolib-1.0.4/setup.cfg
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/src/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.395951 zinolib-1.0.4/src/zinolib/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1146 2023-08-24 07:39:23.000000 zinolib-1.0.4/src/zinolib/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      689 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/compat.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      373 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/models.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     3906 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      917 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1346 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2545 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/config/zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib/controllers/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/controllers/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2015 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/controllers/base.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    19605 2024-05-29 08:01:44.000000 zinolib-1.0.4/src/zinolib/controllers/zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7270 2024-05-29 07:55:29.000000 zinolib-1.0.4/src/zinolib/event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)    38357 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/ritz.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2723 2024-05-22 06:40:42.000000 zinolib-1.0.4/src/zinolib/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      411 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib/version.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4549 2023-08-23 12:45:06.000000 zinolib-1.0.4/src/zinolib/zino_emu.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/src/zinolib.egg-info/
+-rw-r--r--   0 hm        (1000) hm        (1000)    14717 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1401 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/not-zip-safe
+-rw-rw-r--   0 hm        (1000) hm        (1000)       48 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/requires.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        8 2024-05-29 08:05:02.000000 zinolib-1.0.4/src/zinolib.egg-info/top_level.txt
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2023-08-24 07:39:23.000000 zinolib-1.0.4/tests/__init__.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/config/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2840 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_tcl.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1664 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_toml.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1155 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2280 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/config/test_zino1.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-05-29 08:05:02.399951 zinolib-1.0.4/tests/ritz/
+-rw-rw-r--   0 hm        (1000) hm        (1000)        0 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     7530 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/test_default.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1322 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/ritz/test_slow.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9817 2024-05-29 08:01:44.000000 zinolib-1.0.4/tests/test_zinolib_controllers_zino1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     9548 2024-05-29 07:55:29.000000 zinolib-1.0.4/tests/test_zinolib_event_types.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      390 2023-10-12 09:04:56.000000 zinolib-1.0.4/tests/test_zinolib_utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4082 2024-05-22 06:40:42.000000 zinolib-1.0.4/tests/utils.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1573 2024-05-29 08:02:49.000000 zinolib-1.0.4/tox.ini
```

### Comparing `zinolib-1.0.3/.github/workflows/linter.yml` & `zinolib-1.0.4/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/.github/workflows/publish-test-results.yml` & `zinolib-1.0.4/.github/workflows/publish-test-results.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/.github/workflows/test.yml` & `zinolib-1.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/LICENSE` & `zinolib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/PKG-INFO` & `zinolib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.3/README.rst` & `zinolib-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/auth.py` & `zinolib-1.0.4/examples/auth.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/host_up_cleanup.py` & `zinolib-1.0.4/examples/host_up_cleanup.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/monitor.py` & `zinolib-1.0.4/examples/monitor.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/pm-add.py` & `zinolib-1.0.4/examples/pm-add.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/pm-test.py` & `zinolib-1.0.4/examples/pm-test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/pm-test2.py` & `zinolib-1.0.4/examples/pm-test2.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/reboot.py` & `zinolib-1.0.4/examples/reboot.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/schedule_reboot_host.py` & `zinolib-1.0.4/examples/schedule_reboot_host.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/test-with.py` & `zinolib-1.0.4/examples/test-with.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/examples/test.py` & `zinolib-1.0.4/examples/test.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/pyproject.toml` & `zinolib-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/__init__.py` & `zinolib-1.0.4/src/zinolib/__init__.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/compat.py` & `zinolib-1.0.4/src/zinolib/compat.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/config/tcl.py` & `zinolib-1.0.4/src/zinolib/config/tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/config/toml.py` & `zinolib-1.0.4/src/zinolib/config/toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/config/utils.py` & `zinolib-1.0.4/src/zinolib/config/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/config/zino1.py` & `zinolib-1.0.4/src/zinolib/config/zino1.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/controllers/base.py` & `zinolib-1.0.4/src/zinolib/controllers/base.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/controllers/zino1.py` & `zinolib-1.0.4/src/zinolib/controllers/zino1.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 To get a set of removed event ids::
 
     > event_manager.removed_ids
 
 For updates, either regularly use ``get_events()`` or utilize the UpdateHandler::
 
     > updater = UpdateHandler(event_manager)
+    > updater.connect()
     > updated = updater.get_event_update()
 
 The updater is unique per authenticated user and is only available after login.
 
 ``updater.get_event_update()`` updates ``event_manager.events`` and
 ``event_manager.removed_ids`` and returns the id of a changed event on any
 change, falsey otherwise. Check the id against the removed_id's set to see if
@@ -123,37 +124,52 @@
         HISTORY = "history"
         LOG = "log"
         SCAVENGED = "scavenged"
 
     class UpdateError(Zino1Error):
         pass
 
+    class SocketError(UpdateError):
+        pass
+
     def __init__(self, manager, autoremove=False):
+        self._connected = False
         if not manager.is_authenticated:
             msg = "Cannot initiate update handler, not authenticated"
             raise self.UpdateError(msg)
         self.manager = manager
-        if not self.manager.session.push:
-            self.manager.connect_push_channel()
         self.events = manager.events
         self.autoremove = autoremove
 
+    def connect(self):
+        if not self.manager.session.push:
+            self.manager.connect_push_channel()
+        self.check_connection()
+
+    def check_connection(self):
+        if self.manager.session.push._sock.fileno() >= 0:
+            self._connected = True
+            return True
+        self._connected = False
+        raise self.SocketError("Push socket reports failure, fileno = -1")
+
     def get_event_update(self):
         """
         Fetches one update for a single event and runs the appropriate handler
 
         Attributes on the update object:
 
         id: event id
         type: update type, triggers the correct handler
         info: a type-specific string with the actual change
 
         Run in a loop/every N seconds for a lightweight way to update the event
         list
         """
+        self.check_connection()
         update = self.manager.session.push.poll()
         if not update:
             return False
         return self.handle_event_update(update)
 
     def update(self, event_id: int):
         "Refresh an event from the server, refreshing everything"
@@ -264,18 +280,24 @@
         password = password if password else session.request.password
         if not username and password:
             raise ValueError("Both username and password must be set and truthy")
         session.request.authenticate(username, password)
         return session
 
     @staticmethod
-    def close_session(session):
+    def close_push_channel(session):
         if hasattr(session.push, '_sock'):
             session.push._sock.close()
+        session.push = None
+
+    @classmethod
+    def close_session(cls, session):
+        cls.close_push_channel()
         session.request.close()
+        session.request = None
         return None
 
 
 class EventAdapter:
     FIELD_MAP = {
         "state": "adm_state",
         "bfdAddr": "bfd_addr",
```

### Comparing `zinolib-1.0.3/src/zinolib/event_types.py` & `zinolib-1.0.4/src/zinolib/event_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 
     CLOSED = "closed"
     CONFIRM_WAIT = "confirm-wait"
     IGNORED = "ignored"
     OPEN = "open"
     WAITING = "waiting"
     WORKING = "working"
+    UNKNOWN = "unknown"
+
+    @classmethod
+    def _missing_(cls, value):
+        # Python 3.12: "if not value in cls:"
+        if not value in cls._value2member_map_:
+            return cls.UNKNOWN
 
 
 class FlapState(StrEnum):
     FLAPPING = 'flapping'
     STABLE = 'stable'
```

### Comparing `zinolib-1.0.3/src/zinolib/ritz.py` & `zinolib-1.0.4/src/zinolib/ritz.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/utils.py` & `zinolib-1.0.4/src/zinolib/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib/zino_emu.py` & `zinolib-1.0.4/src/zinolib/zino_emu.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/src/zinolib.egg-info/PKG-INFO` & `zinolib-1.0.4/src/zinolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zinolib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python interface to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `zinolib-1.0.3/src/zinolib.egg-info/SOURCES.txt` & `zinolib-1.0.4/src/zinolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/config/test_tcl.py` & `zinolib-1.0.4/tests/config/test_tcl.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/config/test_toml.py` & `zinolib-1.0.4/tests/config/test_toml.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/config/test_utils.py` & `zinolib-1.0.4/tests/config/test_utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/config/test_zino1.py` & `zinolib-1.0.4/tests/config/test_zino1.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/ritz/test_default.py` & `zinolib-1.0.4/tests/ritz/test_default.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/ritz/test_slow.py` & `zinolib-1.0.4/tests/ritz/test_slow.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tests/test_zinolib_controllers_zino1.py` & `zinolib-1.0.4/tests/test_zinolib_controllers_zino1.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,26 @@
 
 class Zino1EventManagerTest(unittest.TestCase):
 
     def init_manager(self):
         zino1 = FakeZino1EventManager.configure(None)
         return zino1
 
+    def test_create_event_from_id_receiving_garbage_admstate_is_safely_handled(self):
+        global raw_attrlist
+        zino1 = self.init_manager()
+        good_attrlist = raw_attrlist[:] # copy
+        try:
+            raw_attrlist[0] = "state: garbage admstate"
+            event = zino1.create_event_from_id(139110)
+            self.assertEqual(event.adm_state, AdmState.UNKNOWN)
+        finally:
+            # reset to known good attrlist for other tests
+            raw_attrlist = good_attrlist
+
     def test_create_event_from_id_may_get_garabage_data(self):
         def falsey(_):
             return False
 
         zino1 = self.init_manager()
         old = zino1._event_adapter.validate_raw_attrlist
         zino1._event_adapter.validate_raw_attrlist = staticmethod(falsey)
```

### Comparing `zinolib-1.0.3/tests/test_zinolib_event_types.py` & `zinolib-1.0.4/tests/test_zinolib_event_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,7 +248,19 @@
         dt = datetime.fromisoformat("2023-06-28T10:41:54+00:00")
         log_list = [{
             "date": dt,
             "log": "fhgj",
         }]
         updated_event = event_manager.set_log_for_event(event, log_list)
         self.assertTrue(event_manager.events[event.id].log)
+
+
+class AdmStateTest(unittest.TestCase):
+
+    def test_golden_path(self):
+        for state in AdmState:
+            enum_state = AdmState(state)
+            self.assertEqual(enum_state.value, state)
+
+    def test_garbage_input_should_be_converted_to_UNKNOWN(self):
+        value = AdmState("random garbage")
+        self.assertEqual(value, AdmState.UNKNOWN)
```

### Comparing `zinolib-1.0.3/tests/utils.py` & `zinolib-1.0.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `zinolib-1.0.3/tox.ini` & `zinolib-1.0.4/tox.ini`

 * *Files identical despite different names*

