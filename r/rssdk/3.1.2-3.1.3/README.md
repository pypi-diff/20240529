# Comparing `tmp/rssdk-3.1.2.tar.gz` & `tmp/rssdk-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssdk-3.1.2.tar", last modified: Fri Dec 23 12:50:22 2022, max compression
+gzip compressed data, was "rssdk-3.1.3.tar", last modified: Wed May 29 18:27:09 2024, max compression
```

## Comparing `rssdk-3.1.2.tar` & `rssdk-3.1.3.tar`

### file list

```diff
@@ -1,94 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.999998 rssdk-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2022-12-23 12:50:10.000000 rssdk-3.1.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-23 12:50:10.000000 rssdk-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-23 12:50:10.000000 rssdk-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2022-12-23 12:50:21.999998 rssdk-3.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/dio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/dio/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/include/rsdio.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/dio/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/dio/src/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/controllers/abstractdiocontroller.h
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/controllers/ite8783.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/controllers/ite8783.h
--rw-r--r--   0 runner    (1001) docker     (123)    11182 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/controllers/ite8786.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      998 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/controllers/ite8786.h
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/rsdioimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-23 12:50:10.000000 rssdk-3.1.2/dio/src/rsdioimpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/driver/
--rw-r--r--   0 runner    (1001) docker     (123)    44032 2022-12-23 12:50:10.000000 rssdk-3.1.2/driver/drv.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/error/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/error/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2022-12-23 12:50:10.000000 rssdk-3.1.2/error/include/rserrors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/error/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2022-12-23 12:50:10.000000 rssdk-3.1.2/error/src/rserrors.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/extras/python/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/pyrsdio.h
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/pyrspoe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/extras/python/rssdk/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/rssdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2022-12-23 12:50:10.000000 rssdk-3.1.2/extras/python/rssdk.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/extras/python/rssdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2022-12-23 12:50:21.000000 rssdk-3.1.2/extras/python/rssdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-12-23 12:50:21.000000 rssdk-3.1.2/extras/python/rssdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 12:50:21.000000 rssdk-3.1.2/extras/python/rssdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 12:50:21.000000 rssdk-3.1.2/extras/python/rssdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-23 12:50:21.000000 rssdk-3.1.2/extras/python/rssdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.991998 rssdk-3.1.2/poe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/poe/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/include/rspoe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/poe/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/poe/src/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/abstractpoecontroller.h
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/ltc4266.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/ltc4266.h
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/pd69104.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/pd69104.h
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/pd69200.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/controllers/pd69200.h
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/rspoeimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-23 12:50:10.000000 rssdk-3.1.2/poe/src/rspoeimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2022-12-23 12:50:10.000000 rssdk-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 12:50:21.999998 rssdk-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2022-12-23 12:50:10.000000 rssdk-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.995998 rssdk-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/diocontroller.h
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/invalid.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/poecontroller.h
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/test_rsdio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/test_rsdioimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/test_rserrors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/test_rspoe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/test_rspoeimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-23 12:50:10.000000 rssdk-3.1.2/tests/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.999998 rssdk-3.1.2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/argparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/argparse.h
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/i801_smbus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/i801_smbus.h
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/portio.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    70848 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/tinyxml2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    68529 2022-12-23 12:50:10.000000 rssdk-3.1.2/utils/tinyxml2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 12:50:21.999998 rssdk-3.1.2/xml/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/R1000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ars2xxx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs4500.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs7000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs8000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs9000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs92xx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs96xx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecs97xx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecx1000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecx14xx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ecx2000.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/evs1xxx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/evs2xxx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ivh9008.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/ivh9016.xml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/pe3004.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/rcs9xxx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-23 12:50:10.000000 rssdk-3.1.2/xml/spc3xxx.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.635999 rssdk-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-29 18:27:03.000000 rssdk-3.1.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 18:27:03.000000 rssdk-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-29 18:27:03.000000 rssdk-3.1.3/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-29 18:27:03.000000 rssdk-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-29 18:27:09.635999 rssdk-3.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-29 18:27:03.000000 rssdk-3.1.3/cmake/TargetArch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.615999 rssdk-3.1.3/dio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/dio/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/include/rsdio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/dio/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/dio/src/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/controllers/abstractdiocontroller.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/controllers/ite8783.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/controllers/ite8783.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/controllers/ite8786.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/controllers/ite8786.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16598 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/rsdioimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 18:27:03.000000 rssdk-3.1.3/dio/src/rsdioimpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/driver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/driver/x32/
+-rw-r--r--   0 runner    (1001) docker     (127)    64912 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x32/drv.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x32/drv32.sys
+-rw-r--r--   0 runner    (1001) docker     (127)    27520 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x32/drv64.sys
+-rw-r--r--   0 runner    (1001) docker     (127)   107392 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x32/install.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/driver/x64/
+-rw-r--r--   0 runner    (1001) docker     (127)    63872 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x64/drv.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    27520 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x64/drv64.sys
+-rw-r--r--   0 runner    (1001) docker     (127)   129408 2024-05-29 18:27:03.000000 rssdk-3.1.3/driver/x64/install.exe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/error/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/error/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-29 18:27:03.000000 rssdk-3.1.3/error/include/rserrors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/error/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-29 18:27:03.000000 rssdk-3.1.3/error/src/rserrors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/extras/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/extras/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/pyrsdio.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/pyrspoe.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.623999 rssdk-3.1.3/extras/python/rssdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/rssdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-29 18:27:03.000000 rssdk-3.1.3/extras/python/rssdk.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.635999 rssdk-3.1.3/extras/python/rssdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-29 18:27:09.000000 rssdk-3.1.3/extras/python/rssdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-29 18:27:09.000000 rssdk-3.1.3/extras/python/rssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:27:09.000000 rssdk-3.1.3/extras/python/rssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:27:09.000000 rssdk-3.1.3/extras/python/rssdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 18:27:09.000000 rssdk-3.1.3/extras/python/rssdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.619999 rssdk-3.1.3/poe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.627999 rssdk-3.1.3/poe/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/include/rspoe.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.627999 rssdk-3.1.3/poe/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.627999 rssdk-3.1.3/poe/src/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/abstractpoecontroller.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/ltc4266.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/ltc4266.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/pd69104.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/pd69104.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/pd69200.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/controllers/pd69200.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11864 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/rspoeimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 18:27:03.000000 rssdk-3.1.3/poe/src/rspoeimpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 18:27:03.000000 rssdk-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:27:09.635999 rssdk-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-29 18:27:03.000000 rssdk-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.627999 rssdk-3.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/diocontroller.h
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/invalid.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/poecontroller.h
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/test_rsdio.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/test_rsdioimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/test_rserrors.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/test_rspoe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/test_rspoeimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 18:27:03.000000 rssdk-3.1.3/tests/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.631999 rssdk-3.1.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/argparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/argparse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/i801_smbus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/i801_smbus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/portio.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    70848 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/tinyxml2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    68529 2024-05-29 18:27:03.000000 rssdk-3.1.3/utils/tinyxml2.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:27:09.635999 rssdk-3.1.3/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/R1000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ars2xxx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs4500.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs7000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs8000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs9000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs92xx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs96xx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecs97xx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecx1000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecx14xx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecx2000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ecx3000.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/evs1xxx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/evs2xxx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ivh9008.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/ivh9016.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/pe3004.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/rcs9xxx.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-29 18:27:03.000000 rssdk-3.1.3/xml/spc3xxx.xml
```

### Comparing `rssdk-3.1.2/CMakeLists.txt` & `rssdk-3.1.3/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,53 @@
 cmake_minimum_required(VERSION 3.4...3.18)
 
 # TODO: Find a way to make this automatic like setuptools_scm
