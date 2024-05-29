# Comparing `tmp/popoll_backend-0.0.59.tar.gz` & `tmp/popoll_backend-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.59.tar", last modified: Tue May 28 12:46:18 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.60.tar", last modified: Wed May 29 12:57:39 2024, max compression
```

## Comparing `popoll_backend-0.0.59.tar` & `popoll_backend-0.0.60.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.354350 popoll_backend-0.0.59/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-28 12:46:18.353350 popoll_backend-0.0.59/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.335350 popoll_backend-0.0.59/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     8225 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.337350 popoll_backend-0.0.59/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.339350 popoll_backend-0.0.59/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.341350 popoll_backend-0.0.59/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/empty.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/polls.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/users.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.348350 popoll_backend-0.0.59/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      757 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/delete_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_all_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_all_sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.353350 popoll_backend-0.0.59/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-28 12:46:18.000000 popoll_backend-0.0.59/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2799 2024-05-28 12:46:18.000000 popoll_backend-0.0.59/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 12:46:18.000000 popoll_backend-0.0.59/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-28 12:46:18.000000 popoll_backend-0.0.59/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-28 12:46:18.000000 popoll_backend-0.0.59/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-28 12:46:12.000000 popoll_backend-0.0.59/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 12:46:18.354350 popoll_backend-0.0.59/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 12:46:18.353350 popoll_backend-0.0.59/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_01_get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_02_create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_03_update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_04_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_08_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_09_create_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_10_get_user.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_11_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_12_delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_13_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_14_create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_15_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_16_update_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_17_delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_18_create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_19_update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_20_delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_21_get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_22_get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_23_get_create_session.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-28 12:45:58.000000 popoll_backend-0.0.59/tests/test_24_get_all_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.726440 popoll_backend-0.0.60/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     8336 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.727440 popoll_backend-0.0.60/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.729440 popoll_backend-0.0.60/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.732440 popoll_backend-0.0.60/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/polls.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.738440 popoll_backend-0.0.60/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_old_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_all_sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-29 12:57:34.000000 popoll_backend-0.0.60/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.742440 popoll_backend-0.0.60/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_23_get_create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_24_get_all_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_25_delete_old_dates.py
```

### Comparing `popoll_backend-0.0.59/PKG-INFO` & `popoll_backend-0.0.60/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.59
+Version: 0.0.60
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
+License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: flask_cors
 Requires-Dist: flask-restful
 Requires-Dist: jsonpickle
 Requires-Dist: werkzeug
 
 # popoll backend
```

### Comparing `popoll_backend-0.0.59/popoll_backend/__main__.py` & `popoll_backend-0.0.60/popoll_backend/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 from flask_restful import Api, Resource
 from functools import wraps
 from typing import Any, Dict
 
 from popoll_backend.model.payload.history import History
 from popoll_backend.query.create_answer import CreateAnswer
 from popoll_backend.query.create_date import CreateDate
-from popoll_backend.query.create_instrument import CreateInstrument
 from popoll_backend.query.create_poll import CreatePoll
 from popoll_backend.query.create_user import CreateUser
 from popoll_backend.query.delete_answer import DeleteAnswer
 from popoll_backend.query.delete_date import DeleteDate
-from popoll_backend.query.delete_instrument import DeleteInstrument
+from popoll_backend.query.delete_old_dates import DeleteOldDates
 from popoll_backend.query.delete_user import DeleteUser
 from popoll_backend.query.get_all_instruments import GetAllInstruments
 from popoll_backend.query.get_all_sessions import GetAllSession
 from popoll_backend.query.get_answer import GetAnswer
 from popoll_backend.query.get_date import GetDate
 from popoll_backend.query.get_date_details import GetDateDetails
 from popoll_backend.query.get_dates import GetDates
