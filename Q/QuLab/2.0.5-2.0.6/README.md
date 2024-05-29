# Comparing `tmp/qulab-2.0.5.tar.gz` & `tmp/qulab-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.5.tar", last modified: Tue May 28 07:37:19 2024, max compression
+gzip compressed data, was "qulab-2.0.6.tar", last modified: Wed May 29 01:11:01 2024, max compression
```

## Comparing `qulab-2.0.5.tar` & `qulab-2.0.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.530429 qulab-2.0.5/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-28 07:36:42.000000 qulab-2.0.5/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-28 07:36:42.000000 qulab-2.0.5/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 07:37:19.530205 qulab-2.0.5/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529869 qulab-2.0.5/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-28 07:37:19.000000 qulab-2.0.5/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-28 07:36:42.000000 qulab-2.0.5/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-28 07:36:42.000000 qulab-2.0.5/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.519186 qulab-2.0.5/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.520628 qulab-2.0.5/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.522219 qulab-2.0.5/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    17938 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    25931 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.523076 qulab-2.0.5/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.523280 qulab-2.0.5/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.524445 qulab-2.0.5/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525010 qulab-2.0.5/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525623 qulab-2.0.5/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.525875 qulab-2.0.5/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.526821 qulab-2.0.5/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.528357 qulab-2.0.5/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529294 qulab-2.0.5/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-28 07:36:42.000000 qulab-2.0.5/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-28 07:37:19.530465 qulab-2.0.5/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-28 07:36:42.000000 qulab-2.0.5/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529417 qulab-2.0.5/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-28 07:36:42.000000 qulab-2.0.5/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-28 07:37:19.529612 qulab-2.0.5/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-28 07:36:42.000000 qulab-2.0.5/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.326820 qulab-2.0.6/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-29 01:10:26.000000 qulab-2.0.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-29 01:10:26.000000 qulab-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 01:11:01.326577 qulab-2.0.6/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.326259 qulab-2.0.6/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-29 01:11:01.000000 qulab-2.0.6/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-29 01:10:26.000000 qulab-2.0.6/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-29 01:10:26.000000 qulab-2.0.6/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.315740 qulab-2.0.6/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.317191 qulab-2.0.6/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.318507 qulab-2.0.6/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    22163 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    26033 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.319375 qulab-2.0.6/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.319577 qulab-2.0.6/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.320631 qulab-2.0.6/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.321174 qulab-2.0.6/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.321633 qulab-2.0.6/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.321869 qulab-2.0.6/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.322851 qulab-2.0.6/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.324560 qulab-2.0.6/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.325667 qulab-2.0.6/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-29 01:10:26.000000 qulab-2.0.6/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-29 01:11:01.326861 qulab-2.0.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-29 01:10:26.000000 qulab-2.0.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.325804 qulab-2.0.6/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-29 01:10:26.000000 qulab-2.0.6/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 01:11:01.326023 qulab-2.0.6/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-29 01:10:26.000000 qulab-2.0.6/tests/test_scan.py
```

### Comparing `qulab-2.0.5/LICENSE` & `qulab-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/PKG-INFO` & `qulab-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.5
+Version: 2.0.6
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.5/QuLab.egg-info/PKG-INFO` & `qulab-2.0.6/QuLab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.5
+Version: 2.0.6
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.5/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.6/QuLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/README.md` & `qulab-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/pyproject.toml` & `qulab-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/config.py` & `qulab-2.0.6/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/dataset.py` & `qulab-2.0.6/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/event_queue.py` & `qulab-2.0.6/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/mainwindow.py` & `qulab-2.0.6/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/monitor.py` & `qulab-2.0.6/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/ploter.py` & `qulab-2.0.6/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/qt_compat.py` & `qulab-2.0.6/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/monitor/toolbar.py` & `qulab-2.0.6/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/curd.py` & `qulab-2.0.6/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/expression.py` & `qulab-2.0.6/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/models.py` & `qulab-2.0.6/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/optimize.py` & `qulab-2.0.6/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/query_record.py` & `qulab-2.0.6/qulab/scan/query_record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/recorder.py` & `qulab-2.0.6/qulab/scan/recorder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import asyncio
+import itertools
 import os
 import pickle
 import sys
 import time
 import uuid
 from collections import defaultdict
 from pathlib import Path
 from threading import Lock
+from types import EllipsisType
 
 import click
 import dill
 import numpy as np
 import zmq
 from loguru import logger
 