-project(rssdk VERSION 3.1.2)
+project(rssdk VERSION 3.1.3)
 
+set(CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_VISIBILITY_PRESET hidden)
 set(CMAKE_VISIBILITY_INLINES_HIDDEN 1)
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
 set(CMAKE_DEBUG_POSTFIX "d")
 
 include(GNUInstallDirs)
 option(BUILD_TESTS "Build all test" OFF)
 option(BUILD_UTILITIES "Build command line control utilities" OFF)
 option(INSTALL_UTILITIES "Installs command line control utilities" OFF)
-option(INSTALL_XML "Installs XML files" ON)
 option(INSTALL_SDK "Install SDK files" ON)
 option(BUILD_SHARED_LIBS "Build as shared library" ON)
 option(BUILD_PYTHON_BINDINGS "Build Python bindings" OFF)
 option(INSTALL_PYTHON_BINDINGS "Install Python bindings to current interpreter" OFF)
 
 if (NOT BUILD_UTILITIES AND INSTALL_UTILITIES)
     message(WARNING 
         " INSTALL_UTILITES is ON but BUILD_UTILITIES is OFF.\n"
         " Not building or installing utilities..."
     )
     set(INSTALL_UTILITIES OFF)
 endif()
 
+# Detect target architecture so we can 
+# copy / install the correct driver dll file.
+include(TargetArch)
+target_architecture(TARGET_ARCH)
+
+message(STATUS "Building for ${TARGET_ARCH}")
+
+if ("${TARGET_ARCH}" STREQUAL "x86_64")
+    set(DRIVER_FILE ${CMAKE_CURRENT_SOURCE_DIR}/driver/x64/drv.dll)
+elseif("${TARGET_ARCH}" STREQUAL "i386")
+    set(DRIVER_FILE ${CMAKE_CURRENT_SOURCE_DIR}/driver/x32/drv.dll)
+endif()
+
+
+if (WIN32)
+    message(STATUS "Using ${DRIVER_FILE}")
+endif()
 
 add_library(rserrors 
     error/src/rserrors.cpp
 )
 target_include_directories(
     rserrors PUBLIC "$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/error/include>"
 )
