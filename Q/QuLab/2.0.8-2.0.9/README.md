# Comparing `tmp/qulab-2.0.8.tar.gz` & `tmp/qulab-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.8.tar", last modified: Wed May 29 02:39:46 2024, max compression
+gzip compressed data, was "qulab-2.0.9.tar", last modified: Wed May 29 08:23:38 2024, max compression
```

## Comparing `qulab-2.0.8.tar` & `qulab-2.0.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.817306 qulab-2.0.8/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-29 02:39:04.000000 qulab-2.0.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-29 02:39:04.000000 qulab-2.0.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 02:39:46.817069 qulab-2.0.8/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.816748 qulab-2.0.8/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-29 02:39:46.000000 qulab-2.0.8/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-29 02:39:04.000000 qulab-2.0.8/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-29 02:39:04.000000 qulab-2.0.8/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.800814 qulab-2.0.8/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.802204 qulab-2.0.8/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.803637 qulab-2.0.8/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    22163 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    28418 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.804478 qulab-2.0.8/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.805435 qulab-2.0.8/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.807655 qulab-2.0.8/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.808252 qulab-2.0.8/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.808757 qulab-2.0.8/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.809703 qulab-2.0.8/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.811639 qulab-2.0.8/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.813498 qulab-2.0.8/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.815645 qulab-2.0.8/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-29 02:39:04.000000 qulab-2.0.8/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-29 02:39:46.817347 qulab-2.0.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-29 02:39:04.000000 qulab-2.0.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.816002 qulab-2.0.8/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-29 02:39:04.000000 qulab-2.0.8/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 02:39:46.816422 qulab-2.0.8/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-29 02:39:04.000000 qulab-2.0.8/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.890203 qulab-2.0.9/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-29 08:22:58.000000 qulab-2.0.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-29 08:22:58.000000 qulab-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 08:23:38.889917 qulab-2.0.9/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.889557 qulab-2.0.9/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-29 08:22:58.000000 qulab-2.0.9/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-29 08:22:58.000000 qulab-2.0.9/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.871085 qulab-2.0.9/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.873479 qulab-2.0.9/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.875719 qulab-2.0.9/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    22532 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    28438 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.876766 qulab-2.0.9/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.876991 qulab-2.0.9/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.878541 qulab-2.0.9/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.879326 qulab-2.0.9/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.880799 qulab-2.0.9/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.881146 qulab-2.0.9/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.882844 qulab-2.0.9/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.886361 qulab-2.0.9/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.887854 qulab-2.0.9/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-29 08:23:38.890242 qulab-2.0.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-29 08:22:58.000000 qulab-2.0.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.887977 qulab-2.0.9/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-29 08:22:58.000000 qulab-2.0.9/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.889326 qulab-2.0.9/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-29 08:22:58.000000 qulab-2.0.9/tests/test_scan.py
```

### Comparing `qulab-2.0.8/LICENSE` & `qulab-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/PKG-INFO` & `qulab-2.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.8
+Version: 2.0.9
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.8/QuLab.egg-info/PKG-INFO` & `qulab-2.0.9/QuLab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.8
+Version: 2.0.9
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.8/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.9/QuLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/README.md` & `qulab-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/pyproject.toml` & `qulab-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/config.py` & `qulab-2.0.9/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/dataset.py` & `qulab-2.0.9/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/event_queue.py` & `qulab-2.0.9/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/mainwindow.py` & `qulab-2.0.9/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/monitor.py` & `qulab-2.0.9/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/ploter.py` & `qulab-2.0.9/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/qt_compat.py` & `qulab-2.0.9/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/monitor/toolbar.py` & `qulab-2.0.9/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/curd.py` & `qulab-2.0.9/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/expression.py` & `qulab-2.0.9/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/models.py` & `qulab-2.0.9/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/optimize.py` & `qulab-2.0.9/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/query_record.py` & `qulab-2.0.9/qulab/scan/query_record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/recorder.py` & `qulab-2.0.9/qulab/scan/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,16 @@
                     | tuple[slice | int | EllipsisType, ...]):
         return super().__getitem__(self._full_slice(slice_tuple))
 
 
 class Record():
 
     def __init__(self, id, database, description=None):
+        from .scan import OptimizeSpace
+
         self.id = id
         self.database = database
         self.description = description
         self._keys = set()
         self._items = {}
         self._index = []
         self._pos = []
@@ -232,30 +234,37 @@
         for name, value in self.description['consts'].items():
             if name not in self._items:
                 self._items[name] = value
             self.constants[name] = value
             self.dims[name] = ()
         for level, range_list in self.description['loops'].items():
             for name, iterable in range_list:
-                if isinstance(iterable, (np.ndarray, list, tuple, range)):
+                if isinstance(iterable, OptimizeSpace):
+                    self.dims[name] = tuple(range(level + 1))
+                    continue
+                elif isinstance(iterable, (np.ndarray, list, tuple, range)):
                     self._items[name] = iterable
                     self.independent_variables[name] = iterable