@@ -40,120 +42,192 @@
     while True:
         s = uuid.uuid4().hex
         path = base / s[:2] / s[2:4] / s[4:6] / s[6:]
         if not path.exists():
             return path
 
 
+def index_in_slice(slice_obj: slice | int, index: int):
+    if isinstance(slice_obj, int):
+        return slice_obj == index
+    start, stop, step = slice_obj.start, slice_obj.stop, slice_obj.step
+    if start is None:
+        start = 0
+    if step is None:
+        step = 1
+    if stop is None:
+        stop = sys.maxsize
+
+    if step > 0:
+        return start <= index < stop and (index - start) % step == 0
+    else:
+        return stop < index <= start and (index - start) % step == 0
+
+
 class BufferList():
 
-    def __init__(self, pos_file=None, value_file=None):
-        self._pos = []
-        self._value = []
+    def __init__(self, file=None, slice=None):
+        self._list = []
         self.lu = ()
         self.rd = ()
-        self.pos_file = pos_file
-        self.value_file = value_file
+        self.inner_shape = None
+        self.file = file
+        self._slice = slice
         self._lock = Lock()
+        self._database = None
+
+    def __repr__(self):
+        return f"<BufferList: lu={self.lu}, rd={self.rd}, slice={self._slice}>"
 
     def __getstate__(self):
+        self.flush()
+        if isinstance(self.file, Path):
+            file = '/'.join(self.file.parts[-4:])
+        else:
+            file = self.file
         return {
-            'pos_file': self.pos_file,
-            'value_file': self.value_file,
-            '_pos': self._pos,
-            '_value': self._value,
+            'file': file,
             'lu': self.lu,
-            'rd': self.rd
+            'rd': self.rd,
+            'inner_shape': self.inner_shape,
         }
 
     def __setstate__(self, state):
-        self.pos_file = state['pos_file']
-        self.value_file = state['value_file']
-        self._pos = state['_pos']
-        self._value = state['_value']
+        self.file = state['file']
         self.lu = state['lu']
         self.rd = state['rd']
+        self.inner_shape = state['inner_shape']
+        self._list = []
+        self._slice = None
         self._lock = Lock()
+        self._database = None
 
     @property
     def shape(self):
         return tuple([i - j for i, j in zip(self.rd, self.lu)])
 
     def flush(self):
-        with self._lock:
-            if self.pos_file is not None:
-                with open(self.pos_file, 'ab') as f:
-                    for pos in self._pos:
-                        dill.dump(pos, f)
-                self._pos.clear()
-            if self.value_file is not None:
-                with open(self.value_file, 'ab') as f:
-                    for value in self._value:
-                        dill.dump(value, f)
-                self._value.clear()
+        if not self._list:
+            return
+        if isinstance(self.file, Path):
+            with self._lock:
+                with open(self.file, 'ab') as f:
+                    for item in self._list:
+                        dill.dump(item, f)
+                self._list.clear()
 
     def append(self, pos, value, dims=None):
         if dims is not None:
             if any([p != 0 for i, p in enumerate(pos) if i not in dims]):
                 return
             pos = tuple([pos[i] for i in dims])
         self.lu = tuple([min(i, j) for i, j in zip(pos, self.lu)])
         self.rd = tuple([max(i + 1, j) for i, j in zip(pos, self.rd)])
-        self._pos.append(pos)
-        self._value.append(value)
-        if len(self._value) > 1000:
+        if hasattr(value, 'shape'):
+            if self.inner_shape is None:
+                self.inner_shape = value.shape
+            elif self.inner_shape != value.shape:
+                self.inner_shape = ()
+        self._list.append((pos, value))
+        if len(self._list) > 1000:
             self.flush()
 
-    def value(self):
-        v = []
-        if self.value_file is not None and self.value_file.exists():
+    def _iter_file(self):
+        if isinstance(self.file, Path) and self.file.exists():
             with self._lock:
-                with open(self.value_file, 'rb') as f:
+                with open(self.file, 'rb') as f:
                     while True:
                         try:
-                            v.append(dill.load(f))
+                            pos, value = dill.load(f)
+                            yield pos, value
                         except EOFError:
                             break
-        v.extend(self._value)
-        return v
+
+    def iter(self):
+        for pos, value in itertools.chain(self._iter_file(), self._list):
+            if not self._slice:
+                yield pos, value
+            elif all([index_in_slice(s, i) for s, i in zip(self._slice, pos)]):
+                yield pos, value[self._slice[len(pos):]]
+
+    def value(self):
+        d = []
+        for pos, value in self.iter():
+            d.append(value)
+        return d
 
     def pos(self):
         p = []