@@ -166,55 +183,44 @@
     )
 endif()
 
 #*********#
 # Install #
 #*********#
 
-include(GNUInstallDirs)
-
 if (INSTALL_SDK)
+    
+    include(GNUInstallDirs)
+
     if (NOT DEFINED rssdk_INSTALL_CMAKEDIR)
         set(rssdk_INSTALL_CMAKEDIR "${CMAKE_INSTALL_LIBDIR}/cmake/rssdk"
             CACHE STRING "Path to rssdk CMake files")
     endif ()
 
-    if (CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT AND UNIX)
-        set (CMAKE_INSTALL_SYSCONFDIR /etc)
-        set (CMAKE_INSTALL_FULL_SYSCONFDIR /etc)
-    endif()
-
     install(TARGETS rserrors rsdio rspoe EXPORT rssdk_Targets
         RUNTIME COMPONENT rssdk_Runtime
         LIBRARY COMPONENT rssdk_Runtime
         NAMELINK_COMPONENT rssdk_Development
         ARCHIVE COMPONENT rssdk_Development
-        INCLUDES DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}"
+        INCLUDES COMPONENT rssdk_Development
     )
     
     install(DIRECTORY 
         "${rssdk_SOURCE_DIR}/error/include/"
         "${rssdk_SOURCE_DIR}/dio/include/"
         "${rssdk_SOURCE_DIR}/poe/include/"
         "${CMAKE_CURRENT_BINARY_DIR}/include/"
         TYPE INCLUDE
     )
 
     if (WIN32)
-        install(FILES "${rssdk_SOURCE_DIR}/driver/drv.dll"
-            TYPE BIN
-        )
+        install(FILES ${DRIVER_FILE} TYPE BIN)
     endif()
 endif()
 
 if(INSTALL_UTILITIES)
     if(MSVC)
         set(CMAKE_INSTALL_SBINDIR bin)
     endif(MSVC)
 
-    install(TARGETS rsdioctl DESTINATION ${CMAKE_INSTALL_SBINDIR})
-    install(TARGETS rspoectl DESTINATION ${CMAKE_INSTALL_SBINDIR})
+    install(TARGETS rsdioctl rspoectl)
 endif(INSTALL_UTILITIES)
