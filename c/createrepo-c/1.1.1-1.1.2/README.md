# Comparing `tmp/createrepo_c-1.1.1.tar.gz` & `tmp/createrepo_c-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createrepo_c-1.1.1.tar", last modified: Thu May  9 02:06:33 2024, max compression
+gzip compressed data, was "createrepo_c-1.1.2.tar", last modified: Wed May 29 15:20:44 2024, max compression
```

## Comparing `createrepo_c-1.1.1.tar` & `createrepo_c-1.1.2.tar`

### file list

```diff
@@ -1,511 +1,531 @@
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.611901 createrepo_c-1.1.1/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      499 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/AUTHORS
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-12-02 05:51:10.000000 createrepo_c-1.1.1/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)    18092 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/COPYING
--rw-r--r--   0 dalley   (29620) dalley   (29620)      198 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/MANIFEST.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-09 02:06:33.610901 createrepo_c-1.1.1/PKG-INFO
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11449 2023-12-05 06:25:38.000000 createrepo_c-1.1.1/README.md
--rw-r--r--   0 dalley   (29620) dalley   (29620)       54 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/VERSION.cmake
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.519899 createrepo_c-1.1.1/doc/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      637 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)   114986 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/Doxyfile.in.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8915 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/doc/createrepo_c.8
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1523 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/logo.png
--rw-r--r--   0 dalley   (29620) dalley   (29620)    80453 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/logo.xcf
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3476 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/mergerepo_c.8
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2164 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/modifyrepo_c.8
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.520899 createrepo_c-1.1.1/doc/python/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      255 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/python/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8128 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/python/conf.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)      307 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/python/index.rst
--rw-r--r--   0 dalley   (29620) dalley   (29620)      550 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/python/lib.rst
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1772 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/doc/sqliterepo_c.8
--rw-r--r--   0 dalley   (29620) dalley   (29620)      140 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/pyproject.toml
--rw-r--r--   0 dalley   (29620) dalley   (29620)       30 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/requirements-dev.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)       38 2024-05-09 02:06:33.611901 createrepo_c-1.1.1/setup.cfg
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2143 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/setup.py
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.538900 createrepo_c-1.1.1/src/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5252 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8242 2023-10-03 22:00:37.000000 createrepo_c-1.1.1/src/checksum.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3660 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/checksum.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4014 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/cleanup.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    30663 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/src/cmd_parser.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9165 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/cmd_parser.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    61067 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/compression_wrapper.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8271 2024-03-11 23:29:36.000000 createrepo_c-1.1.1/src/compression_wrapper.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1138 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/constants.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)   105052 2024-03-11 23:29:36.000000 createrepo_c-1.1.1/src/createrepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1654 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/createrepo_c.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)      345 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/createrepo_c.pc.cmake
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9307 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/createrepo_shared.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4331 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/createrepo_shared.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27830 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/deltarpms.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/deltarpms.h.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27612 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/dumper_thread.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6182 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/dumper_thread.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3422 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/error.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4018 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/error.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15382 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/helpers.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2751 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/helpers.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11353 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/koji.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3679 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/koji.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    23784 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/src/load_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5524 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/load_metadata.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13005 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/locate_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/locate_metadata.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    85295 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/src/mergerepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2547 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/src/mergerepo_c.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2356 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/src/metadata_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    45291 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/misc.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20338 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/misc.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11612 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/modifyrepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    18914 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/src/modifyrepo_shared.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2240 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/modifyrepo_shared.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8081 2023-10-04 01:08:56.000000 createrepo_c-1.1.1/src/package.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7680 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/package.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1303 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/package_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    26982 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/src/parsehdr.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2020 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/parsehdr.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8518 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/parsepkg.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5467 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/parsepkg.h
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.550900 createrepo_c-1.1.1/src/python/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2730 2023-12-02 01:00:35.000000 createrepo_c-1.1.1/src/python/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1473 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/checksum-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1298 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/checksum-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6450 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/compression_wrapper-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1622 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/compression_wrapper-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6696 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/contentstat-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1104 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/contentstat-py.h
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.550900 createrepo_c-1.1.1/src/python/createrepo_c/
--rw-r--r--   0 dalley   (29620) dalley   (29620)    29175 2024-03-11 23:53:11.000000 createrepo_c-1.1.1/src/python/createrepo_c/__init__.py
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.551900 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20682 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)        1 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)      180 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/src/python/createrepo_c.egg-info/top_level.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)    12098 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/python/createrepo_cmodule.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2517 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/exception-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1307 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/exception-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10077 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/load_metadata-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1043 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/load_metadata-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7280 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/locate_metadata-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1143 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/locate_metadata-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2573 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/misc-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1495 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/misc-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    19974 2023-10-03 22:10:33.000000 createrepo_c-1.1.1/src/python/package-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1242 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/package-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4047 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/python/parsepkg-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1444 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/python/parsepkg-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13961 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/repomd-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1069 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/repomd-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13674 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/python/repomdrecord-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/repomdrecord-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5675 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/sqlite-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/sqlite-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7844 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/python/typeconversion.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1849 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/typeconversion.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10308 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollection-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1216 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollection-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7595 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollectionmodule-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1270 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollectionmodule-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8365 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollectionpackage-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1279 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatecollectionpackage-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7867 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updateinfo-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1097 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updateinfo-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15281 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updaterecord-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updaterecord-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6257 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatereference-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1195 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/updatereference-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4938 2023-10-04 01:00:01.000000 createrepo_c-1.1.1/src/python/xml_dump-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2121 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/python/xml_dump-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7503 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/xml_file-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1030 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/python/xml_file-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27454 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/python/xml_parser-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3318 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/python/xml_parser-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    36316 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11634 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/repomd.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1359 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/repomd_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    48204 2023-12-02 05:51:10.000000 createrepo_c-1.1.1/src/sqlite.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5768 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/sqlite.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    34375 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/sqliterepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5190 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/threads.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5854 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/threads.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9476 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/updateinfo.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5407 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/updateinfo.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1312 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/src/version.h.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)    16489 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/src/xml_dump.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7618 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4545 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_deltapackage.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3911 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_filelists.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3145 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4414 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_other.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    12665 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_primary.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8750 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9530 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/src/xml_dump_updateinfo.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15944 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/src/xml_file.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10285 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/xml_file.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9177 2023-12-05 06:25:07.000000 createrepo_c-1.1.1/src/xml_parser.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13838 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/src/xml_parser.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14997 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/xml_parser_filelists.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9269 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/src/xml_parser_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    17385 2023-12-05 06:25:07.000000 createrepo_c-1.1.1/src/xml_parser_main_metadata_together.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13200 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/xml_parser_other.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27752 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/xml_parser_primary.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14399 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/xml_parser_repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20016 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/src/xml_parser_updateinfo.c
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.555900 createrepo_c-1.1.1/tests/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2887 2023-10-15 20:58:41.000000 createrepo_c-1.1.1/tests/CMakeLists.txt
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.566900 createrepo_c-1.1.1/tests/createrepo/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5252 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8242 2023-10-03 22:00:37.000000 createrepo_c-1.1.1/tests/createrepo/checksum.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3660 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/checksum.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4014 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/cleanup.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    30663 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/tests/createrepo/cmd_parser.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9165 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/cmd_parser.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    61067 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/compression_wrapper.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8271 2024-03-11 23:29:36.000000 createrepo_c-1.1.1/tests/createrepo/compression_wrapper.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1138 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/constants.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)   105052 2024-03-11 23:29:36.000000 createrepo_c-1.1.1/tests/createrepo/createrepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1654 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/createrepo_c.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)      345 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/createrepo_c.pc.cmake
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9307 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/createrepo_shared.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4331 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/createrepo_shared.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27830 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/deltarpms.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/deltarpms.h.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27612 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/dumper_thread.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6182 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/dumper_thread.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3422 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/error.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4018 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/error.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15382 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/helpers.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2751 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/helpers.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11353 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/koji.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3679 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/koji.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    23784 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/tests/createrepo/load_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5524 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/load_metadata.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13005 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/locate_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/locate_metadata.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    85295 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/tests/createrepo/mergerepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2547 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/tests/createrepo/mergerepo_c.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2356 2024-02-06 04:49:47.000000 createrepo_c-1.1.1/tests/createrepo/metadata_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    45291 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/misc.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20338 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/misc.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11612 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/modifyrepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    18914 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/tests/createrepo/modifyrepo_shared.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2240 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/modifyrepo_shared.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8081 2023-10-04 01:08:56.000000 createrepo_c-1.1.1/tests/createrepo/package.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7680 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/package.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1303 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/package_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    26982 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/createrepo/parsehdr.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2020 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/parsehdr.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8518 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/parsepkg.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5467 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/parsepkg.h
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.572900 createrepo_c-1.1.1/tests/createrepo/python/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2730 2023-12-02 01:00:35.000000 createrepo_c-1.1.1/tests/createrepo/python/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1473 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/checksum-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1298 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/checksum-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6450 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/compression_wrapper-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1622 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/compression_wrapper-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6696 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/contentstat-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1104 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/contentstat-py.h
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.572900 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c/
--rw-r--r--   0 dalley   (29620) dalley   (29620)    29175 2024-03-11 23:53:11.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c/__init__.py
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.573900 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20682 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)        1 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)      180 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2024-05-09 02:06:33.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)    12098 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/python/createrepo_cmodule.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2517 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/exception-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1307 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/exception-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10077 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/load_metadata-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1043 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/load_metadata-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7280 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/locate_metadata-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1143 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/locate_metadata-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2573 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/misc-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1495 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/misc-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    19974 2023-10-03 22:10:33.000000 createrepo_c-1.1.1/tests/createrepo/python/package-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1242 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/package-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4047 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/python/parsepkg-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1444 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/python/parsepkg-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13961 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/repomd-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1069 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/repomd-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13674 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/python/repomdrecord-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/repomdrecord-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5675 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/sqlite-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/sqlite-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7844 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/python/typeconversion.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1849 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/typeconversion.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10308 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollection-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1216 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollection-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7595 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollectionmodule-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1270 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollectionmodule-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8365 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollectionpackage-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1279 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatecollectionpackage-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7867 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updateinfo-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1097 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updateinfo-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15281 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updaterecord-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updaterecord-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6257 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatereference-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1195 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/updatereference-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4938 2023-10-04 01:00:01.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_dump-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2121 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_dump-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7503 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_file-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1030 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_file-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27454 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_parser-py.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3318 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/python/xml_parser-py.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    36316 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11634 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/repomd.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1359 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/repomd_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    48204 2023-12-02 05:51:10.000000 createrepo_c-1.1.1/tests/createrepo/sqlite.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5768 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/sqlite.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    34375 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/sqliterepo_c.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5190 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/threads.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5854 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/threads.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9476 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/updateinfo.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5407 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/updateinfo.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1312 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/createrepo/version.h.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)    16489 2024-03-11 02:55:15.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7618 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4545 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_deltapackage.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3911 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_filelists.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3145 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4414 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_other.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    12665 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_primary.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8750 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9530 2023-12-02 01:08:50.000000 createrepo_c-1.1.1/tests/createrepo/xml_dump_updateinfo.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15944 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/createrepo/xml_file.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10285 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/xml_file.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9177 2023-12-05 06:25:07.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13838 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14997 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_filelists.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9269 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_internal.h
--rw-r--r--   0 dalley   (29620) dalley   (29620)    17385 2023-12-05 06:25:07.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_main_metadata_together.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13200 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_other.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    27752 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_primary.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14399 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    20016 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/createrepo/xml_parser_updateinfo.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11645 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/fixtures.h
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.573900 createrepo_c-1.1.1/tests/python/
--rw-r--r--   0 dalley   (29620) dalley   (29620)       25 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/CMakeLists.txt
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.578900 createrepo_c-1.1.1/tests/python/tests/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      167 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/CMakeLists.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/__init__.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     9182 2024-03-11 23:29:36.000000 createrepo_c-1.1.1/tests/python/tests/fixtures.py
--rwxr-xr-x   0 dalley   (29620) dalley   (29620)      199 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/run_unittests.sh.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1212 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_checksum.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3564 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/python/tests/test_compression_wrapper.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2514 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/python/tests/test_contentstat.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4166 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_crfile.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3414 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/python/tests/test_load_metadata.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4235 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_locate_metadata.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3223 2024-03-11 23:52:26.000000 createrepo_c-1.1.1/tests/python/tests/test_misc.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10996 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/python/tests/test_package.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2433 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/python/tests/test_parsepkg.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4875 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_repomd.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7982 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/python/tests/test_repomdrecord.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11194 2024-03-11 23:37:22.000000 createrepo_c-1.1.1/tests/python/tests/test_repository.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10668 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/python/tests/test_sqlite.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3063 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updatecollection.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)      938 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updatecollectionmodule.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1760 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updatecollectionpackage.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    13055 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updateinfo.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6315 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updaterecord.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)      710 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_updatereference.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)      317 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/python/tests/test_version.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14747 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/python/tests/test_xml_file.py
--rw-r--r--   0 dalley   (29620) dalley   (29620)    56717 2023-10-03 22:10:33.000000 createrepo_c-1.1.1/tests/python/tests/test_xml_parser.py
--rwxr-xr-x   0 dalley   (29620) dalley   (29620)      688 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/run_tests.sh.in
--rw-r--r--   0 dalley   (29620) dalley   (29620)     5518 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/test_checksum.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    32047 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_compression_wrapper.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    14240 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_koji.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8130 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_load_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10128 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_locate_metadata.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    43471 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_misc.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4673 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_modifyrepo_shared.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     6327 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_sqlite.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4116 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_xml_dump.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    15388 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_xml_dump_primary.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4565 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/test_xml_file.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    17435 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_xml_parser_filelists.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    11263 2023-11-08 04:13:24.000000 createrepo_c-1.1.1/tests/test_xml_parser_main_metadata_together.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4156 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/test_xml_parser_repomd.c
--rw-r--r--   0 dalley   (29620) dalley   (29620)    10261 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/test_xml_parser_updateinfo.c
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.515899 createrepo_c-1.1.1/tests/testdata/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.584900 createrepo_c-1.1.1/tests/testdata/compressed_files/
--rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo0
--rw-r--r--   0 dalley   (29620) dalley   (29620)       33 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo1
--rw-r--r--   0 dalley   (29620) dalley   (29620)       14 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo2
--rw-r--r--   0 dalley   (29620) dalley   (29620)       32 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo3
--rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo4
--rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.foo5
--rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)       14 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)       33 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)       32 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt.xz
--rw-r--r--   0 dalley   (29620) dalley   (29620)       95 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/00_plain.txt.zst
--rw-r--r--   0 dalley   (29620) dalley   (29620)       56 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo0
--rw-r--r--   0 dalley   (29620) dalley   (29620)       64 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo1
--rw-r--r--   0 dalley   (29620) dalley   (29620)       69 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo2
--rw-r--r--   0 dalley   (29620) dalley   (29620)       96 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo3
--rw-r--r--   0 dalley   (29620) dalley   (29620)      169 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo4
--rw-r--r--   0 dalley   (29620) dalley   (29620)       51 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.foo5
--rw-r--r--   0 dalley   (29620) dalley   (29620)       56 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt
--rw-r--r--   0 dalley   (29620) dalley   (29620)       69 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)       64 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)       96 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt.xz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      158 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)       51 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/compressed_files/01_plain.txt.zst
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.584900 createrepo_c-1.1.1/tests/testdata/comps_files/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      638 2024-01-04 19:12:42.000000 createrepo_c-1.1.1/tests/testdata/comps_files/comps_00.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.589901 createrepo_c-1.1.1/tests/testdata/modified_repo_files/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      633 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      570 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      802 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3174 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)    68135 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/long_primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1528 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/missing_type-repomd.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      764 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      985 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3588 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      510 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      767 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/no_pkgid-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      405 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      551 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2239 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      598 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      608 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      840 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3277 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      606 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      838 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3353 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      657 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      889 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-other.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3342 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1277 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.590901 createrepo_c-1.1.1/tests/testdata/other_metadata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      894 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2364 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      760 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      804 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2364 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/other_metadata/comps-f19.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.592901 createrepo_c-1.1.1/tests/testdata/packages/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     7737 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3096 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1717 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1741 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1789 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1488 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/empty-0-0.src.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1401 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/empty-0-0.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2237 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2845 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_00/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.594900 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      134 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      262 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      269 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3381 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_00/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_01/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.595901 createrepo_c-1.1.1/tests/testdata/repo_01/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      783 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      332 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      273 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1497 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_01/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_02/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.596901 createrepo_c-1.1.1/tests/testdata/repo_02/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      341 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      403 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      973 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1497 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_02/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_03/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.598901 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      134 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      262 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1044 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      269 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3838 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_03/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_04/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.599901 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      987 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      397 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      429 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      336 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2012 2023-10-03 22:18:31.000000 createrepo_c-1.1.1/tests/testdata/repo_04/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_koji_01/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.600901 createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      816 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1007 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      487 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1549 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_koji_02/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.601901 createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      338 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      913 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      687 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1547 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.514899 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.605901 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      656 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)     2366 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3775 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)      864 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      864 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      932 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1287 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1519 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)    88281 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      533 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1301 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
--rw-r--r--   0 dalley   (29620) dalley   (29620)      749 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      850 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)    86680 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1482 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
--rw-r--r--   0 dalley   (29620) dalley   (29620)      748 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      687 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     8640 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.515899 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.605901 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      341 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      405 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1017 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1354 2023-10-03 20:21:34.000000 createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.607901 createrepo_c-1.1.1/tests/testdata/repodata_snippets/
--rw-r--r--   0 dalley   (29620) dalley   (29620)      436 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      745 2023-10-03 22:03:10.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/filelists_snippet_01.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      471 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/filelists_snippet_02.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      408 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/other_snippet_01.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      697 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/other_snippet_02.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1918 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/primary_snippet_01.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     3085 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/repodata_snippets/primary_snippet_02.xml
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.608901 createrepo_c-1.1.1/tests/testdata/specs/
--rwxr-xr-x   0 dalley   (29620) dalley   (29620)       67 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/build.sh
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1428 2024-05-07 02:44:46.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-Archer.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-Rimmer.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)      571 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-iso88591.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)      594 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-iso88592.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)      653 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-utf8.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)      176 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-empty.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)      632 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-fake_bash.spec
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1236 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/specs/fake-super_kernel.spec
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.609901 createrepo_c-1.1.1/tests/testdata/test_files/
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1523 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/binary_file
--rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/empty_file
--rw-r--r--   0 dalley   (29620) dalley   (29620)    24576 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/sqlite_file.sqlite
--rw-r--r--   0 dalley   (29620) dalley   (29620)      910 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/text_file
--rw-r--r--   0 dalley   (29620) dalley   (29620)      522 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/text_file.gz
--rw-r--r--   0 dalley   (29620) dalley   (29620)      628 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/test_files/text_file.xz
-drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-09 02:06:33.610901 createrepo_c-1.1.1/tests/testdata/updateinfo_files/
--rw-r--r--   0 dalley   (29620) dalley   (29620)       60 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_00.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)     1222 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_01.xml
--rw-r--r--   0 dalley   (29620) dalley   (29620)      188 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
--rw-r--r--   0 dalley   (29620) dalley   (29620)     4805 2023-03-21 04:57:44.000000 createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_03.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.880885 createrepo_c-1.1.2/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      499 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/AUTHORS
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-12-02 05:51:10.000000 createrepo_c-1.1.2/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    18092 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/COPYING
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      198 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/MANIFEST.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-29 15:20:44.880885 createrepo_c-1.1.2/PKG-INFO
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11449 2023-12-05 06:25:38.000000 createrepo_c-1.1.2/README.md
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       54 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/VERSION.cmake
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.829884 createrepo_c-1.1.2/_skbuild/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.830884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.830884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.830884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.830884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.833884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    29121 2024-05-10 20:52:50.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/__init__.py
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)   358592 2024-05-10 20:47:41.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/_createrepo_c.so
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.830884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.836884 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)   264384 2024-05-10 20:47:41.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/createrepo_c
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)   230752 2024-05-10 20:47:40.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/mergerepo_c
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)   143448 2024-05-10 20:47:40.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/modifyrepo_c
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)   189072 2024-05-10 20:47:40.000000 createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/sqliterepo_c
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.838884 createrepo_c-1.1.2/doc/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      637 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)   114986 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/Doxyfile.in.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8934 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/doc/createrepo_c.8
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1523 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/logo.png
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    80453 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/logo.xcf
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3476 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/mergerepo_c.8
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2164 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/modifyrepo_c.8
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.838884 createrepo_c-1.1.2/doc/python/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      255 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/python/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8128 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/python/conf.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      307 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/python/index.rst
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      550 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/python/lib.rst
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1772 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/doc/sqliterepo_c.8
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      140 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/pyproject.toml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       30 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/requirements-dev.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       38 2024-05-29 15:20:44.880885 createrepo_c-1.1.2/setup.cfg
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2143 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/setup.py
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.845884 createrepo_c-1.1.2/src/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5252 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8242 2023-10-03 22:00:37.000000 createrepo_c-1.1.2/src/checksum.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3660 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/checksum.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4014 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/cleanup.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    30682 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/src/cmd_parser.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9165 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/cmd_parser.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    61067 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/compression_wrapper.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8271 2024-03-11 23:29:36.000000 createrepo_c-1.1.2/src/compression_wrapper.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1138 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/constants.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)   105052 2024-03-11 23:29:36.000000 createrepo_c-1.1.2/src/createrepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1654 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/createrepo_c.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      414 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/src/createrepo_c.pc
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      345 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/createrepo_c.pc.cmake
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9307 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/createrepo_shared.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4331 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/createrepo_shared.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27830 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/deltarpms.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/src/deltarpms.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/deltarpms.h.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27612 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/dumper_thread.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6182 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/dumper_thread.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3422 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/error.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4018 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/error.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15382 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/helpers.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2751 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/helpers.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11353 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/koji.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3679 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/koji.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    23784 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/src/load_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5524 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/load_metadata.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13005 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/locate_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/locate_metadata.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    85295 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/src/mergerepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2547 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/src/mergerepo_c.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2356 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/src/metadata_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    45291 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/misc.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    20338 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/misc.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11612 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/modifyrepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    18914 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/src/modifyrepo_shared.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2240 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/modifyrepo_shared.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8081 2023-10-04 01:08:56.000000 createrepo_c-1.1.2/src/package.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7680 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/package.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1303 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/package_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    26982 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/src/parsehdr.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2020 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/parsehdr.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8518 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/parsepkg.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5467 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/parsepkg.h
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.849884 createrepo_c-1.1.2/src/python/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2730 2023-12-02 01:00:35.000000 createrepo_c-1.1.2/src/python/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1473 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/checksum-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1298 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/checksum-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6450 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/compression_wrapper-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1622 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/compression_wrapper-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6696 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/contentstat-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1104 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/contentstat-py.h
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.849884 createrepo_c-1.1.2/src/python/createrepo_c/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    29121 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/src/python/createrepo_c/__init__.py
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.850885 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    21321 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        1 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      180 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/src/python/createrepo_c.egg-info/top_level.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    12098 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/python/createrepo_cmodule.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2517 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/exception-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1307 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/exception-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10077 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/load_metadata-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1043 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/load_metadata-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7280 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/locate_metadata-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1143 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/locate_metadata-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2573 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/misc-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1495 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/misc-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    19974 2023-10-03 22:10:33.000000 createrepo_c-1.1.2/src/python/package-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1242 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/package-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4047 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/python/parsepkg-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1444 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/python/parsepkg-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13961 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/repomd-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1069 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/repomd-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13674 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/python/repomdrecord-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/repomdrecord-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5675 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/sqlite-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/sqlite-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7844 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/python/typeconversion.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1849 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/typeconversion.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10308 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollection-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1216 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollection-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7595 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollectionmodule-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1270 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollectionmodule-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8365 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollectionpackage-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1279 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatecollectionpackage-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7867 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updateinfo-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1097 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updateinfo-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15281 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updaterecord-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updaterecord-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6257 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatereference-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1195 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/updatereference-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4938 2023-10-04 01:00:01.000000 createrepo_c-1.1.2/src/python/xml_dump-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2121 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/python/xml_dump-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7503 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/xml_file-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1030 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/python/xml_file-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27454 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/python/xml_parser-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3318 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/python/xml_parser-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    36316 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11634 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/repomd.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1359 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/repomd_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    48204 2023-12-02 05:51:10.000000 createrepo_c-1.1.2/src/sqlite.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5768 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/sqlite.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    34375 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/sqliterepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5190 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/threads.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5854 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/threads.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9476 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/updateinfo.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5407 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/updateinfo.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1285 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/src/version.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1312 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/src/version.h.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    16489 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/src/xml_dump.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7618 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4545 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_deltapackage.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3911 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_filelists.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3145 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4414 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_other.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    12665 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_primary.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8750 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9530 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/src/xml_dump_updateinfo.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15944 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/src/xml_file.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10285 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/xml_file.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9177 2023-12-05 06:25:07.000000 createrepo_c-1.1.2/src/xml_parser.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13838 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/src/xml_parser.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14997 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/xml_parser_filelists.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9269 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/src/xml_parser_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    17385 2023-12-05 06:25:07.000000 createrepo_c-1.1.2/src/xml_parser_main_metadata_together.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13200 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/xml_parser_other.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27752 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/xml_parser_primary.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14399 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/xml_parser_repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    20016 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/src/xml_parser_updateinfo.c
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.851884 createrepo_c-1.1.2/tests/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2887 2023-10-15 20:58:41.000000 createrepo_c-1.1.2/tests/CMakeLists.txt
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.858885 createrepo_c-1.1.2/tests/createrepo/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5252 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8242 2023-10-03 22:00:37.000000 createrepo_c-1.1.2/tests/createrepo/checksum.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3660 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/checksum.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4014 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/cleanup.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    30682 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/tests/createrepo/cmd_parser.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9165 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/cmd_parser.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    61067 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/compression_wrapper.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8271 2024-03-11 23:29:36.000000 createrepo_c-1.1.2/tests/createrepo/compression_wrapper.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1138 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/constants.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)   105052 2024-03-11 23:29:36.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1654 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_c.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      414 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_c.pc
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      345 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_c.pc.cmake
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9307 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_shared.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4331 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/createrepo_shared.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27830 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/deltarpms.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/tests/createrepo/deltarpms.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3729 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/deltarpms.h.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27612 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/dumper_thread.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6182 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/dumper_thread.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3422 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/error.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4018 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/error.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15382 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/helpers.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2751 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/helpers.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11353 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/koji.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3679 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/koji.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    23784 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/tests/createrepo/load_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5524 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/load_metadata.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13005 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/locate_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5817 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/locate_metadata.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    85295 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/tests/createrepo/mergerepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2547 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/tests/createrepo/mergerepo_c.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2356 2024-02-06 04:49:47.000000 createrepo_c-1.1.2/tests/createrepo/metadata_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    45291 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/misc.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    20338 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/misc.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11612 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/modifyrepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    18914 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/tests/createrepo/modifyrepo_shared.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2240 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/modifyrepo_shared.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8081 2023-10-04 01:08:56.000000 createrepo_c-1.1.2/tests/createrepo/package.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7680 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/package.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1303 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/package_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    26982 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/createrepo/parsehdr.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2020 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/parsehdr.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8518 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/parsepkg.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5467 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/parsepkg.h
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.862885 createrepo_c-1.1.2/tests/createrepo/python/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2730 2023-12-02 01:00:35.000000 createrepo_c-1.1.2/tests/createrepo/python/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1473 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/checksum-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1298 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/checksum-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6450 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/compression_wrapper-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1622 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/compression_wrapper-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6696 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/contentstat-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1104 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/contentstat-py.h
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.862885 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    29121 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c/__init__.py
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.862885 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      886 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    21321 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        1 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      180 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2024-05-29 15:20:44.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    12098 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/python/createrepo_cmodule.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2517 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/exception-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1307 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/exception-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10077 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/load_metadata-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1043 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/load_metadata-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7280 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/locate_metadata-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1143 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/locate_metadata-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2573 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/misc-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1495 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/misc-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    19974 2023-10-03 22:10:33.000000 createrepo_c-1.1.2/tests/createrepo/python/package-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1242 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/package-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4047 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/python/parsepkg-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1444 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/python/parsepkg-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13961 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/repomd-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1069 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/repomd-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13674 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/python/repomdrecord-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/repomdrecord-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5675 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/sqlite-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/sqlite-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7844 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/python/typeconversion.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1849 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/typeconversion.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10308 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollection-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1216 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollection-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7595 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollectionmodule-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1270 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollectionmodule-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8365 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollectionpackage-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1279 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatecollectionpackage-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7867 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updateinfo-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1097 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updateinfo-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15281 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updaterecord-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1168 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updaterecord-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6257 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatereference-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1195 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/updatereference-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4938 2023-10-04 01:00:01.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_dump-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2121 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_dump-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7503 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_file-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1030 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_file-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27454 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_parser-py.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3318 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/python/xml_parser-py.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    36316 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11634 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/repomd.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1359 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/repomd_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    48204 2023-12-02 05:51:10.000000 createrepo_c-1.1.2/tests/createrepo/sqlite.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5768 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/sqlite.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    34375 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/sqliterepo_c.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5190 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/threads.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5854 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/threads.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9476 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/updateinfo.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5407 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/updateinfo.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1285 2024-05-10 20:47:36.000000 createrepo_c-1.1.2/tests/createrepo/version.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1312 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/createrepo/version.h.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    16489 2024-03-11 02:55:15.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7618 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4545 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_deltapackage.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3911 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_filelists.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3145 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4414 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_other.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    12665 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_primary.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8750 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9530 2023-12-02 01:08:50.000000 createrepo_c-1.1.2/tests/createrepo/xml_dump_updateinfo.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15944 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/createrepo/xml_file.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10285 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/xml_file.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9177 2023-12-05 06:25:07.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13838 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14997 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_filelists.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9269 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_internal.h
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    17385 2023-12-05 06:25:07.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_main_metadata_together.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13200 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_other.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    27752 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_primary.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14399 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    20016 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/createrepo/xml_parser_updateinfo.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11645 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/fixtures.h
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.863885 createrepo_c-1.1.2/tests/python/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       25 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/CMakeLists.txt
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.865885 createrepo_c-1.1.2/tests/python/tests/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      167 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/CMakeLists.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/__init__.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     9182 2024-03-11 23:29:36.000000 createrepo_c-1.1.2/tests/python/tests/fixtures.py
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)      199 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/run_unittests.sh.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1212 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_checksum.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3564 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/python/tests/test_compression_wrapper.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2514 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/python/tests/test_contentstat.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4166 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_crfile.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3414 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/python/tests/test_load_metadata.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4235 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_locate_metadata.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3223 2024-03-11 23:52:26.000000 createrepo_c-1.1.2/tests/python/tests/test_misc.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10996 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/python/tests/test_package.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2433 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/python/tests/test_parsepkg.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4875 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_repomd.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7982 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/python/tests/test_repomdrecord.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    12475 2024-05-29 15:19:40.000000 createrepo_c-1.1.2/tests/python/tests/test_repository.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10668 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/python/tests/test_sqlite.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3063 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updatecollection.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      938 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updatecollectionmodule.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1760 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updatecollectionpackage.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    13055 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updateinfo.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6315 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updaterecord.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      710 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_updatereference.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      317 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/python/tests/test_version.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14747 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/python/tests/test_xml_file.py
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    56717 2023-10-03 22:10:33.000000 createrepo_c-1.1.2/tests/python/tests/test_xml_parser.py
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)      688 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/run_tests.sh.in
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     5518 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/test_checksum.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    32047 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_compression_wrapper.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    14240 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_koji.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8130 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_load_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10128 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_locate_metadata.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    43471 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_misc.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4673 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_modifyrepo_shared.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     6327 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_sqlite.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4116 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_xml_dump.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    15388 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_xml_dump_primary.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4565 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/test_xml_file.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    17435 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_xml_parser_filelists.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    11263 2023-11-08 04:13:24.000000 createrepo_c-1.1.2/tests/test_xml_parser_main_metadata_together.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4156 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/test_xml_parser_repomd.c
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    10261 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/test_xml_parser_updateinfo.c
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.832884 createrepo_c-1.1.2/tests/testdata/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.867885 createrepo_c-1.1.2/tests/testdata/compressed_files/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo0
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       33 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo1
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       14 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       32 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo3
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo4
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.foo5
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       14 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       33 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       32 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt.xz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       95 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       13 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/00_plain.txt.zst
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       56 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo0
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       64 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo1
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       69 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       96 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo3
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      169 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo4
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       51 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.foo5
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       56 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       69 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       64 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       96 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt.xz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      158 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       51 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/compressed_files/01_plain.txt.zst
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.867885 createrepo_c-1.1.2/tests/testdata/comps_files/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      638 2024-01-04 19:12:42.000000 createrepo_c-1.1.2/tests/testdata/comps_files/comps_00.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.869885 createrepo_c-1.1.2/tests/testdata/modified_repo_files/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      633 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      570 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      802 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3174 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    68135 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/long_primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1528 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/missing_type-repomd.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      764 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      985 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3588 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      510 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      767 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/no_pkgid-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      405 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      551 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2239 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      598 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      608 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      840 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3277 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      606 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      838 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3353 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      657 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      889 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-other.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3342 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1277 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.870885 createrepo_c-1.1.2/tests/testdata/other_metadata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      894 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2364 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      760 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      804 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2364 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/other_metadata/comps-f19.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.871885 createrepo_c-1.1.2/tests/testdata/packages/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     7737 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3096 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1717 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1741 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1789 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1488 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/empty-0-0.src.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1401 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/empty-0-0.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2237 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2845 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_00/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.871885 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      134 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      262 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      269 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3381 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_00/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_01/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.872885 createrepo_c-1.1.2/tests/testdata/repo_01/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      783 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      332 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      273 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1497 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_01/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_02/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.872885 createrepo_c-1.1.2/tests/testdata/repo_02/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      341 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      403 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      973 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1497 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_02/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_03/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.873885 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      134 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      262 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1044 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      269 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      123 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3838 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_03/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_04/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.873885 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      987 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      397 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      429 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      336 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2012 2023-10-03 22:18:31.000000 createrepo_c-1.1.2/tests/testdata/repo_04/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_koji_01/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.874885 createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      816 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1007 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      487 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1549 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_koji_02/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.874885 createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      338 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      913 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      687 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1547 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.877885 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      656 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     2366 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3775 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      864 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      864 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      932 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1287 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1519 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    88281 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      533 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1301 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      749 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      850 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    86680 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1482 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      748 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      687 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     8640 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.831884 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.877885 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      341 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      405 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1017 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1354 2023-10-03 20:21:34.000000 createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.878885 createrepo_c-1.1.2/tests/testdata/repodata_snippets/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      436 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      745 2023-10-03 22:03:10.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      263 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/filelists_snippet_01.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      471 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/filelists_snippet_02.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      408 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/other_snippet_01.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      697 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/other_snippet_02.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1918 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/primary_snippet_01.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     3085 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/repodata_snippets/primary_snippet_02.xml
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.878885 createrepo_c-1.1.2/tests/testdata/specs/
+-rwxr-xr-x   0 dalley   (29620) dalley   (29620)       67 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/build.sh
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1428 2024-05-07 02:44:46.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-Archer.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1023 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-Rimmer.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      571 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-iso88591.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      594 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-iso88592.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      653 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-utf8.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      176 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-empty.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      632 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-fake_bash.spec
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1236 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/specs/fake-super_kernel.spec
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.879885 createrepo_c-1.1.2/tests/testdata/test_files/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1523 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/binary_file
+-rw-r--r--   0 dalley   (29620) dalley   (29620)        0 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/empty_file
+-rw-r--r--   0 dalley   (29620) dalley   (29620)    24576 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/sqlite_file.sqlite
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      910 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/text_file
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      522 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/text_file.gz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      628 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/test_files/text_file.xz
+drwxr-xr-x   0 dalley   (29620) dalley   (29620)        0 2024-05-29 15:20:44.880885 createrepo_c-1.1.2/tests/testdata/updateinfo_files/
+-rw-r--r--   0 dalley   (29620) dalley   (29620)       60 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_00.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     1222 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_01.xml
+-rw-r--r--   0 dalley   (29620) dalley   (29620)      188 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
+-rw-r--r--   0 dalley   (29620) dalley   (29620)     4805 2023-03-21 04:57:44.000000 createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_03.xml
```

### Comparing `createrepo_c-1.1.1/CMakeLists.txt` & `createrepo_c-1.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/COPYING` & `createrepo_c-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/PKG-INFO` & `createrepo_c-1.1.2/src/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: createrepo_c
-Version: 1.1.1
+Name: createrepo-c
+Version: 1.1.2
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.1.1/README.md` & `createrepo_c-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/CMakeLists.txt` & `createrepo_c-1.1.2/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/Doxyfile.in.in` & `createrepo_c-1.1.2/doc/Doxyfile.in.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/createrepo_c.8` & `createrepo_c-1.1.2/doc/createrepo_c.8`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 .sp
 Make sure all xml generated is formatted (default)
 .SS \-p \-\-no\-pretty
 .sp
 Minify the generated xml content. On average this reduces compressed size by 2%.
 .SS \-d \-\-database
 .sp
-Generate sqlite databases for use with yum.
+DEPRECATED: Generate sqlite databases for use with yum.
 .SS \-\-no\-database
 .sp
 Do not generate sqlite databases in the repository.
 .SS \-\-update
 .sp
 If metadata already exists in the outputdir and an rpm is unchanged (based on file size and mtime) since the metadata was generated, reuse the existing metadata rather than recalculating it. In the case of a large repository with only a few new or modified rpms this can significantly reduce I/O and processing time.
 .SS \-\-update\-md\-path
@@ -178,15 +178,15 @@
 .sp
 Keep all additional metadata (not primary, filelists and other xml or sqlite files, nor their compressed variants) from source repository during update (default).
 .SS \-\-discard\-additional\-metadata
 .sp
 Discard all additional metadata (not primary, filelists and other xml or sqlite files, nor their compressed variants) from source repository during update.
 .SS \-\-compatibility
 .sp
-Enforce maximal compatibility with classical createrepo (Changes \-\-retain\-old\-md behavior, uses Gzip for compression).
+Enforce maximal compatibility with classical createrepo (Changes \-\-retain\-old\-md behavior, defaults to Gzip for compression).
 .SS \-\-retain\-old\-md\-by\-age AGE
 .sp
 During \-\-update, remove all files in repodata/ which are older then the specified period of time. (e.g. \(aq2h\(aq, \(aq30d\(aq, ...). Available units (m \- minutes, h \- hours, d \- days)
 .SS \-c \-\-cachedir CACHEDIR.
 .sp
 Set path to cache dir
 .SS \-\-deltas
```