@@ -109,15 +108,15 @@
     def post(self, poll: str) -> str: return CreateUser(poll, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
 
 
 
 class PollUserEndpoint(Resource):
     def get(self, poll: str, id:int) -> str: 
         if queryParam(flask.request, 'details'):
-            return GetUserDetails(poll, id).run().toJSON()
+            return GetUserDetails(poll, id, queryParam(flask.request, 'viewOldDates')).run().toJSON()
         else:
             return GetUserWithInstruments(poll, id).run().toJSON()
     
     @history
     def put(self, poll: str, id: int) -> str: return UpdateUser(poll, id, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
     
     @history
@@ -185,18 +184,20 @@
 
 
 
 class SessionEndpoint(Resource):
     def get(self, id: str) -> str: return GetAllSession(id).run().toJSON()
 
 
-
+class DatesEndpoint(Resource):
+    def delete(self) -> str: return DeleteOldDates().run().toJSON()
 
 
 api.add_resource(SessionEndpoint, '/session/<string:id>')
+api.add_resource(DatesEndpoint, '/date')
 
 api.add_resource(PollPollEndpoint, '/<string:poll>')
 api.add_resource(PollInstrumentsEndpoint, '/<string:poll>/instrument')
 api.add_resource(PollUsersEndpoint, '/<string:poll>/user')
 api.add_resource(PollUserEndpoint, '/<string:poll>/user/<int:id>')
 api.add_resource(PollDatesEndpoint, '/<string:poll>/date')
 api.add_resource(PollDateEndpoint, '/<string:poll>/date/<int:id>')
```

### Comparing `popoll_backend-0.0.59/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.60/popoll_backend/model/db/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import sqlite3
+from __future__ import annotations
 
+import datetime
+import sqlite3
 from typing import Any, List
 
 from popoll_backend.model import Payload
-from popoll_backend.model.db import fetchall, fetchone
 
-class Answer(Payload):
+
+class Session(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
-        self.user_id: int = data[1]
-        self.date_id: int = data[2]
-        self.response: bool = bool(data[3])
+        self.session_id: str = data[1]
+        self.user_id: int = data[2]
 
     @classmethod
     def create_table(cls):
-        return """ CREATE TABLE IF NOT EXISTS answers (
-            id integer PRIMARY KEY AUTOINCREMENT,
+        return """CREATE TABLE IF NOT EXISTS sessions (
+            id integer PRIMARY KEY,
+            session_id text NOT NULL,
             user_id integer NOT NULL REFERENCES users(id) ON DELETE CASCADE,
-            date_id integer NOT NULL REFERENCES dates(id) ON DELETE CASCADE,
-            response boolean NOT NULL,
-            UNIQUE(user_id, date_id)
-        ); """
+            datetime text NOT NULL
+        );"""
```

### Comparing `popoll_backend-0.0.59/popoll_backend/model/db/date.py` & `popoll_backend-0.0.60/popoll_backend/model/db/date.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 import datetime
 import sqlite3
 from typing import Any, List, Optional
 
 from popoll_backend.model import Payload
-from popoll_backend.model.db import fetchall, fetchone
 
 
 class Date(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.title: str = data[1]
@@ -21,7 +20,10 @@
         return """ CREATE TABLE IF NOT EXISTS dates (
             id integer PRIMARY KEY AUTOINCREMENT,
             title text NOT NULL,
             date text NOT NULL,
             time text,
             end_time text
         ); """
+        
+    def isOlder(self, compare: datetime.date=datetime.date.today()):
+        return self.date < compare
```

### Comparing `popoll_backend-0.0.59/popoll_backend/model/db/session.py` & `popoll_backend-0.0.60/popoll_backend/model/db/user_instruments.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
-import datetime
 import sqlite3
-from typing import Any, List
+
+from typing import Any, List, Optional, Tuple
 
 from popoll_backend.model import Payload
-from popoll_backend.model.db import fetchone
 
 
-class Session(Payload):
+class UserInstruments(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
-        self.session_id: str = data[1]
-        self.user_id: int = data[2]
+        self.user_id: int = data[1]
+        self.instrument_id: int = data[2]
+        self.is_main: bool = bool(data[3])
 
     @classmethod
     def create_table(cls):
-        return """CREATE TABLE IF NOT EXISTS sessions (
+        return """ CREATE TABLE IF NOT EXISTS user_instruments (
             id integer PRIMARY KEY,
-            session_id text NOT NULL,
             user_id integer NOT NULL REFERENCES users(id) ON DELETE CASCADE,
-            datetime text NOT NULL
-        );"""
+            instrument_id integer NOT NULL REFERENCES instruments(id) ON DELETE CASCADE,
+            is_main boolean NOT NULL
+        ); """
```

### Comparing `popoll_backend-0.0.59/popoll_backend/model/payload/date_details.py` & `popoll_backend-0.0.60/popoll_backend/model/payload/date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.60/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/model/payload/polls.py` & `popoll_backend-0.0.60/popoll_backend/model/payload/polls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import List, Optional
 from popoll_backend.model import Payload
 
 
-class Poll:
+class Poll(Payload):
     
     def __init__(self, id: str, name: str):
         self.id = id
         self.name = name
 
 class Polls(Payload):
     
     def __init__(self, poll: Optional[Poll]=None, polls: Optional[List[Poll]]=None):
         self.polls = []
         if poll != None:
             self.polls.append(poll)
         if polls != None:
-            (self.polls.append(p) for p in polls)
+            for p in polls:
+                self.polls.append(p)
     
     def add(self, poll: Poll):
         self.polls.append(poll)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/model/payload/user_details.py` & `popoll_backend-0.0.60/popoll_backend/model/payload/user_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/model/payload/user_with_instruments.py` & `popoll_backend-0.0.60/popoll_backend/model/payload/user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/query/__init__.py` & `popoll_backend-0.0.60/popoll_backend/query/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,48 @@
+import glob
 import flask
 import os
 import sqlite3
 
 from typing import List, Optional
 
 from popoll_backend.model import Payload
 
+
+def fetchall(cursor: sqlite3.Cursor, ttype: type) -> List[type]:
+        return [ttype(row) for row in cursor.fetchall()]
+
+def fetchlast(cursor: sqlite3.Cursor, ttype: type) -> type:
+        res = fetchall(cursor, ttype)
+        if len(res) > 0:
+            return res[-1]
+        flask.abort(404, 'Not found')
+        
 class Query:
     
     def run(self) -> Payload:
+        answers: List[Payload] = []
+        for db in sorted(glob.glob('*.db')):
+            # We do not want to break in case a db is incorrect
+            try:
+                with sqlite3.connect(db) as connection:
+                    cursor: sqlite3.Cursor = connection.cursor()
+                    self.process(db[0:-3], cursor)
+                    answers.append(self.buildResponse(db[0:-3], cursor))
+            except Exception as e:
+                print(e)
+        return self.mergeResponses(answers)
+    
+    def process(self, db: str, cursor: sqlite3.Cursor) -> None:
+        raise NotImplementedError()
+    
+    def buildResponse(self, db: str, cursor: sqlite3.Cursor) -> Payload:
+        raise NotImplementedError()
+    
+    def mergeResponses(self, answers: List[Payload]) -> Payload:
         raise NotImplementedError()
 
 class PollQuery(Query):
     
     fail_if_db_exists: bool = False
     fail_if_db_not_exists: bool = True
     
@@ -52,15 +82,7 @@
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         raise NotImplementedError()
     
     def error(self, e: sqlite3.Error) -> None:
         pass
     
-    def fetchall(self, cursor: sqlite3.Cursor, ttype: type) -> List[type]:
-        return [ttype(row) for row in cursor.fetchall()]
-
-    def fetchlast(self, cursor: sqlite3.Cursor, ttype: type) -> type:
-        res = self.fetchall(cursor, ttype)
-        if len(res) > 0:
-            return res[-1]
-        flask.abort(404, 'Not found')
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.60/popoll_backend/query/create_answer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class CreateAnswer(PollQuery):
     
     user_id: int
     date_id: int
     
@@ -18,13 +18,13 @@
         self.user_id = user_id
         self.date_id = date_id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         self.id = cursor.execute('INSERT INTO answers(user_id, date_id, response) VALUES (?, ?, ?)', (self.user_id, self.date_id, True)).lastrowid
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> Answer:
-        return self.fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
+        return fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
                 flask.abort(409, f'Answer for this user already exists. PUT should be triggered instead.')
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_date.py` & `popoll_backend-0.0.60/popoll_backend/query/create_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class CreateDate(PollQuery):
     
     title: str
     date: datetime.date
     time: Optional[datetime.time]
@@ -22,8 +22,8 @@
         self.time = time
         self.end_time = end_time
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time) VALUES (?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time)).lastrowid
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
-        return self.fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
+        return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.60/popoll_backend/query/get_instrument.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
-class CreateInstrument(PollQuery):
+class GetInstrument(PollQuery):
     
-    name: str
-    rank: int
+    id: int
     
-    instrument_id: int
-    
-    def __init__(self, poll: str, name: str, rank: int):
+    def __init__(self, poll: str, id: int):
         super().__init__(poll)
-        self.name = name
-        self.rank = rank
-       
-    def process(self, cursor: sqlite3.Cursor) -> None:
-        self.instrument_id = cursor.execute('INSERT INTO instruments.instruments(name, rank) VALUES (?,?)', (self.name, self.rank)).lastrowid
+        self.id = id
     
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        pass
+        
     def buildResponse(self, cursor: sqlite3.Cursor) -> Instrument:
-        return self.fetchlast(cursor.execute('SELECT * FROM instruments.instruments WHERE id=?', (self.id,)), Instrument)
+        return fetchlast(cursor.execute('SELECT * FROM instruments WHERE id=?', (self.id,)), Instrument)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.60/popoll_backend/query/create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_session.py` & `popoll_backend-0.0.60/popoll_backend/query/create_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class CreateSession(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: str, user_id: int):
@@ -15,11 +15,11 @@
         self.user_id = user_id
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         cursor.execute('DELETE FROM sessions WHERE session_id=?', (self.id,))
         return cursor.execute('INSERT INTO sessions(session_id, user_id, datetime) VALUES(?, ?, ?)', (self.id, self.user_id, self.getNow())).lastrowid
 
     def buildResponse(self, cursor: sqlite3.Cursor) -> Session:
-        return self.fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
+        return fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
     
     def getNow(self) -> str:
         return datetime.datetime.now().isoformat(sep='T', timespec='auto')
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/create_user.py` & `popoll_backend-0.0.60/popoll_backend/query/create_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class CreateUser(PollQuery):
     
     name: str
     main_instrument: int
     instruments: List[int]
@@ -27,16 +27,16 @@
     def process(self, cursor: sqlite3.Cursor) -> None:
         self.id = cursor.execute('INSERT INTO users(name) VALUES(?)', (self.name,)).lastrowid
         rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
         cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         return UserWithInstruments(
-            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
-            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
-            user_instruments=self.fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
+            user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
+            user_instruments=fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
         )
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
                 flask.abort(409, f'User with name {self.name} already exists.')
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.60/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.60/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/query/delete_instrument.py` & `popoll_backend-0.0.60/popoll_backend/query/delete_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
-from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import PollQuery
 
 
-class DeleteInstrument(PollQuery):
+class DeleteUser(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('DELETE FROM instruments.instruments WHERE id=?', (self.id,))
+        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
     
     def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
         return Empty()
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.60/popoll_backend/query/get_users.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import sqlite3
-from popoll_backend.model import Payload
-from popoll_backend.model.payload.empty import Empty
-from popoll_backend.model.payload.id_payload import IdPayload
-from popoll_backend.query import PollQuery
+from typing import List
 
+from popoll_backend.model.db.instrument import Instrument
+from popoll_backend.model.db.user import User
+from popoll_backend.model.db.user_instruments import UserInstruments
+from popoll_backend.model.payload.users import Users
+from popoll_backend.query import PollQuery, fetchall
 
-class DeleteUser(PollQuery):
-    
-    id: int
+
+class GetUsers(PollQuery):
     
-    def __init__(self, poll: str, id: int):
+    def __init__(self, poll: str):
         super().__init__(poll)
-        self.id = id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
-    
-    def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
-        return Empty()
-    
+        pass
+
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Users:
+        return Users(fetchall(cursor.execute('SELECT * FROM users ORDER BY name COLLATE NOCASE'), User))
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_all_instruments.py` & `popoll_backend-0.0.60/popoll_backend/query/get_all_instruments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall
 
 
 class GetAllInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
         super().__init__(poll)
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
             
     def buildResponse(self, cursor: sqlite3.Cursor) -> Instruments:
-        return Instruments(self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument))
+        return Instruments(fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument))
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_date.py` & `popoll_backend-0.0.60/popoll_backend/query/get_dates.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sqlite3
+from typing import List
 
-from popoll_backend.model import Payload
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery
+from popoll_backend.model.payload.dates import Dates
+from popoll_backend.query import PollQuery, fetchall
 
 
-class GetDate(PollQuery):
+class GetDates(PollQuery):
     
-    id: int
+    dates: List[Date]
     
-    def __init__(self, poll: str, id: int):
+    def __init__(self, poll: str):
         super().__init__(poll)
-        self.id = id
 
-    def process(self, cursor: sqlite3.Cursor) -> None:
+    def process(self, cursor: sqlite3.Cursor):
         pass
-
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return self.fetchlast(cursor.execute('SELECT * FROM dates WHERE id=? ORDER BY date, time', (self.id,)), Date)
+        
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Dates:
+        return Dates(fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date))
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_date_details.py` & `popoll_backend-0.0.60/popoll_backend/query/get_date_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.date_details import DateDetails
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class GetDateDetails(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
@@ -19,13 +19,13 @@
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
 
     def buildResponse(self, cursor: sqlite3.Cursor) -> DateDetails:
         globally_used_instruments = [row[0] for row in cursor.execute('SELECT DISTINCT instrument_id FROM user_instruments').fetchall()]
         return DateDetails(
-            date=self.fetchlast(cursor.execute('SELECT * FROM dates where id=?', (self.id,)), Date), 
-            answers=self.fetchall(cursor.execute('SELECT * FROM answers where date_id=?', (self.id,)), Answer),
-            users=self.fetchall(cursor.execute('SELECT * FROM users ORDER BY name COLLATE NOCASE'), User),     
-            instruments=[instr for instr in self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments],
-            user_instruments=self.fetchall(cursor.execute('SELECT * FROM user_instruments'), UserInstruments)
+            date=fetchlast(cursor.execute('SELECT * FROM dates where id=?', (self.id,)), Date), 
+            answers=fetchall(cursor.execute('SELECT * FROM answers where date_id=?', (self.id,)), Answer),
+            users=fetchall(cursor.execute('SELECT * FROM users ORDER BY name COLLATE NOCASE'), User),     
+            instruments=[instr for instr in fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments],
+            user_instruments=fetchall(cursor.execute('SELECT * FROM user_instruments'), UserInstruments)
         )
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.60/popoll_backend/query/get_date.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sqlite3
-from typing import List
 
+from popoll_backend.model import Payload
 from popoll_backend.model.db.date import Date
-from popoll_backend.model.payload.dates import Dates
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
-class GetDates(PollQuery):
+class GetDate(PollQuery):
     
-    dates: List[Date]
+    id: int
     
-    def __init__(self, poll: str):
+    def __init__(self, poll: str, id: int):
         super().__init__(poll)
+        self.id = id
 
-    def process(self, cursor: sqlite3.Cursor):
+    def process(self, cursor: sqlite3.Cursor) -> None:
         pass
-        
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Dates:
-        return Dates(self.fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date))
+
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
+        return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=? ORDER BY date, time', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.60/popoll_backend/query/get_instruments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sqlite3
 from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.payload.instruments import Instruments
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall
 
 
 class GetInstruments(PollQuery):
     
     instruments: List[Instrument]
     
     def __init__(self, poll: str):
         super().__init__(poll)
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
             
     def buildResponse(self, cursor: sqlite3.Cursor) -> Instruments:
         globally_used_instruments = [row[0] for row in cursor.execute('SELECT DISTINCT instrument_id FROM user_instruments').fetchall()]
-        return Instruments([instr for instr in self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments])
+        return Instruments([instr for instr in fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments])
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.60/popoll_backend/query/get_search_answer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class GetSearchAnswer(PollQuery):
     
     userId: int
     dateId: int
     
@@ -16,8 +16,8 @@
         self.userId = userId
         self.dateId = dateId
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Answer:
-        return self.fetchlast(cursor.execute('SELECT * FROM answers WHERE user_id=? AND date_id=?', (self.userId, self.dateId)), Answer)
+        return fetchlast(cursor.execute('SELECT * FROM answers WHERE user_id=? AND date_id=?', (self.userId, self.dateId)), Answer)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_session.py` & `popoll_backend-0.0.60/popoll_backend/query/get_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlite3
 
 from popoll_backend.model.db.session import Session
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class GetSession(PollQuery):
     
     id: int
     session: Session
     
@@ -13,8 +13,8 @@
         super().__init__(poll)
         self.id = id
 
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
 
     def buildResponse(self, cursor: sqlite3.Cursor) -> Session:
-        return self.fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
+        return fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_user_details.py` & `popoll_backend-0.0.60/popoll_backend/query/get_user_details.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 import sqlite3
 
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.user import User
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.model.payload.user_details import UserDetails
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class GetUserDetails(PollQuery):
     
     id: int
+    viewOldDates: bool
     
-    def __init__(self, poll: str, id: int):
+    def __init__(self, poll: str, id: int, viewOldDates: bool):
         super().__init__(poll)
         self.id = id
+        self.viewOldDates = viewOldDates
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> UserWithInstruments:
         return UserDetails(
-            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
-            answers=self.fetchall(cursor.execute('SELECT * FROM answers WHERE user_id=?', (self.id,)), Answer),
-            dates=self.fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date)
+            user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            answers=fetchall(cursor.execute('SELECT * FROM answers WHERE user_id=?', (self.id,)), Answer),
+            dates=self.getDates(cursor)
         )
         