-        if self.pos_file is not None and self.pos_file.exists():
-            with self._lock:
-                with open(self.pos_file, 'rb') as f:
-                    while True:
-                        try:
-                            p.append(dill.load(f))
-                        except EOFError:
-                            break
-        p.extend(self._pos)
+        for pos, value in self.iter():
+            p.append(pos)
         return p
 
+    def items(self):
+        p, d = [], []
+        for pos, value in self.iter():
+            p.append(pos)
+            d.append(value)
+        return p, d
+
     def array(self):
-        pos = np.asarray(self.pos()) - np.asarray(self.lu)
-        data = np.asarray(self.value())
+        pos, data = self.items()
+        pos = np.asarray(pos) - np.asarray(self.lu)
+        data = np.asarray(data)
         inner_shape = data.shape[1:]
         x = np.full(self.shape + inner_shape, np.nan, dtype=data[0].dtype)
         x.__setitem__(tuple(pos.T), data)
         return x
 
+    def _full_slice(self, slice_tuple: slice
+                    | tuple[slice | int | EllipsisType, ...]):
+        if isinstance(slice_tuple, slice):
+            slice_tuple = (slice_tuple, ) + (slice(0, sys.maxsize,
+                                                   1), ) * (len(self.lu) - 1)
+        if slice_tuple is Ellipsis:
+            slice_tuple = (slice(0, sys.maxsize, 1), ) * len(self.lu)
+        else:
+            head, tail = [], []
+            for i, s in enumerate(slice_tuple):
+                if s is Ellipsis:
+                    head = slice_tuple[:i]
+                    tail = slice_tuple[i + 1:]
+                    break
+            slice_tuple = head + (slice(0, sys.maxsize, 1), ) * (
+                len(self.lu) - len(head) - len(tail)) + tail
+        slice_list = []
+        for s in slice_tuple:
+            if isinstance(s, int):
+                slice_list.append(s)
+            else:
+                start, stop, step = s.start, s.stop, s.step
+                if start is None:
+                    start = 0
+                if step is None:
+                    step = 1
+                if stop is None:
+                    stop = sys.maxsize
+                slice_list.append(slice(start, stop, step))
+        return tuple(slice_list)
+
+    def __getitem__(self, slice_tuple: slice | EllipsisType
+                    | tuple[slice | int | EllipsisType, ...]):
+        return super().__getitem__(self._full_slice(slice_tuple))
+
 
 class Record():
 
     def __init__(self, id, database, description=None):
         self.id = id
         self.database = database
         self.description = description
         self._keys = set()
         self._items = {}
         self._index = []
         self._pos = []
         self._last_vars = set()
-        self._levels = {}
         self._file = None
         self.independent_variables = {}
         self.constants = {}
         self.dims = {}
 
         for name, value in self.description['consts'].items():
             if name not in self._items:
@@ -166,29 +240,57 @@
                     self._items[name] = iterable
                     self.independent_variables[name] = iterable
                     self.dims[name] = (level, )
 
         for level, group in self.description['order'].items():
             for names in group:
                 for name in names:
-                    self._levels[name] = level
                     if name not in self.dims:
                         if name not in self.description['dependents']:
                             self.dims[name] = (level, )
                         else:
                             d = set()
                             for n in self.description['dependents'][name]:
                                 d.update(self.dims[n])
                             self.dims[name] = tuple(sorted(d))
 
         if self.is_local_record():
             self.database = Path(self.database)
             self._file = random_path(self.database / 'objects')
             self._file.parent.mkdir(parents=True, exist_ok=True)
 
+    def __getstate__(self) -> dict:
+        return {
+            'id': self.id,
+            'database': self.database,
+            'description': self.description,
+            '_keys': self._keys,
+            '_items': self._items,
+            '_index': self._index,
+            '_pos': self._pos,
+            '_last_vars': self._last_vars,
+            'independent_variables': self.independent_variables,
+            'constants': self.constants,
+            'dims': self.dims,
+        }
+
+    def __setstate__(self, state: dict):
+        self.id = state['id']
+        self.database = state['database']
+        self.description = state['description']
+        self._keys = state['_keys']
+        self._items = state['_items']
+        self._index = state['_index']
+        self._pos = state['_pos']
+        self._last_vars = state['_last_vars']
+        self.independent_variables = state['independent_variables']
+        self.constants = state['constants']
+        self.dims = state['dims']
+        self._file = None
+
     def is_local_record(self):
         return not self.is_cache_record() and not self.is_remote_record()
 
     def is_cache_record(self):
         return self.database is None
 
     def is_remote_record(self):