### Comparing `createrepo_c-1.1.1/doc/logo.png` & `createrepo_c-1.1.2/doc/logo.png`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/logo.xcf` & `createrepo_c-1.1.2/doc/logo.xcf`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/mergerepo_c.8` & `createrepo_c-1.1.2/doc/mergerepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/modifyrepo_c.8` & `createrepo_c-1.1.2/doc/modifyrepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/python/conf.py` & `createrepo_c-1.1.2/doc/python/conf.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/python/lib.rst` & `createrepo_c-1.1.2/doc/python/lib.rst`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/doc/sqliterepo_c.8` & `createrepo_c-1.1.2/doc/sqliterepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/setup.py` & `createrepo_c-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/CMakeLists.txt` & `createrepo_c-1.1.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/checksum.c` & `createrepo_c-1.1.2/src/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/checksum.h` & `createrepo_c-1.1.2/src/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/cleanup.h` & `createrepo_c-1.1.2/src/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/cmd_parser.c` & `createrepo_c-1.1.2/src/cmd_parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
       "Choose the checksum type used in repomd.xml and for packages in the "
       "metadata. The default is now \"sha256\".", "CHECKSUM_TYPE" },
     { "pretty", 'p', 0, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "Make sure all xml generated is formatted (default)", NULL },
     { "no-pretty", 0, G_OPTION_FLAG_REVERSE, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "No extra indentation in generated xml", NULL },
     { "database", 'd', 0, G_OPTION_ARG_NONE, &(_cmd_options.database),
-      "Generate sqlite databases for use with yum.", NULL },
+      "DEPRECATED: Generate sqlite databases for use with yum.", NULL },
     { "no-database", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.no_database),
       "Do not generate sqlite databases in the repository (default).", NULL },
     { "filelists-ext", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.filelists_ext),
       "Create filelists-ext metadata with file hashes.", NULL },
     { "update", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.update),
       "If metadata already exists in the outputdir and an rpm is unchanged "
       "(based on file size and mtime) since the metadata was generated, reuse "
