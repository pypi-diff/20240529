# Comparing `tmp/alex_ber_utils-0.8.1a6.tar.gz` & `tmp/alex_ber_utils-0.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alex_ber_utils-0.8.1a6.tar", last modified: Tue May 28 15:28:08 2024, max compression
+gzip compressed data, was "alex_ber_utils-0.9.0a0.tar", last modified: Tue May 28 19:50:09 2024, max compression
```

## Comparing `alex_ber_utils-0.8.1a6.tar` & `alex_ber_utils-0.9.0a0.tar`

### file list

```diff
@@ -1,99 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.991375 alex_ber_utils-0.8.1a6/
--rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.8.1a6/CHANGELOG.md
--rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 15:28:07.992420 alex_ber_utils-0.8.1a6/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3748 2024-05-28 15:27:17.000000 alex_ber_utils-0.8.1a6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.106124 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    31537 2024-05-28 15:28:05.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2227 2024-05-28 15:28:06.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:28:05.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:28:05.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:23:15.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-28 15:28:05.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 15:28:05.000000 alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.117124 alex_ber_utils-0.8.1a6/alexber/
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.409093 alex_ber_utils-0.8.1a6/alexber/utils/
--rwxrwxrwx   0 root         (0) root         (0)      250 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/_ymlparsers_extra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.429279 alex_ber_utils-0.8.1a6/alexber/utils/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a6/alexber/utils/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/deploys.py
--rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/emails.py
--rwxrwxrwx   0 root         (0) root         (0)     1425 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/enums.py
--rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/fabs.py
--rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/files.py
--rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/importer.py
--rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/init_app_conf.py
--rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/inspects.py
--rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/mains.py
--rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/parsers.py
--rwxrwxrwx   0 root         (0) root         (0)     1676 2024-05-28 11:55:39.000000 alex_ber_utils-0.8.1a6/alexber/utils/pprint.py
--rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/processinvokes.py
--rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/props.py
--rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/setups.py
--rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/stdlogging.py
--rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/thread_locals.py
--rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/uuids.py
--rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/alexber/utils/ymlparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.442381 alex_ber_utils-0.8.1a6/data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.8.1a6/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/req-env.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/req-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/req-md.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-28 15:09:21.000000 alex_ber_utils-0.8.1a6/req-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-28 14:48:40.000000 alex_ber_utils-0.8.1a6/req-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/req-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/req.txt
--rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-28 14:53:19.000000 alex_ber_utils-0.8.1a6/requirements-env.txt
--rwxrwxrwx   0 root         (0) root         (0)      670 2024-05-28 14:53:33.000000 alex_ber_utils-0.8.1a6/requirements-fabric.txt
--rwxrwxrwx   0 root         (0) root         (0)      200 2024-05-28 14:53:45.000000 alex_ber_utils-0.8.1a6/requirements-md.txt
--rwxrwxrwx   0 root         (0) root         (0)      601 2024-05-28 15:10:40.000000 alex_ber_utils-0.8.1a6/requirements-piptools.txt
--rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-28 15:10:10.000000 alex_ber_utils-0.8.1a6/requirements-tests.txt
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-05-28 14:54:21.000000 alex_ber_utils-0.8.1a6/requirements-yml.txt
--rwxrwxrwx   0 root         (0) root         (0)      194 2024-05-28 14:53:06.000000 alex_ber_utils-0.8.1a6/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)      190 2024-05-28 15:28:07.998422 alex_ber_utils-0.8.1a6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4905 2024-05-28 15:27:59.000000 alex_ber_utils-0.8.1a6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.464551 alex_ber_utils-0.8.1a6/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.717902 alex_ber_utils-0.8.1a6/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/deploys_test.py
--rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/emails_test.py
--rwxrwxrwx   0 root         (0) root         (0)    10227 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/enums_mixin_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5067 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/importer_test.py
--rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/init_app_conf_test.py
--rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/inspect_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/mains_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2444 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/method_overloading_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5106 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/parsers_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 15:18:02.000000 alex_ber_utils-0.8.1a6/tests/utils/pprint_test.py
--rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/processinvokes_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/properties_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.755998 alex_ber_utils-0.8.1a6/tests/utils/splitpackage/
--rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/splitpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/splitpackage/mymodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.791203 alex_ber_utils-0.8.1a6/tests/utils/splitpackage_cont/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/splitpackage_cont/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/splitpackage_cont/other_module.py
--rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/threadlocal_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/uuids_test.py
--rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/ymlparsers_extra_test.py
--rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests/utils/ymlparsers_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.806243 alex_ber_utils-0.8.1a6/tests_data/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.819243 alex_ber_utils-0.8.1a6/tests_data/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.883912 alex_ber_utils-0.8.1a6/tests_data/tests/utils/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/config.properties
--rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/config2.properties
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.904306 alex_ber_utils-0.8.1a6/tests_data/tests/utils/initappconf/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/initappconf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.948289 alex_ber_utils-0.8.1a6/tests_data/tests/utils/parser/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/parser/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/parser/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:28:07.977151 alex_ber_utils-0.8.1a6/tests_data/tests/utils/ymlparsers/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.8.1a6/tests_data/tests/utils/ymlparsers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.994408 alex_ber_utils-0.9.0a0/
+-rwxrwxrwx   0 root         (0) root         (0)    26584 2024-05-28 09:24:26.000000 alex_ber_utils-0.9.0a0/CHANGELOG.md
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    31518 2024-05-28 19:50:08.995405 alex_ber_utils-0.9.0a0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3748 2024-05-28 15:27:17.000000 alex_ber_utils-0.9.0a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:07.871845 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    31518 2024-05-28 19:50:06.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2102 2024-05-28 19:50:07.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 19:50:06.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 19:50:06.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 19:50:03.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-28 19:50:06.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-28 19:50:06.000000 alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:07.884925 alex_ber_utils-0.9.0a0/alexber/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.239809 alex_ber_utils-0.9.0a0/alexber/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      148 2024-05-28 19:28:20.000000 alex_ber_utils-0.9.0a0/alexber/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8188 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/_ymlparsers_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.261940 alex_ber_utils-0.9.0a0/alexber/utils/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0a0/alexber/utils/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3928 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/deploys.py
+-rwxrwxrwx   0 root         (0) root         (0)    17354 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/emails.py
+-rwxrwxrwx   0 root         (0) root         (0)     1512 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/fabs.py
+-rwxrwxrwx   0 root         (0) root         (0)      857 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/importer.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/init_app_conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     1385 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/inspects.py
+-rwxrwxrwx   0 root         (0) root         (0)    11144 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/mains.py
+-rwxrwxrwx   0 root         (0) root         (0)     4210 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/parsers.py
+-rwxrwxrwx   0 root         (0) root         (0)     1676 2024-05-28 11:55:39.000000 alex_ber_utils-0.9.0a0/alexber/utils/pprint.py
+-rwxrwxrwx   0 root         (0) root         (0)    10390 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/processinvokes.py
+-rwxrwxrwx   0 root         (0) root         (0)    16921 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/props.py
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/setups.py
+-rwxrwxrwx   0 root         (0) root         (0)     3204 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/stdlogging.py
+-rwxrwxrwx   0 root         (0) root         (0)      658 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/thread_locals.py
+-rwxrwxrwx   0 root         (0) root         (0)     1745 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/uuids.py
+-rwxrwxrwx   0 root         (0) root         (0)    11517 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/alexber/utils/ymlparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.277033 alex_ber_utils-0.9.0a0/data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 11:54:41.000000 alex_ber_utils-0.9.0a0/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/req-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/req-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-28 15:09:21.000000 alex_ber_utils-0.9.0a0/req-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-28 14:48:40.000000 alex_ber_utils-0.9.0a0/req-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/req-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/req.txt
+-rwxrwxrwx   0 root         (0) root         (0)      205 2024-05-28 14:53:19.000000 alex_ber_utils-0.9.0a0/requirements-env.txt
+-rwxrwxrwx   0 root         (0) root         (0)      670 2024-05-28 14:53:33.000000 alex_ber_utils-0.9.0a0/requirements-fabric.txt
+-rwxrwxrwx   0 root         (0) root         (0)      601 2024-05-28 15:10:40.000000 alex_ber_utils-0.9.0a0/requirements-piptools.txt
+-rwxrwxrwx   0 root         (0) root         (0)      663 2024-05-28 15:10:10.000000 alex_ber_utils-0.9.0a0/requirements-tests.txt
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-05-28 14:54:21.000000 alex_ber_utils-0.9.0a0/requirements-yml.txt
+-rwxrwxrwx   0 root         (0) root         (0)      194 2024-05-28 14:53:06.000000 alex_ber_utils-0.9.0a0/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      190 2024-05-28 19:50:09.001407 alex_ber_utils-0.9.0a0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4867 2024-05-28 19:49:43.000000 alex_ber_utils-0.9.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.302284 alex_ber_utils-0.9.0a0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1600 2024-05-28 19:37:45.000000 alex_ber_utils-0.9.0a0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.632169 alex_ber_utils-0.9.0a0/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6071 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/deploys_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     8680 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/emails_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5324 2024-05-28 19:41:58.000000 alex_ber_utils-0.9.0a0/tests/utils/importer_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    30475 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/init_app_conf_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3654 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/inspect_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/mains_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5091 2024-05-28 19:34:14.000000 alex_ber_utils-0.9.0a0/tests/utils/parsers_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2157 2024-05-28 15:18:02.000000 alex_ber_utils-0.9.0a0/tests/utils/pprint_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     5372 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/processinvokes_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2047 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/properties_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.694980 alex_ber_utils-0.9.0a0/tests/utils/splitpackage/
+-rwxrwxrwx   0 root         (0) root         (0)      116 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/splitpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/splitpackage/mymodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.748962 alex_ber_utils-0.9.0a0/tests/utils/splitpackage_cont/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/splitpackage_cont/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/splitpackage_cont/other_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     3914 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/threadlocal_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/uuids_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14847 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/ymlparsers_extra_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    27324 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests/utils/ymlparsers_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.779187 alex_ber_utils-0.9.0a0/tests_data/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.796552 alex_ber_utils-0.9.0a0/tests_data/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.875574 alex_ber_utils-0.9.0a0/tests_data/tests/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      135 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/config.properties
+-rwxrwxrwx   0 root         (0) root         (0)       81 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/config2.properties
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.904172 alex_ber_utils-0.9.0a0/tests_data/tests/utils/initappconf/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/initappconf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.952111 alex_ber_utils-0.9.0a0/tests_data/tests/utils/parser/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/parser/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/parser/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:50:08.978782 alex_ber_utils-0.9.0a0/tests_data/tests/utils/ymlparsers/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-01-28 16:24:44.000000 alex_ber_utils-0.9.0a0/tests_data/tests/utils/ymlparsers/__init__.py
```

### Comparing `alex_ber_utils-0.8.1a6/CHANGELOG.md` & `alex_ber_utils-0.9.0a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/LICENSE.txt` & `alex_ber_utils-0.9.0a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/PKG-INFO` & `alex_ber_utils-0.9.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex_ber_utils
-Version: 0.8.1a6
+Version: 0.9.0a0
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,15 +27,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: md
 Provides-Extra: fabric
 Provides-Extra: yaml
 Provides-Extra: yml
 Provides-Extra: env
 Provides-Extra: tests
 Provides-Extra: piptools
 License-File: LICENSE.txt