-        
+    def getDates(self, cursor: sqlite3.Cursor):
+        dates = fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date)
+        if not self.viewOldDates:
+            dates = [date for date in dates if not date.isOlder()]
+        return dates
+
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/get_user_with_instruments.py` & `popoll_backend-0.0.60/popoll_backend/query/get_user_with_instruments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class GetUserWithInstruments(PollQuery):
     
     id: int
     
     def __init__(self, poll: str, id: int):
@@ -16,14 +16,14 @@
         self.id = id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> UserWithInstruments:
         return UserWithInstruments(
-            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
-            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument),
-            user_instruments=self.fetchall(cursor.execute('SELECT * FROM user_instruments WHERE user_id=?', (self.id,)), UserInstruments)
+            user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument),
+            user_instruments=fetchall(cursor.execute('SELECT * FROM user_instruments WHERE user_id=?', (self.id,)), UserInstruments)
         )
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.60/popoll_backend/query/update_answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 from popoll_backend.query.get_answer import GetAnswer
 
 
 class UpdateAnswer(PollQuery):
     
     id: int
     response: Optional[bool]
@@ -17,8 +17,8 @@
         self.id = id
         self.response = response
     
     def process(self, cursor: sqlite3.Cursor):
         cursor.execute('UPDATE answers SET response=? WHERE id=?', (self.response, self.id))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return self.fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