@@ -200,15 +200,15 @@
     { "keep-all-metadata", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.keep_all_metadata),
       "Keep all additional metadata (not primary, filelists and other xml or sqlite files, "
       "nor their compressed variants) from source repository during update (default).", NULL },
     { "discard-additional-metadata", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.discard_additional_metadata),
       "Discard all additional metadata (not primary, filelists and other xml or sqlite files, "
       "nor their compressed variants) from source repository during update.", NULL },
     { "compatibility", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.compatibility),
-      "Enforce maximal compatibility with classical createrepo and yum (Changes --retain-old-md behavior, uses Gzip for compression, produces sqlite metadata by default, leaves group metadata uncompressed).", NULL },
+      "Enforce maximal compatibility with classical createrepo and yum (Changes --retain-old-md behavior, defaults to Gzip for compression, produces sqlite metadata by default, leaves group metadata uncompressed).", NULL },
     { "retain-old-md-by-age", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.retain_old_md_by_age),
       "During --update, remove all files in repodata/ which are older "
       "then the specified period of time. (e.g. '2h', '30d', ...). "
       "Available units (m - minutes, h - hours, d - days)", "AGE" },
     { "cachedir", 'c', 0, G_OPTION_ARG_FILENAME, &(_cmd_options.cachedir),
       "Set path to cache dir", "CACHEDIR." },
 #ifdef CR_DELTA_RPM_SUPPORT
