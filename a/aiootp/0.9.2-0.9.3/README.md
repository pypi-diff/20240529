# Comparing `tmp/aiootp-0.9.2.tar.gz` & `tmp/aiootp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiootp-0.9.2.tar", last modified: Thu Jun 11 14:29:36 2020, max compression
+gzip compressed data, was "dist/aiootp-0.9.3.tar", last modified: Sun Jun 14 02:44:58 2020, max compression
```

## Comparing `aiootp-0.9.2.tar` & `aiootp-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/
--rw-r--r--   0 mon       (1000) mon       (1000)    32739 2020-01-29 02:36:20.000000 aiootp-0.9.2/LICENSE
--rw-r--r--   0 mon       (1000) mon       (1000)      260 2020-06-11 14:29:36.000000 aiootp-0.9.2/setup.cfg
--rw-r--r--   0 mon       (1000) mon       (1000)    22064 2020-06-11 14:18:41.000000 aiootp-0.9.2/CHANGES.rst
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/tests/
--rw-r--r--   0 mon       (1000) mon       (1000)      753 2020-05-27 18:25:23.000000 aiootp-0.9.2/tests/test_ciphers.py
--rw-rw-r--   0 mon       (1000) mon       (1000)     5573 2020-05-10 00:25:41.000000 aiootp-0.9.2/tests/test_Comprende.py
--rw-r--r--   0 mon       (1000) mon       (1000)      549 2020-05-09 23:49:30.000000 aiootp-0.9.2/tests/test_generics.py
--rw-rw-r--   0 mon       (1000) mon       (1000)      471 2020-05-09 23:49:54.000000 aiootp-0.9.2/tests/test_aiootp.py
--rw-rw-r--   0 mon       (1000) mon       (1000)     5383 2020-05-11 21:18:35.000000 aiootp-0.9.2/tests/test_Database_AsyncDatabase.py
--rw-r--r--   0 mon       (1000) mon       (1000)     4021 2020-05-29 03:36:28.000000 aiootp-0.9.2/tests/test_high_level_encryption.py
--rw-r--r--   0 mon       (1000) mon       (1000)       92 2020-06-02 04:07:02.000000 aiootp-0.9.2/.gitignore
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/aiootp.egg-info/
--rw-r--r--   0 mon       (1000) mon       (1000)        1 2020-06-11 14:29:35.000000 aiootp-0.9.2/aiootp.egg-info/dependency_links.txt
--rw-r--r--   0 mon       (1000) mon       (1000)    67042 2020-06-11 14:29:35.000000 aiootp-0.9.2/aiootp.egg-info/PKG-INFO
--rw-r--r--   0 mon       (1000) mon       (1000)        7 2020-06-11 14:29:35.000000 aiootp-0.9.2/aiootp.egg-info/top_level.txt
--rw-r--r--   0 mon       (1000) mon       (1000)       70 2020-06-11 14:29:35.000000 aiootp-0.9.2/aiootp.egg-info/requires.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     1100 2020-06-11 14:29:35.000000 aiootp-0.9.2/aiootp.egg-info/SOURCES.txt
--rw-r--r--   0 mon       (1000) mon       (1000)    52675 2020-06-11 14:29:35.000000 aiootp-0.9.2/README.rst
--rw-r--r--   0 mon       (1000) mon       (1000)    67042 2020-06-11 14:29:36.000000 aiootp-0.9.2/PKG-INFO
--rw-r--r--   0 mon       (1000) mon       (1000)      335 2020-06-11 14:28:53.000000 aiootp-0.9.2/sha256_ROOT_CHECKSUM.sig
--rw-r--r--   0 mon       (1000) mon       (1000)       64 2020-06-11 14:29:35.000000 aiootp-0.9.2/sha256_ROOT_CHECKSUM.txt
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/licenses/
--rw-r--r--   0 mon       (1000) mon       (1000)    11435 2020-04-16 20:20:58.000000 aiootp-0.9.2/licenses/uvloop_LICENSE_1.txt
--rw-r--r--   0 mon       (1000) mon       (1000)    11332 2019-10-09 16:52:31.000000 aiootp-0.9.2/licenses/aiofiles_LICENSE.txt
--rw-rw-rw-   0 mon       (1000) mon       (1000)    12769 2019-12-10 03:29:08.000000 aiootp-0.9.2/licenses/cpython_LICENSE.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     1067 2020-04-20 14:26:15.000000 aiootp-0.9.2/licenses/aioitertools_LICENSE.txt
--rw-rw-rw-   0 mon       (1000) mon       (1000)     1075 2019-12-13 12:12:29.000000 aiootp-0.9.2/licenses/asyncio_contextmanager_LICENSE.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     1101 2020-04-16 20:19:41.000000 aiootp-0.9.2/licenses/uvloop_LICENSE_0.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     1326 2020-04-16 20:29:28.000000 aiootp-0.9.2/licenses/pybase64_LICENSE.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     1226 2020-04-16 21:03:39.000000 aiootp-0.9.2/licenses/async_lru_LICENSE.txt
--rw-rw-rw-   0 mon       (1000) mon       (1000)     1096 2019-12-10 05:16:17.000000 aiootp-0.9.2/licenses/pytest_LICENSE.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     4952 2019-12-20 23:38:02.000000 aiootp-0.9.2/licenses/sympy_LICENSE.txt
--rwxrwxrwx   0 mon       (1000) mon       (1000)     4828 2020-06-11 14:27:04.000000 aiootp-0.9.2/setup.py
--rw-r--r--   0 mon       (1000) mon       (1000)      420 2020-06-11 14:29:05.000000 aiootp-0.9.2/sha512_ROOT_CHECKSUM.sig
--rw-r--r--   0 mon       (1000) mon       (1000)      984 2020-06-02 04:06:16.000000 aiootp-0.9.2/MANIFEST.in
--rw-r--r--   0 mon       (1000) mon       (1000)    30607 2020-06-11 14:14:11.000000 aiootp-0.9.2/PREADME.rst
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/aiootp/
--rw-r--r--   0 mon       (1000) mon       (1000)     4646 2020-05-31 05:42:52.000000 aiootp-0.9.2/aiootp/asynchs.py
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/aiootp/tor/
--rw-rw-r--   0 mon       (1000) mon       (1000)      447 2020-04-20 02:48:31.000000 aiootp-0.9.2/aiootp/tor/README_TOR.rst
--rwxrwxrwx   0 mon       (1000) mon       (1000)   152644 2020-06-11 13:16:10.000000 aiootp-0.9.2/aiootp/ciphers.py
--rw-rw-r--   0 mon       (1000) mon       (1000)     9662 2020-06-11 01:32:57.000000 aiootp-0.9.2/aiootp/__ui_coordination.py
--rwxrwxrwx   0 mon       (1000) mon       (1000)    50822 2020-06-11 03:38:09.000000 aiootp-0.9.2/aiootp/randoms.py
--rwxrwxrwx   0 mon       (1000) mon       (1000)    18989 2020-05-31 05:45:20.000000 aiootp-0.9.2/aiootp/debuggers.py
--rw-rw-r--   0 mon       (1000) mon       (1000)     9000 2020-06-10 01:08:57.000000 aiootp-0.9.2/aiootp/commons.py
--rw-rw-r--   0 mon       (1000) mon       (1000)   644679 2020-06-03 10:46:44.000000 aiootp-0.9.2/aiootp/__datasets.py
-drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-11 14:29:36.000000 aiootp-0.9.2/aiootp/databases/
--rw-rw-r--   0 mon       (1000) mon       (1000)     9895 2020-06-09 04:06:10.000000 aiootp-0.9.2/aiootp/databases/README_DATABASES.rst
--rwxrwxrwx   0 mon       (1000) mon       (1000)    23099 2020-06-11 00:25:32.000000 aiootp-0.9.2/aiootp/keygens.py
--rw-r--r--   0 mon       (1000) mon       (1000)     1049 2020-06-11 14:27:09.000000 aiootp-0.9.2/aiootp/__init__.py
--rwxrwxrwx   0 mon       (1000) mon       (1000)   115412 2020-06-09 23:31:49.000000 aiootp-0.9.2/aiootp/generics.py
--rw-rw-r--   0 mon       (1000) mon       (1000)     1829 2020-05-31 05:39:00.000000 aiootp-0.9.2/aiootp/paths.py
--rw-r--r--   0 mon       (1000) mon       (1000)      128 2020-06-11 14:29:35.000000 aiootp-0.9.2/sha512_ROOT_CHECKSUM.txt
--rw-r--r--   0 mon       (1000) mon       (1000)     6636 2020-06-11 14:29:35.000000 aiootp-0.9.2/CHECKSUMS.txt
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/
+-rw-r--r--   0 mon       (1000) mon       (1000)    32739 2020-01-29 02:36:20.000000 aiootp-0.9.3/LICENSE
+-rw-r--r--   0 mon       (1000) mon       (1000)      260 2020-06-14 02:44:58.000000 aiootp-0.9.3/setup.cfg
+-rw-r--r--   0 mon       (1000) mon       (1000)    22808 2020-06-14 02:17:26.000000 aiootp-0.9.3/CHANGES.rst
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/tests/
+-rw-r--r--   0 mon       (1000) mon       (1000)      753 2020-05-27 18:25:23.000000 aiootp-0.9.3/tests/test_ciphers.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)     5573 2020-05-10 00:25:41.000000 aiootp-0.9.3/tests/test_Comprende.py
+-rw-r--r--   0 mon       (1000) mon       (1000)      549 2020-05-09 23:49:30.000000 aiootp-0.9.3/tests/test_generics.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)      471 2020-05-09 23:49:54.000000 aiootp-0.9.3/tests/test_aiootp.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)     5383 2020-05-11 21:18:35.000000 aiootp-0.9.3/tests/test_Database_AsyncDatabase.py
+-rw-r--r--   0 mon       (1000) mon       (1000)     4021 2020-05-29 03:36:28.000000 aiootp-0.9.3/tests/test_high_level_encryption.py
+-rw-r--r--   0 mon       (1000) mon       (1000)       92 2020-06-02 04:07:02.000000 aiootp-0.9.3/.gitignore
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/
+-rw-r--r--   0 mon       (1000) mon       (1000)        1 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/dependency_links.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)    67978 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/PKG-INFO
+-rw-r--r--   0 mon       (1000) mon       (1000)        7 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/top_level.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)       70 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/requires.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     1100 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp.egg-info/SOURCES.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)    53419 2020-06-14 02:44:58.000000 aiootp-0.9.3/README.rst
+-rw-r--r--   0 mon       (1000) mon       (1000)    67978 2020-06-14 02:44:58.000000 aiootp-0.9.3/PKG-INFO
+-rw-r--r--   0 mon       (1000) mon       (1000)      335 2020-06-14 02:44:12.000000 aiootp-0.9.3/sha256_ROOT_CHECKSUM.sig
+-rw-r--r--   0 mon       (1000) mon       (1000)       64 2020-06-14 02:44:58.000000 aiootp-0.9.3/sha256_ROOT_CHECKSUM.txt
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/licenses/
+-rw-r--r--   0 mon       (1000) mon       (1000)    11435 2020-04-16 20:20:58.000000 aiootp-0.9.3/licenses/uvloop_LICENSE_1.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)    11332 2019-10-09 16:52:31.000000 aiootp-0.9.3/licenses/aiofiles_LICENSE.txt
+-rw-rw-rw-   0 mon       (1000) mon       (1000)    12769 2019-12-10 03:29:08.000000 aiootp-0.9.3/licenses/cpython_LICENSE.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     1067 2020-04-20 14:26:15.000000 aiootp-0.9.3/licenses/aioitertools_LICENSE.txt
+-rw-rw-rw-   0 mon       (1000) mon       (1000)     1075 2019-12-13 12:12:29.000000 aiootp-0.9.3/licenses/asyncio_contextmanager_LICENSE.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     1101 2020-04-16 20:19:41.000000 aiootp-0.9.3/licenses/uvloop_LICENSE_0.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     1326 2020-04-16 20:29:28.000000 aiootp-0.9.3/licenses/pybase64_LICENSE.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     1226 2020-04-16 21:03:39.000000 aiootp-0.9.3/licenses/async_lru_LICENSE.txt
+-rw-rw-rw-   0 mon       (1000) mon       (1000)     1096 2019-12-10 05:16:17.000000 aiootp-0.9.3/licenses/pytest_LICENSE.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     4952 2019-12-20 23:38:02.000000 aiootp-0.9.3/licenses/sympy_LICENSE.txt
+-rwxrwxrwx   0 mon       (1000) mon       (1000)     4828 2020-06-14 02:31:21.000000 aiootp-0.9.3/setup.py
+-rw-r--r--   0 mon       (1000) mon       (1000)      420 2020-06-14 02:44:19.000000 aiootp-0.9.3/sha512_ROOT_CHECKSUM.sig
+-rw-r--r--   0 mon       (1000) mon       (1000)      984 2020-06-02 04:06:16.000000 aiootp-0.9.3/MANIFEST.in
+-rw-r--r--   0 mon       (1000) mon       (1000)    30607 2020-06-11 14:14:11.000000 aiootp-0.9.3/PREADME.rst
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp/
+-rw-r--r--   0 mon       (1000) mon       (1000)     4646 2020-05-31 05:42:52.000000 aiootp-0.9.3/aiootp/asynchs.py
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp/tor/
+-rw-rw-r--   0 mon       (1000) mon       (1000)      447 2020-04-20 02:48:31.000000 aiootp-0.9.3/aiootp/tor/README_TOR.rst
+-rwxrwxrwx   0 mon       (1000) mon       (1000)   152558 2020-06-13 22:21:44.000000 aiootp-0.9.3/aiootp/ciphers.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)     9662 2020-06-11 01:32:57.000000 aiootp-0.9.3/aiootp/__ui_coordination.py
+-rwxrwxrwx   0 mon       (1000) mon       (1000)    51750 2020-06-14 00:59:19.000000 aiootp-0.9.3/aiootp/randoms.py
+-rwxrwxrwx   0 mon       (1000) mon       (1000)    18989 2020-05-31 05:45:20.000000 aiootp-0.9.3/aiootp/debuggers.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)     9000 2020-06-10 01:08:57.000000 aiootp-0.9.3/aiootp/commons.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)   644679 2020-06-03 10:46:44.000000 aiootp-0.9.3/aiootp/__datasets.py
+drwxr-xr-x   0 mon       (1000) mon       (1000)        0 2020-06-14 02:44:58.000000 aiootp-0.9.3/aiootp/databases/
+-rw-rw-r--   0 mon       (1000) mon       (1000)     9895 2020-06-09 04:06:10.000000 aiootp-0.9.3/aiootp/databases/README_DATABASES.rst
+-rwxrwxrwx   0 mon       (1000) mon       (1000)    23099 2020-06-13 15:12:18.000000 aiootp-0.9.3/aiootp/keygens.py
+-rw-r--r--   0 mon       (1000) mon       (1000)     1049 2020-06-14 02:31:30.000000 aiootp-0.9.3/aiootp/__init__.py
+-rwxrwxrwx   0 mon       (1000) mon       (1000)   116729 2020-06-14 00:34:42.000000 aiootp-0.9.3/aiootp/generics.py
+-rw-rw-r--   0 mon       (1000) mon       (1000)     1829 2020-05-31 05:39:00.000000 aiootp-0.9.3/aiootp/paths.py
+-rw-r--r--   0 mon       (1000) mon       (1000)      128 2020-06-14 02:44:58.000000 aiootp-0.9.3/sha512_ROOT_CHECKSUM.txt
+-rw-r--r--   0 mon       (1000) mon       (1000)     6636 2020-06-14 02:44:58.000000 aiootp-0.9.3/CHECKSUMS.txt
```

### Comparing `aiootp-0.9.2/LICENSE` & `aiootp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/CHANGES.rst` & `aiootp-0.9.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 ``Known Issues``
 =================
 
 -  The test suite for this software is under construction, & what tests
    have been published are currently inadequate to the needs of
    cryptography software.
 -  This package is currently in beta testing. Contributions are welcome.