+        return fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/update_date.py` & `popoll_backend-0.0.60/popoll_backend/query/update_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model.db.date import Date
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchlast
 
 
 class UpdateDate(PollQuery):
     
     id: int
     title: str
     date: datetime.date
@@ -22,8 +22,8 @@
         self.time = time
         self.end_time = end_time
         
     def process(self, cursor: sqlite3.Cursor) -> None:
         cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.id))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
-        return self.fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
+        return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.59/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.60/popoll_backend/query/update_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/popoll_backend/query/update_user.py` & `popoll_backend-0.0.60/popoll_backend/query/update_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import flask
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
-from popoll_backend.query import PollQuery
+from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class UpdateUser(PollQuery):
     
     id: int
     name: str
     main_instrument: int
@@ -29,16 +29,16 @@
         cursor.execute('UPDATE users SET name=? WHERE id=?', (self.name, self.id))
         cursor.execute('DELETE FROM user_instruments WHERE user_id=?', (self.id,))
         rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
         cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         return UserWithInstruments(
-            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
-            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
-            user_instruments=self.fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
+            user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
+            user_instruments=fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
         )
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
                 flask.abort(409, f'User with name {self.name} already exists, cannot update.')
```

### Comparing `popoll_backend-0.0.59/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.60/popoll_backend.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.59
+Version: 0.0.60
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
+License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: flask_cors
 Requires-Dist: flask-restful
 Requires-Dist: jsonpickle
 Requires-Dist: werkzeug
 
 # popoll backend