```

### Comparing `createrepo_c-1.1.1/src/cmd_parser.h` & `createrepo_c-1.1.2/src/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/compression_wrapper.c` & `createrepo_c-1.1.2/src/compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/compression_wrapper.h` & `createrepo_c-1.1.2/src/compression_wrapper.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/constants.h` & `createrepo_c-1.1.2/src/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/createrepo_c.c` & `createrepo_c-1.1.2/src/createrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/createrepo_c.h` & `createrepo_c-1.1.2/src/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/createrepo_shared.c` & `createrepo_c-1.1.2/src/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/createrepo_shared.h` & `createrepo_c-1.1.2/src/createrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/deltarpms.c` & `createrepo_c-1.1.2/src/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/deltarpms.h.in` & `createrepo_c-1.1.2/src/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/dumper_thread.c` & `createrepo_c-1.1.2/src/dumper_thread.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/dumper_thread.h` & `createrepo_c-1.1.2/src/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/error.c` & `createrepo_c-1.1.2/src/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/error.h` & `createrepo_c-1.1.2/src/error.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/helpers.c` & `createrepo_c-1.1.2/src/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/helpers.h` & `createrepo_c-1.1.2/src/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/koji.c` & `createrepo_c-1.1.2/src/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/koji.h` & `createrepo_c-1.1.2/src/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/load_metadata.c` & `createrepo_c-1.1.2/src/load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/load_metadata.h` & `createrepo_c-1.1.2/src/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/locate_metadata.c` & `createrepo_c-1.1.2/src/locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/locate_metadata.h` & `createrepo_c-1.1.2/src/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/mergerepo_c.c` & `createrepo_c-1.1.2/src/mergerepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/mergerepo_c.h` & `createrepo_c-1.1.2/src/mergerepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/metadata_internal.h` & `createrepo_c-1.1.2/src/metadata_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/misc.c` & `createrepo_c-1.1.2/src/misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/misc.h` & `createrepo_c-1.1.2/src/misc.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/modifyrepo_c.c` & `createrepo_c-1.1.2/src/modifyrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/modifyrepo_shared.c` & `createrepo_c-1.1.2/src/modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/modifyrepo_shared.h` & `createrepo_c-1.1.2/src/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/package.c` & `createrepo_c-1.1.2/src/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/package.h` & `createrepo_c-1.1.2/src/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/package_internal.h` & `createrepo_c-1.1.2/src/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/parsehdr.c` & `createrepo_c-1.1.2/src/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/parsehdr.h` & `createrepo_c-1.1.2/src/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/parsepkg.c` & `createrepo_c-1.1.2/src/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/parsepkg.h` & `createrepo_c-1.1.2/src/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/CMakeLists.txt` & `createrepo_c-1.1.2/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/checksum-py.c` & `createrepo_c-1.1.2/src/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/checksum-py.h` & `createrepo_c-1.1.2/src/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/compression_wrapper-py.c` & `createrepo_c-1.1.2/src/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/compression_wrapper-py.h` & `createrepo_c-1.1.2/src/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/contentstat-py.c` & `createrepo_c-1.1.2/src/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/contentstat-py.h` & `createrepo_c-1.1.2/src/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/createrepo_c/__init__.py` & `createrepo_c-1.1.2/_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,18 +710,16 @@
         overlapping_records = created_record_names.intersection(added_record_names)
         assert not overlapping_records, "Added repomd metadata {} conflicts with created metadata".format(overlapping_records)
 
         # there's no good way to write this data out incrementally, unfortunately
         if self._updaterecords:
             upd_xml_path = self.repodata_dir / ("updateinfo.xml" + self._compression_suffix)
             writer = UpdateInfoXmlFile(str(upd_xml_path), compressiontype=self._compression)