@@ -14,14 +13,39 @@
 
 
 
 ``Changelog``
 =============
 
 
+Changes for version 0.9.3 
+========================= 
+
+
+Major Changes 
+------------- 
+
+-  Speed & efficiency improvements in the ``Comprende`` class & ``azip``. 
+
+
+Minor Changes 
+------------- 
+
+-  Various refactorings & code cleanups.
+-  Added ``apop`` & ``pop`` ``Comprende`` generators to the library.
+-  Switched the default character table in the ``ato_base``, ``to_base``, 
+   ``afrom_base``, & ``from_base`` chainable generator methods from the 62
+   character ``ASCII_ALPHANUMERIC`` table, to the 95 character ``ASCII_TABLE``.
+-  Made the digits generators in ``randoms.py`` automatically create a new
+   cryptographically secure key if a key isn't passed by a user.
+-  Some extra data processing functions added to ``generics.py``.
+
+
+
+
 Changes for version 0.9.2 
 ========================= 
 
 
 Major Changes 
 -------------
```

### Comparing `aiootp-0.9.2/tests/test_ciphers.py` & `aiootp-0.9.3/tests/test_ciphers.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/tests/test_Comprende.py` & `aiootp-0.9.3/tests/test_Comprende.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/tests/test_generics.py` & `aiootp-0.9.3/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/tests/test_Database_AsyncDatabase.py` & `aiootp-0.9.3/tests/test_Database_AsyncDatabase.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/tests/test_high_level_encryption.py` & `aiootp-0.9.3/tests/test_high_level_encryption.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp.egg-info/PKG-INFO` & `aiootp-0.9.3/aiootp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiootp
-Version: 0.9.2
+Version: 0.9.3
 Summary: aiootp - an asynchronous one-time-pad based crypto and anonymity library.
 Home-page: https://github.com/rmlibre/aiootp
 Author: Gonzo Investigatory Journalism Agency, LLC
 Author-email: gonzo.development@protonmail.ch
 Maintainer: Gonzo Investigatory Journalism Agency, LLC
 Maintainer-email: gonzo.development@protonmail.ch
 License: AGPLv3