```

### Comparing `popoll_backend-0.0.59/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.60/popoll_backend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 popoll_backend/__main__.py
 popoll_backend.egg-info/PKG-INFO
 popoll_backend.egg-info/SOURCES.txt
 popoll_backend.egg-info/dependency_links.txt
 popoll_backend.egg-info/requires.txt
@@ -26,21 +27,20 @@
 popoll_backend/model/payload/user_details.py
 popoll_backend/model/payload/user_with_instruments.py
 popoll_backend/model/payload/users.py
 popoll_backend/model/payload/users_payload_details.py
 popoll_backend/query/__init__.py
 popoll_backend/query/create_answer.py
 popoll_backend/query/create_date.py
-popoll_backend/query/create_instrument.py
 popoll_backend/query/create_poll.py
 popoll_backend/query/create_session.py
 popoll_backend/query/create_user.py
 popoll_backend/query/delete_answer.py
 popoll_backend/query/delete_date.py
-popoll_backend/query/delete_instrument.py
+popoll_backend/query/delete_old_dates.py
 popoll_backend/query/delete_user.py
 popoll_backend/query/get_all_instruments.py
 popoll_backend/query/get_all_sessions.py
 popoll_backend/query/get_answer.py
 popoll_backend/query/get_date.py
 popoll_backend/query/get_date_details.py
 popoll_backend/query/get_dates.py
