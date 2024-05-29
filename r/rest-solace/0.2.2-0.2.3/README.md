# Comparing `tmp/rest_solace-0.2.2.tar.gz` & `tmp/rest_solace-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.2.2.tar", last modified: Wed May 22 07:16:05 2024, max compression
+gzip compressed data, was "rest_solace-0.2.3.tar", last modified: Wed May 29 19:23:33 2024, max compression
```

## Comparing `rest_solace-0.2.2.tar` & `rest_solace-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.853867 rest_solace-0.2.2/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.2/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.2/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1694 2024-05-19 20:16:27.000000 rest_solace-0.2.2/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)    12939 2024-05-22 07:16:05.853867 rest_solace-0.2.2/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)    12002 2024-05-22 07:14:30.000000 rest_solace-0.2.2/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.837867 rest_solace-0.2.2/docs/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      581 2024-05-22 06:25:58.000000 rest_solace-0.2.2/docs/development_refrences.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2301 2024-05-22 06:14:30.000000 rest_solace-0.2.2/docs/getting_started_with_solace.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.2/docs/index.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.2.2/docs/semp_v2_endpoint_support.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2318 2024-05-22 07:14:43.000000 rest_solace-0.2.2/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-22 07:16:05.853867 rest_solace-0.2.2/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.833867 rest_solace-0.2.2/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.841867 rest_solace-0.2.2/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.2/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.849867 rest_solace-0.2.2/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.2/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.2/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.2/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-19 19:45:08.000000 rest_solace-0.2.2/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.2/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    34588 2024-05-19 19:35:16.000000 rest_solace-0.2.2/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.853867 rest_solace-0.2.2/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)    12939 2024-05-22 07:16:05.000000 rest_solace-0.2.2/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1413 2024-05-22 07:16:05.000000 rest_solace-0.2.2/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-22 07:16:05.000000 rest_solace-0.2.2/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-22 07:16:05.000000 rest_solace-0.2.2/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-22 07:16:05.000000 rest_solace-0.2.2/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.853867 rest_solace-0.2.2/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-22 07:16:05.853867 rest_solace-0.2.2/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.2/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.2/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.2/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.2/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.2/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6499 2024-05-19 19:40:09.000000 rest_solace-0.2.2/tests/publisher_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.2/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.3/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.3/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1837 2024-05-29 19:20:47.000000 rest_solace-0.2.3/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-05-29 19:23:33.905680 rest_solace-0.2.3/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    12568 2024-05-29 19:22:53.000000 rest_solace-0.2.3/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.893680 rest_solace-0.2.3/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      581 2024-05-22 06:25:58.000000 rest_solace-0.2.3/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     3067 2024-05-29 16:57:51.000000 rest_solace-0.2.3/docs/getting_started_with_solace.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.3/docs/index.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    23870 2024-05-29 19:15:20.000000 rest_solace-0.2.3/docs/messaging_publisher.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4053 2024-05-29 18:08:44.000000 rest_solace-0.2.3/docs/semp_v2_endpoint_support.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2372 2024-05-29 19:20:12.000000 rest_solace-0.2.3/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-29 19:23:33.905680 rest_solace-0.2.3/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.889680 rest_solace-0.2.3/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.893680 rest_solace-0.2.3/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.3/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.901680 rest_solace-0.2.3/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.3/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.3/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.3/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-29 16:33:53.000000 rest_solace-0.2.3/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.3/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    36989 2024-05-29 18:54:46.000000 rest_solace-0.2.3/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    13505 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1463 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-29 19:23:33.000000 rest_solace-0.2.3/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-29 19:23:33.905680 rest_solace-0.2.3/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.3/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.3/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.3/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.3/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.3/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7776 2024-05-26 20:05:55.000000 rest_solace-0.2.3/tests/publisher_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      422 2024-05-26 20:03:38.000000 rest_solace-0.2.3/tests/test_data.json
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.3/tests/util.py
```

### Comparing `rest_solace-0.2.2/LICENSE.txt` & `rest_solace-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/NOTICE.txt` & `rest_solace-0.2.3/NOTICE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -33,7 +33,10 @@
 
 This software uses "asyncio" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
 This software uses "logging" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