@@ -1020,15 +1020,14 @@
         
         **Q: Why are the modules transformed into ``Namespace`` objects?**
         
         A: We overwrite our modules in this package to have a more fine-grained control over what part of the package's internal state is exposed to users and applications. The goal is make it more difficult for users to inadvertently jeopardize their security tools, and minimize the attack surface available to adversaries. The ``aiootp.Namespace`` class also makes it easier to coordinate and decide the library's UI/UX across the package.
         
         
         
-        
         ``Known Issues``
         =================
         
         -  The test suite for this software is under construction, & what tests
            have been published are currently inadequate to the needs of
            cryptography software.
         -  This package is currently in beta testing. Contributions are welcome.
@@ -1040,14 +1039,39 @@
         
         
         
         ``Changelog``
         =============
         
         
+        Changes for version 0.9.3 
+        ========================= 
+        
+        
+        Major Changes 
+        ------------- 
+        
+        -  Speed & efficiency improvements in the ``Comprende`` class & ``azip``. 
+        
+        
+        Minor Changes 
+        ------------- 
+        
+        -  Various refactorings & code cleanups.
+        -  Added ``apop`` & ``pop`` ``Comprende`` generators to the library.
+        -  Switched the default character table in the ``ato_base``, ``to_base``, 
+           ``afrom_base``, & ``from_base`` chainable generator methods from the 62
+           character ``ASCII_ALPHANUMERIC`` table, to the 95 character ``ASCII_TABLE``.
+        -  Made the digits generators in ``randoms.py`` automatically create a new
+           cryptographically secure key if a key isn't passed by a user.
+        -  Some extra data processing functions added to ``generics.py``.
+        
+        
+        
+        
         Changes for version 0.9.2 
         ========================= 
         
         
         Major Changes 
         -------------
```

### Comparing `aiootp-0.9.2/aiootp.egg-info/SOURCES.txt` & `aiootp-0.9.3/aiootp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/README.rst` & `aiootp-0.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1010,15 +1010,14 @@
 
 **Q: Why are the modules transformed into ``Namespace`` objects?**
 
 A: We overwrite our modules in this package to have a more fine-grained control over what part of the package's internal state is exposed to users and applications. The goal is make it more difficult for users to inadvertently jeopardize their security tools, and minimize the attack surface available to adversaries. The ``aiootp.Namespace`` class also makes it easier to coordinate and decide the library's UI/UX across the package.
 
 
 
-
 ``Known Issues``
 =================
 
 -  The test suite for this software is under construction, & what tests
    have been published are currently inadequate to the needs of
    cryptography software.
 -  This package is currently in beta testing. Contributions are welcome.
@@ -1030,14 +1029,39 @@
 
 
 
 ``Changelog``
 =============
 
 
+Changes for version 0.9.3 
+========================= 
+
+
+Major Changes 
+------------- 
+
+-  Speed & efficiency improvements in the ``Comprende`` class & ``azip``. 
+
+
+Minor Changes 
+------------- 
+
+-  Various refactorings & code cleanups.
+-  Added ``apop`` & ``pop`` ``Comprende`` generators to the library.
+-  Switched the default character table in the ``ato_base``, ``to_base``, 
+   ``afrom_base``, & ``from_base`` chainable generator methods from the 62
+   character ``ASCII_ALPHANUMERIC`` table, to the 95 character ``ASCII_TABLE``.
+-  Made the digits generators in ``randoms.py`` automatically create a new
+   cryptographically secure key if a key isn't passed by a user.
+-  Some extra data processing functions added to ``generics.py``.
+
+
+
+
 Changes for version 0.9.2 
 ========================= 
 
 
 Major Changes 
 -------------
```

### Comparing `aiootp-0.9.2/PKG-INFO` & `aiootp-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aiootp
-Version: 0.9.2
+Version: 0.9.3
 Summary: aiootp - an asynchronous one-time-pad based crypto and anonymity library.
 Home-page: https://github.com/rmlibre/aiootp
 Author: Gonzo Investigatory Journalism Agency, LLC
 Author-email: gonzo.development@protonmail.ch
 Maintainer: Gonzo Investigatory Journalism Agency, LLC
 Maintainer-email: gonzo.development@protonmail.ch
 License: AGPLv3
@@ -1020,15 +1020,14 @@
         
         **Q: Why are the modules transformed into ``Namespace`` objects?**
         
         A: We overwrite our modules in this package to have a more fine-grained control over what part of the package's internal state is exposed to users and applications. The goal is make it more difficult for users to inadvertently jeopardize their security tools, and minimize the attack surface available to adversaries. The ``aiootp.Namespace`` class also makes it easier to coordinate and decide the library's UI/UX across the package.
         
         
         
-        
         ``Known Issues``
         =================
         
         -  The test suite for this software is under construction, & what tests
            have been published are currently inadequate to the needs of
            cryptography software.
         -  This package is currently in beta testing. Contributions are welcome.
@@ -1040,14 +1039,39 @@
         
         
         
         ``Changelog``
         =============
         
         