-                    self.dims[name] = (level, )
+                self.dims[name] = (level, )
 
         for level, group in self.description['order'].items():
             for names in group:
                 for name in names:
-                    if name not in self.dims:
-                        if name not in self.description['dependents']:
+                    if name not in self.description['dependents']:
+                        if name not in self.dims:
                             self.dims[name] = (level, )
-                        else:
-                            d = set()
-                            for n in self.description['dependents'][name]:
-                                d.update(self.dims[n])
+                    else:
+                        d = set()
+                        for n in self.description['dependents'][name]:
+                            d.update(self.dims[n])
+                        if name not in self.dims:
                             self.dims[name] = tuple(sorted(d))
+                        else:
+                            self.dims[name] = tuple(
+                                sorted(set(self.dims[name]) | d))
 
         if self.is_local_record():
             self.database = Path(self.database)
             self._file = random_path(self.database / 'objects')
             self._file.parent.mkdir(parents=True, exist_ok=True)
 
     def __getstate__(self) -> dict:
```

### Comparing `qulab-2.0.8/qulab/scan/scan.py` & `qulab-2.0.9/qulab/scan/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import copy
 import datetime
 import inspect
 import itertools
 import os
 import re
 import sys
 import uuid
@@ -707,26 +708,26 @@
         for name, space in loops:
             try:
                 description['total'][level] = min(description['total'][level],
                                                   len(space))
             except:
                 pass
 
-    dependents = description['dependents'].copy()
+    dependents = copy.deepcopy(description['dependents'])
 
     for level in levels:
         range_list = description['loops'].get(level, [])
         if level > 0:
             if f'#__loop_{level}' not in description['dependents']:
-                dependents[f'#__loop_{level}'] = []
-            dependents[f'#__loop_{level}'].append(f'#__loop_{level-1}')
+                dependents[f'#__loop_{level}'] = set()
+            dependents[f'#__loop_{level}'].add(f'#__loop_{level-1}')
         for name, _ in range_list:
             if name not in description['dependents']:
-                dependents[name] = []
-            dependents[name].append(f'#__loop_{level}')
+                dependents[name] = set()
+            dependents[name].add(f'#__loop_{level}')
 
     def _get_all_depends(key, graph):
         ret = set()
         if key not in graph:
             return ret
 
         for e in graph[key]:
```

### Comparing `qulab-2.0.8/qulab/scan/server.py` & `qulab-2.0.9/qulab/scan/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/scan/utils.py` & `qulab-2.0.9/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/__main__.py` & `qulab-2.0.9/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/backend/redis.py` & `qulab-2.0.9/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/base_dataset.py` & `qulab-2.0.9/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/chunk.py` & `qulab-2.0.9/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/dataset.py` & `qulab-2.0.9/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/file.py` & `qulab-2.0.9/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/__init__.py` & `qulab-2.0.9/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/config.py` & `qulab-2.0.9/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/file.py` & `qulab-2.0.9/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/ipy.py` & `qulab-2.0.9/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/models.py` & `qulab-2.0.9/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/record.py` & `qulab-2.0.9/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/report.py` & `qulab-2.0.9/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/models/tag.py` & `qulab-2.0.9/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/storage/storage.py` & `qulab-2.0.9/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/chat.py` & `qulab-2.0.9/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/device/basedevice.py` & `qulab-2.0.9/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/device/loader.py` & `qulab-2.0.9/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/device/utils.py` & `qulab-2.0.9/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.9/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/ipy_events.py` & `qulab-2.0.9/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/bencoder.py` & `qulab-2.0.9/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/cli.py` & `qulab-2.0.9/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/dhcp.py` & `qulab-2.0.9/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/dhcpd.py` & `qulab-2.0.9/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/kad.py` & `qulab-2.0.9/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/kcp.py` & `qulab-2.0.9/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/net/nginx.py` & `qulab-2.0.9/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/progress.py` & `qulab-2.0.9/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/exceptions.py` & `qulab-2.0.9/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/msgpack.py` & `qulab-2.0.9/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.9/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/rpc.py` & `qulab-2.0.9/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/serialize.py` & `qulab-2.0.9/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/server.py` & `qulab-2.0.9/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/socket.py` & `qulab-2.0.9/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/utils.py` & `qulab-2.0.9/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/sys/rpc/zmq_socket.py` & `qulab-2.0.9/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/__init__.py` & `qulab-2.0.9/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/__main__.py` & `qulab-2.0.9/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/_autoplot.py` & `qulab-2.0.9/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/plot_layout.py` & `qulab-2.0.9/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/plot_seq.py` & `qulab-2.0.9/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/qdat.py` & `qulab-2.0.9/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/qulab/visualization/widgets.py` & `qulab-2.0.9/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.8/setup.py` & `qulab-2.0.9/setup.py`

 * *Files identical despite different names*

