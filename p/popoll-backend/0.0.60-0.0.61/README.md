# Comparing `tmp/popoll_backend-0.0.60.tar.gz` & `tmp/popoll_backend-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.60.tar", last modified: Wed May 29 12:57:39 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.61.tar", last modified: Wed May 29 15:30:11 2024, max compression
```

## Comparing `popoll_backend-0.0.60.tar` & `popoll_backend-0.0.61.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/LICENSE
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.726440 popoll_backend-0.0.60/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     8336 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.727440 popoll_backend-0.0.60/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.729440 popoll_backend-0.0.60/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.732440 popoll_backend-0.0.60/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/dates.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/empty.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/polls.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/users.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.738440 popoll_backend-0.0.60/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_old_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_all_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_all_sessions.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_date_details.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_user_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_user_with_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1948 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2798 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-29 12:57:39.000000 popoll_backend-0.0.60/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-29 12:57:34.000000 popoll_backend-0.0.60/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 12:57:39.743440 popoll_backend-0.0.60/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:57:39.742440 popoll_backend-0.0.60/tests/
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_01_get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_02_create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_03_update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_04_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_08_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_09_create_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_10_get_user.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_11_update_user.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_12_delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_13_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_14_create_date.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_15_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_16_update_date.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_17_delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_18_create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_19_update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_20_delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_21_get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_22_get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_23_get_create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_24_get_all_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-29 12:57:20.000000 popoll_backend-0.0.60/tests/test_25_delete_old_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.353300 popoll_backend-0.0.61/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 15:30:11.353300 popoll_backend-0.0.61/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.336300 popoll_backend-0.0.61/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     8488 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.337300 popoll_backend-0.0.61/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.339300 popoll_backend-0.0.61/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.341300 popoll_backend-0.0.61/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/polls.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.348300 popoll_backend-0.0.61/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     3633 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2402 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1874 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/delete_old_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_all_sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.353300 popoll_backend-0.0.61/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-29 15:30:11.000000 popoll_backend-0.0.61/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2798 2024-05-29 15:30:11.000000 popoll_backend-0.0.61/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 15:30:11.000000 popoll_backend-0.0.61/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-29 15:30:11.000000 popoll_backend-0.0.61/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-29 15:30:11.000000 popoll_backend-0.0.61/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-29 15:30:05.000000 popoll_backend-0.0.61/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 15:30:11.353300 popoll_backend-0.0.61/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 15:30:11.352300 popoll_backend-0.0.61/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_23_get_create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_24_get_all_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-29 15:29:50.000000 popoll_backend-0.0.61/tests/test_25_delete_old_dates.py
```

### Comparing `popoll_backend-0.0.60/PKG-INFO` & `popoll_backend-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.60
+Version: 0.0.61
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.60/popoll_backend/__main__.py` & `popoll_backend-0.0.61/popoll_backend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     def post(self, poll: str) -> str: return CreateUser(poll, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
 
 
 
 class PollUserEndpoint(Resource):
     def get(self, poll: str, id:int) -> str: 
         if queryParam(flask.request, 'details'):
-            return GetUserDetails(poll, id, queryParam(flask.request, 'viewOldDates')).run().toJSON()
+            return GetUserDetails(poll, id).run().toJSON()
         else:
             return GetUserWithInstruments(poll, id).run().toJSON()
     
     @history
     def put(self, poll: str, id: int) -> str: return UpdateUser(poll, id, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
     
     @history
@@ -128,27 +128,42 @@
 
 
 
 class PollDatesEndpoint(Resource):
     def get(self, poll: str) -> str: return GetDates(poll).run().toJSON()
     
     @history
-    def post(self, poll: str) -> str: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run().toJSON()
+    def post(self, poll: str) -> str: return CreateDate(
+        poll, 
+        body(flask.request, 'title'), 
+        body(flask.request, 'date'), 
+        body(flask.request, 'time', mandatory=False), 
+        body(flask.request, 'end_time', mandatory=False),
+        body(flask.request, 'is_frozen'), 
+    ).run().toJSON()
 
 
 
 class PollDateEndpoint(Resource):
     def get(self, poll: str, id:int) -> str:
         if queryParam(flask.request, 'details'):
             return GetDateDetails(poll, id).run().toJSON()
         else:
             return GetDate(poll, id).run().toJSON()
     
     @history
-    def put(self, poll: str, id: int) -> str: return UpdateDate(poll, id, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run().toJSON()
+    def put(self, poll: str, id: int) -> str: return UpdateDate(
+        poll, 
+        id, 
+        body(flask.request, 'title'), 
+        body(flask.request, 'date'), 
+        body(flask.request, 'time', mandatory=False), 
+        body(flask.request, 'end_time', mandatory=False),
+        body(flask.request, 'is_frozen')
+    ).run().toJSON()
     
     @history
     def delete(self, poll: str, id: int) -> str: return DeleteDate(poll, id).run().toJSON()
```

### Comparing `popoll_backend-0.0.60/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.61/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/db/date.py` & `popoll_backend-0.0.61/popoll_backend/model/db/date.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,23 @@
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.title: str = data[1]
         self.date: datetime.date = datetime.date.fromisoformat(data[2])
         self.time: Optional[datetime.time] = datetime.time.fromisoformat(data[3]) if data[3] else None
         self.end_time: Optional[datetime.time] = datetime.time.fromisoformat(data[4]) if data[4] else None
+        self.is_frozen: bool = data[5]
+        self.is_old: bool = self.isOlder()
         
     @classmethod
     def create_table(cls):
         return """ CREATE TABLE IF NOT EXISTS dates (
             id integer PRIMARY KEY AUTOINCREMENT,
             title text NOT NULL,
             date text NOT NULL,
             time text,
-            end_time text
+            end_time text,
+            is_frozen boolean NOT NULL
         ); """
         
     def isOlder(self, compare: datetime.date=datetime.date.today()):
         return self.date < compare
```

### Comparing `popoll_backend-0.0.60/popoll_backend/model/db/session.py` & `popoll_backend-0.0.61/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.61/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/payload/date_details.py` & `popoll_backend-0.0.61/popoll_backend/model/payload/date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.61/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/payload/polls.py` & `popoll_backend-0.0.61/popoll_backend/model/payload/polls.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/payload/user_details.py` & `popoll_backend-0.0.61/popoll_backend/model/payload/user_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/model/payload/user_with_instruments.py` & `popoll_backend-0.0.61/popoll_backend/model/payload/user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/__init__.py` & `popoll_backend-0.0.61/popoll_backend/query/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,29 @@
         return [ttype(row) for row in cursor.fetchall()]
 
 def fetchlast(cursor: sqlite3.Cursor, ttype: type) -> type:
         res = fetchall(cursor, ttype)
         if len(res) > 0:
             return res[-1]
         flask.abort(404, 'Not found')
-        
+
+def is_date_frozen(cursor: sqlite3.Cursor, date_id: int) -> bool:
+    res = cursor.execute('SELECT is_frozen FROM dates WHERE id=?', (date_id,)).fetchone()
+    if res != None and len(res) > 0:
+        return res[0]
+    else:
+        flask.abort(400, 'Not found')
+
+def get_date_id(cursor:sqlite3.Cursor, answer_id: int) -> int:
+    res = cursor.execute('SELECT date_id FROM answers WHERE id=?', (answer_id,)).fetchone()
+    if res != None and len(res) > 0:
+        return res[0]
+    else:
+        flask.abort(404, 'Not found')
+
 class Query:
     
     def run(self) -> Payload:
         answers: List[Payload] = []
         for db in sorted(glob.glob('*.db')):
             # We do not want to break in case a db is incorrect
             try:
```

### Comparing `popoll_backend-0.0.60/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.61/popoll_backend/query/create_answer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sqlite3
 
 import flask
 
 from popoll_backend.model.db.answer import Answer
-from popoll_backend.query import PollQuery, fetchlast
+from popoll_backend.query import PollQuery, fetchlast, is_date_frozen
 
 
 class CreateAnswer(PollQuery):
     
     user_id: int
     date_id: int
     
@@ -15,14 +15,16 @@
     
     def __init__(self, poll:str, user_id: int, date_id: int):
         super().__init__(poll)
         self.user_id = user_id
         self.date_id = date_id
     
     def process(self, cursor: sqlite3.Cursor) -> None:
+        if is_date_frozen(cursor, self.date_id):
+            flask.abort(403, 'Date is frozen. Cannot modify')
         self.id = cursor.execute('INSERT INTO answers(user_id, date_id, response) VALUES (?, ?, ?)', (self.user_id, self.date_id, True)).lastrowid
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> Answer:
         return fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
```

### Comparing `popoll_backend-0.0.60/popoll_backend/query/create_date.py` & `popoll_backend-0.0.61/popoll_backend/query/create_date.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 class CreateDate(PollQuery):
     
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
+    is_frozen: bool
     
     id: int
     
-    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
+    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
         super().__init__(poll)
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
+        self.is_frozen = is_frozen
     
     def process(self, cursor: sqlite3.Cursor) -> None:
-        self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time) VALUES (?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time)).lastrowid
+        self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time, is_frozen) VALUES (?, ?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time, self.is_frozen)).lastrowid
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
         return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.60/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.61/popoll_backend/query/create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/create_session.py` & `popoll_backend-0.0.61/popoll_backend/query/create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/create_user.py` & `popoll_backend-0.0.61/popoll_backend/query/create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.61/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.61/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/delete_old_dates.py` & `popoll_backend-0.0.61/popoll_backend/query/delete_old_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.61/popoll_backend/query/delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_all_instruments.py` & `popoll_backend-0.0.61/popoll_backend/query/get_all_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_all_sessions.py` & `popoll_backend-0.0.61/popoll_backend/query/get_all_sessions.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_date.py` & `popoll_backend-0.0.61/popoll_backend/query/get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_date_details.py` & `popoll_backend-0.0.61/popoll_backend/query/get_date_details.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.61/popoll_backend/query/get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_instrument.py` & `popoll_backend-0.0.61/popoll_backend/query/get_instrument.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.61/popoll_backend/query/get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.61/popoll_backend/query/get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_session.py` & `popoll_backend-0.0.61/popoll_backend/query/get_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_user_details.py` & `popoll_backend-0.0.61/popoll_backend/query/get_user_details.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,31 +7,23 @@
 from popoll_backend.model.payload.user_details import UserDetails
 from popoll_backend.query import PollQuery, fetchall, fetchlast
 
 
 class GetUserDetails(PollQuery):
     
     id: int