```

### Comparing `alex_ber_utils-0.8.1a6/README.md` & `alex_ber_utils-0.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/PKG-INFO` & `alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alex-ber-utils
-Version: 0.8.1a6
+Version: 0.9.0a0
 Summary: AlexBerUtils is collection of the small utilities
 Home-page: https://github.com/alex-ber/AlexBerUtils
 Author: Alexander Berkovich
 License: Apache 2.0
 Keywords: tools tool utils enum enums threadlocal UploadCommand upload uuid1mc uuid UUID UUID1 UUID4 UU1DMC issetdescriptor ismethod importer new_instance safe_eval is_empty parse_boolean Properties java.util.Properties
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -27,15 +27,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: md
 Provides-Extra: fabric
 Provides-Extra: yaml
 Provides-Extra: yml
 Provides-Extra: env
 Provides-Extra: tests
 Provides-Extra: piptools
 License-File: LICENSE.txt
```

### Comparing `alex_ber_utils-0.8.1a6/alex_ber_utils.egg-info/SOURCES.txt` & `alex_ber_utils-0.9.0a0/alex_ber_utils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 req-env.txt
 req-fabric.txt
-req-md.txt
 req-piptools.txt
 req-tests.txt
 req-yml.txt
 req.txt
 requirements-env.txt
 requirements-fabric.txt