@@ -197,43 +299,54 @@
 
     def __del__(self):
         self.flush()
 
     def __getitem__(self, key):
         return self.get(key)
 
-    def get(self, key, default=_notgiven, buffer_to_array=True):
+    def get(self, key, default=_notgiven, buffer_to_array=True, slice=None):
         if self.is_remote_record():
             with ZMQContextManager(zmq.DEALER,
                                    connect=self.database) as socket:
                 socket.send_pyobj({
                     'method': 'record_getitem',
                     'record_id': self.id,
                     'key': key
                 })
                 ret = socket.recv_pyobj()
-                if isinstance(ret, BufferList) and buffer_to_array:
-                    return ret.array()
+                if isinstance(ret, BufferList):
+                    socket.send_pyobj({
+                        'method': 'bufferlist_slice',
+                        'record_id': self.id,
+                        'key': key,
+                        'slice': slice
+                    })
+                    lst = socket.recv_pyobj()
+                    ret._list = lst
+                    ret._slice = slice
+                    if buffer_to_array:
+                        return ret.array()
+                    else:
+                        ret._database = self.database
+                        return ret
                 else:
                     return ret
         else:
             if default is _notgiven:
                 d = self._items.get(key)
             else:
                 d = self._items.get(key, default)
             if isinstance(d, BufferList):
+                if isinstance(d.file, str):
+                    d.file = self._file.parent.parent.parent.parent / d.file
+                d._slice = slice
                 if buffer_to_array:
                     return d.array()
                 else:
-                    ret = BufferList()
-                    ret._pos = d.pos()
-                    ret._value = d.value()
-                    ret.lu = d.lu
-                    ret.rd = d.rd
-                    return ret
+                    return d
             else:
                 return d
 
     def keys(self):
         if self.is_remote_record():
             with ZMQContextManager(zmq.DEALER,
                                    connect=self.database) as socket:
@@ -247,16 +360,15 @@
 
     def append(self, level, step, position, variables):
         if level < 0:
             self.flush()
             return
 
         for key in set(variables.keys()) - self._last_vars:
-            if key not in self._levels:
-                self._levels[key] = level
+            if key not in self.dims:
                 self.dims[key] = tuple(range(level + 1))
 
         self._last_vars = set(variables.keys())
         self._keys.update(variables.keys())
 
         if level >= len(self._pos):
             l = level + 1 - len(self._pos)
@@ -272,46 +384,47 @@
             self._pos = self._pos[:level + 1]
             self._index[-1] = step + 1
             self._pos[-1] = position
             pos = tuple(self._pos)
             self._pos[-1] += 1
 
         for key, value in variables.items():
-            if level == self._levels[key]:
+            if self.dims[key] == ():
+                if key not in self._items:
+                    self._items[key] = value
+            elif level == self.dims[key][-1]:
                 if key not in self._items:
                     if self.is_local_record():
-                        f1 = random_path(self.database / 'objects')
-                        f1.parent.mkdir(parents=True, exist_ok=True)
-                        f2 = random_path(self.database / 'objects')
-                        f2.parent.mkdir(parents=True, exist_ok=True)
-                        self._items[key] = BufferList(f1, f2)
+                        bufferlist_file = random_path(self.database /
+                                                      'objects')
+                        bufferlist_file.parent.mkdir(parents=True,
+                                                     exist_ok=True)
+                        self._items[key] = BufferList(bufferlist_file)
                     else:
                         self._items[key] = BufferList()
                     self._items[key].lu = pos
                     self._items[key].rd = tuple([i + 1 for i in pos])
                     self._items[key].append(pos, value, self.dims[key])
                 elif isinstance(self._items[key], BufferList):
                     self._items[key].append(pos, value, self.dims[key])
-            elif self._levels[key] == -1 and key not in self._items:
-                self._items[key] = value
 
     def flush(self):
         if self.is_remote_record() or self.is_cache_record():
             return
 
         for key, value in self._items.items():
             if isinstance(value, BufferList):
                 value.flush()
 
         with open(self._file, 'wb') as f:
             dill.dump(self, f)
 
     def __repr__(self):
         return f"<Record: id={self.id} app={self.description['app']}, keys={self.keys()}>"
-    
+
     # def _repr_html_(self):
     #     return f"""
     #     <h3>Record: id={self.id}, app={self.description['app']}</h3>
     #     <p>keys={self.keys()}</p>
     #     <p>dims={self.dims}</p>
     #     """
 