-    viewOldDates: bool
     
-    def __init__(self, poll: str, id: int, viewOldDates: bool):
+    def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
-        self.viewOldDates = viewOldDates
     
     def process(self, cursor: sqlite3.Cursor) -> None:
         pass
         
     def buildResponse(self, cursor: sqlite3.Cursor) -> UserWithInstruments:
         return UserDetails(
             user=fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
             answers=fetchall(cursor.execute('SELECT * FROM answers WHERE user_id=?', (self.id,)), Answer),
-            dates=self.getDates(cursor)
+            dates=fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date)
         )
-        
-    def getDates(self, cursor: sqlite3.Cursor):
-        dates = fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date)
-        if not self.viewOldDates:
-            dates = [date for date in dates if not date.isOlder()]
-        return dates
```

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_user_with_instruments.py` & `popoll_backend-0.0.61/popoll_backend/query/get_user_with_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/get_users.py` & `popoll_backend-0.0.61/popoll_backend/query/get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/update_date.py` & `popoll_backend-0.0.61/popoll_backend/query/update_date.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 class UpdateDate(PollQuery):
     
     id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
+    is_frozen: bool
     
-    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
+    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time], is_frozen: bool):
         super().__init__(poll)
         self.id = id
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
+        self.is_frozen = is_frozen
         
     def process(self, cursor: sqlite3.Cursor) -> None:
-        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.id))
+        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=?, is_frozen=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.is_frozen, self.id))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
         return fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.60/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.61/popoll_backend/query/update_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend/query/update_user.py` & `popoll_backend-0.0.61/popoll_backend/query/update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.61/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.60
+Version: 0.0.61
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 License: Free
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `popoll_backend-0.0.60/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.61/popoll_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/pyproject.toml` & `popoll_backend-0.0.61/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.60"
+version = "0.0.61"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.60/tests/test_01_get_poll.py` & `popoll_backend-0.0.61/tests/test_01_get_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_02_create_poll.py` & `popoll_backend-0.0.61/tests/test_02_create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_04_get_instruments.py` & `popoll_backend-0.0.61/tests/test_04_get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_08_get_users.py` & `popoll_backend-0.0.61/tests/test_08_get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_09_create_user.py` & `popoll_backend-0.0.61/tests/test_09_create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_10_get_user.py` & `popoll_backend-0.0.61/tests/test_10_get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
     def test_get_user_details(self):
         self.date1_id = self.create_date(date='2028-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
         self.date2_id = self.create_date(date='2022-03-10', time='15:00:00', title='oldDate', end_time='18:00:00')['id']
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)['id']
         _json = self.get_user(self.user1_id, True)
         self.assertUser(_json['user'], self.user1_id, 'user1')