-requirements-md.txt
 requirements-piptools.txt
 requirements-tests.txt
 requirements-yml.txt
 requirements.txt
 setup.cfg
 setup.py
 alex_ber_utils.egg-info/PKG-INFO
@@ -26,15 +24,14 @@
 alex_ber_utils.egg-info/requires.txt
 alex_ber_utils.egg-info/top_level.txt
 alexber/__init__.py
 alexber/utils/__init__.py
 alexber/utils/_ymlparsers_extra.py
 alexber/utils/deploys.py
 alexber/utils/emails.py
-alexber/utils/enums.py
 alexber/utils/fabs.py
 alexber/utils/files.py
 alexber/utils/importer.py
 alexber/utils/init_app_conf.py
 alexber/utils/inspects.py
 alexber/utils/mains.py
 alexber/utils/parsers.py
@@ -49,20 +46,18 @@
 alexber/utils/data/__init__.py
 data/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/utils/__init__.py
 tests/utils/deploys_test.py
 tests/utils/emails_test.py
-tests/utils/enums_mixin_test.py
 tests/utils/importer_test.py
 tests/utils/init_app_conf_test.py
 tests/utils/inspect_test.py
 tests/utils/mains_test.py
-tests/utils/method_overloading_test.py
 tests/utils/parsers_test.py
 tests/utils/pprint_test.py
 tests/utils/processinvokes_test.py
 tests/utils/properties_test.py
 tests/utils/threadlocal_test.py
 tests/utils/uuids_test.py
 tests/utils/ymlparsers_extra_test.py