-            updateinfo = UpdateInfo()
             for rec in self._updaterecords:
-                updateinfo.append(rec)
-            writer.add_chunk(updateinfo.xml_dump())
+                writer.add_chunk(_createrepo_c.xml_dump_updaterecord(rec))
             self.working_metadata_files["updateinfo"] = MetadataInfoHolder(upd_xml_path, writer)
 
         # Create all the repomdrecords for the standard metadata
         for record_name, metadata_info in self.working_metadata_files.items():
             # Close all of the metadata files being actively edited
             metadata_info.writer.close()
             record = RepomdRecord(record_name, str(metadata_info.path))
```

### Comparing `createrepo_c-1.1.1/src/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo-c
-Version: 1.1.1
+Version: 1.1.2
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.1.1/src/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.1.2/src/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 COPYING
 MANIFEST.in
 README.md
 VERSION.cmake
 pyproject.toml
 requirements-dev.txt
 setup.py
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/__init__.py
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/_createrepo_c.so
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/createrepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/mergerepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/modifyrepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/sqliterepo_c
 doc/CMakeLists.txt
 doc/Doxyfile.in.in
 doc/createrepo_c.8
 doc/logo.png
 doc/logo.xcf
 doc/mergerepo_c.8
 doc/modifyrepo_c.8
@@ -26,18 +32,20 @@
 src/cmd_parser.c
 src/cmd_parser.h
 src/compression_wrapper.c
 src/compression_wrapper.h
 src/constants.h
 src/createrepo_c.c
 src/createrepo_c.h
+src/createrepo_c.pc
 src/createrepo_c.pc.cmake
 src/createrepo_shared.c
 src/createrepo_shared.h
 src/deltarpms.c
+src/deltarpms.h
 src/deltarpms.h.in
 src/dumper_thread.c
 src/dumper_thread.h
 src/error.c
 src/error.h
 src/helpers.c
 src/helpers.h
@@ -68,14 +76,15 @@
 src/sqlite.c
 src/sqlite.h
 src/sqliterepo_c.c
 src/threads.c
 src/threads.h
 src/updateinfo.c
 src/updateinfo.h
+src/version.h
 src/version.h.in
 src/xml_dump.c
 src/xml_dump.h
 src/xml_dump_deltapackage.c
 src/xml_dump_filelists.c
 src/xml_dump_internal.h
 src/xml_dump_other.c
@@ -170,18 +179,20 @@
 tests/createrepo/cmd_parser.c
 tests/createrepo/cmd_parser.h
 tests/createrepo/compression_wrapper.c
 tests/createrepo/compression_wrapper.h
 tests/createrepo/constants.h
 tests/createrepo/createrepo_c.c
 tests/createrepo/createrepo_c.h
+tests/createrepo/createrepo_c.pc
 tests/createrepo/createrepo_c.pc.cmake
 tests/createrepo/createrepo_shared.c
 tests/createrepo/createrepo_shared.h
 tests/createrepo/deltarpms.c
+tests/createrepo/deltarpms.h
 tests/createrepo/deltarpms.h.in
 tests/createrepo/dumper_thread.c
 tests/createrepo/dumper_thread.h
 tests/createrepo/error.c
 tests/createrepo/error.h
 tests/createrepo/helpers.c
 tests/createrepo/helpers.h