+This software uses "warnings" library by The Python Software Foundation.
+It is licensed under "The Python Software Foundation License (PSFL)"
+
```

### Comparing `rest_solace-0.2.2/PKG-INFO` & `rest_solace-0.2.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-Metadata-Version: 2.1
-Name: rest-solace
-Version: 0.2.2
-Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
-Author-email: Skyler Guha <skylerguha@gmail.com>
-Maintainer-email: Skyler Guha <skylerguha@gmail.com>
-License: apache 2.0
-Project-URL: pypi, https://pypi.org/project/rest-solace/
-Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
-Project-URL: repository, https://github.com/skyler-guha/rest-solace
-Keywords: solace,rest,REST API,rest-solace,rest_solace,rest solace,python,pythonic
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-License-File: NOTICE.txt
-Requires-Dist: requests>=2.30.0
-Requires-Dist: aiohttp>=3.9.5
-
-rest-solace
+rest-solace 
 ===============
 
+.. image:: https://img.shields.io/badge/dynamic/xml?url=https%3A%2F%2Fpypistats.org%2Fpackages%2Frest-solace&query=substring-after(%2Fhtml%2Fbody%2Fdiv%2Fsection%2Fp%20%2C%20'Downloads%20last%20month%3A')&label=PyPI%20downloads%20last%20month%3A&color=%2332CD32
+   :alt: Dynamic XML Badge
+
+
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
 Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
 |
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_. 
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 -----------------------------
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
@@ -297,13 +279,19 @@
                                  queueBindingName= 'my_queue',
                                  postRequestTarget= '/')
 
 
     #Turning your RDP off and on again (Useful if solace has trouble connecting to your consumer)
     manager.restart_rest_delivery_point(msgVpnName= NEW_VPN_NAME, restDeliveryPointName= 'myRDP')
 
-    
+..
+   _url to get download data: https://pypistats.org/packages/rest-solace
+
+..
+    _xpath string to get download data: substring-after(/html/body/div/section/p , 'Downloads last month:')
 
+..
+    _Create badge using XML/HTML data at: https://shields.io/badges/dynamic-xml-badge 
 
     
 ..
    _Note: Make sure to indent using spaces in the code blocks!
```

### Comparing `rest_solace-0.2.2/README.rst` & `rest_solace-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,49 @@
-rest-solace
+Metadata-Version: 2.1
+Name: rest-solace
+Version: 0.2.3
+Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
+Author-email: Skyler Guha <skylerguha@gmail.com>
+Maintainer-email: Skyler Guha <skylerguha@gmail.com>
+License: apache 2.0
+Project-URL: pypi, https://pypi.org/project/rest-solace/
+Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
+Project-URL: repository, https://github.com/skyler-guha/rest-solace
+Keywords: solace,rest,REST API,rest-solace,rest_solace,rest solace,python,pythonic
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+License-File: NOTICE.txt
+Requires-Dist: requests>=2.30.0
+Requires-Dist: aiohttp>=3.9.5
+
+rest-solace 
 ===============
 
+.. image:: https://img.shields.io/badge/dynamic/xml?url=https%3A%2F%2Fpypistats.org%2Fpackages%2Frest-solace&query=substring-after(%2Fhtml%2Fbody%2Fdiv%2Fsection%2Fp%20%2C%20'Downloads%20last%20month%3A')&label=PyPI%20downloads%20last%20month%3A&color=%2332CD32
+   :alt: Dynamic XML Badge
+
+
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
 Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
 |
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_. 
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 -----------------------------
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
@@ -275,13 +301,19 @@
                                  queueBindingName= 'my_queue',
                                  postRequestTarget= '/')
 
 
     #Turning your RDP off and on again (Useful if solace has trouble connecting to your consumer)
     manager.restart_rest_delivery_point(msgVpnName= NEW_VPN_NAME, restDeliveryPointName= 'myRDP')
 
-    
+..
+   _url to get download data: https://pypistats.org/packages/rest-solace
+
+..
+    _xpath string to get download data: substring-after(/html/body/div/section/p , 'Downloads last month:')
 
+..
+    _Create badge using XML/HTML data at: https://shields.io/badges/dynamic-xml-badge 
 
     
 ..
    _Note: Make sure to indent using spaces in the code blocks!
```

### Comparing `rest_solace-0.2.2/docs/development_refrences.rst` & `rest_solace-0.2.3/docs/development_refrences.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/docs/getting_started_with_solace.rst` & `rest_solace-0.2.3/docs/getting_started_with_solace.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,65 @@
 This is a short into to get you started if you are new to solace.
 Solace is a message broking software.
 