@@ -72,8 +72,9 @@
 tests/test_17_delete_date.py
 tests/test_18_create_answer.py
 tests/test_19_update_answer.py
 tests/test_20_delete_answer.py
 tests/test_21_get_answer.py
 tests/test_22_get_search_answer.py
 tests/test_23_get_create_session.py
-tests/test_24_get_all_session.py
+tests/test_24_get_all_session.py
+tests/test_25_delete_old_dates.py
```

### Comparing `popoll_backend-0.0.59/tests/test_01_get_poll.py` & `popoll_backend-0.0.60/tests/test_01_get_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_02_create_poll.py` & `popoll_backend-0.0.60/tests/test_02_create_poll.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 import os
 from tests import DB_NAME, IntegrationTest
 
 class TestCreatePoll(IntegrationTest):
     
-    DB_NAME_2 = 'DB2'
+    DB_NAME_2 = 'test_integration_2'
     
     def test_db_creation(self):
         _json = self.get_instruments(False)
         
         self.assertEqual(self.instru1_id, _json['instruments'][0]['id'])
         self.assertEqual(self.INSTRU1, _json['instruments'][0]['name'])
         self.assertEqual(self.instru2_id, _json['instruments'][1]['id'])
```

### Comparing `popoll_backend-0.0.59/tests/test_04_get_instruments.py` & `popoll_backend-0.0.60/tests/test_04_get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_08_get_users.py` & `popoll_backend-0.0.60/tests/test_08_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_09_create_user.py` & `popoll_backend-0.0.60/tests/test_09_create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_10_get_user.py` & `popoll_backend-0.0.60/tests/test_22_get_search_answer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from tests import IntegrationTest
 