@@ -212,14 +223,15 @@
 tests/createrepo/sqlite.c
 tests/createrepo/sqlite.h
 tests/createrepo/sqliterepo_c.c
 tests/createrepo/threads.c
 tests/createrepo/threads.h
 tests/createrepo/updateinfo.c
 tests/createrepo/updateinfo.h
+tests/createrepo/version.h
 tests/createrepo/version.h.in
 tests/createrepo/xml_dump.c
 tests/createrepo/xml_dump.h
 tests/createrepo/xml_dump_deltapackage.c
 tests/createrepo/xml_dump_filelists.c
 tests/createrepo/xml_dump_internal.h
 tests/createrepo/xml_dump_other.c
```

### Comparing `createrepo_c-1.1.1/src/python/createrepo_cmodule.c` & `createrepo_c-1.1.2/src/python/createrepo_cmodule.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/exception-py.c` & `createrepo_c-1.1.2/src/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/exception-py.h` & `createrepo_c-1.1.2/src/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/load_metadata-py.c` & `createrepo_c-1.1.2/src/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/load_metadata-py.h` & `createrepo_c-1.1.2/src/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/locate_metadata-py.c` & `createrepo_c-1.1.2/src/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/locate_metadata-py.h` & `createrepo_c-1.1.2/src/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/misc-py.c` & `createrepo_c-1.1.2/src/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/misc-py.h` & `createrepo_c-1.1.2/src/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/package-py.c` & `createrepo_c-1.1.2/src/python/package-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/package-py.h` & `createrepo_c-1.1.2/src/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/parsepkg-py.c` & `createrepo_c-1.1.2/src/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/parsepkg-py.h` & `createrepo_c-1.1.2/src/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/repomd-py.c` & `createrepo_c-1.1.2/src/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/repomd-py.h` & `createrepo_c-1.1.2/src/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/repomdrecord-py.c` & `createrepo_c-1.1.2/src/python/repomdrecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/repomdrecord-py.h` & `createrepo_c-1.1.2/src/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/sqlite-py.c` & `createrepo_c-1.1.2/src/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/sqlite-py.h` & `createrepo_c-1.1.2/src/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/typeconversion.c` & `createrepo_c-1.1.2/src/python/typeconversion.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/typeconversion.h` & `createrepo_c-1.1.2/src/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollection-py.c` & `createrepo_c-1.1.2/src/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollection-py.h` & `createrepo_c-1.1.2/src/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollectionmodule-py.c` & `createrepo_c-1.1.2/src/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollectionmodule-py.h` & `createrepo_c-1.1.2/src/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollectionpackage-py.c` & `createrepo_c-1.1.2/src/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatecollectionpackage-py.h` & `createrepo_c-1.1.2/src/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updateinfo-py.c` & `createrepo_c-1.1.2/src/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updateinfo-py.h` & `createrepo_c-1.1.2/src/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updaterecord-py.c` & `createrepo_c-1.1.2/src/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updaterecord-py.h` & `createrepo_c-1.1.2/src/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatereference-py.c` & `createrepo_c-1.1.2/src/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/updatereference-py.h` & `createrepo_c-1.1.2/src/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_dump-py.c` & `createrepo_c-1.1.2/src/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_dump-py.h` & `createrepo_c-1.1.2/src/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_file-py.c` & `createrepo_c-1.1.2/src/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_file-py.h` & `createrepo_c-1.1.2/src/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_parser-py.c` & `createrepo_c-1.1.2/src/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/python/xml_parser-py.h` & `createrepo_c-1.1.2/src/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/repomd.c` & `createrepo_c-1.1.2/src/repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/repomd.h` & `createrepo_c-1.1.2/src/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/repomd_internal.h` & `createrepo_c-1.1.2/src/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/sqlite.c` & `createrepo_c-1.1.2/src/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/sqlite.h` & `createrepo_c-1.1.2/src/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/sqliterepo_c.c` & `createrepo_c-1.1.2/src/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/threads.c` & `createrepo_c-1.1.2/src/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/threads.h` & `createrepo_c-1.1.2/src/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/updateinfo.c` & `createrepo_c-1.1.2/src/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/updateinfo.h` & `createrepo_c-1.1.2/src/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/version.h.in` & `createrepo_c-1.1.2/src/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump.c` & `createrepo_c-1.1.2/src/xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump.h` & `createrepo_c-1.1.2/src/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_deltapackage.c` & `createrepo_c-1.1.2/src/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_filelists.c` & `createrepo_c-1.1.2/src/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_internal.h` & `createrepo_c-1.1.2/src/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_other.c` & `createrepo_c-1.1.2/src/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_primary.c` & `createrepo_c-1.1.2/src/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_repomd.c` & `createrepo_c-1.1.2/src/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_dump_updateinfo.c` & `createrepo_c-1.1.2/src/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_file.c` & `createrepo_c-1.1.2/src/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_file.h` & `createrepo_c-1.1.2/src/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser.c` & `createrepo_c-1.1.2/src/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser.h` & `createrepo_c-1.1.2/src/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_filelists.c` & `createrepo_c-1.1.2/src/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_internal.h` & `createrepo_c-1.1.2/src/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_main_metadata_together.c` & `createrepo_c-1.1.2/src/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_other.c` & `createrepo_c-1.1.2/src/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_primary.c` & `createrepo_c-1.1.2/src/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_repomd.c` & `createrepo_c-1.1.2/src/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/src/xml_parser_updateinfo.c` & `createrepo_c-1.1.2/src/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/CMakeLists.txt` & `createrepo_c-1.1.2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/CMakeLists.txt` & `createrepo_c-1.1.2/tests/createrepo/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/checksum.c` & `createrepo_c-1.1.2/tests/createrepo/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/checksum.h` & `createrepo_c-1.1.2/tests/createrepo/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/cleanup.h` & `createrepo_c-1.1.2/tests/createrepo/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/cmd_parser.c` & `createrepo_c-1.1.2/tests/createrepo/cmd_parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
       "Choose the checksum type used in repomd.xml and for packages in the "
       "metadata. The default is now \"sha256\".", "CHECKSUM_TYPE" },
     { "pretty", 'p', 0, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "Make sure all xml generated is formatted (default)", NULL },
     { "no-pretty", 0, G_OPTION_FLAG_REVERSE, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "No extra indentation in generated xml", NULL },
     { "database", 'd', 0, G_OPTION_ARG_NONE, &(_cmd_options.database),
-      "Generate sqlite databases for use with yum.", NULL },
+      "DEPRECATED: Generate sqlite databases for use with yum.", NULL },
     { "no-database", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.no_database),
       "Do not generate sqlite databases in the repository (default).", NULL },
     { "filelists-ext", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.filelists_ext),
       "Create filelists-ext metadata with file hashes.", NULL },
     { "update", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.update),
       "If metadata already exists in the outputdir and an rpm is unchanged "
       "(based on file size and mtime) since the metadata was generated, reuse "
@@ -200,15 +200,15 @@
     { "keep-all-metadata", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.keep_all_metadata),
       "Keep all additional metadata (not primary, filelists and other xml or sqlite files, "
       "nor their compressed variants) from source repository during update (default).", NULL },
     { "discard-additional-metadata", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.discard_additional_metadata),
       "Discard all additional metadata (not primary, filelists and other xml or sqlite files, "
       "nor their compressed variants) from source repository during update.", NULL },
     { "compatibility", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.compatibility),
-      "Enforce maximal compatibility with classical createrepo and yum (Changes --retain-old-md behavior, uses Gzip for compression, produces sqlite metadata by default, leaves group metadata uncompressed).", NULL },
+      "Enforce maximal compatibility with classical createrepo and yum (Changes --retain-old-md behavior, defaults to Gzip for compression, produces sqlite metadata by default, leaves group metadata uncompressed).", NULL },
     { "retain-old-md-by-age", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.retain_old_md_by_age),
       "During --update, remove all files in repodata/ which are older "
       "then the specified period of time. (e.g. '2h', '30d', ...). "
       "Available units (m - minutes, h - hours, d - days)", "AGE" },
     { "cachedir", 'c', 0, G_OPTION_ARG_FILENAME, &(_cmd_options.cachedir),
       "Set path to cache dir", "CACHEDIR." },
 #ifdef CR_DELTA_RPM_SUPPORT