-        self.assertEqual(1, len(_json['dates']))
-        self.assertDate(_json['dates'][0]['date'], self.date1_id, '2028-03-10', '15:00:00', '18:00:00', 'firstDate')
-        self.assertAnswer(_json['dates'][0]['answer'], self.answer1_id, self.user1_id, self.date1_id, True)
+        self.assertEqual(2, len(_json['dates']))
+        self.assertDate(_json['dates'][0]['date'], self.date2_id, '2022-03-10', '15:00:00', '18:00:00', 'oldDate', False, True)
+        self.assertDate(_json['dates'][1]['date'], self.date1_id, '2028-03-10', '15:00:00', '18:00:00', 'firstDate', False, False)
+        self.assertAnswer(_json['dates'][1]['answer'], self.answer1_id, self.user1_id, self.date1_id, True)
         
     def test_get_user_details_with_old_dates(self):
         self.date1_id = self.create_date(date='2028-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
         self.date2_id = self.create_date(date='2022-03-10', time='15:00:00', title='oldDate', end_time='18:00:00')['id']
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)['id']
-        _json = self.get_user(self.user1_id, True, viewOldDates=True)
+        _json = self.get_user(self.user1_id, True)
         self.assertEqual(2, len(_json['dates']))
```

### Comparing `popoll_backend-0.0.60/tests/test_11_update_user.py` & `popoll_backend-0.0.61/tests/test_11_update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_12_delete_user.py` & `popoll_backend-0.0.61/tests/test_12_delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_13_get_dates.py` & `popoll_backend-0.0.61/tests/test_13_get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_14_create_date.py` & `popoll_backend-0.0.61/tests/test_14_create_date.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,13 +2,20 @@
 
 class TestCreateDate(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.date1_id = self.create_date(date='2025-03-12', time='15:00:00', title='firstDate', end_time=None)['id']
         
-    def test_get_dates(self):
+    def test_create_date(self):
         self.assertEqual(1, len(self.get_dates()['dates']))
         self.date2_id = self.create_date(date='2025-03-10', title='secondDate', time=None, end_time=None)['id']
         _json = self.get_dates()
         self.assertEqual(2, len(_json['dates']))
         self.assertDates(_json['dates'], 0, self.date2_id, '2025-03-10', None, None, 'secondDate')
+        
+    def test_create_date_only_end_time(self):
+        self.assertEqual(1, len(self.get_dates()['dates']))
+        self.date2_id = self.create_date(date='2025-03-10', title='secondDate', time=None, end_time='18:00:00')['id']
+        _json = self.get_dates()
+        self.assertEqual(2, len(_json['dates']))
+        self.assertDates(_json['dates'], 0, self.date2_id, '2025-03-10', None, '18:00:00', 'secondDate')
```

### Comparing `popoll_backend-0.0.60/tests/test_15_get_date.py` & `popoll_backend-0.0.61/tests/test_15_get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_17_delete_date.py` & `popoll_backend-0.0.61/tests/test_17_delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_18_create_answer.py` & `popoll_backend-0.0.61/tests/test_18_create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_19_update_answer.py` & `popoll_backend-0.0.61/tests/test_19_update_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_20_delete_answer.py` & `popoll_backend-0.0.61/tests/test_20_delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_21_get_answer.py` & `popoll_backend-0.0.61/tests/test_21_get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_22_get_search_answer.py` & `popoll_backend-0.0.61/tests/test_22_get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_23_get_create_session.py` & `popoll_backend-0.0.61/tests/test_23_get_create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_24_get_all_session.py` & `popoll_backend-0.0.61/tests/test_24_get_all_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.60/tests/test_25_delete_old_dates.py` & `popoll_backend-0.0.61/tests/test_25_delete_old_dates.py`

 * *Files identical despite different names*