```

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/_ymlparsers_extra.py` & `alex_ber_utils-0.9.0a0/alexber/utils/_ymlparsers_extra.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/deploys.py` & `alex_ber_utils-0.9.0a0/alexber/utils/deploys.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/emails.py` & `alex_ber_utils-0.9.0a0/alexber/utils/emails.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/fabs.py` & `alex_ber_utils-0.9.0a0/alexber/utils/fabs.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/files.py` & `alex_ber_utils-0.9.0a0/alexber/utils/files.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/importer.py` & `alex_ber_utils-0.9.0a0/alexber/utils/importer.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/init_app_conf.py` & `alex_ber_utils-0.9.0a0/alexber/utils/init_app_conf.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/inspects.py` & `alex_ber_utils-0.9.0a0/alexber/utils/inspects.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/mains.py` & `alex_ber_utils-0.9.0a0/alexber/utils/mains.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/parsers.py` & `alex_ber_utils-0.9.0a0/alexber/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/pprint.py` & `alex_ber_utils-0.9.0a0/alexber/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/processinvokes.py` & `alex_ber_utils-0.9.0a0/alexber/utils/processinvokes.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/props.py` & `alex_ber_utils-0.9.0a0/alexber/utils/props.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/setups.py` & `alex_ber_utils-0.9.0a0/alexber/utils/setups.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/stdlogging.py` & `alex_ber_utils-0.9.0a0/alexber/utils/stdlogging.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/thread_locals.py` & `alex_ber_utils-0.9.0a0/alexber/utils/thread_locals.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/uuids.py` & `alex_ber_utils-0.9.0a0/alexber/utils/uuids.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/alexber/utils/ymlparsers.py` & `alex_ber_utils-0.9.0a0/alexber/utils/ymlparsers.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/requirements-fabric.txt` & `alex_ber_utils-0.9.0a0/requirements-fabric.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/requirements-piptools.txt` & `alex_ber_utils-0.9.0a0/requirements-piptools.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/requirements-tests.txt` & `alex_ber_utils-0.9.0a0/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/setup.py` & `alex_ber_utils-0.9.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import setuptools
 from setuptools import setup
 
 
 #VERSION should be defined before importing UploadCommand
-VERSION = '0.8.1a6'
+VERSION = '0.9.0a0'
 from alexber.utils import UploadCommand
 NAME = 'alex_ber_utils'
 SHORT_NAME = 'utils'
 VCS_URL = 'https://github.com/alex-ber/AlexBerUtils'
 DESCRIPTION = 'AlexBerUtils is collection of the small utilities'
 AUTHOR = 'Alexander Berkovich'
 
@@ -21,15 +21,14 @@
         content = f.read().splitlines()
     return content
 
 install_requires = get_content('requirements.txt')
 tests_require = get_content('requirements-tests.txt')
 
 extras = {
-    'md': get_content('req-md.txt'),
     'fabric' : get_content('req-fabric.txt'),
     'yaml' : get_content('req-yml.txt'),
     'yml' : get_content('req-yml.txt'),
     'env' : get_content('req-env.txt'),
     'tests': tests_require,
     'piptools' : get_content('req-env.txt')
 }
```