+Message VPNs
+=============
+
 A solace message broker can have multiple Message VPNs, 
 which are segregated spaces for message communication to take place.
 Each such VPN will have its own unique listening PORT for receiving messages, 
 and you can define a separate PORT for each message sending protocol (like REST, MQTT, AMQP, etc).
 When sending a message, you have to specify the message VPN, 
 and you will have to do that with its listening PORT number (incase of this library, the REST listening port).
 
+
+Endpoints
+===========
+
 A VPN can contain many endpoints called "queues" which are used to 
 receive, store, and pass along incoming messages 
 (there is another kind of endpoint called "topic_endpoint", but you can ignore it as it is just a vestigial feature.).
 
 There is also the concept of "topic" strings (not to be confused with topic-endpoints).
 Each queue can subscribe to a topic string. And instead of punishing a message directly to a queue,
 you could send the broker a message for a topic string, and every queue with the matching 
 topic string will get the message. Topic strings also have other features like wildcards, and 
 you can read all about it `here <https://docs.solace.com/Get-Started/what-are-topics.htm>`_.
 
+Publisher, Consumer, and Subscriber
+======================================
+
 The one sending the message is called the "Publisher". 
 
-When it comes to receving messages, there are 2 terms that are often use interchangebly, 
+When it comes to receiving messages, there are 2 terms that are often use interchangeably, 
 but for this library will be defined as 2 distinct concepts. They are:
 
 * Subscriber- This is when someone subscribes to a queue by creating a session with the broker. 
   This is the case with the Solace Java Message Service (JMS) API. 
   More info can be found about it `here <https://tutorials.solace.dev/jms/publish-subscribe/#Connecting-to-Solace-Messaging>`_.
 * Consumer- This is when you start a server on a certain host and port, 
   then add that server (its host address and port) to the list of consumers for a given queue.
-  When a message comes to the queue, the broker automaticly sends the message to the relevent consumers, 
-  without a need for there to be a constent session between the two. 
+  When a message comes to the queue, the broker automatically sends the message to the relevant consumers, 
+  without a need for there to be a consent session between the two. 
   Rest consumers work in this way. When you make a consumer using this library, you are creating a server which is
   going to listen for incoming messages.
+
+
+Direct VS Persistent message delivery modes:
+============================================
+
+Direct Mode:
+--------------
+This uses TCP protocol and does not confirm if the message was spooled (stored) into a queue or received by a consumer.
+It is good for cases where always getting the data is not important.
+
+Persistent Mode:
+-----------------
+This also uses TCP protocol but also does additional set of acknowledgments. It can tell you if a message was spooled into a queue,
+or received by the consumer.
+
+You may learn more about this topic here:
+https://solace.com/blog/delivery-modes-direct-messaging-vs-persistent-messaging/
+
+
+
+
```

### Comparing `rest_solace-0.2.2/pyproject.toml` & `rest_solace-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,17 @@
     #"queue",           #part of the standard library
     #"threading",       #part of the standard library
     #"time"             #part of the standard library
     #"json",            #part of the standard library
     #"urllib"           #part of the standard library
     #"asyncio"          #part of the standard library
     #"logging"          #part of the standard library
+    #"warnings"         #part of the standard library
 ]
-version = "0.2.2"
+version = "0.2.3"
 
 [project.urls]
 pypi = "https://pypi.org/project/rest-solace/"
 documentation = "https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst"
 repository = "https://github.com/skyler-guha/rest-solace"
 
 #Doing an editable install: pip install --editable .