@@ -347,14 +460,15 @@
 def get_record(session: Session, id: int, datapath: Path) -> Record:
     if id not in record_cache:
         record_in_db = session.get(RecordInDB, id)
         record_in_db.atime = utcnow()
         path = datapath / 'objects' / record_in_db.file
         with open(path, 'rb') as f:
             record = dill.load(f)
+            record._file = path
     else:
         record = record_cache[id][1]
     clear_cache()
     record_cache[id] = time.time(), record
     return record
 
 
@@ -396,14 +510,20 @@
 async def handle(session: Session, request: Request, datapath: Path):
 
     msg = request.msg
 
     match request.method:
         case 'ping':
             await reply(request, 'pong')
+        case 'bufferlist_slice':
+            record = get_record(session, msg['record_id'], datapath)
+            bufferlist = record.get(msg['key'],
+                                    buffer_to_array=False,
+                                    slice=msg['slice'])
+            await reply(request, list(bufferlist.iter()))
         case 'record_create':
             description = dill.loads(msg['description'])
             await reply(request, record_create(session, description, datapath))
         case 'record_append':
             record_append(session, msg['record_id'], msg['level'], msg['step'],
                           msg['position'], msg['variables'], datapath)
         case 'record_description':
```

### Comparing `qulab-2.0.5/qulab/scan/scan.py` & `qulab-2.0.6/qulab/scan/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,18 +557,21 @@
 
         Args:
             awaitable: An awaitable object.
 
         Returns:
             Promise: A promise object.
         """
-        async with self._sem:
-            task = asyncio.create_task(self._await(awaitable))
-            self._task_queue.put_nowait(task)
-            return Promise(task)
+        if inspect.isawaitable(awaitable):
+            async with self._sem:
+                task = asyncio.create_task(self._await(awaitable))
+                self._task_queue.put_nowait(task)
+                return Promise(task)
+        else:
+            return awaitable
 
     async def _await(self, awaitable: Awaitable):
         async with self._sem:
             return await awaitable
 
 
 class Unpicklable:
```

### Comparing `qulab-2.0.5/qulab/scan/server.py` & `qulab-2.0.6/qulab/scan/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/scan/utils.py` & `qulab-2.0.6/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/__main__.py` & `qulab-2.0.6/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/backend/redis.py` & `qulab-2.0.6/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/base_dataset.py` & `qulab-2.0.6/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/chunk.py` & `qulab-2.0.6/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/dataset.py` & `qulab-2.0.6/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/file.py` & `qulab-2.0.6/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/__init__.py` & `qulab-2.0.6/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/config.py` & `qulab-2.0.6/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/file.py` & `qulab-2.0.6/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/ipy.py` & `qulab-2.0.6/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/models.py` & `qulab-2.0.6/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/record.py` & `qulab-2.0.6/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/report.py` & `qulab-2.0.6/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/models/tag.py` & `qulab-2.0.6/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/storage/storage.py` & `qulab-2.0.6/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/chat.py` & `qulab-2.0.6/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/device/basedevice.py` & `qulab-2.0.6/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/device/loader.py` & `qulab-2.0.6/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/device/utils.py` & `qulab-2.0.6/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.6/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/ipy_events.py` & `qulab-2.0.6/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/bencoder.py` & `qulab-2.0.6/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/cli.py` & `qulab-2.0.6/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/dhcp.py` & `qulab-2.0.6/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/dhcpd.py` & `qulab-2.0.6/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/kad.py` & `qulab-2.0.6/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/kcp.py` & `qulab-2.0.6/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/net/nginx.py` & `qulab-2.0.6/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/progress.py` & `qulab-2.0.6/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/exceptions.py` & `qulab-2.0.6/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/msgpack.py` & `qulab-2.0.6/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.6/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/rpc.py` & `qulab-2.0.6/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/serialize.py` & `qulab-2.0.6/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/server.py` & `qulab-2.0.6/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/socket.py` & `qulab-2.0.6/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/utils.py` & `qulab-2.0.6/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/sys/rpc/zmq_socket.py` & `qulab-2.0.6/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/__init__.py` & `qulab-2.0.6/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/__main__.py` & `qulab-2.0.6/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/_autoplot.py` & `qulab-2.0.6/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/plot_layout.py` & `qulab-2.0.6/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/plot_seq.py` & `qulab-2.0.6/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/qdat.py` & `qulab-2.0.6/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/qulab/visualization/widgets.py` & `qulab-2.0.6/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.5/setup.py` & `qulab-2.0.6/setup.py`

 * *Files identical despite different names*