-class TestGetUser(IntegrationTest):
+class TestGetSearchAnswer(IntegrationTest):
 
     def setUp(self):
         super().setUp()
-        self.user1_id = self.create_user('user1', self.instru2_id, [self.instru3_id, self.instru1_id])['user']['id']
-        
-    def test_get_user(self):
-        _json = self.get_user(self.user1_id, False)
-        self.assertUserWithInstruments(_json, self.user1_id, 'user1', self.instru2_id, [self.instru1_id, self.instru3_id])
-
-    def test_get_user_details(self):
+        self.user1_id = self.create_user('user1', self.instru2_id, [self.instru1_id])['user']['id']
         self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
-        self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)['id']
-        _json = self.get_user(self.user1_id, True)
-        self.assertUser(_json['user'], self.user1_id, 'user1')
-        self.assertEqual(1, len(_json['dates']))
-        self.assertDate(_json['dates'][0]['date'], self.date1_id, '2025-03-10', '15:00:00', '18:00:00', 'firstDate')
-        self.assertAnswer(_json['dates'][0]['answer'], self.answer1_id, self.user1_id, self.date1_id, True)
+        self.answer1_id = self.create_answer(self.user1_id, self.date1_id)['id']
+        
+    def test_get_search_answer_userId_dateId(self):
+        _json = self.get_search_answer(self.user1_id, self.date1_id)
+        self.assertAnswer(_json, self.answer1_id, self.user1_id, self.date1_id, True)
+        
+    def test_get_search_answer_userId_dateId_notFound(self):
+        _rs = self.get_search_answer(99, self.date1_id, fail=True)
+        self.assertEqual(404, _rs.status_code)
```

### Comparing `popoll_backend-0.0.59/tests/test_11_update_user.py` & `popoll_backend-0.0.60/tests/test_11_update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_12_delete_user.py` & `popoll_backend-0.0.60/tests/test_12_delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_13_get_dates.py` & `popoll_backend-0.0.60/tests/test_13_get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_14_create_date.py` & `popoll_backend-0.0.60/tests/test_14_create_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_15_get_date.py` & `popoll_backend-0.0.60/tests/test_15_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_16_update_date.py` & `popoll_backend-0.0.60/tests/test_16_update_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_17_delete_date.py` & `popoll_backend-0.0.60/tests/test_17_delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_18_create_answer.py` & `popoll_backend-0.0.60/tests/test_18_create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_19_update_answer.py` & `popoll_backend-0.0.60/tests/test_19_update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_20_delete_answer.py` & `popoll_backend-0.0.60/tests/test_20_delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_21_get_answer.py` & `popoll_backend-0.0.60/tests/test_21_get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.59/tests/test_22_get_search_answer.py` & `popoll_backend-0.0.60/tests/test_23_get_create_session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from tests import IntegrationTest
 