+        Changes for version 0.9.3 
+        ========================= 
+        
+        
+        Major Changes 
+        ------------- 
+        
+        -  Speed & efficiency improvements in the ``Comprende`` class & ``azip``. 
+        
+        
+        Minor Changes 
+        ------------- 
+        
+        -  Various refactorings & code cleanups.
+        -  Added ``apop`` & ``pop`` ``Comprende`` generators to the library.
+        -  Switched the default character table in the ``ato_base``, ``to_base``, 
+           ``afrom_base``, & ``from_base`` chainable generator methods from the 62
+           character ``ASCII_ALPHANUMERIC`` table, to the 95 character ``ASCII_TABLE``.
+        -  Made the digits generators in ``randoms.py`` automatically create a new
+           cryptographically secure key if a key isn't passed by a user.
+        -  Some extra data processing functions added to ``generics.py``.
+        
+        
+        
+        
         Changes for version 0.9.2 
         ========================= 
         
         
         Major Changes 
         -------------
```

### Comparing `aiootp-0.9.2/licenses/uvloop_LICENSE_1.txt` & `aiootp-0.9.3/licenses/uvloop_LICENSE_1.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/aiofiles_LICENSE.txt` & `aiootp-0.9.3/licenses/aiofiles_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/cpython_LICENSE.txt` & `aiootp-0.9.3/licenses/cpython_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/aioitertools_LICENSE.txt` & `aiootp-0.9.3/licenses/aioitertools_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/asyncio_contextmanager_LICENSE.txt` & `aiootp-0.9.3/licenses/asyncio_contextmanager_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/uvloop_LICENSE_0.txt` & `aiootp-0.9.3/licenses/uvloop_LICENSE_0.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/pybase64_LICENSE.txt` & `aiootp-0.9.3/licenses/pybase64_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/async_lru_LICENSE.txt` & `aiootp-0.9.3/licenses/async_lru_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/pytest_LICENSE.txt` & `aiootp-0.9.3/licenses/pytest_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/licenses/sympy_LICENSE.txt` & `aiootp-0.9.3/licenses/sympy_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/setup.py` & `aiootp-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         sha256sum = sha256(package_checksums.encode()).hexdigest()
         root_hash_256.write(sha256sum)
 
 
 setup(
     name="aiootp",
     license="AGPLv3",
-    version="0.9.2",
+    version="0.9.3",
     description=description,
     long_description=long_description,
     url="https://github.com/rmlibre/aiootp",
     author="Gonzo Investigatory Journalism Agency, LLC",
     author_email="gonzo.development@protonmail.ch",
     maintainer="Gonzo Investigatory Journalism Agency, LLC",
     maintainer_email="gonzo.development@protonmail.ch",
```

### Comparing `aiootp-0.9.2/MANIFEST.in` & `aiootp-0.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/PREADME.rst` & `aiootp-0.9.3/PREADME.rst`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/asynchs.py` & `aiootp-0.9.3/aiootp/asynchs.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/ciphers.py` & `aiootp-0.9.3/aiootp/ciphers.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,21 +75,19 @@
 from .generics import data, adata
 from .generics import pick, apick
 from .generics import cycle, acycle
 from .generics import order, aorder
 from .generics import birth, abirth
 from .generics import unpack, aunpack
 from .generics import ignore, aignore
-from .generics import nc_512, anc_512
 from .generics import sha_256, asha_256
 from .generics import sha_512, asha_512
 from .generics import lru_cache, alru_cache
 from .generics import Comprende, comprehension
 from .generics import json_encode, ajson_encode
-from .generics import json_decode, ajson_decode
 from .generics import sha_256_hmac, asha_256_hmac
 from .generics import sha_512_hmac, asha_512_hmac
 
 
 @comprehension()
 async def axor(
     *datastreams, key=None, buffer_size=power10[20], convert=True
```

### Comparing `aiootp-0.9.2/aiootp/__ui_coordination.py` & `aiootp-0.9.3/aiootp/__ui_coordination.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/randoms.py` & `aiootp-0.9.3/aiootp/randoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,15 +417,15 @@
 
     Usage Example:
 
     numbers = list(range(10))
     multiply = await asalted_multiply().aprime()
     randomized_number = await multiply(numbers)
     """
-    if offset == None:
+    if not offset:
         offset = token_bits(int(math.log2(mod) + 128))
     mix = int(sha_512(mod, offset), 16)
     start = seed = int(sha_256(mix, offset), 16)
     numbers = (mix * seed * offset,)
     while True:
         mix ^= abs(sum((seed, offset, *numbers)))
         mix %= mod
@@ -456,15 +456,15 @@
 
     Usage Example:
 
     numbers = list(range(10))
     multiply = salted_multiply().prime()
     randomized_number = multiply(numbers)
     """
-    if offset == None:
+    if not offset:
         offset = token_bits(int(math.log2(mod) + 128))
     mix = int(sha_512(mod, offset), 16)
     start = seed = int(sha_256(mix, offset), 16)
     numbers = (mix * seed * offset,)
     while True:
         mix ^= abs(sum((seed, offset, *numbers)))
         mix %= mod
@@ -1149,54 +1149,86 @@
         kdf.update(seed + seed_key + entropy)
         seed = kdf.digest()
         kdf.update(seed + seed_key + entropy)
         entropy = yield kdf.hexdigest()
 
 
 @comprehension()
-async def anon_0_digits(key=sha_512(_salt()), stream_key=""):
+async def anon_0_digits(key=None, stream_key=""):
     """
     Creates a deterministic stream of non-zero digits from a key.
     """
+    key = key if key else await acsprng()
     seed = await asha_512(key)
     while True:
         stream_key = await aint(await anc_512(seed, key, stream_key), 16)
         for char in (await astr(stream_key)).replace("0", "")[8:]:
             yield await aint(char)
 
 
 @comprehension()
-def non_0_digits(key=sha_512(_salt()), stream_key=""):
+def non_0_digits(key=None, stream_key=""):
     """
     Creates a deterministic stream of non-zero digits from a key.
     """
+    key = key if key else csprng()
     seed = sha_512(key)
     while True:
         stream_key = int(nc_512(seed, key, stream_key), 16)
         for char in str(stream_key).replace("0", "")[8:]:
             yield int(char)
 
 
 @comprehension()
-async def adigits(key=sha_512(_salt()), stream_key=""):
+async def abytes_digits(key=None, stream_key=""):
+    """
+    Creates a deterministic stream of bytes numbers from a key.
+    """
+    key = key if key else await acsprng()
+    seed = await asha_512(key)
+    from_hex = bytes.fromhex
+    while True:
+        stream_key = from_hex(await anc_512(seed, key, stream_key))
+        for char in stream_key[4:]:
+            yield char
+
+
+@comprehension()
+def bytes_digits(key=None, stream_key=""):
+    """
+    Creates a deterministic stream of bytes numbers from a key.
+    """
+    key = key if key else csprng()
+    seed = sha_512(key)
+    from_hex = bytes.fromhex
+    while True:
+        stream_key = from_hex(nc_512(seed, key, stream_key))
+        for char in stream_key[4:]:
+            yield char
+
+
+@comprehension()
+async def adigits(key=None, stream_key=""):
     """
     Creates a deterministic stream of digits from a key.
     """
+    key = key if key else await acsprng()
     seed = await asha_512(key)
     while True:
         stream_key = await aint(await anc_512(seed, key, stream_key), 16)
         for char in (await astr(stream_key))[8:]:
             yield await aint(char)
 
 
 @comprehension()
-def digits(key=sha_512(_salt()), stream_key=""):
+def digits(key=None, stream_key=""):
     """
     Creates a deterministic stream of digits from a key.
     """
+    key = key if key else csprng()
     seed = sha_512(key)
     while True:
         stream_key = int(nc_512(seed, key, stream_key), 16)
         for char in str(stream_key)[8:]:
             yield int(char)
 
 
@@ -1433,14 +1465,15 @@
     raise failure from error
 
 
 __extras = {
     "__doc__": __doc__,
     "__main_exports__": __all__,
     "__package__": "aiootp",
+    "abytes_digits": abytes_digits,
     "achoice": achoice,
     "acreate_prime": acreate_prime,
     "acsprng": acsprng,
     "adigits": adigits,
     "agenerate_big_range_bounds": agenerate_big_range_bounds,
     "agenerate_small_range_bounds": agenerate_small_range_bounds,
     "agenerate_unique_range_bounds": agenerate_unique_range_bounds,
@@ -1472,14 +1505,15 @@
     "aunique_integer": aunique_integer,
     "aunique_lower_bound": aunique_lower_bound,
     "aunique_upper_bound": aunique_upper_bound,
     "aunshuffle": aunshuffle,
     "aurandom": aurandom,
     "aurandom_hash": aurandom_hash,
     "aurandom_number": aurandom_number,
+    "bytes_digits": bytes_digits,
     "choice": choice,
     "create_prime": create_prime,
     "csprng": csprng,
     "digits": digits,
     "generate_big_range_bounds": generate_big_range_bounds,
     "generate_small_range_bounds": generate_small_range_bounds,
     "generate_unique_range_bounds": generate_unique_range_bounds,
```

### Comparing `aiootp-0.9.2/aiootp/debuggers.py` & `aiootp-0.9.3/aiootp/debuggers.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/commons.py` & `aiootp-0.9.3/aiootp/commons.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/__datasets.py` & `aiootp-0.9.3/aiootp/__datasets.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/databases/README_DATABASES.rst` & `aiootp-0.9.3/aiootp/databases/README_DATABASES.rst`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/keygens.py` & `aiootp-0.9.3/aiootp/keygens.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/aiootp/__init__.py` & `aiootp-0.9.3/aiootp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright © 2019-2020 Gonzo Investigatory Journalism Agency, LLC
 #            <gonzo.development@protonmail.ch>
 #           © 2019-2020 Richard Machado <rmlibre@riseup.net>
 # All rights reserved.
 #
 
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 
 __license__ = "AGPLv3"
 
 
 __doc__ = """
 aiootp - an asynchronous one-time-pad based crypto and anonymity library.
```

### Comparing `aiootp-0.9.2/aiootp/generics.py` & `aiootp-0.9.3/aiootp/generics.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     "data",
     "aorder",
     "order",
     "apick",
     "pick",
     "acycle",
     "cycle",
+    "apop",
+    "pop",
     "apopleft",
     "popleft",
     "ajson_decode",
     "json_decode",
     "ajson_encode",
     "json_encode",
     "asha_256",
@@ -828,27 +830,19 @@
         have a mechanism for returning values. So this async context
         manager handles catching return values from UserWarning
         exceptions & appends those results to ``self._return``. Items
         in the result queue are accessible from ``self.aresult()``.
         """
         try:
             yield self
-        except RuntimeError as done:
-            if (
-                self.ASYNC_GEN_DONE not in done.args
-                and self.ASYNC_GEN_THROWN not in done.args
-            ):
-                raise done
         except UserWarning as done:
             if done.args:
                 self._return.append(done.args[0])
         except StopAsyncIteration:
             pass
-        except GeneratorExit as error:
-            raise GeneratorExit from error
 
     @contextmanager
     def catch(self):
         """
         Handles catching the return values passed through exceptions
         from sync generators & makes sure other errors are propagated
         correctly up to user code. Synchronous generators already have
@@ -879,16 +873,14 @@
         try:
             source = source if source else self
             yield self
         except UserWarning:
             if result != None:
                 raise UserWarning(result)
             raise UserWarning(await source.aresult(exit=True))
-        except GeneratorExit as error:
-            raise GeneratorExit from error
 
     @contextmanager
     def relay(self, result=None, source=None):
         """
         This is a lower level context manager for users who've created
         sync generators that need to propagate results up to calling
         code. Code in this context manager's block will relay a ``result``
@@ -1502,35 +1494,40 @@
     def tag(self, of=None):
         """
         By default behaves like ``enumerate`` for each value yielded
         from the underlying Comprende sync generator. Optionally, ``of``
         can be passed an iterable & prepends those values to the
         generator's results.
         """
-        names = of if of != None else count()
-        for name, item in zip(names, self):
-            yield name, item
+        if of != None:
+            for name, item in zip(of, self):
+                yield name, item
+        else:
+            for name, item in enumerate(self):
+                yield name, item
 
     async def aheappop(self, span=None, *, of=None):
         """
         Exhausts the underlying Comprende async generator upto ``span``
         number of iterations, then yields the results in sorted order
         based on the ``heapq.heappop`` function.
         """
         if of != None:
-            async with aunpack(of)[:span] as accumulator:
+            target = aunpack(of)[:span] if span else aunpack(of)
+            async with target as accumulator:
                 results = await accumulator.alist()
             heapq.heapify(results)
             async for result in self:
                 try:
                     yield result, heapq.heappop(results)
                 except IndexError:
                     break
         else:
-            async with aunpack(self)[:span] as accumulator:
+            target = self[:span] if span else self
+            async with target as accumulator:
                 results = await accumulator.alist()
             heapq.heapify(results)
             while True:
                 try:
                     yield heapq.heappop(results)
                 except IndexError:
                     break
@@ -1538,61 +1535,67 @@
     def heappop(self, span=None, *, of=None):
         """
         Exhausts the underlying Comprende sync generator upto ``span``
         number of iterations, then yields the results in sorted order
         based on the ``heapq.heappop`` function.
         """
         if of != None:
-            with unpack(of)[:span] as accumulator:
+            target = unpack(of)[:span] if span else unpack(of)
+            with target as accumulator:
                 results = accumulator.list()
             heapq.heapify(results)
             for result in self:
                 try:
                     yield result, heapq.heappop(results)
                 except IndexError:
                     break
         else:
-            with unpack(self)[:span] as accumulator:
+            target = self[:span] if span else self
+            with target as accumulator:
                 results = accumulator.list()
             heapq.heapify(results)
             while True:
                 try:
                     yield heapq.heappop(results)
                 except IndexError:
                     break
 
     async def areversed(self, span=None, *, of=None):
         """
         Exhausts the underlying Comprende async generator upto ``span``
         number of iterations, then yields the results in reversed order.
         """
         if of != None:
-            async with unpack(of)[:span] as accumulator:
+            target = aunpack(of)[:span] if span else aunpack(of)
+            async with target as accumulator:
                 results = await accumulator.adeque()
             async for prev, result in azip(self, reversed(results)):
                 yield prev, result
         else:
-            async with unpack(self)[:span] as accumulator:
+            target = self[:span] if span else self
+            async with target as accumulator:
                 results = await accumulator.adeque()
             for result in reversed(results):
                 await switch()
                 yield result
 
     def reversed(self, span=None, *, of=None):
         """
         Exhausts the underlying Comprende sync generator upto ``span``
         number of iterations, then yields the results in reversed order.
         """
         if of != None:
-            with unpack(of)[:span] as accumulator:
+            target = unpack(of)[:span] if span else unpack(of)
+            with target as accumulator:
                 results = accumulator.deque()
             for prev, result in zip(self, reversed(results)):
                 yield prev, result
         else:
-            with unpack(self)[:span] as accumulator:
+            target = self[:span] if span else self
+            with target as accumulator:
                 results = accumulator.deque()
             for result in reversed(results):
                 yield result
 
     async def asort(self, key=None, span=None, *, of=None):
         """
         Exhausts the underlying Comprende async generator upto ``span``
@@ -1635,72 +1638,72 @@
                 yield result
 
     async def aresize(self, size=128, *, of=None):
         """
         Buffers the output from the underlying Comprende async generator
         to yield the results in chunks of length ``size``.
         """
-        iterable_self = aiter(self)
+        next_self = self.anext
         if of != None:
-            new_source = aiter(of)
-            result = await anext(new_source)
+            next_source = aiter(of).__anext__
+            result = await next_source()
             while True:
                 while len(result) >= size:
                     cache = result[size:]
-                    yield await anext(iterable_self), result[:size]
+                    yield await next_self(), result[:size]
                     result = cache
                 try:
-                    result += await anext(new_source)
+                    result += await next_source()
                 except StopAsyncIteration:
                     break
             if result:
-                yield await anext(iterable_self), result
+                yield await next_self(), result
         else:
-            result = await anext(iterable_self)
+            result = await next_self()
             while True:
                 while len(result) >= size:
                     cache = result[size:]
                     yield result[:size]
                     result = cache
                 try:
-                    result += await anext(iterable_self)
+                    result += await next_self()
                 except StopAsyncIteration:
                     break
             if result:
                 yield result
 
     def resize(self, size=128, *, of=None):
         """
         Buffers the output from the underlying Comprende sync generator
         to yield the results in chunks of length ``size``.
         """
-        iterable_self = iter(self)
+        next_self = self.next
         if of != None:
-            new_source = iter(of)
-            result = next(new_source)
+            next_source = iter(of).__next__
+            result = next_source()
             while True:
                 while len(result) >= size:
                     cache = result[size:]
-                    yield next(iterable_self), result[:size]
+                    yield next_self(), result[:size]
                     result = cache
                 try:
-                    result += next(new_source)
+                    result += next_source()
                 except StopIteration:
                     break
             if result:
-                yield next(iterable_self), result
+                yield next_self(), result
         else:
-            result = next(iterable_self)
+            result = next_self()
             while True:
                 while len(result) >= size:
                     cache = result[size:]
                     yield result[:size]
                     result = cache
                 try:
-                    result += next(iterable_self)
+                    result += next_self()
                 except StopIteration:
                     break
             if result:
                 yield result
 
     async def adelimit(self, delimiter=" "):
         """
@@ -2204,53 +2207,53 @@
         if of != None:
             for prev, result in zip(self, of):
                 yield prev, bytes.hex(result)
         else:
             for result in self:
                 yield bytes.hex(result)
 
-    async def ato_base(self, base=16, table=ASCII_ALPHANUMERIC, *, of=None):
+    async def ato_base(self, base=95, table=ASCII_TABLE, *, of=None):
         """
         Converts each integer value that's yielded from the underlying
         Comprende async generator to a string in ``base`` before yielding
         the result.
         """
         if of != None:
             async for prev, result in azip(self, of):
                 yield prev, await ainverse_int(result, base, table)
         else:
             async for result in self:
                 yield await ainverse_int(result, base, table)
 
-    def to_base(self, base=16, table=ASCII_ALPHANUMERIC, *, of=None):
+    def to_base(self, base=95, table=ASCII_TABLE, *, of=None):
         """
         Converts each integer value that's yielded from the underlying
         Comprende sync generator to a string in ``base`` before yielding
         the result.
         """
         if of != None:
             for prev, result in zip(self, of):
                 yield prev, inverse_int(result, base, table)
         else:
             for result in self:
                 yield inverse_int(result, base, table)
 
-    async def afrom_base(self, base, table=ASCII_ALPHANUMERIC, *, of=None):
+    async def afrom_base(self, base=95, table=ASCII_TABLE, *, of=None):
         """
         Convert string results of generator results in numerical ``base``
         into decimal.
         """
         if of != None:
             async for prev, result in azip(self, of):
                 yield prev, await abase_to_decimal(result, base, table)
         else:
             async for result in self:
                 yield await abase_to_decimal(result, base, table)
 
-    def from_base(self, base, table=ASCII_ALPHANUMERIC, *, of=None):
+    def from_base(self, base=95, table=ASCII_TABLE, *, of=None):
         """
         Convert ``string`` in numerical ``base`` into decimal.
         """
         if of != None:
             for prev, result in zip(self, of):
                 yield prev, base_to_decimal(result, base, table)
         else:
@@ -2797,15 +2800,15 @@
 async def azip(*coros):
     """
     Creates an asynchronous version of the ``builtins.zip`` function.
     """
     coros = [aiter(coro).__anext__ for coro in coros]
     try:
         while True:
-            yield await gather(*[coro() for coro in coros])
+            yield [await coro() for coro in coros]
     except StopAsyncIteration:
         pass
 
 
 @comprehension()
 def _zip(*iterables):
     """
@@ -3111,14 +3114,40 @@
         try:
             yield queue.popleft()
         except IndexError:
             break
 
 
 @comprehension()
+async def apop(queue):
+    """
+    An async generator which calls the ``pop()`` method on ``queue``
+    for every iteration, & exits on ``IndexError``.
+    """
+    while True:
+        try:
+            yield queue.pop()
+        except IndexError:
+            break
+
+
+@comprehension()
+def pop(queue):
+    """
+    A generator which calls the ``pop()`` method on ``queue`` for
+    every iteration, & exits on ``IndexError``.
+    """
+    while True:
+        try:
+            yield queue.pop()
+        except IndexError:
+            break
+
+
+@comprehension()
 async def apick(names=None, mapping=None):
     """
     Does a bracketed lookup on ``mapping`` for each name in ``names``.
     """
     async for name in names:
         try:
             yield mapping[name]
@@ -3524,14 +3553,44 @@
 def int_to_bytes(bytes_object, size=128, byte_order="big"):
     """
     Returns the bytes object representation of an integer.
     """
     return int.to_bytes(bytes_object, size, byte_order)
 
 
+async def ahex_to_bytes(data):
+    """
+    Applies ``bytes.fromhex(data)`` to ``data`` & returns the bytes
+    result.
+    """
+    yield bytes.fromhex(result)
+
+
+def hex_to_bytes(data):
+    """
+    Applies ``bytes.fromhex(data)`` to ``data`` & returns the bytes
+    result.
+    """
+    yield bytes.fromhex(result)
+
+
+async def abytes_to_hex(data):
+    """
+    Applies ``bytes.hex(data)`` to ``data`` & returns the hex result.
+    """
+    return bytes.hex(result)
+
+
+def bytes_to_hex(data):
+    """
+    Applies ``bytes.hex(data)`` to ``data`` & returns the hex result.
+    """
+    return bytes.hex(result)
+
+
 async def abinary_tree(depth=4, leaf={}, current=0):
     """
     Recursively builds a binary tree ``depth`` branches deep & places
     the placeholder value ``leaf`` at each endpoint of the tree.  The
     kwarg ``current`` is only to be used internally by the function to
     keep track of which recursion is being run.
     """
@@ -3575,36 +3634,39 @@
     "__package__": "aiootp",
     "aabs": aabs,
     "aappend": aappend,
     "aascii_to_int": aascii_to_int,
     "abase_to_decimal": abase_to_decimal,
     "abinary_tree": abinary_tree,
     "abirth": abirth,
+    "abytes_to_hex": abytes_to_hex,
     "abytes_to_int": abytes_to_int,
     "acompact": acompact,
     "acount": acount,
     "acustomize_parameters": acustomize_parameters,
     "acycle": acycle,
     "adata": adata,
     "afrom_b64": afrom_b64,
-    "apick": apick,
+    "ahex_to_bytes": ahex_to_bytes,
     "aignore": aignore,
     "aint": aint,
     "aint_to_ascii": aint_to_ascii,
     "aint_to_bytes": aint_to_bytes,
     "ainverse_int": ainverse_int,
     "aiter": _aiter,
     "ajson_decode": ajson_decode,
     "ajson_encode": ajson_encode,
     "anc_256": anc_256,
     "anc_256_hmac": anc_256_hmac,
     "anc_512": anc_512,
     "anc_512_hmac": anc_512_hmac,
     "anext": anext,
     "aorder": aorder,
+    "apick": apick,
+    "apop": apop,
     "apopleft": apopleft,
     "arange": arange,
     "ascii_to_int": ascii_to_int,
     "aseedrange": aseedrange,
     "asha_256": asha_256,
     "asha_256_hmac": asha_256_hmac,
     "asha_512": asha_512,
@@ -3613,25 +3675,26 @@
     "astr": astr,
     "ato_b64": ato_b64,
     "aunpack": aunpack,
     "azip": azip,
     "base_to_decimal": base_to_decimal,
     "binary_tree": binary_tree,
     "birth": birth,
+    "bytes_to_hex": bytes_to_hex,
     "bytes_to_int": bytes_to_int,
     "compact": compact,
     "comprehension": comprehension,
     "convert_static_method_to_member": convert_static_method_to_member,
     "count": count,
     "customize_parameters": customize_parameters,
     "cycle": cycle,
     "data": data,
     "display_exception_info": display_exception_info,
     "from_b64": from_b64,
-    "pick": pick,
+    "hex_to_bytes": hex_to_bytes,
     "ignore": ignore,
     "int_to_ascii": int_to_ascii,
     "int_to_bytes": int_to_bytes,
     "inverse_int": inverse_int,
     "is_async_function": is_async_function,
     "is_async_gen_function": is_async_gen_function,
     "is_async_generator": is_async_generator,
@@ -3648,14 +3711,16 @@
     "json_decode": json_decode,
     "json_encode": json_encode,
     "nc_256": nc_256,
     "nc_256_hmac": nc_256_hmac,
     "nc_512": nc_512,
     "nc_512_hmac": nc_512_hmac,
     "order": order,
+    "pick": pick,
+    "pop": pop,
     "popleft": popleft,
     "range": _range,
     "seedrange": seedrange,
     "sha3_256": sha3_256,
     "sha3_512": sha3_512,
     "sha_256": sha_256,
     "sha_256_hmac": sha_256_hmac,
```

### Comparing `aiootp-0.9.2/aiootp/paths.py` & `aiootp-0.9.3/aiootp/paths.py`

 * *Files identical despite different names*

### Comparing `aiootp-0.9.2/CHECKSUMS.txt` & `aiootp-0.9.3/CHECKSUMS.txt`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9351851851851851%*

 * *Differences: {"'sha256'": "{'setup.py': 'ef207212e1316a325f579e453709fc1a396195e5d97c6cc89ba07c8241377d4c', "*

 * *             "'README.rst': 'd5d9d2086b890f1077a62c7df0c16d12483b13dc4cc40d798efb7b786623ab5d', "*

 * *             "'CHANGES.rst': '1c7c022431179e0018220023c4c7bc717f90ad2ffe6ee8b5cf4e1c36a37209ae', "*

 * *             "'aiootp/generics.py': "*

 * *             "'15391fec0008da25f70634e92be43d31e4026f18c7caadf02b5fa58c745481f0', "*

 * *             "'aiootp/randoms.py': "*

 * *             "'a9bd79e73349ba4b0c65480823960d020c7570a90a9f […]*

```diff
@@ -1,59 +1,59 @@
 {
     "sha256": {
         ".gitignore": "edc08dfcd3167481c58f4f41a426d968e3969ed0b0c44f83d51fe7556bfb7851",
-        "CHANGES.rst": "d560357f8594d60dd1599bc3acca82763f235559d202c0cf14b6872b8d271a52",
+        "CHANGES.rst": "1c7c022431179e0018220023c4c7bc717f90ad2ffe6ee8b5cf4e1c36a37209ae",
         "LICENSE": "bd5675b3ddabf9d9f1d3c70ef1d30ad6016114779fe1e52d5282987f007703ba",
         "MANIFEST.in": "30616c2b42358e0452ab5aa2f1dd6ba3a5a85a5158a5bdf3cf6f541533ddb288",
         "PREADME.rst": "b10182e0140ce06ed18f2489a8efa1f7603f99fd0902d341efb66cfa3d8f7353",
-        "README.rst": "af5f712acddc1469e76dbdf17e65719486b81ded9492176ce6648346a9480251",
+        "README.rst": "d5d9d2086b890f1077a62c7df0c16d12483b13dc4cc40d798efb7b786623ab5d",
         "aiootp/__datasets.py": "b0abeffb213e6f2ee4278647f290f365fb0440f599fbd1f822cc61e26f23b19e",
-        "aiootp/__init__.py": "2c7b7aa5380ba4092f8e2ad39c23bf18fbfbc1b9f7bd1be5c8f42071f3ff1b39",
+        "aiootp/__init__.py": "dece389b7a3dcc110a00ba2f202acc83d246bd8dabb6a86654421c88486666a7",
         "aiootp/__ui_coordination.py": "8f4b700c538df254b9e4093d62a5c62d83ca9aee75243a7c44553c0f70bc3ab0",
         "aiootp/asynchs.py": "2de51692a7f44d3a7f44aa604153d29ccf761be1038d71c5d17a14d900e8ac3e",
-        "aiootp/ciphers.py": "90eacdd597008399e9c83afb82258ce240f7eeb1cec8b7d19985a544baeafadb",
+        "aiootp/ciphers.py": "46f45cac25e856107964700aacb03af84cd1fd8077b11d1dacd754dcbd8c35cd",
         "aiootp/commons.py": "6fe441eda5a710fb368582d07263538bda182d22be1c9de084c92b978215e4ed",
         "aiootp/databases/README_DATABASES.rst": "9d67c9142d0bd41f0487a1d41f03789156215ca067b12bb0f1a3267db4079991",
         "aiootp/debuggers.py": "5ddda3705bd0ad3ef841ee30ab843efc99e3f8fa9f47104e0b6d0eac3f32d0b6",
-        "aiootp/generics.py": "41758e29063b6e39c98653071ac7b5efeee20707d37e7d57bd46331dfc573c43",
+        "aiootp/generics.py": "15391fec0008da25f70634e92be43d31e4026f18c7caadf02b5fa58c745481f0",
         "aiootp/keygens.py": "7c7c4ab42bbe6d6a9d8fc8fae102ace16c99b4fef2f7eea405f69891881f4779",
         "aiootp/paths.py": "c785585653de54e00c8cf3038d3c347de10bfbe7c6e693fc08496b5105baa5da",
-        "aiootp/randoms.py": "f646f6259ab99c04978cf7002edaddc7f1ab49d313ee9c682d80970d0ab5332d",
+        "aiootp/randoms.py": "a9bd79e73349ba4b0c65480823960d020c7570a90a9fba431193b1af317dd5da",
         "aiootp/tor/README_TOR.rst": "221c2b779c88ed2847d01413ac374bce8ffc2c6d3648a690a7a26ffcc64b6781",
         "setup.cfg": "22a14fd256f941817e97ef1f239ed5d4faaabfd2f11380eee999815313d1f844",
-        "setup.py": "58606e03d864a5f59ac5a7355eb8968069b784773e1056245ebdd9e662cd8c4a",
+        "setup.py": "ef207212e1316a325f579e453709fc1a396195e5d97c6cc89ba07c8241377d4c",
         "tests/test_Comprende.py": "1aa166a3561836ddbdc2823340b3699f88b7d241ba3183375ed489ba7c83ad4f",
         "tests/test_Database_AsyncDatabase.py": "867cc2c477269c5945689709780de4bf5444774411b60948b6fbe1ba8999745b",
         "tests/test_aiootp.py": "4e8005967184d4509af032a1bbc60e6628aadadd7ab0904a2071bf22ae93a21a",
         "tests/test_ciphers.py": "5a9b1ebf00f9f0299a0a48748a007fdb366cdef6b173557600095201cba93a69",
         "tests/test_generics.py": "d66dabc9f28c183f57133361ca19b21d11833e2501bc0ef1fcea7efb2ac25a6c",
         "tests/test_high_level_encryption.py": "40ba0baba0b0358b6d472973ac99334ba0b3d78f1d6e9398771f289c7d5e78a0"
     },
     "sha512": {
         ".gitignore": "70970707f1331f017b2b1e4d0a6cd8e33421c1bc34ddfac15899be373a2bfd7f72f69ac46348468182edf91afe8495d300be2e8bda0958eb84abfdda5362537b",
-        "CHANGES.rst": "863d90a1038559778116f8df8a17c160378ebb54ec7986dd6b61e2be75939d478ec821975dda0e84b7ea138139dd0b1e267e9371c64deacc46e280b902c675f7",
+        "CHANGES.rst": "092ca0c01d8602b31c512e1771fb8d8f615dfd41dd1b049985188808ffb2523b303bbab363c905ab3bfe7b4bf1aabcae60ace9d84a4af2ea3572a07b129a2616",
         "LICENSE": "46b675fc02a6f9a6fa17955a0aef2856d796e16d18b5da1fc60df6d87650edf0e91b61c84cb9836cff7bbd981a4f2378c36fe37e0871fa832fbfb76b70109005",
         "MANIFEST.in": "7c8cd20eec083dd7f233b98a990ccdb7b694709cf4831ff6a4350b173cad302c98ca95c48fb4176515a22e9f2c0008bc88c98a49c2a768c4573fe9a07fe0efa7",
         "PREADME.rst": "6166f31d10468ae1b6fa0fdadbae29a9622c67b69cebefa6f4884018a6e59822839bf7fc0b672df123f3550ced0d4166b32c5068024fcd61d401515ebb0a40d3",
-        "README.rst": "943e8b4320cadb9c410029bed25534fcd797681610331191345f3f8eb38edcb853f0cd62a45498d8778dc20c94b0c757dad760bed0af9b3fc3ee1679e97f2f45",
+        "README.rst": "36a10ccf242a346a51a329cb17ebbfdf63266e007535ff343a904db1453fd30acaa178fadb3e8c3ff6cf9b6b6ec6ade0c440cb4448bbdb9764961923d0ef5578",
         "aiootp/__datasets.py": "6ab23aae6bd9a26ff23bb717c6942fd055ec6800aeb5cd082699e76054ea4cfcfcb6c047af636e48d600098f98e132a8100d2ae458badc2e1a1339c7cbd76fae",
-        "aiootp/__init__.py": "f7c70424d37c9b3ad1d490facb1595d4cb03ba68d50dd4b880959a5dbaccd4a2083fc5d5dead6aa3b5182fb0ba736a6576e0f51391f9264b11c6851583d2acc3",
+        "aiootp/__init__.py": "3fbf0fa1d92237564292700b83e700451de1c9f0699f24f460b746030ed34610cbd3c4d7ebef4c749ac9bd2dc7870db06c4a5407eb8a06f9fdf1d1057ee5f8bf",
         "aiootp/__ui_coordination.py": "839eda6ebe96e74a1242c14d301396b4174f5cd42dd55eb161228475c4260b0396f9f5d368313fbba05542fdd4a9fd804524d8ff5de7d3833a662f4d57720e9e",
         "aiootp/asynchs.py": "6ef204217e94bf18494479c7ef307f02fcd8567b3bd2e6a63f74030923df61562701d021d51751a1e23404070b953b1aa783f05ff288ff23d4ce944f12cf15f2",
-        "aiootp/ciphers.py": "20652d292edab197275552d38472cd01d173195e0b6302a252c539f3e215546d82c5ddb273126ac2b803f0c08e11b22a2fa8d1a5c92b7a3ca2a9c60cc5ee4c09",
+        "aiootp/ciphers.py": "e2161381c237bb63bab2137c29716c75e37506eb0d757a4523e4f8a22ea3127e124551c7a482a132e8f0986c466a9a4831053bb5649cc381dfaa99d40ca886a6",
         "aiootp/commons.py": "db4e247ea6cb947555b5eb56a5d767d791de270e0a2925489636e6472393f18bd6b45afb37d8fe26d3dd661841cbaa2805714d6bb7b7da78e4fa453805e9b6eb",
         "aiootp/databases/README_DATABASES.rst": "fd3a882a5cbdf7d03a30eb757bf4c8ff5e9cbf6c89870aced29105603ae1da701fb72c623edcbe43a0b17e79f172035862ff24ad46e68476b8d079428cd17df4",
         "aiootp/debuggers.py": "660ebfcf74322544609acc5b5843a64f637695d8c7770f2b2876fa282c09b56858b2338b60dd6e8dd46e552f8f9cdf0973581c7d86826be9d2abea771058cb97",
-        "aiootp/generics.py": "5394a7fce6ca28a2f1862025c9cc016b211227c876ab16429c4116ec8d5fee86b7f6b5ffa3936b38e7f9183e067a75fc34da9b9b64152342dac3f6a84c2da73f",
+        "aiootp/generics.py": "084a73d9ad789b0ac407e2f6aa55708c2cfc9bfa369e15a2a8aed823a50855053671ff01c35aa21a4f30ea999313d7a690d31ea85038ce89de907513e02f88c6",
         "aiootp/keygens.py": "41aaaf4f947ac6b2783ab9dace640b50f90785d8f0f44a716a496a548596d575495c7223eb6e3fa1a9bc736437d531bbefb2b6e8c0b565c644580257ffc074fd",
         "aiootp/paths.py": "6645822ea830548f269cfe511e88e8741b8d63cb76b9cf70e60561cbaa2cdc7d66ec570ad65b66084b3afab18f57c30d68b5c29cbafdd2bf620d191738a87f47",
-        "aiootp/randoms.py": "ab4c3c1ae855f37932afcc9d646e71ff899d9bb1a21c7e8350337e5f674c4a73538576913705c17c9d8dcca4a017ff14931032523ffb340c5241f9087a0242d5",
+        "aiootp/randoms.py": "b7136ce06d8924a80029c5cdbcbf2b942313d2504bd64ac3799b08df05ccf7a533a60123733ac40a56f862a7ddd061c2eeb35f17bde534efd92c3632b2273683",
         "aiootp/tor/README_TOR.rst": "bb0950ae04248fe3ea66cfe7e4d2bf92e948f8c48b463a773c1968028c6cfeeb78ad0fcad62d14b6e02019a995643c9f6aa698f37b63c253ca44eb4133958563",
         "setup.cfg": "82853df80764bd1ca558dcb9aa6c8be823a4f4eac939a7ddfd086bcde36591243b4cfd682c16307804c35014dbc74a15b6634ca9a8cb9e309b2ef402ee07e7f8",
-        "setup.py": "599ac7c288bfef43c015b5a931d49014db2cbe2cfdb66699d55797d999ef7a1084cfdee868031ef9358062e160b880f348d8905e5bb198de3ddd25a11c6c2c45",
+        "setup.py": "162639c518d0a1000179d95f52ba96ebe2c1eacf958ea4cf65754056b5825a5b7f3aa8e1ad20b469d02ddeb8fb3255ef25970529b31b36a0ce96fd974190d5c2",
         "tests/test_Comprende.py": "30017a34aff432aac9f5b35ad3b28408112ec1e42f48d7fad641828ceee501b0717d992d1f2cf5c451f02759cf0636389024a703d609fa0c724d5c056fe5bfcc",
         "tests/test_Database_AsyncDatabase.py": "aa4a0e3972717d73887698019742b7ed44d175cdddcf2a2371f2c2037762a7009168876c8d0ae60c054207eb5d3c40a9f8192cf67195d51f6ca949a3ff212e99",
         "tests/test_aiootp.py": "b8b46d364508673c51ea6ac8992aa0d439de64980d16e343b8958d06dc12541738731818eb27d56c8c75904c317bd0a5bcf3d238b63ced4a0403edcc210e3f5d",
         "tests/test_ciphers.py": "6f9d9b9e728e4ab5ba9d8c8679c5f01f67f38d95ed23f20e87567ffdadac35ecde959d3446790856d3544faf32d3f9003f4e05ac7d3757eed0d9b9b0d92af9ec",
         "tests/test_generics.py": "62a125a2e0b5ebc2d282249c92aaab1bc312847f2a55c2e64919f6f156068cf66f29db150cc7c9b2fa930573c98e624364078c2b7615f543872f28505aa6a439",
         "tests/test_high_level_encryption.py": "6a80923ef52b0f64206ce125f2fc8a0094e1886fdd8fa515990d936da308965ecbfa6fd6281fc79886aa2870a2e77269ca9b8dd4859403ad5bbdf2d9eed56e0e"
     }
```