```

### Comparing `createrepo_c-1.1.1/tests/createrepo/cmd_parser.h` & `createrepo_c-1.1.2/tests/createrepo/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/compression_wrapper.c` & `createrepo_c-1.1.2/tests/createrepo/compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/compression_wrapper.h` & `createrepo_c-1.1.2/tests/createrepo/compression_wrapper.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/constants.h` & `createrepo_c-1.1.2/tests/createrepo/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/createrepo_c.c` & `createrepo_c-1.1.2/tests/createrepo/createrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/createrepo_c.h` & `createrepo_c-1.1.2/tests/createrepo/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/createrepo_shared.c` & `createrepo_c-1.1.2/tests/createrepo/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/createrepo_shared.h` & `createrepo_c-1.1.2/tests/createrepo/createrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/deltarpms.c` & `createrepo_c-1.1.2/tests/createrepo/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/deltarpms.h.in` & `createrepo_c-1.1.2/tests/createrepo/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/dumper_thread.c` & `createrepo_c-1.1.2/tests/createrepo/dumper_thread.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/dumper_thread.h` & `createrepo_c-1.1.2/tests/createrepo/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/error.c` & `createrepo_c-1.1.2/tests/createrepo/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/error.h` & `createrepo_c-1.1.2/tests/createrepo/error.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/helpers.c` & `createrepo_c-1.1.2/tests/createrepo/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/helpers.h` & `createrepo_c-1.1.2/tests/createrepo/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/koji.c` & `createrepo_c-1.1.2/tests/createrepo/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/koji.h` & `createrepo_c-1.1.2/tests/createrepo/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/load_metadata.c` & `createrepo_c-1.1.2/tests/createrepo/load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/load_metadata.h` & `createrepo_c-1.1.2/tests/createrepo/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/locate_metadata.c` & `createrepo_c-1.1.2/tests/createrepo/locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/locate_metadata.h` & `createrepo_c-1.1.2/tests/createrepo/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/mergerepo_c.c` & `createrepo_c-1.1.2/tests/createrepo/mergerepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/mergerepo_c.h` & `createrepo_c-1.1.2/tests/createrepo/mergerepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/metadata_internal.h` & `createrepo_c-1.1.2/tests/createrepo/metadata_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/misc.c` & `createrepo_c-1.1.2/tests/createrepo/misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/misc.h` & `createrepo_c-1.1.2/tests/createrepo/misc.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/modifyrepo_c.c` & `createrepo_c-1.1.2/tests/createrepo/modifyrepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/modifyrepo_shared.c` & `createrepo_c-1.1.2/tests/createrepo/modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/modifyrepo_shared.h` & `createrepo_c-1.1.2/tests/createrepo/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/package.c` & `createrepo_c-1.1.2/tests/createrepo/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/package.h` & `createrepo_c-1.1.2/tests/createrepo/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/package_internal.h` & `createrepo_c-1.1.2/tests/createrepo/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/parsehdr.c` & `createrepo_c-1.1.2/tests/createrepo/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/parsehdr.h` & `createrepo_c-1.1.2/tests/createrepo/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/parsepkg.c` & `createrepo_c-1.1.2/tests/createrepo/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/parsepkg.h` & `createrepo_c-1.1.2/tests/createrepo/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/CMakeLists.txt` & `createrepo_c-1.1.2/tests/createrepo/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/checksum-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/checksum-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/compression_wrapper-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/compression_wrapper-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/contentstat-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/contentstat-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/createrepo_c/__init__.py` & `createrepo_c-1.1.2/src/python/createrepo_c/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,18 +710,16 @@
         overlapping_records = created_record_names.intersection(added_record_names)
         assert not overlapping_records, "Added repomd metadata {} conflicts with created metadata".format(overlapping_records)
 
         # there's no good way to write this data out incrementally, unfortunately
         if self._updaterecords:
             upd_xml_path = self.repodata_dir / ("updateinfo.xml" + self._compression_suffix)
             writer = UpdateInfoXmlFile(str(upd_xml_path), compressiontype=self._compression)
-            updateinfo = UpdateInfo()
             for rec in self._updaterecords:
-                updateinfo.append(rec)
-            writer.add_chunk(updateinfo.xml_dump())
+                writer.add_chunk(_createrepo_c.xml_dump_updaterecord(rec))
             self.working_metadata_files["updateinfo"] = MetadataInfoHolder(upd_xml_path, writer)
 
         # Create all the repomdrecords for the standard metadata
         for record_name, metadata_info in self.working_metadata_files.items():
             # Close all of the metadata files being actively edited
             metadata_info.writer.close()
             record = RepomdRecord(record_name, str(metadata_info.path))
```

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: createrepo-c
-Version: 1.1.1
+Name: createrepo_c
+Version: 1.1.2
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.1.2/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 COPYING
 MANIFEST.in
 README.md
 VERSION.cmake
 pyproject.toml
 requirements-dev.txt
 setup.py
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/__init__.py
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/_createrepo_c.so
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/createrepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/mergerepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/modifyrepo_c
+_skbuild/linux-x86_64-3.9/cmake-install/src/python/createrepo_c/data/bin/sqliterepo_c
 doc/CMakeLists.txt
 doc/Doxyfile.in.in
 doc/createrepo_c.8
 doc/logo.png
 doc/logo.xcf
 doc/mergerepo_c.8
 doc/modifyrepo_c.8
@@ -26,18 +32,20 @@
 src/cmd_parser.c
 src/cmd_parser.h
 src/compression_wrapper.c
 src/compression_wrapper.h
 src/constants.h
 src/createrepo_c.c
 src/createrepo_c.h
+src/createrepo_c.pc
 src/createrepo_c.pc.cmake
 src/createrepo_shared.c
 src/createrepo_shared.h
 src/deltarpms.c
+src/deltarpms.h
 src/deltarpms.h.in
 src/dumper_thread.c
 src/dumper_thread.h
 src/error.c
 src/error.h
 src/helpers.c
 src/helpers.h
@@ -68,14 +76,15 @@
 src/sqlite.c
 src/sqlite.h
 src/sqliterepo_c.c
 src/threads.c
 src/threads.h
 src/updateinfo.c
 src/updateinfo.h
+src/version.h
 src/version.h.in
 src/xml_dump.c
 src/xml_dump.h
 src/xml_dump_deltapackage.c
 src/xml_dump_filelists.c
 src/xml_dump_internal.h
 src/xml_dump_other.c
@@ -170,18 +179,20 @@
 tests/createrepo/cmd_parser.c
 tests/createrepo/cmd_parser.h
 tests/createrepo/compression_wrapper.c
 tests/createrepo/compression_wrapper.h
 tests/createrepo/constants.h
 tests/createrepo/createrepo_c.c
 tests/createrepo/createrepo_c.h
+tests/createrepo/createrepo_c.pc
 tests/createrepo/createrepo_c.pc.cmake
 tests/createrepo/createrepo_shared.c
 tests/createrepo/createrepo_shared.h
 tests/createrepo/deltarpms.c
+tests/createrepo/deltarpms.h
 tests/createrepo/deltarpms.h.in
 tests/createrepo/dumper_thread.c
 tests/createrepo/dumper_thread.h
 tests/createrepo/error.c
 tests/createrepo/error.h
 tests/createrepo/helpers.c
 tests/createrepo/helpers.h
@@ -212,14 +223,15 @@
 tests/createrepo/sqlite.c
 tests/createrepo/sqlite.h
 tests/createrepo/sqliterepo_c.c
 tests/createrepo/threads.c
 tests/createrepo/threads.h
 tests/createrepo/updateinfo.c
 tests/createrepo/updateinfo.h
+tests/createrepo/version.h
 tests/createrepo/version.h.in
 tests/createrepo/xml_dump.c
 tests/createrepo/xml_dump.h
 tests/createrepo/xml_dump_deltapackage.c
 tests/createrepo/xml_dump_filelists.c
 tests/createrepo/xml_dump_internal.h
 tests/createrepo/xml_dump_other.c
```

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/createrepo_cmodule.c` & `createrepo_c-1.1.2/tests/createrepo/python/createrepo_cmodule.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/exception-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/exception-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/load_metadata-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/load_metadata-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/locate_metadata-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/locate_metadata-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/misc-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/misc-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/package-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/package-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/package-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/parsepkg-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/parsepkg-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/repomd-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/repomd-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/repomdrecord-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/repomdrecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/repomdrecord-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/sqlite-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/sqlite-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/typeconversion.c` & `createrepo_c-1.1.2/tests/createrepo/python/typeconversion.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/typeconversion.h` & `createrepo_c-1.1.2/tests/createrepo/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollection-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollection-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollectionmodule-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollectionmodule-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollectionpackage-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatecollectionpackage-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updateinfo-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updateinfo-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updaterecord-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updaterecord-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatereference-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/updatereference-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_dump-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_dump-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_file-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_file-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_parser-py.c` & `createrepo_c-1.1.2/tests/createrepo/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/python/xml_parser-py.h` & `createrepo_c-1.1.2/tests/createrepo/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/repomd.c` & `createrepo_c-1.1.2/tests/createrepo/repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/repomd.h` & `createrepo_c-1.1.2/tests/createrepo/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/repomd_internal.h` & `createrepo_c-1.1.2/tests/createrepo/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/sqlite.c` & `createrepo_c-1.1.2/tests/createrepo/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/sqlite.h` & `createrepo_c-1.1.2/tests/createrepo/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/sqliterepo_c.c` & `createrepo_c-1.1.2/tests/createrepo/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/threads.c` & `createrepo_c-1.1.2/tests/createrepo/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/threads.h` & `createrepo_c-1.1.2/tests/createrepo/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/updateinfo.c` & `createrepo_c-1.1.2/tests/createrepo/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/updateinfo.h` & `createrepo_c-1.1.2/tests/createrepo/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/version.h.in` & `createrepo_c-1.1.2/tests/createrepo/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump.h` & `createrepo_c-1.1.2/tests/createrepo/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_deltapackage.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_filelists.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_internal.h` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_other.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_primary.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_repomd.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_dump_updateinfo.c` & `createrepo_c-1.1.2/tests/createrepo/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_file.c` & `createrepo_c-1.1.2/tests/createrepo/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_file.h` & `createrepo_c-1.1.2/tests/createrepo/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser.h` & `createrepo_c-1.1.2/tests/createrepo/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_filelists.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_internal.h` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_main_metadata_together.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_other.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_primary.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_repomd.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/createrepo/xml_parser_updateinfo.c` & `createrepo_c-1.1.2/tests/createrepo/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/fixtures.h` & `createrepo_c-1.1.2/tests/fixtures.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/fixtures.py` & `createrepo_c-1.1.2/tests/python/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_checksum.py` & `createrepo_c-1.1.2/tests/python/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_compression_wrapper.py` & `createrepo_c-1.1.2/tests/python/tests/test_compression_wrapper.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_contentstat.py` & `createrepo_c-1.1.2/tests/python/tests/test_contentstat.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_crfile.py` & `createrepo_c-1.1.2/tests/python/tests/test_crfile.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_load_metadata.py` & `createrepo_c-1.1.2/tests/python/tests/test_load_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_locate_metadata.py` & `createrepo_c-1.1.2/tests/python/tests/test_locate_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_misc.py` & `createrepo_c-1.1.2/tests/python/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_package.py` & `createrepo_c-1.1.2/tests/python/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_parsepkg.py` & `createrepo_c-1.1.2/tests/python/tests/test_parsepkg.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_repomd.py` & `createrepo_c-1.1.2/tests/python/tests/test_repomd.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_repomdrecord.py` & `createrepo_c-1.1.2/tests/python/tests/test_repomdrecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_repository.py` & `createrepo_c-1.1.2/tests/python/tests/test_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         assert len(list(reader.advisories())) == 1
 
     def test_count_packages(self):
         reader = cr.RepositoryReader.from_path(REPO_01_PATH)
 
         assert reader.package_count() == 1
 