-class TestGetSearchAnswer(IntegrationTest):
+class TestGetSession(IntegrationTest):
+    
+    SESSION = 'XXXXX'
 
     def setUp(self):
         super().setUp()
-        self.user1_id = self.create_user('user1', self.instru2_id, [self.instru1_id])['user']['id']
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
-        self.answer1_id = self.create_answer(self.user1_id, self.date1_id)['id']
         
-    def test_get_search_answer_userId_dateId(self):
-        _json = self.get_search_answer(self.user1_id, self.date1_id)
-        self.assertAnswer(_json, self.answer1_id, self.user1_id, self.date1_id, True)
+    def test_create_session_noUser(self):
+        _rs = self.create_session(self.SESSION, 1, fail=True)
+        self.assertEqual(400, _rs.status_code)
         
-    def test_get_search_answer_userId_dateId_notFound(self):
-        _rs = self.get_search_answer(99, self.date1_id, fail=True)
-        self.assertEqual(404, _rs.status_code)
+    def test_create_session(self):
+        self.user1_id = self.create_user('user1', self.instru1_id, [])['user']['id']
+        _json = self.create_session(self.SESSION, self.user1_id)
+        self.assertSession(_json, self.SESSION, self.user1_id)
+
```

### Comparing `popoll_backend-0.0.59/tests/test_23_get_create_session.py` & `popoll_backend-0.0.60/tests/test_24_get_all_session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-from tests import IntegrationTest
+from tests import DB_NAME, IntegrationTest
 
 class TestGetSession(IntegrationTest):
     
+    DB_2 = 'test_integration_2'
+    DB_3 = 'test_integration_3'
+    
     SESSION = 'XXXXX'
 
     def setUp(self):
         super().setUp()
+        self.user1_id: int = self.create_user('user1', self.instru1_id, [])['user']['id']
+        self.create_session(self.SESSION, self.user1_id)
+        
+        self.create_poll(self.DB_2, self.DB_2, '#ff8b01')
+        self.create_user('user1', self.instru1_id, [], db=self.DB_2)
+        self.create_session(self.SESSION, self.user1_id, db=self.DB_2)
         
-    def test_create_session_noUser(self):
-        _rs = self.create_session(self.SESSION, 1, fail=True)
-        self.assertEqual(400, _rs.status_code)
+        self.create_poll(self.DB_3, self.DB_3, '#ff8b02')
         
-    def test_create_session(self):
-        self.user1_id = self.create_user('user1', self.instru1_id, [])['user']['id']
-        _json = self.create_session(self.SESSION, self.user1_id)
-        self.assertSession(_json, self.SESSION, self.user1_id)
-        
+    def test_get_all_session(self):
+        _json = self.get_all_session(self.SESSION)
+        self.assertEqual(2, len(_json['polls']))
+        self.assertPoll(_json['polls'][0], DB_NAME, 'TESTTEST')
+        self.assertPoll(_json['polls'][1], self.DB_2, self.DB_2)
+
+    def tearDown(self):
+        self.tearDown_db(self.DB_2)
+        self.tearDown_db(self.DB_3)
```