### Comparing `alex_ber_utils-0.8.1a6/tests/conftest.py` & `alex_ber_utils-0.9.0a0/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,14 @@
 import os
 cwd = os.getcwd()
 if cwd.endswith('AlexBerUtils'):
     os.chdir(os.path.join(cwd, 'data'))
 
 import pytest
 
-ismultidispatchfound = False
-try:
-    # pip install multidispatch==0.2
-    #python3 -m pip install .[md]
-    from multidispatch import multimethod
-    ismultidispatchfound = True
-except ImportError:
-    pass
 
 isyamlrelatedfound = False
 try:
     #python3 -m pip install .[yaml]
     import alexber.utils._ymlparsers_extra as ymlparsers_extra
     if ymlparsers_extra._isHiYaPyCoAvailable and ymlparsers_extra._isJinja2DefaultAvailable:
         isyamlrelatedfound = True
@@ -41,17 +33,14 @@
         if keyword in item.keywords:
             item.add_marker(skip)
 
 
 
 #see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
 def pytest_collection_modifyitems(config, items):
-    if not ismultidispatchfound:
-        skip_tests(items=items, keyword="md", reason="multidispatch is not installed..")
-
     if not isyamlrelatedfound:
         skip_tests(items=items, keyword="yml", reason="yml is not installed..")
 
 #see https://docs.pytest.org/en/latest/mark.html
 #see https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
 def pytest_configure(config):
     config.addinivalue_line(
```

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/deploys_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/deploys_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/emails_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/emails_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/importer_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/importer_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,25 @@
         self = super().__new__(cls)
         return self
 
     def __init__(self, *args, **kwargs):
         pass
 
 
+class PlayerPhilosopher:
+    def __init_subclass__(cls, default_name, **kwargs):
+        super().__init_subclass__(**kwargs)
+        logger.debug(f"Called __init_subclass({cls}, {default_name})")
+        cls.default_name = default_name
+
+
+class PlayerAustralianPhilosopher(PlayerPhilosopher, default_name="Bruce"):
+    pass
+
+
 
 def test_new_instance_arg(request, mocker):
     logger.info(f'{request._pyfuncitem.name}()')
     mock = mocker.spy(PlayerInitArg, '__init__')
 
     input = '.'.join([__name__, PlayerInitArg.__name__])
     first_name = 'John'
@@ -142,16 +153,15 @@
     input = '.'.join([__name__, plcls.__name__])
     player = new_instance(input)
     assert player is not None
 
 
 def test_new_instance_init_subclass(request):
     logger.info(f'{request._pyfuncitem.name}()')
-    module_name, _ = __name__.rsplit(".", 1)
-    input = '.'.join([module_name, 'method_overloading_test', 'PlayerAustralianPhilosopher'])
+    input = '.'.join([__name__, PlayerAustralianPhilosopher.__name__])
 
     player=new_instance(input)
     assert player is not None
 
 
 def test_new_instance_abstract_method(request):
     logger.info(f'{request._pyfuncitem.name}()')
```

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/init_app_conf_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/init_app_conf_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/inspect_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/inspect_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/mains_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/mains_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/parsers_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/parsers_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import enum
 import logging
-
+import enum
+from enum import Enum
 import pytest
 
-from alexber.utils.enums import Enum
+
 from alexber.utils.parsers import ConfigParser, ArgumentParser, safe_eval, is_empty, parse_boolean, parse_sys_args
 
 logger = logging.getLogger(__name__)
 from decimal import Decimal
 from datetime import datetime
 from importlib.resources import path
```

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/pprint_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/pprint_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/processinvokes_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/processinvokes_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/properties_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/properties_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/threadlocal_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/threadlocal_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/uuids_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/uuids_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/ymlparsers_extra_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/ymlparsers_extra_test.py`

 * *Files identical despite different names*

### Comparing `alex_ber_utils-0.8.1a6/tests/utils/ymlparsers_test.py` & `alex_ber_utils-0.9.0a0/tests/utils/ymlparsers_test.py`

 * *Files identical despite different names*