```

### Comparing `rest_solace-0.2.2/src/rest_solace/__init__.py` & `rest_solace-0.2.3/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.2.3/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/consumer.py` & `rest_solace-0.2.3/src/rest_solace/consumer.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/http_client.py` & `rest_solace-0.2.3/src/rest_solace/http_client.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/manager.py` & `rest_solace-0.2.3/src/rest_solace/manager.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/src/rest_solace/publisher.py` & `rest_solace-0.2.3/src/rest_solace/publisher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import json
+import asyncio
+import warnings
 from .http_client import HttpClient
 from requests.exceptions import ReadTimeout
 from aiohttp.client_exceptions import ServerTimeoutError
 
 class MessagingPublisher():
     
     def __init__(self, user_name:str, password:str,
@@ -10,42 +13,46 @@
 
         Args:
             username (str): Username of user with admin level access to the broker.
             password (str): Password for the username provided.
             host (str): Broker address (IPv4)
             rest_vpn_port (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
                                 We use this port so specify which VPN we wish to send our messages to.
+            verify_ssl (bool): Enable SSL (Does not work as of yet)
         """
 
+        #Default client params
         self.http_client = HttpClient(host= host,
                                       port= rest_vpn_port,
                                       user_name= user_name,
                                       password= password,
                                       verify_ssl= verify_ssl)
         
     def update_parameters(self, user_name:str, password:str,
-                          host:str, rest_vpn_port:str, verify_ssl=False):
-        """Update parameters used to connect with the broker.
+                          host:str, rest_vpn_port:str, verify_ssl=False)->None:
+        """Update the default parameters used to connect with the broker.
 
         Args:
             username (str): Username of user with admin level access to the broker.
             password (str): Password for the username provided.
             host (str): Broker address (IPv4)
             rest_vpn_port (str): The port assigned on your vpn of interest where you wish to send messages through REST messaging.
-                                We use this port so specify which VPN we wish to send our messages to.        """
+                                We use this port so specify which VPN we wish to send our messages to.        
+            verify_ssl (bool): Enable SSL (Does not work as of yet)
+        """
         
         self.http_client = HttpClient(host= host,
                                       port= rest_vpn_port,
                                       user_name= user_name,
                                       password= password,
                                       verify_ssl= verify_ssl)
 
     def direct_message_to_queue(self, queue_name:str, message:str, 
                                 reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                                timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                timeout:int|None= 120, throw_exception:bool= False)->dict:
         
         """Publish a message to a queue endpoint in direct mode.
         'direct' mode is for sending messages without expecting a reply.
 
         Args:
             queue_name (str): Name of the queue endpoint you wish to publish to.
             message (str): The message you wish to send.
@@ -58,14 +65,15 @@
                                                     chose which topic string the consumer reply will go to if provided.
                                                     The value must be a topic string (NOT the name of a topic endpoint).
                                                     Only works in 'direct' delivery mode.
                                                     Defaults to None.
             timeout (str | None, optional): http/https request timeout set on the client side. Defaults to 120.
             throw_exception (bool, optional): Throw exception incase request error code indicates an error or timeout has been reached.
                                               Defaults to False.
+            client_params (dict, optional): Use custom http client params instead of using the ones 
 
         Raises:
             ValueError: Can only select either 'reply_to_queue' or 'reply_for_topic', not both.
             HTTPError: Return code for request indicates an error
 
         Returns:
             dict: Dictionary containing request information and {'timeout':False}.
@@ -99,15 +107,15 @@
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
        
     def direct_message_for_topic(self, topic_string:str, message:str, 
                         reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                        timeout:str|None= 120, throw_exception:bool= False)->dict:
+                        timeout:int|None= 120, throw_exception:bool= False)->dict:
 
         """Publish a message for a specific topic. 
         'direct' mode is for sending messages without expecting a reply.
         A topic is a string that allows for attracting specific messages to specific endpoints.
         Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
         Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
 
@@ -173,15 +181,15 @@
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
        
     def persistent_message_to_queue(self, queue_name:str, message:str, request_reply:bool= False,
                                     time_to_live:int|None= None, DMQ_eligible:bool= False,
-                                    timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                    timeout:int|None= 120, throw_exception:bool= False)->dict:
         
         """Publish a message to a queue endpoint in persistent mode.
         'persistent' mode is for sending a message and getting a confirmation from the broker if the message was spooled into a queue,
         or for sending a message and getting reply from a consumer to confirm for sure the message was not just spooled but also received.
 
         Args:
             queue_name (str): Name of the queue endpoint you wish to publish to.