-
-if (INSTALL_XML)
-    install(DIRECTORY xml/ DESTINATION ${CMAKE_INSTALL_SYSCONFDIR}/${CMAKE_PROJECT_NAME})
-endif(INSTALL_XML)
```

### Comparing `rssdk-3.1.2/LICENSE` & `rssdk-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/PKG-INFO` & `rssdk-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssdk
-Version: 3.1.2
+Version: 3.1.3
 Summary: Rugged Science SDK Python Bindings
 Author-email: Timothy Lassiter <tim.lassiter@ruggedscience.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE-3RD-PARTY.txt
 
 # Python SDK
 This is a wrapper around the [Rugged Science SDK](https://github.com/RuggedScience/SDK) with the only difference being that exceptions are automatically thrown. There are no `getLastError` or `getLastErrorString` functions.
 
 
 ## Installing
 The package can be installed either by [compiling the sources](#compiling) or installing via `python -m pip install rssdk`.
```

### Comparing `rssdk-3.1.2/dio/include/rsdio.h` & `rssdk-3.1.3/dio/include/rsdio.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/controllers/abstractdiocontroller.h` & `rssdk-3.1.3/dio/src/controllers/abstractdiocontroller.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/controllers/ite8783.cpp` & `rssdk-3.1.3/dio/src/controllers/ite8783.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/controllers/ite8783.h` & `rssdk-3.1.3/dio/src/controllers/ite8783.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/controllers/ite8786.cpp` & `rssdk-3.1.3/dio/src/controllers/ite8786.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/controllers/ite8786.h` & `rssdk-3.1.3/dio/src/controllers/ite8786.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/dio/src/rsdioimpl.cpp` & `rssdk-3.1.3/dio/src/rsdioimpl.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -36,30 +36,32 @@
 
 static tinyxml2::XMLError
 getExternalPinInfo(const tinyxml2::XMLElement *pin, int &pinId, PinConfig &info)
 {
     using namespace tinyxml2;
 
     int id, bit, gpio;
-    bool invert, input, output;
+    bool invert, input, output, pullup = false;
     XMLError e = pin->QueryAttribute("id", &id);
     if (e != XML_SUCCESS) return e;
     e = pin->QueryAttribute("bit", &bit);
     if (e != XML_SUCCESS) return e;
     e = pin->QueryAttribute("gpio", &gpio);
     if (e != XML_SUCCESS) return e;
     e = pin->QueryAttribute("invert", &invert);
     if (e != XML_SUCCESS) return e;
     e = pin->QueryAttribute("input", &input);
     if (e != XML_SUCCESS) return e;
     e = pin->QueryAttribute("output", &output);
     if (e != XML_SUCCESS) return e;
+    e = pin->QueryAttribute("pullup", &pullup);
+    if (e != XML_SUCCESS && e != XML_NO_ATTRIBUTE) return e;
 
     pinId = id;
-    info = PinConfig(bit, gpio, invert, false, input, output);
+    info = PinConfig(bit, gpio, invert, pullup, input, output);
     return XML_SUCCESS;
 }
 
 static tinyxml2::XMLError
 get8786RegData(const tinyxml2::XMLElement *reg, Ite8786::RegisterData &data)
 {
     using namespace tinyxml2;
```

### Comparing `rssdk-3.1.2/dio/src/rsdioimpl.h` & `rssdk-3.1.3/dio/src/rsdioimpl.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/error/include/rserrors.h` & `rssdk-3.1.3/error/include/rserrors.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/error/src/rserrors.cpp` & `rssdk-3.1.3/error/src/rserrors.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/CMakeLists.txt` & `rssdk-3.1.3/extras/python/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -53,35 +53,46 @@
 set(CMAKE_DEBUG_POSTFIX "")
 set(PYBIND11_CPP_STANDARD -std=c++11)
 
 pybind11_add_module(rssdkpy MODULE rssdk.cpp)
 target_link_libraries(rssdkpy PRIVATE rserrors rsdio rspoe)
 set_target_properties(rssdkpy PROPERTIES OUTPUT_NAME "rssdk")
 
+# We need the libs in the same directory on Windows
+# when building as a shared library.
+if (BUILD_SHARED_LIBS AND WIN32)
+  add_custom_command(TARGET rssdkpy POST_BUILD
+    COMMAND ${CMAKE_COMMAND} -E copy "$<TARGET_FILE:rserrors>" "$<TARGET_FILE_DIR:rssdkpy>"
+    COMMAND ${CMAKE_COMMAND} -E copy "$<TARGET_FILE:rsdio>" "$<TARGET_FILE_DIR:rssdkpy>"
+    COMMAND ${CMAKE_COMMAND} -E copy "$<TARGET_FILE:rspoe>" "$<TARGET_FILE_DIR:rssdkpy>"
+    COMMENT "Copying shared libs to Python build folder"
+  )
+endif()
+
 #************#
 # Stub Files #
 # ***********#
 find_program(_STUBGEN_EXISTS stubgen)
 if (_STUBGEN_EXISTS)
   add_custom_command(TARGET rssdkpy POST_BUILD
     COMMAND stubgen -v -p rssdk -o .
     COMMAND ${CMAKE_COMMAND} -E touch py.typed
     WORKING_DIRECTORY "$<TARGET_FILE_DIR:rssdkpy>"
-    COMMENT "Generating Python stub files"
+    COMMENT "Generating Python stub files in Python build folder"
   )
 else()
   message(WARNING 
     " stubgen not found. Stub files will not be generated.\n"
     " To generate stub files install mypy with `python -m pip install mypy`."
   )
 endif()
 
 if (WIN32)
   add_custom_command(TARGET rssdkpy
-    COMMAND ${CMAKE_COMMAND} -E copy ${rssdk_SOURCE_DIR}/driver/drv.dll $<TARGET_FILE_DIR:rssdkpy>
+    COMMAND ${CMAKE_COMMAND} -E copy ${DRIVER_FILE} $<TARGET_FILE_DIR:rssdkpy>
   )
 endif()
 
 #*********#
 # Install #
 #*********#
 if (INSTALL_PYTHON_BINDINGS)
@@ -113,31 +124,35 @@
   file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/METADATA "")
   file(APPEND ${CMAKE_CURRENT_BINARY_DIR}/METADATA "Metadata-Version: 2.1\n")
   file(APPEND ${CMAKE_CURRENT_BINARY_DIR}/METADATA "Name: ${PROJECT_NAME}\n")
   file(APPEND ${CMAKE_CURRENT_BINARY_DIR}/METADATA "Version: ${RSSDKPY_VERSION}\n")
   file(WRITE ${CMAKE_CURRENT_BINARY_DIR}/INSTALLER "cmake\n")
 
   install(TARGETS rssdkpy COMPONENT python DESTINATION "${RSSDKPY_INSTDIR}")
+  # Install the shared libs with the package
+  # on Windows to prevent import error.
+  # On Linux we use RPATH
+  if (BUILD_SHARED_LIBS AND WIN32)
+    install(TARGETS rserrors rsdio rspoe COMPONENT python DESTINATION "${RSSDKPY_INSTDIR}")
+  endif()
+
   install(FILES 
       "${CMAKE_CURRENT_SOURCE_DIR}/rssdk/__init__.py"
       "$<TARGET_FILE_DIR:rssdkpy>/rssdk.pyi"
       "$<TARGET_FILE_DIR:rssdkpy>/py.typed"
     DESTINATION "${RSSDKPY_INSTDIR}"
   )
   
   install(
     FILES "${CMAKE_CURRENT_BINARY_DIR}/METADATA" "${CMAKE_CURRENT_BINARY_DIR}/INSTALLER"
     DESTINATION ${RSSDKPY_METADIR}
   )
 
   if (WIN32)
-    install(
-      FILES "${rssdk_SOURCE_DIR}/driver/drv.dll"
-      DESTINATION ${RSSDKPY_INSTDIR}
-    )
+    install(FILES ${DRIVER_FILE} DESTINATION ${RSSDKPY_INSTDIR})
   endif()
 
   # Install the libraries with the Python package if 
   # they are built as shared libs and not being installed.
   if (BUILD_SHARED_LIBS AND NOT INSTALL_SDK)
     install(
       TARGETS rserrors rsdio rspoe
```

### Comparing `rssdk-3.1.2/extras/python/README.md` & `rssdk-3.1.3/extras/python/README.md`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/pyrsdio.h` & `rssdk-3.1.3/extras/python/pyrsdio.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/pyrspoe.h` & `rssdk-3.1.3/extras/python/pyrspoe.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/rssdk/__init__.py` & `rssdk-3.1.3/extras/python/rssdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/rssdk.cpp` & `rssdk-3.1.3/extras/python/rssdk.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/extras/python/rssdk.egg-info/PKG-INFO` & `rssdk-3.1.3/extras/python/rssdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssdk
-Version: 3.1.2
+Version: 3.1.3
 Summary: Rugged Science SDK Python Bindings
 Author-email: Timothy Lassiter <tim.lassiter@ruggedscience.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE-3RD-PARTY.txt
 
 # Python SDK
 This is a wrapper around the [Rugged Science SDK](https://github.com/RuggedScience/SDK) with the only difference being that exceptions are automatically thrown. There are no `getLastError` or `getLastErrorString` functions.
 
 
 ## Installing
 The package can be installed either by [compiling the sources](#compiling) or installing via `python -m pip install rssdk`.
```

### Comparing `rssdk-3.1.2/extras/python/rssdk.egg-info/SOURCES.txt` & `rssdk-3.1.3/extras/python/rssdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 CMakeLists.txt
 LICENSE
+LICENSE-3RD-PARTY.txt
 MANIFEST.in
 pyproject.toml
 setup.py
+cmake/TargetArch.cmake
 dio/include/rsdio.h
 dio/src/rsdioimpl.cpp
 dio/src/rsdioimpl.h
 dio/src/controllers/abstractdiocontroller.h
 dio/src/controllers/ite8783.cpp
 dio/src/controllers/ite8783.h
 dio/src/controllers/ite8786.cpp
 dio/src/controllers/ite8786.h
-driver/drv.dll
+driver/x32/drv.dll
+driver/x32/drv32.sys
+driver/x32/drv64.sys
+driver/x32/install.exe
+driver/x64/drv.dll
+driver/x64/drv64.sys
+driver/x64/install.exe
 error/include/rserrors.h
 error/src/rserrors.cpp
 extras/python/CMakeLists.txt
 extras/python/README.md
 extras/python/pyrsdio.h
 extras/python/pyrspoe.h
 extras/python/rssdk.cpp
@@ -59,14 +67,15 @@
 xml/ecs9000.xml
 xml/ecs92xx.xml
 xml/ecs96xx.xml
 xml/ecs97xx.xml
 xml/ecx1000.xml
 xml/ecx14xx.xml
 xml/ecx2000.xml
+xml/ecx3000.xml
 xml/evs1xxx.xml
 xml/evs2xxx.xml
 xml/ivh9008.xml
 xml/ivh9016.xml
 xml/pe3004.xml
 xml/rcs9xxx.xml
 xml/spc3xxx.xml
```

### Comparing `rssdk-3.1.2/poe/include/rspoe.h` & `rssdk-3.1.3/poe/include/rspoe.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/abstractpoecontroller.h` & `rssdk-3.1.3/poe/src/controllers/abstractpoecontroller.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/ltc4266.cpp` & `rssdk-3.1.3/poe/src/controllers/ltc4266.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/ltc4266.h` & `rssdk-3.1.3/poe/src/controllers/ltc4266.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/pd69104.cpp` & `rssdk-3.1.3/poe/src/controllers/pd69104.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/pd69104.h` & `rssdk-3.1.3/poe/src/controllers/pd69104.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/pd69200.cpp` & `rssdk-3.1.3/poe/src/controllers/pd69200.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/controllers/pd69200.h` & `rssdk-3.1.3/poe/src/controllers/pd69200.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/rspoeimpl.cpp` & `rssdk-3.1.3/poe/src/rspoeimpl.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/poe/src/rspoeimpl.h` & `rssdk-3.1.3/poe/src/rspoeimpl.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/pyproject.toml` & `rssdk-3.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/setup.py` & `rssdk-3.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,18 +119,14 @@
         subprocess.run(
             ["cmake", ext.sourcedir] + cmake_args, cwd=build_temp, check=True
         )
         subprocess.run(
             ["cmake", "--build", "."] + build_args, cwd=build_temp, check=True
         )
 
-package_data = {"rssdk": ["*.py", "*.pyi", "py.typed"]}
-if os.name == "nt":
-    package_data["rssdk"].append("driver/*.dll")
-
 setup(
     ext_modules=[CMakeExtension(name="rssdk")],
     cmdclass=dict(build_ext=CMakeBuild),
     package_dir={"": "extras/python"},
     packages=["rssdk"],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `rssdk-3.1.2/tests/diocontroller.h` & `rssdk-3.1.3/tests/diocontroller.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/poecontroller.h` & `rssdk-3.1.3/tests/poecontroller.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/test_rsdio.cpp` & `rssdk-3.1.3/tests/test_rsdio.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/test_rsdioimpl.cpp` & `rssdk-3.1.3/tests/test_rsdioimpl.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/test_rserrors.cpp` & `rssdk-3.1.3/tests/test_rserrors.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/test_rspoe.cpp` & `rssdk-3.1.3/tests/test_rspoe.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/test_rspoeimpl.cpp` & `rssdk-3.1.3/tests/test_rspoeimpl.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/tests/utils.h` & `rssdk-3.1.3/tests/utils.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/argparse.cpp` & `rssdk-3.1.3/utils/argparse.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/argparse.h` & `rssdk-3.1.3/utils/argparse.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/i801_smbus.cpp` & `rssdk-3.1.3/utils/i801_smbus.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/portio.hpp` & `rssdk-3.1.3/utils/portio.hpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/tinyxml2.cpp` & `rssdk-3.1.3/utils/tinyxml2.cpp`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/utils/tinyxml2.h` & `rssdk-3.1.3/utils/tinyxml2.h`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/R1000.xml` & `rssdk-3.1.3/xml/R1000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ars2xxx.xml` & `rssdk-3.1.3/xml/ars2xxx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs4500.xml` & `rssdk-3.1.3/xml/ecs4500.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs7000.xml` & `rssdk-3.1.3/xml/ecs7000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs8000.xml` & `rssdk-3.1.3/xml/ecs8000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs9000.xml` & `rssdk-3.1.3/xml/ecs9000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs92xx.xml` & `rssdk-3.1.3/xml/ecs92xx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs96xx.xml` & `rssdk-3.1.3/xml/ecs96xx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecs97xx.xml` & `rssdk-3.1.3/xml/ecs97xx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecx1000.xml` & `rssdk-3.1.3/xml/ecx1000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecx14xx.xml` & `rssdk-3.1.3/xml/ecx14xx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ecx2000.xml` & `rssdk-3.1.3/xml/ecx2000.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/evs1xxx.xml` & `rssdk-3.1.3/xml/evs1xxx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/evs2xxx.xml` & `rssdk-3.1.3/xml/evs2xxx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ivh9008.xml` & `rssdk-3.1.3/xml/ivh9008.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/ivh9016.xml` & `rssdk-3.1.3/xml/ivh9016.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/rcs9xxx.xml` & `rssdk-3.1.3/xml/rcs9xxx.xml`

 * *Files identical despite different names*

### Comparing `rssdk-3.1.2/xml/spc3xxx.xml` & `rssdk-3.1.3/xml/spc3xxx.xml`

 * *Files identical despite different names*