+
 class TestCaseRepositoryWriter(unittest.TestCase):
 
     def setUp(self):
         self.tmpdir = tempfile.mkdtemp(prefix="createrepo_ctest-")
 
     def tearDown(self):
         shutil.rmtree(self.tmpdir)
@@ -95,21 +96,26 @@
             else:
                 assert record.location_href == f"repodata/{record.checksum}-{record.type}.xml.zst"
 
             # test that the metadata files were created on disk
             record_path = os.path.join(self.tmpdir, record.location_href)
             assert os.path.exists(record_path)
 
-            reader = cr.RepositoryReader.from_path(self.tmpdir)
-            for pkg in reader.iter_packages():
-                # test that the package files are present where expected
-                pkg_path = os.path.join(self.tmpdir, pkg.location_href)
-                assert os.path.exists(pkg_path)
-                # test that the package checksum type is correct
-                assert pkg.checksum_type == "sha256"
+        reader = cr.RepositoryReader.from_path(self.tmpdir)
+        for pkg in reader.iter_packages():
+            # test that the package files are present where expected
+            pkg_path = os.path.join(self.tmpdir, pkg.location_href)
+            assert os.path.exists(pkg_path)
+            # test that the package checksum type is correct
+            assert pkg.checksum_type == "sha256"
+
+        expected_updaterecords = [TEST_UPDATERECORD_UPDATE1]
+        for expected, actual in zip(expected_updaterecords, reader.advisories()):
+            assert_updaterecord_equal(expected, actual)
+
 
     def test_options(self):
         """Test that overriding default options works as intended"""
         with cr.RepositoryWriter(
             self.tmpdir,
             num_packages=3,
             unique_md_filenames=False,
@@ -138,23 +144,28 @@
             else:
                 assert record.location_href == f"repodata/{record.type}.xml.xz"
 
             # test that the metadata files were created on disk
             record_path = os.path.join(self.tmpdir, record.location_href)
             assert os.path.exists(record_path)
 
-            reader = cr.RepositoryReader.from_path(self.tmpdir)
-            for pkg in reader.iter_packages():
-                # test that the package files are present where expected
-                pkg_path = os.path.join(self.tmpdir, pkg.location_href)
-                assert os.path.exists(pkg_path)
-                # test that changelog_limit works
-                assert len(pkg.changelogs) <= 1
-                # test that the package checksum type is correct
-                assert pkg.checksum_type == "sha512"
+        reader = cr.RepositoryReader.from_path(self.tmpdir)
+        for pkg in reader.iter_packages():
+            # test that the package files are present where expected
+            pkg_path = os.path.join(self.tmpdir, pkg.location_href)
+            assert os.path.exists(pkg_path)
+            # test that changelog_limit works
+            assert len(pkg.changelogs) <= 1
+            # test that the package checksum type is correct
+            assert pkg.checksum_type == "sha512"
+
+        expected_updaterecords = [TEST_UPDATERECORD_UPDATE1]
+        for expected, actual in zip(expected_updaterecords, reader.advisories()):
+            assert_updaterecord_equal(expected, actual)
+
 
     def test_add_repo_metadata(self):
         """Test adding an additional repo metadata file to the repository."""
         basename = os.path.basename(TEST_COMPS_00)
 
         with cr.RepositoryWriter(self.tmpdir) as writer:
             writer.add_repomd_metadata("group", TEST_COMPS_00, use_compression=False)
@@ -235,8 +246,29 @@
 
         reader = cr.RepositoryReader.from_path(self.tmpdir)
         for pkg in reader.iter_packages():
             # test that the packages were relocated to package_dir
             assert pkg.location_href.startswith("Packages/")
             # test that the package files are present where expected
             pkg_path = os.path.join(self.tmpdir, pkg.location_href)
-            assert os.path.exists(pkg_path)
+            assert os.path.exists(pkg_path)
+
+
+def assert_updaterecord_equal(expected, actual):
+    assert expected.fromstr == actual.fromstr
+    assert expected.status == actual.status
+    assert expected.type == actual.type
+    assert expected.version == actual.version
+    assert expected.id == actual.id
+    assert expected.title == actual.title
+    assert expected.issued_date == actual.issued_date
+    assert expected.updated_date == actual.updated_date
+    assert expected.rights == actual.rights
+    assert expected.release == actual.release
+    assert expected.pushcount == actual.pushcount
+    assert expected.severity == actual.severity
+    assert expected.summary == actual.summary
+    assert expected.reboot_suggested == actual.reboot_suggested
+    assert expected.description == actual.description
+    assert expected.solution == actual.solution
+    assert len(expected.references) == len(actual.references)
+    assert len(expected.collections) == len(actual.collections)
```

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_sqlite.py` & `createrepo_c-1.1.2/tests/python/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updatecollection.py` & `createrepo_c-1.1.2/tests/python/tests/test_updatecollection.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updatecollectionmodule.py` & `createrepo_c-1.1.2/tests/python/tests/test_updatecollectionmodule.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updatecollectionpackage.py` & `createrepo_c-1.1.2/tests/python/tests/test_updatecollectionpackage.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updateinfo.py` & `createrepo_c-1.1.2/tests/python/tests/test_updateinfo.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updaterecord.py` & `createrepo_c-1.1.2/tests/python/tests/test_updaterecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_updatereference.py` & `createrepo_c-1.1.2/tests/python/tests/test_updatereference.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_xml_file.py` & `createrepo_c-1.1.2/tests/python/tests/test_xml_file.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/python/tests/test_xml_parser.py` & `createrepo_c-1.1.2/tests/python/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/run_tests.sh.in` & `createrepo_c-1.1.2/tests/run_tests.sh.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_checksum.c` & `createrepo_c-1.1.2/tests/test_checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_compression_wrapper.c` & `createrepo_c-1.1.2/tests/test_compression_wrapper.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_koji.c` & `createrepo_c-1.1.2/tests/test_koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_load_metadata.c` & `createrepo_c-1.1.2/tests/test_load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_locate_metadata.c` & `createrepo_c-1.1.2/tests/test_locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_misc.c` & `createrepo_c-1.1.2/tests/test_misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_modifyrepo_shared.c` & `createrepo_c-1.1.2/tests/test_modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_sqlite.c` & `createrepo_c-1.1.2/tests/test_sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_dump.c` & `createrepo_c-1.1.2/tests/test_xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_dump_primary.c` & `createrepo_c-1.1.2/tests/test_xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_file.c` & `createrepo_c-1.1.2/tests/test_xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_parser_filelists.c` & `createrepo_c-1.1.2/tests/test_xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_parser_main_metadata_together.c` & `createrepo_c-1.1.2/tests/test_xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_parser_repomd.c` & `createrepo_c-1.1.2/tests/test_xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/test_xml_parser_updateinfo.c` & `createrepo_c-1.1.2/tests/test_xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/comps_files/comps_00.xml` & `createrepo_c-1.1.2/tests/testdata/comps_files/comps_00.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/bad_file_type-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/bad_file_type-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/error_00-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/error_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/long_primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/long_primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/missing_type-repomd.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/missing_type-repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/no_pkgid-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/no_pkgid-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_00-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_01-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_01-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-other.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/unknown_element_02-primary.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/unknown_element_02-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/modified_repo_files/updateinfo_ampersand.xml` & `createrepo_c-1.1.2/tests/testdata/modified_repo_files/updateinfo_ampersand.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2` & `createrepo_c-1.1.2/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml` & `createrepo_c-1.1.2/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz` & `createrepo_c-1.1.2/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz` & `createrepo_c-1.1.2/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/other_metadata/comps-f19.xml` & `createrepo_c-1.1.2/tests/testdata/other_metadata/comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/empty-0-0.src.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/empty-0-0.src.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/empty-0-0.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/empty-0-0.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm` & `createrepo_c-1.1.2/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_00/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_00/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_01/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_02/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz` & `createrepo_c-1.1.2/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_03/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_03/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_04/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_04/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_01/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_koji_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_koji_02/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_koji_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz` & `createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml` & `createrepo_c-1.1.2/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml` & `createrepo_c-1.1.2/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repodata_snippets/other_snippet_02.xml` & `createrepo_c-1.1.2/tests/testdata/repodata_snippets/other_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repodata_snippets/primary_snippet_01.xml` & `createrepo_c-1.1.2/tests/testdata/repodata_snippets/primary_snippet_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/repodata_snippets/primary_snippet_02.xml` & `createrepo_c-1.1.2/tests/testdata/repodata_snippets/primary_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-Archer.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-Archer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-Rimmer.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-Rimmer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-iso88591.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-iso88591.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-iso88592.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-iso88592.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-balicek-utf8.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-balicek-utf8.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-fake_bash.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-fake_bash.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/specs/fake-super_kernel.spec` & `createrepo_c-1.1.2/tests/testdata/specs/fake-super_kernel.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/test_files/binary_file` & `createrepo_c-1.1.2/tests/testdata/test_files/binary_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/test_files/sqlite_file.sqlite` & `createrepo_c-1.1.2/tests/testdata/test_files/sqlite_file.sqlite`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/test_files/text_file` & `createrepo_c-1.1.2/tests/testdata/test_files/text_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/test_files/text_file.gz` & `createrepo_c-1.1.2/tests/testdata/test_files/text_file.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/test_files/text_file.xz` & `createrepo_c-1.1.2/tests/testdata/test_files/text_file.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_01.xml` & `createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-1.1.1/tests/testdata/updateinfo_files/updateinfo_03.xml` & `createrepo_c-1.1.2/tests/testdata/updateinfo_files/updateinfo_03.xml`

 * *Files identical despite different names*