@@ -237,15 +245,15 @@
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
 
     def persistent_message_for_topic(self, topic_string:str, message:str, request_reply:bool= False,
                                     time_to_live:int|None= None, DMQ_eligible:bool= False,
-                                    timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                    timeout:int|None= 120, throw_exception:bool= False)->dict:
 
         """Publish a message for a specific topic. 
         'persistent' mode is for sending a message and getting a confirmation from the broker if the message was spooled into a queue,
         or for sending a message and getting reply from a consumer to confirm for sure the message was not just spooled but also received.
         A topic is a string that allows for attracting specific messages to specific endpoints.
         Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
         Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
@@ -310,21 +318,19 @@
         
         if res != None:
             if throw_exception:
                 res.raise_for_status()
             return {"status_code":res.status_code, "headers":res.headers, 
                     "content":res.content, 'timeout':False}
 
-    #Async functions of the above 4 functions. (you will have to remake each one and with aiohttp)
-
     async def async_direct_message_to_queue(self, queue_name:str, message:str, 
                                             reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                                            timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                            timeout:int|None= 120, throw_exception:bool= False)->dict:
         
-        """Publish a message to a queue endpoint in direct mode.
+        """Publish a message to a queue endpoint in direct mode asynchronously.
         'direct' mode is for sending messages without expecting a reply.
 
         Args:
             queue_name (str): Name of the queue endpoint you wish to publish to.
             message (str): The message you wish to send.
             reply_to_queue (str | None, optional): After the message is received by the consumer, 
                                                    chose which queue the consumer reply will go to if provided.
@@ -378,17 +384,17 @@
             
             content = await res.content.read()
             return {"status_code":res.status, "headers":dict(res.headers), 
                     "content":content.decode("utf8"), 'timeout':False}
        
     async def async_direct_message_for_topic(self, topic_string:str, message:str, 
                                              reply_to_queue:str|None= None, reply_for_topic:str|None= None, 
-                                             timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                             timeout:int|None= 120, throw_exception:bool= False)->dict:
 
-        """Publish a message for a specific topic. 
+        """Publish a message for a specific topic asynchronously.
         'direct' mode is for sending messages without expecting a reply.
         A topic is a string that allows for attracting specific messages to specific endpoints.
         Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
         Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
 
         Note: 
             This is not to be confused with publishing to a topic endpoint.
@@ -454,17 +460,17 @@
 
             content = await res.content.read()
             return {"status_code":res.status, "headers":dict(res.headers), 
                     "content":content.decode("utf8"), 'timeout':False}
        
     async def async_persistent_message_to_queue(self, queue_name:str, message:str, request_reply:bool= False,
                                                 time_to_live:int|None= None, DMQ_eligible:bool= False,
-                                                timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                                timeout:int|None= 120, throw_exception:bool= False)->dict:
         
-        """Publish a message to a queue endpoint in persistent mode.
+        """Publish a message to a queue endpoint in persistent mode asynchronously.
         'persistent' mode is for sending a message and getting a confirmation from the broker if the message was spooled into a queue,
         or for sending a message and getting reply from a consumer to confirm for sure the message was not just spooled but also received.
 
         Args:
             queue_name (str): Name of the queue endpoint you wish to publish to.
             message (str): The message you wish to send.
             request_reply (bool): If false, tells the broker to just conform if the message was spooled into a queue.
@@ -520,17 +526,17 @@
 
             content = await res.content.read()
             return {"status_code":res.status, "headers":dict(res.headers), 
                     "content":content.decode("utf8"), 'timeout':False}
 
     async def async_persistent_message_for_topic(self, topic_string:str, message:str, request_reply:bool= False,
                                                  time_to_live:int|None= None, DMQ_eligible:bool= False,
-                                                 timeout:str|None= 120, throw_exception:bool= False)->dict:
+                                                 timeout:int|None= 120, throw_exception:bool= False)->dict:
 
-        """Publish a message for a specific topic. 
+        """Publish a message for a specific topic asynchronously.
         'persistent' mode is for sending a message and getting a confirmation from the broker if the message was spooled into a queue,
         or for sending a message and getting reply from a consumer to confirm for sure the message was not just spooled but also received.
         A topic is a string that allows for attracting specific messages to specific endpoints.
         Endpoints subscribe to a specific topic string, and messages with matching strings go to those endpoints.
         Learn more at: https://docs.solace.com/Get-Started/what-are-topics.htm   
 
         Note: 
@@ -596,15 +602,79 @@
                 res.raise_for_status()
 
             content = await res.content.read()
             return {"status_code":res.status, "headers":dict(res.headers), 
                     "content":content.decode("utf8"), 'timeout':False}
 
 
+    def send_messages(self, data:list|str, async_mode= True):
+        """Send multiple messages in a batch.
+
+        Args:
+            data (list | str): Either a list of dictionaries containing message data, 
+            or a string containing path to a json file with the data.
+            async_mode (bool, optional): To send the message asynchronously or not. Defaults to True.
+
+        Returns:
+            list: Output values.
+        """
+        
+        warnings.warn('This function is experimental.\
+                      It does no validation nor is designed to properly handel errors. \
+                      Its features can be changed in the future.')
+        
+        if isinstance(data, str):
+
+            with open(file=data, encoding='utf-8') as json_file:
+                data = json.load(json_file)
+
+        if async_mode == True:
+
+            async_functions= {"direct_message_to_queue": self.async_direct_message_to_queue,
+                              "direct_message_for_topic": self.async_direct_message_for_topic,
+                              "persistent_message_to_queue": self.async_persistent_message_to_queue,
+                              "persistent_message_for_topic": self.async_persistent_message_for_topic}
+
+            async def run_functions(data):
+
+                coroutines = list()
 
-    #A single sync function to send many messages based on parameters from list of dictionary (That you could import from a CSV)
-    #Should have flag to turn on and off async
-    #https://www.geeksforgeeks.org/load-csv-data-into-list-and-dictionary-using-python/
+                for message_object in data:
 
+                    func_name = list(message_object)[0]
+
+                    func_params = message_object[func_name]
+
+                    func_obj = async_functions[func_name]
+
+                    coroutines.append( func_obj( **func_params ))
+
+                awaited_results = await asyncio.gather(*coroutines)
+                return awaited_results
+
+            
+            results = asyncio.run(run_functions(data))
+
+            return results                
+
+        elif async_mode == False:
+            
+            sync_functions= {"direct_message_to_queue": self.direct_message_to_queue,
+                             "direct_message_for_topic": self.direct_message_for_topic,
+                             "persistent_message_to_queue": self.persistent_message_to_queue,
+                             "persistent_message_for_topic": self.persistent_message_for_topic}
+            
+            for message_object in data:
+
+                func_name = list(message_object)[0]
+
+                func_params = message_object[func_name]
+
+                func_obj = sync_functions[func_name]
+
+                func_obj( **func_params )
+            
+        else:
+
+            pass
 
-#Add a class to validate inputs for the different functions.
-#this would validate input for all functions. Also makes it so you can validate all the input for the multi message function first.
+
```

### Comparing `rest_solace-0.2.2/src/rest_solace.egg-info/PKG-INFO` & `rest_solace-0.2.3/src/rest_solace.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.2.2
+Version: 0.2.3
 Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
@@ -16,30 +16,34 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: requests>=2.30.0
 Requires-Dist: aiohttp>=3.9.5
 
-rest-solace
+rest-solace 
 ===============
 
+.. image:: https://img.shields.io/badge/dynamic/xml?url=https%3A%2F%2Fpypistats.org%2Fpackages%2Frest-solace&query=substring-after(%2Fhtml%2Fbody%2Fdiv%2Fsection%2Fp%20%2C%20'Downloads%20last%20month%3A')&label=PyPI%20downloads%20last%20month%3A&color=%2332CD32
+   :alt: Dynamic XML Badge
+
+
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
 It is written with the intent to be easy to understand, functional, and pythonic.
 Input and output parameters for almost every function is always one of int, float, str, bool, list, dict and None; 
 making them directly compatible with json data types. 
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
     | This library currently uses SEMPv2 for management. 
 
 |
-| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
+| Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_. 
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 -----------------------------
 Getting started with Solace:
 -----------------------------
 If you are new to solace and confused about the terminology and workflows around it, it is **highly** recommended 
@@ -297,13 +301,19 @@
                                  queueBindingName= 'my_queue',
                                  postRequestTarget= '/')
 
 
     #Turning your RDP off and on again (Useful if solace has trouble connecting to your consumer)
     manager.restart_rest_delivery_point(msgVpnName= NEW_VPN_NAME, restDeliveryPointName= 'myRDP')
 
-    
+..
+   _url to get download data: https://pypistats.org/packages/rest-solace
 
+..
+    _xpath string to get download data: substring-after(/html/body/div/section/p , 'Downloads last month:')
+
+..
+    _Create badge using XML/HTML data at: https://shields.io/badges/dynamic-xml-badge 
 
     
 ..
    _Note: Make sure to indent using spaces in the code blocks!
```

### Comparing `rest_solace-0.2.2/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.2.3/src/rest_solace.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE.txt
 NOTICE.txt
 README.rst
 pyproject.toml
 docs/development_refrences.rst
 docs/getting_started_with_solace.rst
 docs/index.rst
+docs/messaging_publisher.rst
 docs/semp_v2_endpoint_support.rst
 src/rest_solace/__init__.py
 src/rest_solace/consumer.py
 src/rest_solace/exceptions.py
 src/rest_solace/http_client.py
 src/rest_solace/manager.py
 src/rest_solace/publisher.py
@@ -32,9 +33,10 @@
 src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
 src/rest_solace/__pycache__/subscriber.cpython-311.pyc
 tests/consumer_test.py
 tests/empty_test.py
 tests/manager_test.py
 tests/pub_sub_test.py
 tests/publisher_test.py
+tests/test_data.json
 tests/util.py
 tests/__pycache__/manager_unittest.cpython-311.pyc
```

### Comparing `rest_solace-0.2.2/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.2.3/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/tests/consumer_test.py` & `rest_solace-0.2.3/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/tests/empty_test.py` & `rest_solace-0.2.3/tests/empty_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/tests/manager_test.py` & `rest_solace-0.2.3/tests/manager_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/tests/pub_sub_test.py` & `rest_solace-0.2.3/tests/pub_sub_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.2.2/tests/publisher_test.py` & `rest_solace-0.2.3/tests/publisher_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -154,36 +154,63 @@
                                                                timeout=5,
                                                                request_reply= True)
         print("\nResponse:\n",res)
     except Exception as e:
         print(e)
     teardown()
 
+def test_send_messages():
+    print("\nTesting Function: 'send_messages'")
+    #setup()
+
+    manager.create_message_vpn(msgVpnName= NEW_VPN_NAME,
+                           serviceRestIncomingPlainTextListenPort= NEW_VPN_PORT)
+
+    manager.auto_rest_messaging_setup_utility(msgVpnName= NEW_VPN_NAME, queueName= 'queue_rest_consumer', subscriptionTopic='my_topic', 
+                                              restDeliveryPointName='myRDP', restConsumerName='myConsumer', 
+                                              remoteHost= CONSUMER_HOST, remotePort= CONSUMER_PORT)
+
+    try:
+        res = publish.send_messages(data= "test_data.json")
+        print("\nResponse:\n",res)
+    except Exception as e:
+        print(e)
+
+    manager.delete_queue_endpoint(msgVpnName= NEW_VPN_NAME, queueName= 'queue_rest_consumer')
+    manager.delete_rest_delivery_point(msgVpnName= NEW_VPN_NAME, restDeliveryPointName= 'myRDP')
+    manager.delete_message_vpn(msgVpnName= NEW_VPN_NAME)
+    #teardown()
 
 #Running all sync tests
-test_direct_message_to_queue()
-time.sleep(10)
-test_direct_message_for_topic()
-time.sleep(10)
-test_persistent_message_to_queue()
-time.sleep(10)
-test_persistent_message_for_topic()
-time.sleep(10)
-
-#Running all async tests
-asyncio.run(test_async_direct_message_to_queue())
-time.sleep(15)
-asyncio.run(test_async_direct_message_for_topic())
-time.sleep(15)
-asyncio.run(test_async_persistent_message_to_queue())
-time.sleep(15)
-asyncio.run(test_async_persistent_message_for_topic())
+# test_direct_message_to_queue()
+# time.sleep(10)
+# test_direct_message_for_topic()
+# time.sleep(10)
+# test_persistent_message_to_queue()
+# time.sleep(10)
+# test_persistent_message_for_topic()
+# time.sleep(10)
+
+# #Running all async tests
+# asyncio.run(test_async_direct_message_to_queue())
+# time.sleep(15)
+# asyncio.run(test_async_direct_message_for_topic())
+# time.sleep(15)
+# asyncio.run(test_async_persistent_message_to_queue())
+# time.sleep(15)
+# asyncio.run(test_async_persistent_message_for_topic())
+
+test_send_messages()
+
+#co = publish.async_direct_message_to_queue(queue_name= "my_queue", message= "hello world!!")
 
 
+#coroutine_obj=  asyncio.run(publish.async_direct_message_to_queue(queue_name= "my_queue", message= "hello world!!"))
 
+#print(coroutine_obj)
```

### Comparing `rest_solace-0.2.2/tests/util.py` & `rest_solace-0.2.3/tests/util.py`

 * *Files identical despite different names*

