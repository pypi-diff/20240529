# Comparing `tmp/ftio-hpc-0.0.3.tar.gz` & `tmp/ftio_hpc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftio-hpc-0.0.3.tar", last modified: Wed Feb 28 15:25:26 2024, max compression
+gzip compressed data, was "ftio_hpc-0.0.4.tar", last modified: Tue May 28 22:21:39 2024, max compression
```

## Comparing `ftio-hpc-0.0.3.tar` & `ftio_hpc-0.0.4.tar`

### file list

```diff
@@ -1,100 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.457426 ftio-hpc-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.457426 ftio-hpc-0.0.3/examples/txt/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/examples/txt/custom_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.457426 ftio-hpc-0.0.3/ftio/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.457426 ftio-hpc-0.0.3/ftio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/cli/ftio_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/cli/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.461426 ftio-hpc-0.0.3/ftio/freq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/_dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/_wavelet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15968 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/anomaly_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/anomaly_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/discretize.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/freq_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/freq_html.py
--rw-r--r--   0 runner    (1001) docker     (127)    49479 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/freq_plot_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/freq/perodicity_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.465426 ftio-hpc-0.0.3/ftio/parse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/custom_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9692 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/darshan_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/ftio_to_extrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/input_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/msgpack_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/overlap_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/parse_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/parse_darshan.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/parse_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/parse_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/parse_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/percent.py
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/recorder_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/scales.py
--rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/simrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/time_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/parse/txt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.465426 ftio-hpc-0.0.3/ftio/plot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.465426 ftio-hpc-0.0.3/ftio/plot/dash_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.465426 ftio-hpc-0.0.3/ftio/plot/dash_files/callback_files/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/callback_files/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/callback_files/io_mode_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.465426 ftio-hpc-0.0.3/ftio/plot/dash_files/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/constants/graph_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/constants/id.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/constants/io_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/constants/legend_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/dash_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/dash_files/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    80656 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/plot_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/plot_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/print_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/stack_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/plot/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/ftio/prediction/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/async_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/prediction/unify_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/ftio/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/util/ioparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/ftio/util/ioplot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/ftio_hpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-28 15:25:26.000000 ftio-hpc-0.0.3/ftio_hpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:25:26.469426 ftio-hpc-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/test/test_ftio.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/test/test_ioparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-28 15:25:18.000000 ftio-hpc-0.0.3/test/test_ioplot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.776329 ftio_hpc-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 22:21:34.000000 ftio_hpc-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-05-28 22:21:39.776329 ftio_hpc-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2024-05-28 22:21:34.000000 ftio_hpc-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.756329 ftio_hpc-0.0.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/examples/API/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/examples/API/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.756329 ftio_hpc-0.0.4/examples/custom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/examples/custom/txt/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/examples/custom/txt/custom_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/ftio/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.756329 ftio_hpc-0.0.4/ftio/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/ftio/api/gekkoFs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/gekkoFs/ftio_gekko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/gekkoFs/parse_gekko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/gekkoFs/predictor_gekko.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/gekkoFs/predictor_gekko_zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/ftio/api/metric_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/metric_proxy/parse_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/api/metric_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.760329 ftio_hpc-0.0.4/ftio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/cli/ftio_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/cli/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.764329 ftio_hpc-0.0.4/ftio/freq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/_dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/_wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15968 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/anomaly_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/anomaly_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/discretize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/freq_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/freq_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49352 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/freq_plot_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/perodicity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/freq/time_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.768329 ftio_hpc-0.0.4/ftio/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/custom_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9692 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/darshan_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/ftio_to_extrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/input_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/msgpack_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/overlap_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_darshan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_jsonl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/parse_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18973 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/recorder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/scales.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/simrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/time_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/txt_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/parse/zmq_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.768329 ftio_hpc-0.0.4/ftio/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.768329 ftio_hpc-0.0.4/ftio/plot/dash_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.768329 ftio_hpc-0.0.4/ftio/plot/dash_files/callback_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/callback_files/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/callback_files/io_mode_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.768329 ftio_hpc-0.0.4/ftio/plot/dash_files/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/constants/graph_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/constants/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/constants/io_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/constants/legend_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/dash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/dash_files/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80679 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/plot_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/plot_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/print_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/stack_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/plot/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.772329 ftio_hpc-0.0.4/ftio/post/
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/post/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.772329 ftio_hpc-0.0.4/ftio/prediction/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/async_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/probability_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/processes_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/prediction/unify_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.772329 ftio_hpc-0.0.4/ftio/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/util/ioparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/ftio/util/ioplot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.776329 ftio_hpc-0.0.4/ftio_hpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16635 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 22:21:39.000000 ftio_hpc-0.0.4/ftio_hpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:21:39.776329 ftio_hpc-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:21:39.772329 ftio_hpc-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/test/test_ftio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/test/test_ioparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 22:21:35.000000 ftio_hpc-0.0.4/test/test_ioplot.py
```

### Comparing `ftio-hpc-0.0.3/LICENSE` & `ftio_hpc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/PKG-INFO` & `ftio_hpc-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftio-hpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Frequency Techniques for I/O
 Author-email: Ahmad Tarraf <ahmad.tarraf@tu-darmstadt.de>
 Maintainer-email: Ahmad Tarraf <ahmad.tarraf@tu-darmstadt.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Parallel Programming @ TU Darmstadt
         
@@ -54,14 +54,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
+Requires-Dist: zmq
 Requires-Dist: numba
 Requires-Dist: darshan
 Requires-Dist: fastdtw
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: jsonlines
 Requires-Dist: plotly
@@ -69,14 +70,15 @@
 Requires-Dist: kneed
 Requires-Dist: PyWavelets
 Requires-Dist: trace_updater
 Requires-Dist: plotly_resampler
 Requires-Dist: msgpack
 Requires-Dist: rich
 Requires-Dist: dash_extensions
+Requires-Dist: pytest
 
 <!-- # FTIO -->
 ![GitHub Release](https://img.shields.io/github/v/release/tuda-parallel/FTIO)
 ![GitHub Release Date](https://img.shields.io/github/release-date/tuda-parallel/FTIO)
 ![](https://img.shields.io/github/last-commit/tuda-parallel/FTIO)
 ![contributors](https://img.shields.io/github/contributors/tuda-parallel/FTIO)
 ![issues](https://img.shields.io/github/issues/tuda-parallel/FTIO)
@@ -233,15 +235,15 @@
 
 Several flags can be specified. The most relevant settings are:
 
 | Flag                        | Description|
 |---                          | --- |
 |file                         | file, file list (file 0 ... file n), folder, or folder list (folder 0.. folder n) containing traces  (positional argument)|
 |-h, --help                   | show this help message and exit|
-|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: async_write, async_read, sync_write, sync_read|
+|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: write_async, read_async, write_sync, read_sync|
 |-r RENDER, --render RENDER   | specifies how the plots are rendered. Either dynamic (default) or static|
 |-f FREQ, --freq FREQ         | specifies the sampling rate with which the continuous signal is discretized (default=10Hz). This directly affects the highest captured frequency (Nyquist). The value is specified in Hz. In case this value is set to -1, the auto mode is launched which sets the sampling frequency automatically to the smallest change in the bandwidth detected. Note that the lowest allowed frequency in the auto mode is 2000 Hz|
 |-ts TS, --ts TS              | Modifies the start time of the examined time window
 |-te TE, --te TE              | Modifies the end time of the examined time window
 |-tr TRANSFORMATION, --transformation TRANSFORMATION| specifies the frequency technique to use. Supported modes are: dft (default), wave_disc, and wave_cont|
 |-e ENGINE, --engine ENGINE   | specifies the engine used to display the figures. Either plotly (default) or mathplotlib can be used. Plotly is used to generate interactive plots as HTML files. Set this value to no if you do not want to generate plots
 |-o OUTLIER, --outlier OUTLIER| outlier detection method: Z-score (default), DB-Scan, Isolation_forest, or LOF|
@@ -294,15 +296,15 @@
 
 <p align="right"><a href="#ftio">⬆</a></p>
 
 ## License
 
 ![license][license.bedge]
 
-Distributed under the BSD 3-Clause License. See [LISCENCE](./LICENSE) for more information.
+Distributed under the BSD 3-Clause License. See [LICENCE](./LICENSE) for more information.
 <p align="right"><a href="#ftio">⬆</a></p>
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
 
 Authors:
```

### Comparing `ftio-hpc-0.0.3/README.md` & `ftio_hpc-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 Several flags can be specified. The most relevant settings are:
 
 | Flag                        | Description|
 |---                          | --- |
 |file                         | file, file list (file 0 ... file n), folder, or folder list (folder 0.. folder n) containing traces  (positional argument)|
 |-h, --help                   | show this help message and exit|
-|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: async_write, async_read, sync_write, sync_read|
+|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: write_async, read_async, write_sync, read_sync|
 |-r RENDER, --render RENDER   | specifies how the plots are rendered. Either dynamic (default) or static|
 |-f FREQ, --freq FREQ         | specifies the sampling rate with which the continuous signal is discretized (default=10Hz). This directly affects the highest captured frequency (Nyquist). The value is specified in Hz. In case this value is set to -1, the auto mode is launched which sets the sampling frequency automatically to the smallest change in the bandwidth detected. Note that the lowest allowed frequency in the auto mode is 2000 Hz|
 |-ts TS, --ts TS              | Modifies the start time of the examined time window
 |-te TE, --te TE              | Modifies the end time of the examined time window
 |-tr TRANSFORMATION, --transformation TRANSFORMATION| specifies the frequency technique to use. Supported modes are: dft (default), wave_disc, and wave_cont|
 |-e ENGINE, --engine ENGINE   | specifies the engine used to display the figures. Either plotly (default) or mathplotlib can be used. Plotly is used to generate interactive plots as HTML files. Set this value to no if you do not want to generate plots
 |-o OUTLIER, --outlier OUTLIER| outlier detection method: Z-score (default), DB-Scan, Isolation_forest, or LOF|
@@ -218,15 +218,15 @@
 
 <p align="right"><a href="#ftio">⬆</a></p>
 
 ## License
 
 ![license][license.bedge]
 
-Distributed under the BSD 3-Clause License. See [LISCENCE](./LICENSE) for more information.
+Distributed under the BSD 3-Clause License. See [LICENCE](./LICENSE) for more information.
 <p align="right"><a href="#ftio">⬆</a></p>
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
 
 Authors:
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_y3nx9ppa_/tmpal3tdwgc_TarContainer/0/3.md", line 19, column 55: Levels of opening and closing headings don't match*

```diff
@@ -91,16 +91,16 @@
 Isolation forest, peak detection, or LOF)â 2. Optionally: Autocorrelation +
 Peak detection (`-c` flag) 3. If step 2. is performed, the results from both
 predictions aer merged automatically Several flags can be specified. The most
 relevant settings are: | Flag | Description| |--- | --- | |file | file, file
 list (file 0 ... file n), folder, or folder list (folder 0.. folder n)
 containing traces (positional argument)| |-h, --help | show this help message
 and exit| |-m MODE, --mode MODE | if the trace file contains several I/O modes,
-a specific mode can be selected. Supported modes are: async_write, async_read,
-sync_write, sync_read| |-r RENDER, --render RENDER | specifies how the plots
+a specific mode can be selected. Supported modes are: write_async, read_async,
+write_sync, read_sync| |-r RENDER, --render RENDER | specifies how the plots
 are rendered. Either dynamic (default) or static| |-f FREQ, --freq FREQ |
 specifies the sampling rate with which the continuous signal is discretized
 (default=10Hz). This directly affects the highest captured frequency (Nyquist).
 The value is specified in Hz. In case this value is set to -1, the auto mode is
 launched which sets the sampling frequency automatically to the smallest change
 in the bandwidth detected. Note that the lowest allowed frequency in the auto
 mode is 2000 Hz| |-ts TS, --ts TS | Modifies the start time of the examined
@@ -142,15 +142,15 @@
 changes (`git commit -m 'Add some AmazingFeature'`) 4. Push to the branch (`git
 push origin feature/AmazingFeature`) 5. Open a pull request
                                                                             _â_¬_
 ## Contact [![][parallel.bedge]][parallel_website] - Ahmad Tarraf:
 tu-darmstadt.de>
                                                                             _â_¬_
 ## License ![license][license.bedge] Distributed under the BSD 3-Clause
-License. See [LISCENCE](./LICENSE) for more information.
+License. See [LICENCE](./LICENSE) for more information.
                                                                             _â_¬_
 ## Acknowledgments Authors: - Ahmad Tarraf This work is a result of cooperation
 between the Technical University of Darmstadt and INRIA in scope of the
 [EuroHPC ADMIRE project](https://admire-eurohpc.eu/).
                                                                             _â_¬_
 ## Citation ``` @inproceedings{Tarraf_Bandet_Boito_Pallez_Wolf_2024, author=
 {Tarraf, Ahmad and Bandet, Alexis and Boito, Francieli and Pallez, Guillaume
```

### Comparing `ftio-hpc-0.0.3/examples/txt/custom_input.py` & `ftio_hpc-0.0.4/examples/custom/txt/custom_input.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/__init__.py` & `ftio_hpc-0.0.4/ftio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # Copyright (c) 2023-2024, Technical University of Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of a BSD-style license.
 # See the LICENSE file in the base directory for details.
 
 __title__ = "FTIO"
-__version__ = "0.0.3"
-__liscence__ = "BSD 3"
+__version__ = "0.0.4"
+__license__ = "BSD 3"
 __description__ = "FTIO: Capturing Periodic I/O Using Frequency Techniques"
 __copyright__ = "Copyright (c) 2023-2024 Technical University of Darmstadt, Darmstadt, Germany"
 __documentation_link__ = f"https://github.com/tuda-parallel/FTIO/tree/v{__version__}/docs"
 __current_version_api__ = "https://pypi.org/pypi/extrap/json"
 __developed_by_html__ = 'FTIO is developed by <a href="https://www.parallel.informatik.tu-darmstadt.de/">' 
 __support_email__ = "ahmad.tarraf@tu-darmstadt.de"
 __repo__='https://github.com/tuda-parallel/FTIO'
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # This file is part of the FTIO software # # Copyright (c) 2023-2024, Technical
 University of Darmstadt, Germany # # This software may be modified and
 distributed under the terms of a BSD-style license. # See the LICENSE file in
-the base directory for details. __title__ = "FTIO" __version__ = "0.0.3"
-__liscence__ = "BSD 3" __description__ = "FTIO: Capturing Periodic I/O Using
+the base directory for details. __title__ = "FTIO" __version__ = "0.0.4"
+__license__ = "BSD 3" __description__ = "FTIO: Capturing Periodic I/O Using
 Frequency Techniques" __copyright__ = "Copyright (c) 2023-2024 Technical
 University of Darmstadt, Darmstadt, Germany" __documentation_link__ = f"https:/
 /github.com/tuda-parallel/FTIO/tree/v{__version__}/docs"
 __current_version_api__ = "https://pypi.org/pypi/extrap/json"
 __developed_by_html__ = 'FTIO is developed by _'_ _____s_u_p_p_o_r_t___e_m_a_i_l_____ _=
 _"_a_h_m_a_d_._t_a_r_r_a_f_@_t_u_-_d_a_r_m_s_t_a_d_t_._d_e_"_ _____r_e_p_o_____=_'_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_u_d_a_-_p_a_r_a_l_l_e_l_/_F_T_I_O_'
```

### Comparing `ftio-hpc-0.0.3/ftio/cli/ftio_core.py` & `ftio_hpc-0.0.4/ftio/cli/ftio_core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,127 @@
 """This functions calculates the frequency based on the input data provided. 
-Currently darshan, recorder, and traces generated with our internal tool are supported. 
+Currently Darshan, recorder, and traces generated with our internal tool are supported. 
 
-call ftio -h to see list of suppoerted argurmnts. 
+call ftio -h to see list of supported arguments. 
 """
 
 from __future__ import annotations
 import time
 import sys
 import numpy as np
 from rich.console import Group
 from rich.panel import Panel
 from ftio.parse.scales import Scales
 from ftio.parse.extract import get_time_behavior
 from ftio.freq.freq_plot_core import convert_and_plot
-from ftio.freq.helper import get_mode, MyConsole
+from ftio.freq.helper import get_mode, MyConsole, merge_results
 from ftio.freq.autocorrelation import find_autocorrelation
 from ftio.freq.anomaly_detection import outlier_detection
 from ftio.freq.discretize import sample_data
-from ftio.freq._wavelet import wavelet_disc, plot_wave_disc, wavelet_cont, plot_wave_cont#, welch
+from ftio.freq._wavelet import (
+    wavelet_disc,
+    plot_wave_disc,
+    wavelet_cont,
+    plot_wave_cont,
+)  # , welch
 from ftio.freq._dft import dft, prepare_plot_dfs, display_prediction, precision_dft
 from ftio.prediction.unify_predictions import merge_predictions
+from ftio.freq.time_window import data_in_time_window
+
 
 CONSOLE = MyConsole()
 
 
-def main(cmd_input: list[str]):# -> dict[Any, Any]:
-    """Pass varibales and call main_core. The extraction of the traces
+def main(cmd_input: list[str], msgs=None):  # -> dict[Any, Any]:
+    """Pass variables and call main_core. The extraction of the traces
     and the parsing of the arguments is done in this function.
     """
+    # prepare data
     start = time.time()
-    data = Scales(cmd_input)
+    data = Scales(cmd_input, msgs)
     data.get_data()
     args = data.args
     df = get_mode(data, args.mode)
+    data = get_time_behavior(df)
     CONSOLE.set(args.verbose)
     CONSOLE.print(f"\n[cyan]Data imported in:[/] {time.time() - start:.2f} s")
     CONSOLE.print(f"[cyan]Frequency Analysis:[/] {args.transformation.upper()}")
     CONSOLE.print(f"[cyan]Mode:[/] {args.mode}")
 
-    data = get_time_behavior(df)
+    # get prediction
+    prediction, dfs = core(data, args)
+
+    # plot and print info
+    convert_and_plot(data, dfs, args)
+    display_prediction(cmd_input, prediction)
+    CONSOLE.print(f"[cyan]Total elapsed time:[/] {time.time()-start:.3f} s\n")
+
+    return prediction, args
+
+
+def core(data: list[dict], args) -> tuple[dict, list]:
+    """ftio core function
+
+    Args:
+        data: {
+            "time": time (np.ndarray),
+            "bandwidth": bandwidth (np.ndarray),
+            "total_bytes": total_bytes (int),
+            "ranks": i (int)
+            }
+        args (_type_): argparse
+
+    Returns:
+        tuple[dict,list[list[float]]]: _description_
+    """
+    # init
     prediction = {}
     share = {}
-    dfs = [[], [], [], []]
+    dfs_out = [[],[],[],[]]
+
+    # get predictions
     for sim in data:
-        # perform frequency anylsis (dft/wavelet)
+        # Perform frequency analysis (dft/wavelet)
         prediction_dft, dfs, share = freq_analysis(args, sim)
         # Perform autocorrelation if args.autocorrelation is true + Merge the results into a single prediction
         prediction_auto = find_autocorrelation(args, sim, share)
+        # Merge results
         prediction = merge_predictions(args, prediction_dft, prediction_auto)
+        # merge plots
+        dfs_out = merge_results(dfs_out, dfs)
 
-    convert_and_plot(data, dfs, args)
-    CONSOLE.print(f"[cyan]Total elapsed time:[/] {time.time()-start:.3f} s\n")
-    display_prediction(cmd_input, prediction)
-    return prediction, args
+    return prediction, dfs_out
 
 
 def freq_analysis(args, data: dict) -> tuple[dict, tuple[list, list, list, list], dict]:
-    """Discription:
+    """Description:
     performs sampling and that frequency technique (dft, wave_cont, or wave_disc),
     followed by creating
-    a datframe with the information for plotting
+    a dataframe with the information for plotting
 
     Args:
         args (argparse): see io_args.py
-        data (dict): containing 4 fields:
+        data (dict[str,np.ndarray]): containing 4 fields:
             1. bandwidth (np.array): bandwidth array
-            2. time (np.array): time array indicating when bandwidth time points chaged
+            2. time (np.array): time array indicating when bandwidth time points changed
             3. total_bytes (int): total transferred bytes
             4. ranks: number of ranks that did I/O
 
     Raises:
         Exception: _description_
 
     Returns:
-        dict: Conating the predicition with the following fields:
-            1. dict:  Containing result of prediction includeing: 
+        dict: Containing the prediction with the following fields:
+            1. dict:  Containing result of prediction including:
                 "dominant_freq" (list), "conf" (np.array), "t_start" (int), "t_end" (int), "total_bytes" (int).
             2. tuple[list, list, list, list]: for plot
-            3. dict: Conating sampled data including:
+            3. dict: Containing sampled data including:
                 b_sampled, "freq", "t_start", "t_end", "total_bytes"
     """
+    #! Init
     k = 0
     share = {}
     df_out = [[], [], [], []]
     prediction = {
         "source": {args.transformation},
         "dominant_freq": [],
         "conf": [],
@@ -93,122 +131,125 @@
         "freq": 0,
         "ranks": 0,
     }
     bandwidth = data["bandwidth"] if "bandwidth" in data else np.array([])
     time_b = data["time"] if "time" in data else np.array([])
     total_bytes = data["total_bytes"] if "total_bytes" in data else 0
     ranks = data["ranks"] if "ranks" in data else 0
-    text = f"Ranks: [cyan]{ranks}[/]\n"
-    ignored_bytes = total_bytes
 
-    if args.ts:  # shorten data
-        indecies = np.where(time_b >= args.ts)
-        time_b = time_b[indecies]
-        bandwidth = bandwidth[indecies]
-        total_bytes = np.sum(
-            bandwidth * (np.concatenate([time_b[1:], time_b[-1:]]) - time_b)
-        )
-        text += f"[green]Start time set to {args.ts:.2f}[/] s\n"
-    else:
-        text += f"Start time: [cyan]{time_b[0]:.2f}[/] s \n"
-
-    if args.te:  # shorten data
-        indecies = np.where(time_b <= args.te)
-        time_b = time_b[indecies]
-        bandwidth = bandwidth[indecies]
-        total_bytes = np.sum(
-            bandwidth * (np.concatenate([time_b[1:], time_b[-1:]]) - time_b)
-        )
-        text += f"[green]End time set to {args.te:.2f}[/] s\n"
-    else:
-        text += f"End time: [cyan]{time_b[-1]:.2f}[/] s\n"
-
-    ignored_bytes = (ignored_bytes - total_bytes)
-    text += f"Total bytes: [cyan]{total_bytes:.2e} bytes[/]\n"
-    text += f"Ignored bytes: [cyan]{ignored_bytes:.2e} bytes[/]\n"
+    #! extract relevant data
+    bandwidth, time_b, text = data_in_time_window(
+        args, bandwidth, time_b, total_bytes, ranks
+    )
+
+    #! Discretize signal: sample the bandwidth
     tik = time.time()
     CONSOLE.print("[cyan]Executing:[/] Discretization\n")
-
-    #! Discretize signal
-    # sample the bandwidth bandwidth
-    b_sampled, freq, text_disc = sample_data(bandwidth, time_b, args.freq)  
-    CONSOLE.print(Panel.fit(text_disc, style="white", border_style='yellow', title="Discretization", title_align='left'))
+    b_sampled, freq, text_disc = sample_data(bandwidth, time_b, args.freq)
+    CONSOLE.print(
+        Panel.fit(
+            text_disc,
+            style="white",
+            border_style="yellow",
+            title="Discretization",
+            title_align="left",
+        )
+    )
     CONSOLE.print(f"\n[cyan]Discretization finished:[/] {time.time() - tik:.3f} s")
-    CONSOLE.print(f"[cyan]Executing:[/] {args.transformation.upper()} + {args.outlier}\n")
+
+    #! Perform transformation
+    CONSOLE.print(
+        f"[cyan]Executing:[/] {args.transformation.upper()} + {args.outlier}\n"
+    )
     tik = time.time()
 
-    #! Choose Method
+    ##! Choose Method
     if "dft" in args.transformation:
-        # calculate DFT
+        ##? calculate DFT
         X = dft(b_sampled)
         N = len(X)
-        amp = abs(X)  
-
-        # welch(bandwidth,freq)
+        amp = abs(X)
         freq_arr = freq * np.arange(0, N) / N
         phi = np.arctan2(X.imag, X.real)
         conf = np.zeros(len(amp))
+        # welch(bandwidth,freq)
 
-        # Find dominant frequency
+        ##? Find dominant frequency
         (
             dominant_index,
             conf[1 : int(len(amp) / 2) + 1],
             outlier_text,
         ) = outlier_detection(amp, freq_arr, args)
 
+        ##? ignore DC offset
         conf[0] = np.inf
         if len(amp) % 2 == 0:
             conf[int(len(amp) / 2) + 1 :] = np.flip(conf[1 : int(len(amp) / 2)])
         else:
             conf[int(len(amp) / 2) + 1 :] = np.flip(conf[1 : int(len(amp) / 2) + 1])
 
+        ##? Assign data
         prediction["dominant_freq"] = freq_arr[dominant_index]
-        prediction["conf"] = conf[dominant_index]
-        prediction["t_start"] = time_b[0]
-        prediction["t_end"] = time_b[-1]
-        prediction["total_bytes"] = total_bytes
-        prediction["freq"] = freq
-        prediction["ranks"] = ranks
-
+        prediction["conf"]          = conf[dominant_index]
+        prediction["amp"]           = amp[dominant_index]
+        prediction["phi"]           = phi[dominant_index]
+        prediction["t_start"]       = time_b[0]
+        prediction["t_end"]         = time_b[-1]
+        prediction["freq"]          = freq
+        prediction["ranks"]         = ranks
+        prediction["total_bytes"]   = total_bytes
+
+        #? save up to n_freq from the top candidates
+        if args.n_freq > 0:
+            #TODO use amp instead of conf
+            arr = amp[0:int(np.ceil(len(amp)/2))]
+            top_candidates = np.argsort(-arr) # from max to min
+            n_freq = int(min(len(arr),args.n_freq))
+            prediction["top_freq"] = {
+                "freq": freq_arr[top_candidates[0:n_freq]],
+                "conf": conf[top_candidates[0:n_freq]],
+                "amp":  amp[top_candidates[0:n_freq]],
+                "phi":  phi[top_candidates[0:n_freq]]
+            }
+            
         if args.autocorrelation:
-            share["b_sampled"] = b_sampled
-            share["freq"] = freq
-            share["t_start"] = prediction["t_start"]
-            share["t_end"] = prediction["t_end"]
+            share["b_sampled"]   = b_sampled
+            share["freq"]        = freq
+            share["t_start"]     = prediction["t_start"]
+            share["t_end"]       = prediction["t_end"]
             share["total_bytes"] = prediction["total_bytes"]
 
         precision_text = ""
         # precision_text = precision_dft(
         #     amp, phi, dominant_index, b_sampled, time_b[0] + np.arange(0, N) * 1 / freq, freq_arr, args.engine
         # )
 
         text = Group(text, outlier_text, precision_text[:-1])
 
-        if any(x in args.engine for x in ["mat","plot"]):
+        if any(x in args.engine for x in ["mat", "plot"]):
             df_out = prepare_plot_dfs(
                 k,
                 freq,
                 freq_arr,
                 conf,
                 dominant_index,
                 amp,
                 phi,
                 b_sampled,
                 time_b,
                 ranks,
-                N,
                 bandwidth,
             )
         k += 1
 
     elif "wave_disc" in args.transformation:
-        # discrete wavlet decomposition:
+        # discrete wavelet decomposition:
         # https://edisciplinas.usp.br/pluginfile.php/4452162/mod_resource/content/1/V1-Parte%20de%20Slides%20de%20p%C3%B3sgrad%20PSI5880_PDF4%20em%20Wavelets%20-%202010%20-%20Rede_AIASYB2.pdf
         # https://www.youtube.com/watch?v=hAQQwvKsWCY&ab_channel=NathanKutz
-        print("    '-> \033[1;32mPerforming discret wavelet decomposition\033[1;0m")
+        print("    '-> \033[1;32mPerforming discrete wavelet decomposition\033[1;0m")
         wavelet = "db1"  # dmey might be better https://pywavelets.readthedocs.io/en/latest/ref/wavelets.html
         # wavelet = 'haar' # dmey might be better https://pywavelets.readthedocs.io/en/latest/ref/wavelets.html
         coffs = wavelet_disc(b_sampled, wavelet, args.level)
         cc, f = plot_wave_disc(
             b_sampled, coffs, time_b, args.freq, args.level, wavelet, bandwidth
         )
         for fig in f:
@@ -225,16 +266,16 @@
                 "ranks": ranks,
             }
             freq_analysis(args, tmp)
 
         sys.exit()
 
     elif "wave_cont" in args.transformation:
-        # Continous wavelets
-        print("    '-> \033[1;32mPerforming discret wavelet decomposition\033[1;0m")
+        # Continuous wavelets
+        print("    '-> \033[1;32mPerforming discrete wavelet decomposition\033[1;0m")
         wavelet = "morl"
         # wavelet = 'cmor'
         # wavelet = 'mexh'
         [coefficients, frequencies, scale] = wavelet_cont(
             b_sampled, wavelet, args.level, args.freq
         )
         fig = plot_wave_cont(
```

### Comparing `ftio-hpc-0.0.3/ftio/cli/predictor.py` & `ftio_hpc-0.0.4/ftio/cli/predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """This functions performs the prediction with the the help of ftio.py
 """
 from __future__ import annotations
 import sys
 from multiprocessing import Manager
 from ftio.prediction.pools import predictor_with_pools
+from ftio.prediction.processes_zmq import predictor_with_processes_zmq
 from ftio.prediction.processes import predictor_with_processes
 
 def main(args: list[str] = sys.argv) -> None:
-    """runs the prediction and launches new threads whenever data is avilable
+    """runs the prediction and launches new threads whenever data is available
 
     Args:
         args (list[str]): arguments passed from command line
     """
     # Init
     manager = Manager()
     filename = args[1]
     queue = manager.Queue()
     data = manager.list() # stores prediction
     aggregated_bytes = manager.Value("d", 0.0)
     hits = manager.Value("d", 0.0)
     start_time = manager.Value("d", 0.0)
     count = manager.Value('i', 0)
-
+    b_app = manager.list()
+    t_app = manager.list()
+    
     mode = "procs" # "procs" or "pool"
     
     if "pool" in mode.lower():
         # prediction with a Pool of process and a callback mechanism
         predictor_with_pools(filename, data, queue, count, hits, start_time, aggregated_bytes, args)
     else:
-        # prediction with Processes of process and a callback mechanism
-        predictor_with_processes(filename, data, queue, count, hits, start_time, aggregated_bytes, args)
+        if any("zmq" in x for x in args):
+            # prediction with Processes of process and a callback mechanism + zmq
+            predictor_with_processes_zmq(data, queue, count, hits, start_time, aggregated_bytes, args, b_app, t_app)
+        else:
+            # prediction with Processes of process and a callback mechanism
+            predictor_with_processes(filename, data, queue, count, hits, start_time, aggregated_bytes, args)
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `ftio-hpc-0.0.3/ftio/freq/_dft.py` & `ftio_hpc-0.0.4/ftio/freq/_dft.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+"""Contains DFT methods and accuracy calculation 
+"""
 import numpy as np
 import pandas as pd
+import matplotlib.pyplot as plt
 from ftio.prediction.unify_predictions import  color_pred
 from ftio.prediction.helper import get_dominant_and_conf
-import matplotlib.pyplot as plt
 from ftio.freq.helper import MyConsole
 
+
 CONSOLE = MyConsole()
 
 
 #!################
 #! DFT flavors
 #!################
-
-# Wrapper 
+# Wrapper
 def dft(b):
     return numpy_dft(b)
 
 
 #1) Custome implementation
 def dft_fast(b):
     N = len(b)
@@ -36,15 +38,17 @@
     n = np.arange(N)
     k = n.reshape((N, 1))
     e = np.exp(-2j * np.pi * k * n / N)
     X = np.dot(e, b)
     return X
 
 
-
+#!################
+#! DFT Precision
+#!################
 def precision_dft(
     amp: np.ndarray, phi:np.ndarray, dominant_index:np.ndarray, b_sampled:np.ndarray, t_disc:np.ndarray, freq_arr:np.ndarray, plt_engine:str
 ) -> str:
     """calculates the precision of the dft
 
     Args:
         amp (np.ndarray): amplitude array from DFT
@@ -72,19 +76,14 @@
         x_2 = x.copy()
         total = np.sum(b_sampled)
         for i, _ in enumerate(x):
             if x[i] > b_sampled[i]:
                 x_2[i] = b_sampled[i]
                 x[i] = -x[i] + b_sampled[i]
 
-        # print(
-        #     f"        '-> \033[1;32mPrecision of {freq_arr[index]:.2f} Hz "
-        #     f"is {float(np.sum(x)) / total * 100:.2f}%% "
-        #     f"(Positive only: {float(np.sum(x_2)) / total * 100:.2f}%%)\033[1;0m"
-        # )
         text += f"Precision of [cyan]{freq_arr[index]:.2f}[/] Hz is [cyan]{float(np.sum(x)) / total * 100:.2f}% [/]"
         text += f"(Positive only: [cyan]{float(np.sum(x_2)) / total * 100:.2f}%[/])\n"
 
         if showplot and ("mat" in plt_engine or "plotly" in plt_engine):
             plt.plot(t_disc, x, label=f"f = {freq_arr[index]:.2f} Hz")
 
     if showplot and ("mat" in plt_engine or "plotly" in plt_engine):
@@ -110,21 +109,22 @@
     conf,
     dominant_index,
     amp,
     phi,
     b_sampled,
     time_b,
     ranks,
-    N,
     bandwidth,
 ) -> tuple[list, list, list, list]:
     df0 = []
     df1 = []
     df2 = []
     df3 = []
+    N = len(b_sampled)
+
     df3.append(
         pd.DataFrame(
             {
                 "dominant": freq_arr[dominant_index],
                 "k": dominant_index,
                 "conf": conf[dominant_index],
                 "ranks": np.repeat(ranks, len(dominant_index)),
@@ -161,25 +161,35 @@
         pd.DataFrame(
             {"b": bandwidth, "t": time_b, "ranks": np.repeat(ranks, len(time_b))}
         )
     )
     return df0, df1, df2, df3
 
 
-def display_prediction(argv: list, prediction: dict) -> None:
-    func_name = argv[0][argv[0].rfind("/") + 1:]
+def display_prediction(argv: list[str]|str, prediction: dict) -> None:
+    """Displays the result of the prediction from ftio
+
+    Args:
+        argv (list[str]): command line arguments
+        prediction (dict): the result from ftio
+    """
+
+    if isinstance(argv,list):
+        func_name = argv[0][argv[0].rfind("/") + 1:]
+    else:
+        func_name = argv
+
     if "ftio" in func_name:
         if prediction:
             freq, conf = get_dominant_and_conf(prediction)
             if not np.isnan(freq):
                 CONSOLE.info(
                     f"[cyan underline]Prediction results:[/]\n[cyan]Frequency:[/] {freq:.3e} Hz"
                     f"[cyan] ->[/] {np.round(1/freq,4)} s\n"
                     f"[cyan]Confidence:[/] {color_pred(conf)}"
                     f"{np.round(conf*100,2)}[/] %\n"
                 )
             else:
                 CONSOLE.info(
                         "[cyan underline]Prediction results:[/]\n"
                         "[red]No dominant frequency found[/]\n"
-                    )
-
+                    )
```

### Comparing `ftio-hpc-0.0.3/ftio/freq/_wavelet.py` & `ftio_hpc-0.0.4/ftio/freq/_wavelet.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/freq/anomaly_detection.py` & `ftio_hpc-0.0.4/ftio/freq/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/freq/anomaly_plot.py` & `ftio_hpc-0.0.4/ftio/freq/anomaly_plot.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/freq/autocorrelation.py` & `ftio_hpc-0.0.4/ftio/freq/autocorrelation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # try:
 # except ImportError:
 #     PLOT_MODE = "empty"
 
 CONSOLE = MyConsole()
 
 def find_autocorrelation(args, data: dict, share:dict) -> dict:
-    """Finds perodicity using autocorreleation
+    """Finds the period using autocorreleation
 
     Args:
         args (argparse): command line arguments
         data (dict): sampled data
 
     Returns:
         dict: predictions containing 4 fields: 
             1. bandwidth (np.array): bandwidth array
-            2. time (np.array): time array indicating when bandwidth time points chaged
+            2. time (np.array): time array indicating when bandwidth time points changed
             3. total_bytes (int): total transferred bytes
             4. ranks: number of ranks that did I/O
     """
     prediction = {}
     candidates = np.array([])
     fig = []
     CONSOLE.set(args.verbose)
@@ -156,32 +156,32 @@
                     angle=0,
                     line=dict(width=1, color="DarkSlateGrey")
                 ),
                 mode="markers",
                 name="peaks",
             )
 
-        # finde outliers
+        # find outliers
         text  = ""
         outliers, text = filter_outliers(freq, candidates, weights)
         # remove outliers
         if len(outliers) != 0:
             candidates = np.delete(candidates, outliers)
             weights = np.delete(weights, outliers)
         # calculate period
         mean = np.average(candidates, weights=weights) if len(weights) > 0 else 0 
         std =  np.sqrt(np.abs(np.average((candidates-mean)**2, weights=weights))) if len(weights) > 0 else 0
         tmp = 1 / candidates if len(candidates) > 0 and any(candidates > 0) else 0
         if isinstance(tmp,list) and len(tmp) > 0:
             tmp = [f"{i:.4f}" for i in tmp]
 
-        text += f"Found perodicities are [purple]{candidates}[/]\n"
-        text += f"Matching Frequncies are [purple]{tmp}[/]\n"
+        text += f"Found periods are [purple]{candidates}[/]\n"
+        text += f"Matching frequencies are [purple]{tmp}[/]\n"
         periodicity = mean if len(candidates) > 0 else np.nan
-        text += f"Average petrodicity is [purple]{periodicity:.2f} [/]sec\n"
+        text += f"Average periods is [purple]{periodicity:.2f} [/]sec\n"
         text += f"Average frequency is [purple]{1/periodicity if periodicity > 0 else np.nan:.4f} [/]Hz\n"
 
         # calculate confidence using "Coefficient of variation": https://en.wikipedia.org/wiki/Coefficient_of_variation
         coef_var = np.abs(std / mean ) if len(candidates) > 0 else np.nan
         # coef_var = np.abs(np.std(candidates) / np.mean(candidates) ) if len(candidates) > 0 else np.nan
         conf = np.abs(1 - coef_var)
         text += f"confidence is [purple]{conf*100:.2f} [/]%\n"
```

### Comparing `ftio-hpc-0.0.3/ftio/freq/discretize.py` & `ftio_hpc-0.0.4/ftio/freq/discretize.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def sample_data(b: np.ndarray, t: np.ndarray, freq=-1) -> tuple[np.ndarray, float, str]:
     """Discretize the data according to the frequency
 
     Args:
         b (array): bandwidth
         t (array): time
         freq (int, optional): sampling frequency. Defaults to -1, calculates the optimal sampling
-        frequency inside this funciton
+        frequency inside this function
 
     Returns:
         _type_: b_sampled, sampling frequency (in case -1), and text 
         
     """
     text = ""
     text += f"Time window: {t[-1]-t[0]:.2f} s\n"
@@ -30,17 +30,19 @@
         for i in range(0, len(t) - 1):
             if (
                 t_rec > (t[i + 1] - t[i])
                 and (t[i + 1] - t[i]) != 0
                 and (t[i + 1] - t[i]) >= 0.001
             ):
                 t_rec = t[i + 1] - t[i]
-                # print("tre_c",t_rec, "t[i+1] ",t[i+1], "t[i]", t[i])
         freq = 2 / t_rec
-        text += f"Recomended sampling frequency: {freq:.3e} Hz\n"
+        text += f"Recommended sampling frequency: {freq:.3e} Hz\n"
+    elif freq == -2:
+        N = 10000
+        freq = N/np.floor((t[-1] - t[0]))
     else:
         text += f"Sampling frequency:  {freq:.3e} Hz\n"
     N = int(np.floor((t[-1] - t[0]) * freq))
     text += f"Expected samples: {N}\n"
     # print("    '-> \033[1;Start time: %f s \033[1;0m"%t[0])
 
     # ? sample the data with the recommended frequency
@@ -64,25 +66,28 @@
     #! Abstraction error
     v_a = np.sum(np.abs(b_sampled * np.repeat(1 / freq, len(b_sampled))))
     v_0 = np.sum(b * (np.concatenate([t[1:], t[-1:]]) - t))
     # E = (abs(error))/(V0) if V0 > 0 else 0
     error = (abs(v_a - v_0)) / v_0 if v_0 > 0 else 0
     text += f"Abstraction error: {error:.5f}\n"
 
+    if len(b_sampled) == 0:
+        raise RuntimeError("No data in sampled bandwidth.\n Try increasing the sampling frequency")
+
     return b_sampled, freq, text[:-1]
 
 
 def sample_data_same_size(b: np.ndarray, t:np.ndarray, freq=-1, n_bins=-1) -> tuple[np.ndarray,np.ndarray]:
     """Dsicretize the data according to the frequency and holds value
 
     Args:
         b (array): bandwidth
         t (array): time
         freq (int, optional): sampling frequency. Defaults to -1, calculates the optimal sampling
-        frequency inside this funciton
+        frequency inside this function
         n_bins (int,optinal): number of desired bins
 
     Returns:
         _type_: b_sampled and sampling frequency (in case -1)
     """
     print(f"    '-> \033[1;34mBins: {n_bins}  \033[1;0m")
     b_sampled = np.zeros(n_bins)
```

### Comparing `ftio-hpc-0.0.3/ftio/freq/freq_html.py` & `ftio_hpc-0.0.4/ftio/freq/freq_html.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/freq/freq_plot_core.py` & `ftio_hpc-0.0.4/ftio/freq/freq_plot_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 import os
-from sys import platform
 from threading import Thread
 import datetime
 import json
 import numpy as np
 import pandas as pd
 from scipy.spatial.distance import euclidean
 from fastdtw import fastdtw
@@ -23,15 +22,14 @@
 from ftio.plot.units import set_unit
 from ftio.freq.freq_html import create_html
 
 # import plotly.io as pio
 
 matplotlib.rcParams["backend"] = "TkAgg"
 
-
 class FreqPlot:
     """For plotting the result of ftio"""
 
     def __init__(self, argv):
         self.render = "dynamic"
         self.plot_engine = "plotly"
         self.dtw = True
@@ -40,17 +38,17 @@
         self.psd = False
         if not isinstance(argv, bool):
             D1 = []
             D2 = []
             D3 = []
             j = 0
             self.check = 0
-            self.modes = ["async_write", "sync_write", "async_read", "sync_read"]
+            self.modes = ["write_async", "write_sync", "read_async", "read_sync"]
             self.s = []
-            mode = "async_write"
+            mode = "write_async"
             if isinstance(argv, list):
                 if len(argv) <= 1:
                     self.paths = ["."]
                 else:
                     self.paths = []
                     for i in range(1, len(argv)):
                         if "sync_" in str(argv[i]):
@@ -303,18 +301,20 @@
 
         ranks = np.sort(pd.unique(self.D.settings_df["ranks"]))
         for r in ranks:
             index_set = self.D.settings_df["ranks"].isin([r])
             index_data = self.D.data_df["ranks"].isin([r])
             if not self.D.original_df.empty:
                 index_original = self.D.original_df["ranks"].isin([r])
+
             samples = np.arange(0, self.D.settings_df["N"][index_set].values)
-            amp = self.D.data_df[index_data]["A"]
-            freq = self.D.data_df[index_data]["freq"]
-            found = False
+            amp     = np.array(self.D.data_df[index_data]["A"])
+            freq    = np.array(self.D.data_df[index_data]["freq"])
+            phi     = np.array(self.D.data_df[index_data]["phi"])
+            found   = False
 
             # reconstruct time
             time = (
                 self.D.settings_df[index_set]["t_start"].values
                 + samples * self.D.settings_df[index_set]["T_s"].values
             )
 
@@ -347,26 +347,27 @@
                 # top_x = self.D.data_df[index_data].sort_values('A').tail(20).index
                 top_x = self.D.data_df[index_data].sort_values("A").tail(5).index
                 top_x = top_x[top_x < limit[0]]
 
             name_dominant = ""
             # set the unit and order
             unit, order = set_unit(self.D.data_df[index_data]["b_sampled"])
-            # unit = "MB/s" compatibility with old version
+            #
+            # unit, order = set_unit(self.D.data_df[index_data]["b_sampled"]*1000) #compatibility with old version (For BWLIMIT)
             for k in samples:
                 x = (
                     (1 / len(samples))
-                    * amp.values[k]
+                    * amp[k]
                     * np.cos(
                         2
                         * np.pi
                         * samples
                         * k
                         / (self.D.settings_df[index_set]["N"].values)
-                        + self.D.data_df[index_data]["phi"].values[k]
+                        + phi[k]
                     )
                 )
                 if k == 0:
                     sum_all_components = x
                     sum_dominant = np.zeros(x.size)
                     # recon with DC offset
                     if self.recon:
@@ -403,50 +404,50 @@
                             dominant_X2 + 2 * x if not all_or_10 else dominant_X2 + x
                         )
 
                 length = len(samples)
                 if "mat" in self.plot_engine:
                     if all_or_10:
                         s = "%.1e*cos(2\u03C0*%.1f*t%+.2f)" % (
-                            order * amp.values[k] / length,
+                            order * amp[k] / length,
                             k,
-                            self.D.data_df[index_data]["phi"].values[k],
+                            phi[k],
                         )
                         plt.plot(time, x * order, linewidth=0.7, label="_nolegend_")
                     else:
                         if self.D.data_df[index_data].index[k] in top_x:
                             if k == 0 or k == len(samples) / 2:
                                 a = 1
                             else:
                                 a = 2
 
-                            if round(freq.values[k], 2) > 0:
-                                s = f"{a / length * order*amp.values[k]:.1e}*cos(2\u03C0*{freq.values[k]:.2f}*t+{self.D.data_df[index_data]['phi'].values[k]:.2f})"
+                            if round(freq[k], 2) > 0:
+                                s = f"{a / length * order*amp[k]:.1e}*cos(2\u03C0*{freq[k]:.2f}*t+{phi[k]:.2f})"
                             else:
-                                s = f"{a / length * order*amp.values[k]:.1e}*cos(2\u03C0*{freq.values[k]:.2e}*t+{self.D.data_df[index_data]['phi'].values[k]:.2e})"
+                                s = f"{a / length * order*amp[k]:.1e}*cos(2\u03C0*{freq[k]:.2e}*t+{phi[k]:.2e})"
                             plt.plot(time, a * x * order, linewidth=0.9, label=s)
                             # if (k in dominant ):
                             if k in dominant and k != 0:
                                 if name_dominant:
                                     name_dominant = name_dominant + "\n+ " + s
                                 else:
                                     name_dominant = s
                 else:  # pltoly
                     if self.D.data_df[index_data].index[k] in top_x:
                         # plot only real
                         if k == 0 or k == len(samples) / 2:
                             a = 1
                         else:
                             a = 2
-                        if round(freq.values[k], 1) > 0 and amp.values[k] < 100:
-                            s = f"{a / length * order*amp.values[k]:.1f}*cos(2\u03C0*{freq.values[k]:.2f}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
+                        if round(freq[k], 1) > 0 and amp[k] < 100:
+                            s = f"{a / length * order*amp[k]:.1f}*cos(2\u03C0*{freq[k]:.2f}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
                         else:
-                            s = f"{a / length * order*amp.values[k]:.1e}*cos(2\u03C0*{freq.values[k]:.2e}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
+                            s = f"{a / length * order*amp[k]:.1e}*cos(2\u03C0*{freq[k]:.2e}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
                         ## For the paper
-                        # s = f"{a / length * order*amp.values[k]:.0f}*cos(2\u03C0*{freq.values[k]:.2f}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
+                        # s = f"{a / length * order*amp[k]:.0f}*cos(2\u03C0*{freq[k]:.2f}*t{self.D.data_df[index_data]['phi'].values[k]:+.2f})"
                         f[-1].add_trace(
                             Scatter(
                                 x=time,
                                 y=a * x * order,
                                 mode="lines",
                                 name=s,
                                 hovertemplate="<b>Time</b>: %{x:.2f} s"
@@ -466,18 +467,18 @@
                         if k in dominant and k != 0:
                             if name_dominant:
                                 name_dominant = name_dominant + " + " + s
                             else:
                                 name_dominant = s
                         # in reality it is k/N instead of t
                         # if (k == 0 or k == len(samples)/2):
-                        #     s = "%.1ecos(2pi*%.2f*t%+.2f)" % (amp.values[k], freq.values[k], self.D.data_df[index_data]["phi"].values[k])
+                        #     s = "%.1ecos(2pi*%.2f*t%+.2f)" % (amp[k], freq[k], self.D.data_df[index_data]["phi"].values[k])
                         #     f[-1].add_trace(Scatter(x=time,y=x,mode='lines',name=s, hovertemplate ='<b>Time</b>: %{x:.2f} s'+ '<br><b>Amplitude</b>: %{y}'+'<br><b>T</b>: %{text} s',text = len(samples)*['%.2f'%(self.D.data_df[index_data]["T"].values[k])]))
                         # else:
-                        #     s = "%.1ecos(2pi*%.2f*t%+.2f)" % (a*amp.values[k], freq.values[k], self.D.data_df[index_data]["phi"].values[k])
+                        #     s = "%.1ecos(2pi*%.2f*t%+.2f)" % (a*amp[k], freq[k], self.D.data_df[index_data]["phi"].values[k])
                         #     f[-1].add_trace(Scatter(x=time,y=a*x,mode='lines',name=s, hovertemplate ='<b>Time</b>: %{x:.2f} s'+ '<br><b>Amplitude</b>: %{y}'+'<br><b>T</b>: %{text} s',text = len(samples)*['%.2f'%(self.D.data_df[index_data]["T"].values[k])]))
             if self.dtw:
                 threads = []
                 print("    '-> \033[1;35mCalculating DTW\033[1;0m")
                 threads.append(
                     Thread(
                         target=evaluate_dtw,
```

### Comparing `ftio-hpc-0.0.3/ftio/freq/helper.py` & `ftio_hpc-0.0.4/ftio/freq/helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,124 @@
 """Helper function for frequency techniques    
 """
+
 import plotly.graph_objects as go
 from rich.console import Console
 
 
-def get_mode(data,mode):
-    """used after get_data() to exract df. The df 
+def get_mode(data, mode):
+    """used after get_data() to extract df. The df
     contains all sims group by mode
 
     Args:
         data (Scales): simulation data
         mode (str): "read_sync", "write_sync", "read_async" or "write_async"
 
     Raises:
-        Exception: unsported mode
+        Exception: unsupported mode
 
     Returns:
-        df: pandas dataframe containg data group by mode
+        df: pandas dataframe containing data group by mode
     """
     mode = mode.lower()
     if "read" in mode:
         if "async" in mode:
             return data.df_rat
         elif "sync" in mode:
             return data.df_rst
     if "write" in mode:
         if "async" in mode:
             return data.df_wat
         elif "sync" in mode:
             return data.df_wst
-    raise Exception("undifined mode set")
+    raise Exception("undefined mode set")
 
 
-def get_sim(data,mode):
+def get_sim(data, mode):
     mode = mode.lower()
     if "read" in mode:
         if "async" in mode:
             return data.read_async_t
         elif "sync" in mode:
             return data.read_sync
     if "write" in mode:
         if "async" in mode:
             return data.write_async_t
         elif "sync" in mode:
             return data.write_sync
-    raise Exception("undifined mode set")
-
-
-def match_modes(mode):
-    mode = mode.lower()
-    if isinstance(mode,list):
-        for i in range(0,len(mode)):
-            mode[i] = match(mode[i])
-    else:
-        mode = [match(mode)]
-    return mode
-
-
-def match(mode):
-    if "read" in mode:
-        if "async" in mode:
-            return "read_async"
-        elif "sync" in mode:
-            return "read_sync"
-    if "write" in mode:
-        if "async" in mode:
-            return "write_async"
-        elif "sync" in mode:
-            return "write_sync"
+    raise Exception("undefined mode set")
 
 
 
 def format_plot(fig) -> go.Figure:
     """makes plots uniform
 
     Args:
         fig (pltoly figure)
     """
     fig.update_layout(
-    plot_bgcolor='white',
+        plot_bgcolor="white",
         legend=dict(
-        bgcolor="rgba(255,255,255,.99)",
-        bordercolor="Black",
-        borderwidth=1,
-    ),
-        font = dict(
-            family="Courier New, monospace", 
-            size= 24, 
-            color= "black"
-            ),
+            bgcolor="rgba(255,255,255,.99)",
+            bordercolor="Black",
+            borderwidth=1,
+        ),
+        font=dict(family="Courier New, monospace", size=24, color="black"),
         # margin=dict(l=5, r=5, t=5, b=5) #IEEE
-        margin=dict(t=25) 
+        margin=dict(t=25),
     )
 
     fig.update_xaxes(
-        ticks='outside',
+        ticks="outside",
         # tickwidth=1,
         ticklen=10,
         showgrid=True,
         # gridwidth=1,
         mirror=True,
         showline=True,
-        linecolor='black',
-        gridcolor='lightgrey',
-        minor_ticks='outside',
-        minor=dict(ticklen=2)
+        linecolor="black",
+        gridcolor="lightgrey",
+        minor_ticks="outside",
+        minor=dict(ticklen=2),
     )
 
     fig.update_yaxes(
-        ticks='outside',
+        ticks="outside",
         # tickwidth=1,
         ticklen=10,
         showgrid=True,
         # gridwidth=1,
         mirror=True,
         showline=True,
-        linecolor='black',
-        gridcolor='lightgrey',
-        minor_ticks='outside',
-        minor=dict(ticklen=2)
-    )  
+        linecolor="black",
+        gridcolor="lightgrey",
+        minor_ticks="outside",
+        minor=dict(ticklen=2),
+    )
 
     return fig
 
 
+def merge_results(
+    df0: tuple[list, list, list, list], df1: tuple[list, list, list, list]
+) -> tuple[list, list, list, list]:
+    """merges results for several files
+
+    Args:
+        df0 (list): _description_
+        df1 (list): _description_
+
+    Returns:
+        list: _description_
+    """
+    for i in range(0, len(df0)):
+        df0[i].extend(df1[i])
+
+    return df0
+
 
 class MyConsole(Console):
     """Console child class that overwrites
     the print method for silent version
 
     Args:
         Console (_type_): _description_
@@ -139,13 +130,13 @@
 
     def set(self, flag):
         if flag:
             self.verbose = True
         else:
             self.verbose = False
 
-    def print(self,s):
+    def print(self, s):
         if self.verbose:
             Console.print(self, s)
 
     def info(self, s):
-        Console.print(self, s)
+        Console.print(self, s)
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/args.py` & `ftio_hpc-0.0.4/ftio/parse/args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from __future__ import annotations
 import argparse
-from ftio import __copyright__, __repo__, __version__, __liscence__
+from ftio import __copyright__, __repo__, __version__, __license__
 
 
 
-def parse_args(argv:list) -> argparse.Namespace:
-    name = argv[0]
-    # name = name[name.rfind('/')+1:-3]
-    name = name[name.rfind('/')+1:]
+def parse_args(argv:list, name='') -> argparse.Namespace:
+    flag = True
+    if name == '':
+        name = argv[0]
+        name = name[name.rfind('/')+1:]
+    else:
+        #API call
+        flag = False
+        
 
     if 'plot' in name:
         disc = 'Plots result stored in Json file to a HTML page or PDF document.'
     elif 'ftio' in name:
-        disc = 'Captures the period of the I/O phases. Uses freqeuncy techniques (default=discrete fourier transformation) and outlier detection methods (Z-score) on the provided file. Supported file formats are Json, Jsonlines, Msgpack, Darshan, and REcorder (folder). TMIO can be used to generate the tracing file needed. There are several parameters which can be controlled by the arguments bellow.'
+        disc = 'Captures the period of the I/O phases. Uses frequency techniques (default=discrete fourier transformation) and outlier detection methods (Z-score) on the provided file. Supported file formats are Json, Jsonlines, Msgpack, Darshan, and REcorder (folder). TMIO can be used to generate the tracing file needed. There are several parameters which can be controlled by the arguments bellow.'
     elif 'predictor' in name:
         disc = 'Wrapper code to execute ftio online. Monitors a file for changes. Whenever the file is modified (i.e., new traces are appended) a new prediction process is executed and the result is store in a shared memory space. All parameters that can be passed to ftio are supported by predictor.'
     elif 'parse' in name:
         disc = 'Parses to an extra-p format.'
     else:
         disc = ''
 
@@ -30,37 +35,44 @@
 
 Report any bugs to:
 {__repo__}/issues
 
 COPYRIGHT:
 {__copyright__} 
 
-LISCENCE:
-{__liscence__} 
+LICENCE:
+{__license__} 
 
 Full documentation:
 {__repo__}
 --------------------------------------------
 ''',
         formatter_class=argparse.RawDescriptionHelpFormatter
         )
+
+    #! If CLI call not API, add files
+    if flag:
+        parser.add_argument('files', metavar='files', type = str, nargs='+', help='file, file list (file 0 ... file n), folder, or folder list (folder 0.. folder n)')    
+
+    parser.add_argument('-m', '--mode', dest = 'mode',      type = str ,  help ='if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: write_async, read_async, write_sync, read_sync')
+    parser.add_argument('-s','--source', dest='source', type = str, help = 'the source of the files: tmio, or custom. See https://github.com/tuda-parallel/FTIO/blob/main/docs/file_formats.md')
+    parser.set_defaults(source = 'unspecified')
     
-    parser.add_argument('files', metavar='files', type = str, nargs='+', help='file, file list (file 0 ... file n), folder, or folder list (folder 0.. folder n)')    
-    parser.add_argument('-m', '--mode', dest = 'mode',      type = str ,  help ='if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: async_write, async_read, sync_write, sync_read')
-    
-    
+    #! PARSE Settings
     if 'parse' not in name.lower():
         parser.add_argument('-r', '--render', dest='render',  type = str ,  help ='specifies how the plots are rendered. Either dynamic (default) or static' )
         parser.set_defaults(render='dynamic')
 
+    #! PLAY Settings
     if 'play' in name.lower():
         parser.add_argument('-f', '--freq', dest='freq', type = float, help ='specifies the sampling rate with which the continuous signal is discretized (default=10Hz). This directly affects the highest captured frequency (Nyquist). The value is specified in Hz. In case this value is set to -1, the auto mode is launched which sets the sampling frequency automatically to the smallest change in the bandwidth detected. Note that the lowest allowed frequency in the auto mode is 2000 Hz')
         parser.add_argument('-e', '--engine',         type = str, help = 'plot engine. Either plotly (default) or mathplotlib. Specifies the engine used to display the figures. Plotly is used to generate HTML files')
         parser.set_defaults(engine = 'plotly')
 
+    #! FTIO and Predictor Settings
     if 'ftio' in name.lower() or 'predictor' in name.lower():
         parser.set_defaults(mode='sync write')
         parser.add_argument('-f', '--freq', dest='freq', type = float, help ='specifies the sampling rate with which the continuous signal is discretized (default=10Hz). This directly affects the highest captured frequency (Nyquist). The value is specified in Hz. In case this value is set to -1, the auto mode is launched which sets the sampling frequency automatically to the smallest change in the bandwidth detected. Note that the lowest allowed frequency in the auto mode is 2000 Hz')
         parser.set_defaults(freq = 10)
         parser.add_argument('-ts', '--ts',         type = float, help = 'modifies the start time of the examined time window')
         parser.add_argument('-te', '--te',         type = float, help = 'modifies the end time of the examined time window')
         parser.add_argument('-tr', '--transformation', dest='transformation',  type = str, help = 'Specifies the frequency technique to use. Supported modes are: dft (default), wave_disc, and wave_cont')
@@ -75,52 +87,66 @@
         parser.set_defaults(tol =  0.8)
         parser.add_argument('-d', '--dtw', action='store_true', help ='performs dynamic time wrapping on the top 3 frequencies (highest contribution) calculated using the DFT if set (default=False)')
         parser.set_defaults(dtw=False)
         parser.add_argument('-re', '--reconstruction', action='store_true', help ='plots reconstruction of top 10 signals on figure')
         parser.set_defaults(reconstruction=False)
         parser.add_argument('-np','--no-psd', dest='psd', action='store_false', help='if set, replace the power density spectrum (a*a/N) with the amplitude spectrum (a)')
         parser.set_defaults(psd=True)
+        parser.add_argument('-n', '--n_freq', dest= 'n_freq',   type = float, help ='number of frequencies to extract. By default FTIO finds the dominant frequency. With this flag, up to "n_freq" can be extracted from FTIO')
+        parser.set_defaults(n_freq =  0)
         parser.add_argument('-c', '--autocorrelation', dest='autocorrelation', action='store_true', help ='if set, autocorrelation is calculated in addition to DFT. The results are merged to a single prediction at the end')
         parser.set_defaults(autocorrelation=False)
         parser.add_argument('-w', '--window_adaptation', dest='window_adaptation', action='store_true', help ='online time window adaptation. If set to true, the time window is shifted on X hits to X times the previous phases from the current instance. X corresponds to frequency_hits')
         parser.set_defaults(window_adaptation=False)
         parser.add_argument('-fh', '--frequency_hits', dest= 'frequency_hits',   type = float, help ='specifies the number of hits needed to adapt the time window. A hit occurs once a dominant frequency is found')
         parser.set_defaults(frequency_hits =  3)
         parser.add_argument('-v', '--verbose', dest= 'verbose',   action = 'store_true', help ='sets verbose on or off (default=False)')
         parser.set_defaults(verbose =  False)
+        parser.add_argument('--zmq', action='store_true', help='avoids opening the generated HTML file since zmq is used')
+        parser.set_defaults(zmq=False)
+        parser.add_argument('--zmq_source',         type = str, help = 'the source of zmq: TMIO, direct, etc.')
+        parser.set_defaults(zmq_source = 'direct')
+        parser.add_argument('--zmq_address', '--zmq_address', dest='zmq_address', type = str, help = 'zmq address for communication')
+        parser.set_defaults(zmq_address = '*')
+        parser.add_argument('--zmq_port', '--zmq_port', dest='zmq_port', type = str, help = 'zmq port for communication')
+        parser.set_defaults(zmq_port = '5555')
 
+
+    #! IOPLOT Settings
     if 'plot' in name.lower():
         parser.set_defaults(mode='')
         parser.add_argument('-z', '--zoom',       type = float, help ='upper zoom limit on the y-axis')
         parser.add_argument('-nt', '--no-threaded', dest='threaded', action='store_false', help= 'turn multithreading off (default=on)')
         parser.set_defaults(threaded=True)
         parser.add_argument('-e', '--engine',         type = str, help = 'plot engine to use. Either plotly (default), dash, or matplotlib')
         parser.set_defaults(engine = 'plotly')
         parser.add_argument('--n_shown_samples', type=int, help='only for dash: Number of shown samples per trace (default: 20_000). Caution: Too small numbers could lead to incorrect representations!')
         parser.set_defaults(n_shown_samples=20_000)
         parser.add_argument('--merge_plots', action='store_true', help='only for dash: Merges the plots to one plot for each io mode. Note: The file dropdown menu then has no functionality')
         parser.set_defaults(merge_plots=False)
         parser.add_argument('--no_disp', action='store_true', help='avoids opening the generated HTML file')
         parser.set_defaults(no_disp=False)
+
+    #! PARSE Settings
     if 'parse' in name.lower():
         parser.add_argument('--scale',  action='store_true', help ='scales the Y-axis')
         parser.set_defaults(scale=False)    
-    # Data modes
-    parser.add_argument('-s', '--sum', action='store_true', help ='sum plot: True (default) or False')
-    parser.add_argument('-ns', '--no_sum', dest='sum', action='store_false')
+
+    #! Data modes (for all)
+    parser.add_argument('--sum', action='store_true', help ='sum plot: True (default) or False')
+    parser.add_argument('--no_sum', dest='sum', action='store_false')
     parser.set_defaults(sum=True)
-    parser.add_argument('-a', '--avr', action='store_true', help ='avr plot: True (default) or False')
-    parser.add_argument('-na', '--no_avr', dest='avr', action='store_false')
+    parser.add_argument('--avr', action='store_true', help ='avr plot: True (default) or False')
+    parser.add_argument('--no_avr', dest='avr', action='store_false')
     parser.set_defaults(avr=True)
-    parser.add_argument('-i', '--ind', action='store_true', help ='ind plot: True or False (default)')
-    parser.add_argument('-ni', '--no_ind', dest='ind', action='store_false')
+    parser.add_argument('--ind', action='store_true', help ='ind plot: True or False (default)')
+    parser.add_argument('--no_ind', dest='ind', action='store_false')
     parser.set_defaults(ind=False)
-    parser.add_argument('-cf', '--custom_file',   type = str, help = 'passes a [path/filename.py] file containing the translation and pattern for a custom file format similiar to:\n https://github.com/tuda-parallel/FTIO/blob/main/examples/txt/custom_input.py')
+    parser.add_argument('-cf', '--custom_file',   type = str, help = 'passes a [path/filename.py] file containing the translation and pattern for a custom file format similar to:\n https://github.com/tuda-parallel/FTIO/blob/main/examples/custom/txt/custom_input.py')
     parser.set_defaults(custom_file = '')
-    
     parser.add_argument('-x', '--dxt_mode', dest='dxt_mode',  type = str ,  help ='select data to extract from Darshan traces (DXT_POSIX or DXT_MPIIO (default))')
     parser.set_defaults(dxt_mode='DXT_MPIIO')
     parser.add_argument('-l', '--limit',      type = int,   help ='max ranks to consider when reading a folder')
     parser.set_defaults(limit=-1)
 
 
     args = parser.parse_args(argv)
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/bandwidth.py` & `ftio_hpc-0.0.4/ftio/parse/bandwidth.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         1) request level: subscripted ind (for individual requests)
     _ovr
         2) Rank level metrics: avrerage (avr) or sum. Represent either the
         sum/avr of the ind level metrics during a phase.
 
         3) Application level metrics:  subscripted overlap. Calculated by
         overlapping the previous metrics. The most accurate one is ind, however,
-        it has the higest overhead.
+        it has the highest overhead.
     """
 
     def __init__(self, b, io_type, args):  # b = values["bandwidth"]
         # App level
         self.b_overlap_sum = []
         self.b_overlap_avr = []
         self.t_overlap = []
@@ -90,20 +90,20 @@
                 if "b_rank_sum" in b:
                     self.t_rank_s.extend(np.zeros(len(b["b_rank_sum"])))
                     self.t_rank_e.extend(np.zeros(len(b["b_rank_sum"])))
                 elif "b_rank_avr" in b:
                     self.t_rank_s.extend(np.zeros(len(b["b_rank_avr"])))
                     self.t_rank_e.extend(np.zeros(len(b["b_rank_avr"])))
 
-            # 2) Calcluate bandwidth overlapping at rank level
-            if ("t_rank_s" in b) and "b_overlap_avr" not in b and args.avr:
+            # 2) Calculate bandwidth overlapping at rank level
+            if "t_rank_s" in b  and "b_rank_avr" in b and "b_overlap_avr" not in b and args.avr:
                 self.b_overlap_avr, self.t_overlap = overlap(
                     b["b_rank_avr"], b["t_rank_s"], b["t_rank_e"]
                 )
-            if ("t_rank_s" in b) and "b_overlap_sum" not in b and args.sum:
+            if "t_rank_s" in b and "b_rank_sum" in b and "b_overlap_sum" not in b and args.sum:
                 self.b_overlap_sum, self.t_overlap = overlap(
                     b["b_rank_sum"], b["t_rank_s"], b["t_rank_e"]
                 )
 
         # overlapping thread level
         if args.ind:
             # Thread level metrics
@@ -149,31 +149,32 @@
     def assign(self, b, name):
         if name in b:
             return b[name] if not np.isnan(b[name]) else -1
         else:
             return -1
 
 
-#! ----------------------- I/O anaylsis ------------------------------
+#! ----------------------- I/O analysis ------------------------------
 # **********************************************************************
 # *                       1. Overlap
 # **********************************************************************
 
 
 def overlap(b, t_s, t_e):
     t_s = np.array(t_s)
     t_e = np.array(t_e)
     b = np.array(b)
     id_s = np.argsort(t_s)
     id_e = np.argsort(t_e)
     try:
-        b_ovrlap, t_ovrlap = overlap_core(b, t_s, t_e, id_s, id_e)
+        b_overlap, t_overlap = overlap_core(b, t_s, t_e, id_s, id_e)
     except:
-        b_ovrlap, t_ovrlap = overlap_core_safe(b, t_s, t_e, id_s, id_e)
-    return list(b_ovrlap), list(t_ovrlap)
+        b_overlap, t_overlap = overlap_core_safe(b, t_s, t_e, id_s, id_e)
+
+    return list(b_overlap), list(t_overlap)
 
 
 @jit(nopython=True, cache=True)
 def overlap_core(b, t_s, t_e, id_s, id_e):
     agg_phases = len(t_s)
 
     b_out = np.zeros(2 * agg_phases)
@@ -197,15 +198,14 @@
             k_s += 1
         # b_out.append(b_tmp)
         b_out[counter] = b_tmp
         counter += 1
 
     return b_out, t_out
 
-
 def overlap_core_safe(b, t_s, t_e, id_s, id_e):
     agg_phases = len(t_s)
 
     b_out = []
     t_out = []
     b_tmp = 0
     k_s = 0
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/custom_patterns.py` & `ftio_hpc-0.0.4/ftio/parse/custom_patterns.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,20 @@
             (1) pattern (dict[str,str]): dictionary containing name and a regex 
                         expression to find the custom pattern.
             (2) translate (dict[str,tuple[str,(optional)float]]): dictionary 
                         containing matching filed from sample.py and the matching 
                         the name from the pattern. The unit can be optionally specified
     """
     pattern = {
-        "avg_thruput_mib": r"avg_thruput_mib:\s+\[([\d.\d,\s]+)\]",
-        "end_t_micro": r"end_t_micro:\s+\[([\d,\s]+)\]",
-        "start_t_micro": r"start_t_micro:\s+\[([\d,\s]+)\]",
+        "avg_thruput_mib": r"avg_thruput_mib:\s*\[([\d.\d,\s*]+)\]",
+        "end_t_micro": r"end_t_micro:\s*\[([\d,\s*]+)\]",
+        "start_t_micro": r"start_t_micro:\s*\[([\d,\s*]+)\]",
         # "req_size": r"req_size:\s+\[([\d,\s]+)\]",
-        "total_bytes": r"total_bytes:\s+(\d+)",
-        "total_iops": r"total_iops:\s+(\d+)",
+        "total_bytes": r"total_bytes:\s*+(\d+)",
+        "total_iops": r"total_iops:\s*+(\d+)",
         }
 
     # Define map according to sample.py class, along with the scale if any:
     # ftio_field: ("custom_name", scale)
     # ftio unit are default in bytes, b/s, ...
     # scale applies ftio_field = custom_name*scale
     translate = {
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/darshan_reader.py` & `ftio_hpc-0.0.4/ftio/parse/darshan_reader.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/extract.py` & `ftio_hpc-0.0.4/ftio/parse/extract.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/input_template.py` & `ftio_hpc-0.0.4/ftio/parse/input_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def init_data(args:list) -> tuple[str, dict[str, int|dict], dict[str, int]]:
+def init_data(args:list) -> tuple[str, dict[str, dict|int], dict[str, int]]:
     """init data set
 
     Returns:
         tuple[dict[str, int], dict[str, int]]: empty data
     """
     
     io_data = {
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/metrics.py` & `ftio_hpc-0.0.4/ftio/parse/metrics.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/msgpack_reader.py` & `ftio_hpc-0.0.4/ftio/parse/msgpack_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             return convert_to_iotime(arr)
         else:
             raise ValueError(f"Parse error: type is {io_type}")
             
 
 
 def convert_to_iosample(arr: list, io_type: str) -> list:
-    """Brings the data into an strucutre similar to Sample/Time 
+    """Brings the data into an structure similar to Sample/Time 
     depending on the type of the I/O (read/write + sync/async | time)
 
     Args:
         arr (list): metrics
         io_type (str): type of the I/O (read/write + sync/async | time)
 
     Returns:
@@ -137,33 +137,34 @@
     Args:
         file (str): file name
 
     Returns:
         list[dict]: file content
     """
     data = []
-    # print(f"File is {file}")
     # Open the MessagePack binary file for reading
     with open(file, "rb") as in_file:
         # Read the binary data
         binary_data = in_file.read()
 
+    data = extract_data(binary_data, data)
 
+
+def extract_data(binary_data, data):
     # Deserialize the MessagePack data into the class instances
     unpacker = msgpack.Unpacker()
     unpacker.feed(binary_data)
     for item in unpacker:
         io_type = get_type(item)
         data.extend(convert_to_class(item, io_type))
     return data
 
-
 def main(args) -> None:
-    """Pass varibales and call main_core. The extraction of the traces
+    """Pass variables and call main_core. The extraction of the traces
     and the parsing of the arguments is done in this function.
     """
     file = args[1]
-    _ = extract(file)
+    extract(file)
 
 
 if __name__ == "__main__":
     main(sys.argv)
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/overlap_thread.py` & `ftio_hpc-0.0.4/ftio/parse/overlap_thread.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/parse_custom.py` & `ftio_hpc-0.0.4/ftio/parse/parse_custom.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/parse_darshan.py` & `ftio_hpc-0.0.4/ftio/parse/parse_darshan.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/parse_msgpack.py` & `ftio_hpc-0.0.4/ftio/parse/parse_msgpack.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/parse_recorder.py` & `ftio_hpc-0.0.4/ftio/parse/parse_recorder.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/parse_txt.py` & `ftio_hpc-0.0.4/ftio/parse/parse_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Parse text file contaiting three fields: 
+"""Parse text file containing three fields: 
 the bandwidth, the start time, and the end time.
 """
 from ftio.parse.simrun import Simrun
 from ftio.parse.txt_reader import extract
 
 class ParseTxt:
     """class to parse txt file
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/percent.py` & `ftio_hpc-0.0.4/ftio/parse/percent.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/parse/print.py` & `ftio_hpc-0.0.4/ftio/parse/print.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self.file.write("\n")
         self.file.close()
         print("\033[1;32m------------------- done -------------------\n\033[1;0m")
 
     def print_json_lines(self):
         self.file = open("./scale.jsonl", "w")
         self.print_regions_jsonl()
+        self.file.close()
         print("\033[1;32m------------------- done -------------------\n\033[1;0m")
 
     def print_regions_jsonl(self):
         self.print_io_read_sync("jsonl")
         self.print_io_write_sync("jsonl")
         self.print_io_read_async_t("jsonl")
         self.print_io_read_async_b("jsonl")
@@ -195,74 +196,74 @@
                 "Time (s)",
                 print_type=type,
             )
 
             self.print_data(
                 "io_time",
                 "delta_t_sr",
-                "io_time->total_time->total_app_time->total_io_time->sync_read",
+                "io_time->total_time->total_app_time->total_io_time->read_sync",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_ar_lost",
                 "io_time->total_time->total_app_time->total_io_time->delta_t_ar_lost",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_sw",
-                "io_time->total_time->total_app_time->total_io_time->sync_write",
+                "io_time->total_time->total_app_time->total_io_time->write_sync",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_aw_lost",
                 "io_time->total_time->total_app_time->total_io_time->delta_t_aw_lost",
                 "Time (s)",
                 print_type=type,
             )
-            # self.print_data('io_time', 'delta_t_sr',      'io_time->sync_read',       'time', print_type = type)
+            # self.print_data('io_time', 'delta_t_sr',      'io_time->read_sync',       'time', print_type = type)
             self.print_data(
                 "io_time",
                 "delta_t_ara",
-                "io_time->async_read_t",
+                "io_time->read_async_t",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_arr",
-                "io_time->async_read_b",
+                "io_time->read_async_b",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_ar_lost",
                 "io_time->delta_t_ar_lost",
                 "Time (s)",
                 print_type=type,
             )
 
-            # self.print_data('io_time', 'delta_t_sw',      'io_time->sync_write',      'time', print_type = type)
+            # self.print_data('io_time', 'delta_t_sw',      'io_time->write_sync',      'time', print_type = type)
             self.print_data(
                 "io_time",
                 "delta_t_awa",
-                "io_time->async_write_t",
+                "io_time->write_async_t",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_awr",
-                "io_time->async_write_b",
+                "io_time->write_async_b",
                 "Time (s)",
                 print_type=type,
             )
             self.print_data(
                 "io_time",
                 "delta_t_aw_lost",
                 "io_time->delta_t_aw_lost",
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/recorder_reader.py` & `ftio_hpc-0.0.4/ftio/parse/recorder_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,26 +45,26 @@
         for file in sorted(files,key=len):
             file = os.path.join(root, file)
             current_file = open(file, 'r')
             current_file = current_file.readlines()
             # data.extend([k for k in f if 'MPI_File_w' in k or 'MPI_File_r' in k])
             data.extend([k for k in current_file if ' write ' in k or ' read ' in k])
         rank = max([int(x.replace(".txt", "")) for x in files])+1
-        break #no recusive walk
+        break #no recursive walk
     return data, rank
 
 
 def extract_recorder(data:list, ranks:int) -> tuple[dict, dict]:
-    """Extract reorcer traces
+    """Extract recorder traces
 
     Args:
         data (array): simulation data
 
     Returns:
-        w,r: returns two dicts contaiting the data
+        w,r: returns two dicts containing the data
     """
     # FIXME: This needs to ne b_ind t_ind_s and t_ind_e, however required ind overlaping alorithm in bandiwdth.py 
     write ={'number_of_ranks': ranks, 'bandwidth':{'b_rank_sum': [], 'b_rank_avr': [] ,'t_rank_s':[], 't_rank_e':[] }}
     read = {'number_of_ranks': ranks, 'bandwidth':{'b_rank_sum': [], 'b_rank_avr': [] ,'t_rank_s':[], 't_rank_e':[] }}
     for line in data:
         if 'write' in line or 'read' in line:
             s_line  = line.find(' ')
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/sample.py` & `ftio_hpc-0.0.4/ftio/parse/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.max_bytes_per_phase         = self.assign(values,"max_bytes_per_phase")
         self.max_io_phases_per_rank      = self.assign(values,"max_io_phases_per_rank")
         self.total_io_phases             = self.assign(values,"total_io_phases")
         self.max_io_ops_per_rank         = self.assign(values,"max_io_ops_per_rank")
         self.max_io_ops_in_phase         = self.assign(values,"max_io_ops_in_phase")
         self.total_io_ops                = self.assign(values,"total_io_ops")
         self.number_of_ranks             = self.assign(values,"number_of_ranks")
-        self.bandwidth                   = Bandwidth(values["bandwidth"], io_type, args)
+        self.bandwidth                   = self.assign_bandwidth(values, io_type, args)
         self.file_index                  = args.file_index
 
     def get_data(self):
         #! append list is much faster than append data frame
         name0 = []
         data0 = []
         common        = ['number_of_ranks','file_index']
@@ -57,14 +57,20 @@
 
 
     def assign(self,values, name):
         if name in values:
             return values[name]
         else:
             return float('NaN')
+    
+    def assign_bandwidth(self, values, name, args):
+        if "bandwidth" in values:
+            return Bandwidth(values["bandwidth"], name, args)
+        else:
+            return Bandwidth({}, name, args)
 
     def find_data(self,name,common):
         #remove empty:
         for i in name:
             if not getattr(self.bandwidth,i):
                 name.remove(i)
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/scales.py` & `ftio_hpc-0.0.4/ftio/parse/scales.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,99 +1,127 @@
-"""Handels the importing of modules
+"""Handles the importing of modules
 """
-import json
+
 import os
 import datetime
-import jsonlines
 import pandas as pd
 import numpy as np
 from rich.panel import Panel
 from rich.console import Console
 from rich.text import Text
 from ftio import __version__
-from ftio.parse.simrun import Simrun
+from ftio.parse.parse_json import ParseJson
+from ftio.parse.parse_jsonl import ParseJsonl
 from ftio.parse.parse_recorder import ParseRecorder
 from ftio.parse.parse_darshan import ParseDarshan
 from ftio.parse.parse_msgpack import ParseMsgpack
 from ftio.parse.parse_txt import ParseTxt
 from ftio.parse.parse_custom import ParseCustom
+from ftio.parse.parse_zmq import ParseZmq
 from ftio.parse.args import parse_args
 
 
 class Scales:
-    """load the data. Supports single files (json, jsonl, darshan) or folders (+ recorder)
-    """
-    def __init__(self, argv):
+    """load the data. Supports single files (json, jsonl, darshan) or folders (+ recorder)"""
+
+    def __init__(self, argv, msg=None):
         self.Print_info(argv[0])
         self.render = ""
         self.plot_mode = ""
         self.mode = ""
         self.ts = -1
         self.threaded = ""
         self.zoom = -1
         self.same_path = False
         self.names = []
+        self.msg = msg
         self.s = []
 
         # save call
         self.save_call(argv)
 
         # Parse arguments
         self.args = parse_args(argv)
 
+        if "zmq" in self.args and self.args.zmq:
+            self.s.append(ParseZmq(self.msg).to_simrun(self.args, 0))
+            self.n = 1
+        else:
+            self.load_setup()
+
+    def load_setup(self)-> None:
         if isinstance(self.args.files, list):
             if len(self.args.files) <= 1:
                 self.paths = ["."]
             else:
                 self.paths = []
                 for i in range(1, len(self.args.files)):
                     self.paths.append(str(self.args.files[i]))
         else:
             self.paths = [self.args.files]
 
-        # data = []
         self.Check_Same_Path()
         console = Console()
         for path in self.paths:
             #! load folders
             # Recorder folder
             if "_text" in path[-5:]:
-                console.print(f"\n[cyan]Loading Recorder folder({self.paths.index(path) + 1},{len(self.paths)}):[/] {path}")
+                console.print(
+                    f"\n[cyan]Loading Recorder folder({self.paths.index(path) + 1},{len(self.paths)}):[/] {path}"
+                )
                 run = ParseRecorder(path).to_simrun(self.args)
                 self.s.append(run)
 
             # Folder
-            elif (os.path.isdir(path)):
-                console.print(f"\n[cyan]Loading  folder({self.paths.index(path) + 1},{len(self.paths)}):[/] {path}")
+            elif os.path.isdir(path):
+                console.print(
+                    f"\n[cyan]Loading folder({self.paths.index(path) + 1},{len(self.paths)}):[/] {path}"
+                )
                 if path[-1] == "/":
                     path = path[:-1]
 
                 for root, _, files in os.walk(path):
+                    # remove unneeded folders
                     if "io_results" in root or "exported_images" in root:
                         console.print(f"[yellow]Skipping folder:  {root}[/]")
                         continue
-                    if "scale.jsonl" in files:
-                        console.print(f"[yellow]Skipping folder:  {root}/scale.jsonl[/]")
-                        files.remove("scale.jsonl")
+
+                    # remove unneeded files
+                    skip_files = ["scale.jsonl",".call.txt"]
+                    for unwanted in skip_files:
+                        if unwanted in files:
+                            console.print(
+                                f"[yellow]Skipping file: {root}/{unwanted}[/]"
+                            )
+                            files.remove(unwanted)
+
+                    # sort the files
                     sorted_files = sorted(files, key=len)
 
                     for file in sorted_files:
-                        if any(ext in file for ext in ['json','darshan','msgpack','txt']):
+                        if any(
+                            ext in file for ext in ["json", "darshan", "msgpack", "txt"]
+                        ):
                             file_path = os.path.join(root, file)
                             # Limit the number of ranks to consider if self.limit is defined
                             try:
-                                if self.args.limit > 0 and get_rank(file) >= self.args.limit:
+                                if (
+                                    self.args.limit > 0
+                                    and get_rank(file) >= self.args.limit
+                                ):
                                     console.print(f"[yellow]Skipping file: {file}[/]")
                                     continue
                             except Exception as error:
-                                console.print(f"[red]Something went wrong with the limit. Error is {error}[/]")
+                                console.print(
+                                    f"[red]Something went wrong with the limit. Error is {error}[/]"
+                                )
                             self.names.append(root[root.rfind("/") + 1 :])
                             console.print(f"[cyan]Current file:[/] {file}")
                             self.load_file(file_path, self.paths.index(path))
-                    break  # no recusive walk
+                    break  # no reclusive walk
 
             # Compare Several files
             elif not self.same_path and ".json" in path[-6:]:
                 self.names.append(path)
                 console.print(f"[cyan]Current file:[/] {path}")
                 self.load_file(path, self.paths.index(path))
 
@@ -108,58 +136,58 @@
         if self.names:
             names = self.names
             self.names = []
             for i in names:
                 if i not in self.names:
                     self.names.append(i)
 
-    def load_file(self, file_path:str, file_index = 0) -> None:
+    def load_file(self, file_path: str, file_index=0) -> None:
         """Load file content into an Simrun object
 
         Args:
             file_path (str): filename + absolute path
         """
         check_open(file_path)
         if self.args.custom_file:
             run = ParseCustom(file_path).to_simrun(self.args, file_index)
         elif ".json" in file_path[-5:]:
-            with open(file_path,"rt") as file:
-                data = json.load(file)
-            run = Simrun(data, "json", file_path, self.args, file_index)
+            run = ParseJson(file_path).to_simrun(self.args, file_index)
         elif ".jsonl" in file_path[-6:]:
-            with jsonlines.open(file_path, "r") as jsonl_f:
-                data = [obj for obj in jsonl_f]
-            run = Simrun(data, "jsonl", file_path, self.args, file_index)
+            run = ParseJsonl(file_path).to_simrun(self.args, file_index)
         elif "darshan" in file_path[-10:]:
             run = ParseDarshan(file_path).to_simrun(self.args, file_index)
         elif "msgpack" in file_path[-10:]:
             run = ParseMsgpack(file_path).to_simrun(self.args, file_index)
         elif "txt" in file_path[-10:]:
             run = ParseTxt(file_path).to_simrun(self.args, file_index)
         self.s.append(run)
 
     def save_call(self, argv):
-        """save the call as a hidden file
-        """
+        """save the call as a hidden file"""
         self.call = ""
         for i in argv:
             self.call = self.call + " " + i
         f = open("%s/.call.txt" % (os.getcwd()), "a")
         f.write(
             datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
             + " :"
             + self.call
             + "\n\n"
         )
         f.close()
 
-    def Print_info(self, text:str)-> None:
-        name = text[text.rfind("/") + 1 : ].capitalize()
+    def Print_info(self, text: str) -> None:
+        name = text[text.rfind("/") + 1 :].capitalize()
         console = Console()
-        title = Panel(Text(name, justify="center"), style="bold white on cyan", border_style="white", title_align="left")
+        title = Panel(
+            Text(name, justify="center"),
+            style="bold white on cyan",
+            border_style="white",
+            title_align="left",
+        )
         text = "\n[cyan]Author:[/]  Ahmad Tarraf\n"
         text += f"[cyan]Date:[/]    {str(datetime.date.today())}\n"
         text += f"[cyan]Version:[/]  {__version__}\n"
         text += "[cyan]License:[/]  BSD\n"
         # console.print(Panel(Group(title,text), style="white", border_style='blue'))
         console.print(title)
         console.print(text)
@@ -174,18 +202,14 @@
                 else:
                     if same_path != i[: i.rfind("/")]:
                         self.same_path = False
                         break
         else:
             self.same_path = True
 
-    
-
-
-
     #! ----------------------- Pandas dataset functions ------------------------------
     # **********************************************************************
     # *                       1. get_data
     # **********************************************************************
     def get_data(self):
         self.df_rst = self.get_data_io("read_sync")
         self.df_wst = self.get_data_io("write_sync")
@@ -197,37 +221,37 @@
 
         # df = pd.concat([df,self.get_data_core('write_async_b')])
 
     # **********************************************************************
     # *                       2. get_data_io
     # **********************************************************************
     def get_data_io(self, io_mode="read_sync"):
-        """Extract data from the file(s) and gathers in dataframes. 
-        The fields name are store in "name_[level]" and their values are stored 
+        """Extract data from the file(s) and gathers in dataframes.
+        The fields name are store in "name_[level]" and their values are stored
         in "data_[level]". There are 4 levels provided:
-        (1) Application level (overlap or rank matrics): [..]_rank_ovr
+        (1) Application level (overlap or rank metrics): [..]_rank_ovr
         (2) rank level (sum/average of I/O requests): [..]_rank
-        (3) high precesion rank level (overlap of I/O requests): [..]_ind_ovr
+        (3) high precision rank level (overlap of I/O requests): [..]_ind_ovr
         (4) I/O request level (lowest level): [..]_rank_over
 
-        if the 'ind' flag is not provieded, level (3) and (4) are skipped as they are 
-        expensive to calculate. 
-        
+        if the 'ind' flag is not provided, level (3) and (4) are skipped as they are
+        expensive to calculate.
+
 
         Args:
-            io_mode (str, optional): Can be read or write and 
+            io_mode (str, optional): Can be read or write and
             sync or async (required [b] or actual [t]). Supported modes are:
-            "read_sync", "write_sync", "read_async_t", "read_async_b", "write_async_t", 
+            "read_sync", "write_sync", "read_async_t", "read_async_b", "write_async_t",
             and "write_async_b".Defaults to "read_sync".
 
         Returns:
-            tuple[pd.DataFrame,pd.DataFrame, 
-            pd.DataFrame, pd.DataFrame, pd.DataFrame,]: Five dataframes are 
-            returned. The first one contains metrics like total bytes transfered, number 
-            of phases, etc.. The next 4 dataframes contain the I/O data at the 4 
+            tuple[pd.DataFrame,pd.DataFrame,
+            pd.DataFrame, pd.DataFrame, pd.DataFrame,]: Five dataframes are
+            returned. The first one contains metrics like total bytes transferred, number
+            of phases, etc.. The next 4 dataframes contain the I/O data at the 4
             levels explained above
         """
         name = ""
         data_metrics = np.array([])
         for i in range(0, self.n):
             value = getattr(self.s[i], io_mode)
             data = value.get_data()
@@ -248,16 +272,18 @@
                 data_rank_ovr = np.concatenate((data_rank_ovr, data[3]), axis=1)
                 data_rank = np.concatenate((data_rank, data[5]), axis=1)
                 data_ind_ovr = np.concatenate((data_ind_ovr, data[7]), axis=1)
                 data_ind = np.concatenate((data_ind, data[9]), axis=1)
             # data.append(d0)
         # check if there is data
         if data_metrics.size == 0:
-            raise RuntimeError(f"The mode {self.args.mode} contains no values\nChange the mode by using the -m argument.")
-        
+            raise RuntimeError(
+                f"The mode {self.args.mode} contains no values\nChange the mode by using the -m argument."
+            )
+
         df0 = pd.DataFrame(data_metrics, columns=name)
         df0 = df0.sort_values(by=["number_of_ranks"])
         df1 = pd.DataFrame(data_rank_ovr.transpose(), columns=name_rank_ovr)
         df1 = df1.astype({"number_of_ranks": "int"})
         df2 = pd.DataFrame(data_rank.transpose(), columns=name_rank)
         df3 = pd.DataFrame(data_ind_ovr.transpose(), columns=name_ind_ovr)
         df4 = pd.DataFrame(data_ind.transpose(), columns=name_ind)
@@ -279,64 +305,61 @@
 
             data.append(d0)
         df0 = pd.DataFrame(data, columns=name)
         df0 = df0.sort_values(by=["number_of_ranks"])
         return df0
 
 
-def check_open(file:str) -> None:
-    """Checks that the file is accessible 
+def check_open(file: str) -> None:
+    """Checks that the file is accessible
 
     Args:
         file (str): filename
     """
     if os.path.isfile(file):
         pass
     else:
         console = Console()
-        console.print(f"[red]--- Error  --- [/]\n"
+        console.print(
+            f"[red]--- Error  --- [/]\n"
             f"[red]-> Could not open file [b]{file}[/b]. \n[/]"
             f"[yellow]Make sure [b]{file}[/b] exists in [b]{os.getcwd()}[/b]. \n\n[/]"
         )
         exit()
 
 
-def get_rank(name:str) -> int:
+def get_rank(name: str) -> int:
     """Get the number of ranks from the name of the file
 
     Args:
         name (str): name of file
 
     Returns:
         int: number of ranks
     """
     if isinstance(name, int):
         return name
     else:
         start = name.rfind("/")
-        end = max(
-            name.rfind(".json"),
-            name.rfind(".darshan"),
-            name.rfind(".msgpack")
-        )
+        end = max(name.rfind(".json"), name.rfind(".darshan"), name.rfind(".msgpack"))
         rank = name[start + 1 : end]
         strs = ["_", "-", " "]
         if any(x in rank for x in strs):
             for x in strs:
                 if x in rank:
                     end = rank.rfind(x)
                     rank = rank[:end]
         return int(rank)
 
 
-def get_filename(path:str) -> str:
+def get_filename(path: str) -> str:
     """Reutrns filename from absolute path
 
     Args:
         path (str): absolute path to file (including name)
 
     Returns:
         str: filename
     """
     tmp = path.rfind("/")
     out = path[tmp + 1 :] if tmp > 0 else path
-    return out
+    return out
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/simrun.py` & `ftio_hpc-0.0.4/ftio/parse/simrun.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,88 @@
 from __future__ import annotations
+import re 
 import statistics as st
 from ftio.parse.sample import Sample
 from ftio.parse.time_io import Time
 from ftio.parse.percent import Percent
-import re 
+from ftio.parse.helper import match_mode
 class Simrun:
     """Stores the result from a single simulation including the:
     1. read sync
     2. read async
     3. write sync
     4. write async
-    5. I/O time (if avilable)
-    6. I/O percent (if avilable)
+    5. I/O time (if available)
+    6. I/O percent (if available)
     """
     def __init__(self, data, ext: str,  name: str, args, file_index: int = 0):
-        """create Simrun objct
+        """create Simrun object
 
         Args:
             data (array): contains data from simulation
             ext (str): 'json', 'jsonl', 'recorder', 'darshan', 'msgpack', or 'txt'
             name (str): name of simulation (e.g., 192.json)
-            args (argparse): comand line arguments
+            args (argparse): command line arguments
             file_index (int, optional): file index, in case several files have the same name
         """
         self.name       = name
         self.ranks      = self.get_rank(ext)
-        mode            = args.mode if args.mode else ''
+        mode            = match_mode(args.mode) if args.mode else ''
         args.file_index = file_index
-
-        #! list = jsonlines
+        supported_modes = ['read_sync', 'write_sync', 'read_async', 'write_async']
+        
+        #! list = JSONL
         if isinstance(data,list):
-            #! jsonlines need to be converted to a dict
+            #! JSONL need to be converted to a dict
             # if 'Time' in data[-1]:
             if 'jsonl' in ext or 'msgpack' in ext:
-                if mode and mode in ['sync_read', 'sync_write', 'async_read', 'async_write']:
+                if mode and mode in supported_modes:
                     self.reset(args)
                     self.assign(data, args, mode,'jsonl')
                 else:
                     self.read_sync     = self.merge_parts(data,'read_sync', args)
+                    self.write_sync    = self.merge_parts(data,'write_sync', args)
                     self.read_async_t  = self.merge_parts(data,'read_async_t', args)
                     self.read_async_b  = self.merge_parts(data,'read_async_b', args)
                     self.write_async_t = self.merge_parts(data,'write_async_t', args)
                     self.write_async_b = self.merge_parts(data,'write_async_b', args)
-                    self.write_sync    = self.merge_parts(data,'write_sync', args)
                     if any('io_time' in d for d in data):
                         self.io_time       = self.merge_parts(data,'io_time',args)
-                        self.io_percent    = Percent(self.io_time)
+                    else:
+                        self.io_time       = Time({},self.ranks,args)
+                    self.io_percent    = Percent(self.io_time)
             else:
                 raise ValueError('Data format empty or not supported')
 
         #! Darshan files or recorder files
         elif 'darshan' in ext or 'recorder' in ext:
             self.reset(args)
             self.read_sync         = Sample(data['read_sync'],'read_sync',args)
             self.write_sync        = Sample(data['write_sync'],'write_sync',args)
             self.io_time           = Time(data['io_time'],self.ranks,args)
 
         elif 'txt' in ext:
             self.reset(args)
-            mymode = self.getmode(mode)
-            setattr(self,mymode,Sample(data[mymode],mymode,args))
+            setattr(self,mode,Sample(data[mode],mode,args))
             self.io_time           = Time(data['io_time'],self.ranks,args)
 
         #! json files
         else:
             #! for dft to make it faster
-            if mode and mode in ['sync_read', 'sync_write', 'async_read', 'async_write']:
+            if mode and mode in supported_modes:
                 self.reset(args)
                 self.assign(data,args,mode)
                 return
             #! standard json files
             self.read_sync     = Sample(data['read_sync'],    'read_sync',args)
+            self.write_sync    = Sample(data['write_sync'],   'write_sync',args)
             self.read_async_t  = Sample(data['read_async_t'], 'read_async_t',args)
             self.read_async_b  = Sample(data['read_async_b'], 'read_async_b',args)
             self.write_async_t = Sample(data['write_async_t'],'write_async_t',args)
             self.write_async_b = Sample(data['write_async_b'],'write_async_b',args)
-            self.write_sync    = Sample(data['write_sync'],   'write_sync',args)
             if 'io_time' in data:
                 self.io_time       = Time(data['io_time'],self.ranks,args)
                 self.io_percent    = Percent(self.io_time)
 
 
 #---------------------------------------------------------------------------------------------------
 #?=======================
@@ -91,39 +94,43 @@
         Args:
             data (array): sim data
             args (argparse): command line arguments
             mode (str): mode to assign
             format (str, optional): json or jsonl. Defaults to 'json'.
         """
         if 'jsonl' in file_format:
-            if 'sync_read' == mode:
+            if 'read_sync' == mode:
                 self.read_sync     = self.merge_parts(data,'read_sync',args)
-            elif 'async_read' == mode:
+            elif 'read_async' == mode:
                 self.read_async_t  = self.merge_parts(data,'read_async_t',args)
                 self.read_async_b  = self.merge_parts(data,'read_async_b',args)
-            elif 'sync_write' == mode:
+            elif 'write_sync' == mode:
                 self.write_sync     = self.merge_parts(data,'write_sync',args)
-            elif 'async_write' == mode:
+            elif 'write_async' == mode:
                 self.write_async_t  = self.merge_parts(data,'write_async_t',args)
                 self.write_async_b  = self.merge_parts(data,'write_async_b',args)
             else:
                 pass
 
             if any('io_time' in d for d in data):
                 self.io_time       = self.merge_parts(data,'io_time',args)
                 self.io_percent    = Percent(self.io_time)
 
         else:
-            if 'sync_read' == mode:
+            if 'read_sync' == mode:
                 self.read_sync     = Sample(data['read_sync'],    'read_sync',args)
-            elif 'async_read' == mode:
+            elif 'read_async' == mode:
                 self.read_async_t  = Sample(data['read_async_t'], 'read_async_t',args)
-            elif 'async_write' == mode:
+                if 'read_async_b' in data:
+                    self.read_async_b  = Sample(data['read_async_b'], 'read_async_b',args)
+            elif 'write_async' == mode:
                 self.write_async_t = Sample(data['write_async_t'],'write_async_t',args)
-            elif 'sync_write' == mode:
+                if 'write_async_b' in data:
+                    self.write_async_b = Sample(data['write_async_b'],'write_async_b',args)
+            elif 'write_sync' == mode:
                 self.write_sync    = Sample(data['write_sync'],   'write_sync',args)
 
 
     def reset(self, args):
         """sets all fields to empty. This is usually followed by a assign call
 
         Args:
@@ -135,15 +142,15 @@
         self.write_async_t = Sample({'bandwidth':[]},'write_async_t', args)
         self.write_async_b = Sample({'bandwidth':[]},'write_async_b', args)
         self.write_sync    = Sample({'bandwidth':[]},'write_sync', args)
         self.io_time       = Time({}, self.ranks, args)
 
 
     def get_rank(self,ext:str) -> int:
-        """Get rank name from exetension
+        """Get rank name from extension
 
         Args:
             ext (str): extension type
 
         Returns:
             int: number of ranks that did I/O
         """
@@ -169,54 +176,54 @@
             except ValueError:
                 rank = re.findall(r'\d+', "hello 42 I'm a 32 string 30")
                 out = int(rank[-1])
         return out
 
 
     def print_rank(self,file):
-        """print rank maped to POINTS. This is used for 
+        """print rank mapped to POINTS. This is used for 
         Extra-P with the text file format.
 
         Args:
             file (fileptr): file pointer
         """
         file.write(f"POINTS ( {self.ranks:i} )\n")
 
 
-    def merge_parts(self,data,mode,args):
+    def merge_parts(self, data, mode, args):
         """merge jsonl parts to a single simulation
 
         Args:
-            data (2d array): array fo data elelements
+            data (2d array): array fo data elements
             mode (str): mode to merge
             args (argparse): command line arguments
 
         Returns:
-            io_sampe object: iosample of the whole simulation
+            io_sample object: iosample of the whole simulation
         """
         data_array     = [item[mode] for item in data if mode in item]
         out = []
         if len(data_array) <= 1:
             if "time" in mode:
-                out = Time(data_array[0],self.ranks,args)
+                out = Time(data_array[0],self.ranks,args) if len(data_array) > 0 else Time({},self.ranks,args)
             else:
-                out = Sample(data_array[0],mode,args)
+                out = Sample(data_array[0],mode,args)  if len(data_array) > 0 else Sample({},mode,args)
         else:
             data_array = self.merge_fields(data_array)
             if "time" in mode:
                 out = Time(data_array,self.ranks,args)
             else:
                 out = Sample(data_array,mode,args)
         return out
 
 
     def merge_fields(self,data_array, keys: list[str] = []) -> dict:
         """Merges the metrics field from different files. For example,
         JsonlLines file constantly append new data. To merge the previous 
-        metrics with the new one, this function itterates over the fields 
+        metrics with the new one, this function iterates over the fields 
         and merges them.
 
         Args:
             data_array (dataframe): Metrics
             keys (list[str], optional): _description_. Defaults to list[str].
 
         Returns:
@@ -242,21 +249,8 @@
                     elif any([x in field for x in ['max','number']]):
                         my_dict[field] = max(x[field] for x in data_array)
                     elif 'min' in field:
                         my_dict[field] = min(x[field] for x in data_array)
                     elif 'arithmetic_mean' in field:
                         my_dict[field] = st.mean(x[field] for x in data_array)
 
-        return my_dict
-
-    def getmode(self, mode:str) -> str:
-        if "w" in mode:
-            out = "write"
-        else:
-            out = "read"
-            
-        if "async" in mode:
-            out = out + "_async_t"
-        else:
-            out = out + "_sync"
-
-        return out 
+        return my_dict
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/time_io.py` & `ftio_hpc-0.0.4/ftio/parse/time_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         self.delta_t_total    = self.delta_t_overhead + self.delta_t_agg
         self.rank = rank
 
         self.delta_t_rank0                       = self.assign(data,"delta_t_rank0") 
         self.delta_t_rank0_app                   = self.assign(data,"delta_t_rank0_app") 
         self.delta_t_rank0_overhead_post_runtime = self.assign(data,"delta_t_rank0_overhead_post_runtime") 
         self.delta_t_rank0_overhead_peri_runtime = self.assign(data,name="delta_t_rank0_overhead_peri_runtime") 
-        # TODO: compatibility mode with erlier versions
+        # TODO: compatibility mode with earlier versions
         if "delta_t_rank0_overhead_peri_runtime" not in data:
             self.delta_t_rank0_overhead_peri_runtime = self.assign(data,name="delta_t_rank0_overhead_runtime") 
 
     def get_data(self):
-		#! append list is much faster than appen data frame
+		#! append list is much faster than append data frame
         name0 = []
         data0 = []
         name0.append("number_of_ranks")
         data0.append(self.rank)
         for attr, value in self.__dict__.items():
             name0.append(attr)
             data0.append(value)
```

### Comparing `ftio-hpc-0.0.3/ftio/parse/txt_reader.py` & `ftio_hpc-0.0.4/ftio/parse/txt_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     with open(file_path, 'r') as file:
         data = file.read()
         for key, pattern in patterns.items():
             match = re.search(pattern, data)
             if match:
                 if ',' in match.group(1):
                     # If the matched group contains commas, split and convert to integers
-                    results[key] = list(float(val) if '.' in val else int(val) for val in match.group(1).split(','))
+                    tmp = match.group(1).replace(', ',',')
+                    results[key] = list(float(val) if '.' in val else int(val) for val in tmp.split(','))
 
                 else:
                     results[key] = int(match.group(1))
             else:
                 print(f"Unable to extract data for {key} from the file.")
 
     return results
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/callback_files/callbacks.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/callback_files/callbacks.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/callback_files/io_mode_callbacks.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/callback_files/io_mode_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 from plotly_resampler.figure_resampler import figure_resampler_interface
 
 figure_resampler_interface.PlotlyAggregatorParser = patched_parser
 # end of problem solving issue #257
 # -------
 
 
-def _create_id_figure(data: DataSource, file: str = ""):
-    return f"{data.io_mode}-{file}"
+def _create_id_figure(data: DataSource, filename: str = ""):
+    return f"{data.io_mode}-{filename}"
 
 
 def _find_x_min_and_max(file_data: FileData, data: DataSource) -> tuple[float, float]:
     x_min = np.inf
     x_max = -np.inf
     if file_data.data_actual_is_not_empty:
         x_min = min(x_min, min(file_data.actual_time_overlap, default=0.0))
@@ -178,15 +178,15 @@
         title = "{} Ranks (Run {}: {})".format(file_data.rank, file_data.run, file_data.name)
 
     fig.update_layout(
         margin=dict(l=10, r=10, t=50, b=70),
         yaxis_rangemode="nonnegative",
         barmode="stack",
         xaxis_title="Time (s)",
-        yaxis_title="Transfer Rate (B/s)",
+        yaxis_title="Transfer Rate (MB/s)",
         font=dict(family=data.fontfamily, size=data.fontsize),
         width=data.width_figure,
         height=data.height_figure,
         title=title,
     )
 
 
@@ -213,64 +213,64 @@
             tickmode="auto",
             nticks=10,
             showgrid=True,
         ),
     )
 
 
-def _create_separate_figures(files: list[str], data: DataSource) -> dict:
+def _create_separate_figures(filenames: list[str], data: DataSource) -> dict:
     figure_by_id_figure = dict()
 
-    for file in files:
-        file_data = data.file_data_by_file[file]
+    for filename in filenames:
+        file_data = data.file_data_by_filename[filename]
         fig = FigureResampler(
             default_n_shown_samples=data.n_shown_samples,
             default_downsampler=MinMaxAggregator(),
             default_gap_handler=NoGapHandler(),
         )
         _add_traces(fig, file_data, data)
 
         _update_layout(fig, file_data, data)
         _update_axes(fig)
 
-        id_figure = _create_id_figure(data, file)
+        id_figure = _create_id_figure(data, filename)
         figure_by_id_figure[id_figure] = fig
     return figure_by_id_figure
 
 
-def _create_one_figure(files: list[str], data: DataSource) -> dict:
+def _create_one_common_figure(filenames: list[str], data: DataSource) -> dict:
     figure_by_id_figure = dict()
 
     fig = FigureResampler(
         default_n_shown_samples=data.n_shown_samples,
         default_downsampler=MinMaxAggregator(),
         default_gap_handler=NoGapHandler(),
     )
 
-    for file in files:
-        file_data = data.file_data_by_file[file]
+    for filename in filenames:
+        file_data = data.file_data_by_filename[filename]
         _add_traces(fig, file_data, data)
 
     _update_layout(fig, file_data, data)
     _update_axes(fig)
     id_figure = _create_id_figure(data)
     figure_by_id_figure[id_figure] = fig
     return figure_by_id_figure
 
 
 def _append_merged_plot(
-    div_children: html.Div, figure_by_id_figure: dict[str, FigureResampler], data: DataSource
+    div_children: list[html.Div], figure_by_id_figure: dict[str, FigureResampler], data: DataSource
 ) -> html.Div:
     id_figure = _create_id_figure(data)
     new_child = html.Div(
         children=[
             dcc.Graph(
                 id={"type": id.TYPE_DYNAMIC_GRAPH, "index": id_figure},
                 figure=figure_by_id_figure[id_figure],
-                mathjax=True,
+                mathjax=True, responsive=True,
             ),
             TraceUpdater(
                 id={
                     "type": id.TYPE_DYNAMIC_UPDATER_BY_IO_MODE[data.io_mode],
                     "index": id_figure,
                 },
                 gdID=f"{id_figure}",
@@ -280,28 +280,28 @@
     div_children.append(new_child)
     return div_children
 
 
 def _append_each_figure_separately(
     div_children: list[html.Div],
     figure_by_id_figure: dict[str, FigureResampler],
-    files: list[str],
+    filenames: list[str],
     data: DataSource,
 ) -> html.Div:
-    for rank in data.ranks:
-        for file in files:
-            if data.file_data_by_file[file].rank != rank:
+    for rank in data.ranks_unique:
+        for filename in filenames:
+            if data.file_data_by_filename[filename].rank != rank:
                 continue
-            id_figure = _create_id_figure(data, file)
+            id_figure = _create_id_figure(data, filename)
             new_child = html.Div(
                 children=[
                     dcc.Graph(
                         id={"type": id.TYPE_DYNAMIC_GRAPH, "index": id_figure},
                         figure=figure_by_id_figure[id_figure],
-                        mathjax=True,
+                        mathjax=True, responsive=True,
                     ),
                     TraceUpdater(
                         id={
                             "type": id.TYPE_DYNAMIC_UPDATER_BY_IO_MODE[data.io_mode],
                             "index": id_figure,
                         },
                         gdID=f"{id_figure}",
@@ -320,35 +320,35 @@
         data (DataSource): data_source belonging to the io_mode
     """
 
     @app.callback(
         Output(id.STORE_FIGURES_BY_IO_MODE[data.io_mode], "data"),
         Input(id.DROPDOWN_FILE, "options"),
     )
-    def create_figures(files: list[str]) -> dict[str, FigureResampler]:
+    def create_figures(filenames: list[str]) -> dict[str, FigureResampler]:
         figure_by_id_figure = dict()
 
         if data.merge_plots_is_selected:
-            figure_by_id_figure = _create_one_figure(files, data)
+            figure_by_id_figure = _create_one_common_figure(filenames, data)
         else:
-            figure_by_id_figure = _create_separate_figures(files, data)
+            figure_by_id_figure = _create_separate_figures(filenames, data)
 
         return Serverside(figure_by_id_figure)
 
     @app.callback(
         Output(id.DIV_IO_BY_IO_MODE[data.io_mode], "children"),
         State(id.CHECKLIST_IO_MODE, "value"),
         State(id.DROPDOWN_FILE, "value"),
         State(id.STORE_FIGURES_BY_IO_MODE[data.io_mode], "data"),
         Input(id.BUTTON_SHOW, "n_clicks"),
         prevent_initial_call=True,
     )
     def fill_div_graph(
         io_modes: list[str],
-        files: list[str],
+        filenames: list[str],
         figure_by_id_figure: dict[str, FigureResampler],
         n_clicks: int,
     ):
         if data.io_mode not in io_modes:
             return []
 
         div_children = [
@@ -360,15 +360,15 @@
             )
         ]
 
         if data.merge_plots_is_selected:
             div_children = _append_merged_plot(div_children, figure_by_id_figure, data)
         else:
             div_children = _append_each_figure_separately(
-                div_children, figure_by_id_figure, files, data
+                div_children, figure_by_id_figure, filenames, data
             )
 
         return div_children
 
     @app.callback(
         Output(
             {"type": id.TYPE_DYNAMIC_UPDATER_BY_IO_MODE[data.io_mode], "index": MATCH},
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/constants/id.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/constants/id.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/constants/legend_group.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/constants/legend_group.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/dash_app.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/dash_app.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/dash_files/data_source.py` & `ftio_hpc-0.0.4/ftio/plot/dash_files/data_source.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         name: str,
         data_actual: list[pd.DataFrame],
         data_required: list[pd.DataFrame],
     ):
         self._run = run
         self._rank = rank
         self._name = name
-
         self._data_actual = data_actual
         self._data_required = data_required
         self._init_masks()
 
     def _init_masks(self):
         self._mask = self._data_actual[1]["number_of_ranks"].isin([self.rank])
         self._mask_ind = self._data_actual[3]["number_of_ranks"].isin([self.rank])
@@ -87,113 +86,122 @@
         return self._data_required[3]["b_overlap_ind"][self._mask_ind][self._mask2_ind]
 
 
 class DataSource:
     def __init__(self, plot_core, io_mode: str):
         self._io_mode = io_mode
         self._plot_core = plot_core
-        self._names = plot_core.names
+
         self._data = plot_core.data
 
         self._init_data_actual_and_required()
-        self._init_ranks()
+        self._init_names_and_ranks()
         self._init_file_data_dictionary()
 
     def _init_data_actual_and_required(self):
         match self.io_mode:
             case io_mode.ASYNC_READ:
-                self._data_actual = (
+                self._data_actual: list[pd.DataFrame] = (
                     self._data.df_rat
                     if not (self._data.df_rat is None or self._data.df_rat[1].empty)
                     else []
                 )
-                self._data_required = (
+                self._data_required: list[pd.DataFrame] = (
                     self._data.df_rab
                     if not (self._data.df_rab is None or self._data.df_rab[1].empty)
                     else []
                 )
             case io_mode.ASYNC_WRITE:
-                self._data_actual = (
+                self._data_actual: list[pd.DataFrame] = (
                     self._data.df_wat
                     if not (self._data.df_wat is None or self._data.df_wat[1].empty)
                     else []
                 )
-                self._data_required = (
+                self._data_required: list[pd.DataFrame] = (
                     self._data.df_wab
                     if not (self._data.df_wab is None or self._data.df_wab[1].empty)
                     else []
                 )
             case io_mode.SYNC_READ:
-                self._data_actual = (
+                self._data_actual: list[pd.DataFrame] = (
                     self._data.df_rst
                     if not (self._data.df_rst is None or self._data.df_rst[1].empty)
                     else []
                 )
-                self._data_required = []
+                self._data_required: list[pd.DataFrame] = []
             case io_mode.SYNC_WRITE:
-                self._data_actual = (
+                self._data_actual: list[pd.DataFrame] = (
                     self._data.df_wst
                     if not (self._data.df_wst is None or self._data.df_wst[1].empty)
                     else []
                 )
-                self._data_required = []
+                self._data_required: list[pd.DataFrame] = []
             case _:
                 raise Exception("invalid mode")
 
-    def _init_ranks(self) -> None:
-        self._ranks = []
+    def _init_names_and_ranks(self) -> None:
+        self._ranks: pd.Series = pd.Series()
         if len(self._data_actual) != 0:
-            self._ranks = self._data_actual[0]["number_of_ranks"]
+            self._ranks = self._data_actual[0]["number_of_ranks"].astype(int)
         elif len(self._data_required) != 0:
-            self._ranks = self._data_required[0]["number_of_ranks"]
-        self._ranks: list[int] = pd.unique(self._ranks).astype(int).tolist()
-        self._ranks.sort()
+            self._ranks = self._data_required[0]["number_of_ranks"].astype(int)
+        names_and_ranks_df = pd.concat(
+            [pd.Series(self._plot_core.names, name="filenames"), self._ranks], axis=1
+        )
+        self._filenames = names_and_ranks_df["filenames"].to_list()
+        self._ranks = names_and_ranks_df["number_of_ranks"].to_list()
+        self._ranks_unique = pd.unique(self.ranks)
+        self._ranks_unique.sort()
 
     def _init_file_data_dictionary(self):
-        self._file_data_by_file: dict[str, FileData] = dict()
-        for idx, file in enumerate(self._data.paths):
-            self._file_data_by_file[file] = FileData(
+        self._file_data_by_filename: dict[str, FileData] = dict()
+        for idx, filename in enumerate(self._filenames):
+            self._file_data_by_filename[filename] = FileData(
                 idx,
                 self._ranks[idx],
-                self.names[idx],
+                self._filenames[idx],
                 self._data_actual,
                 self._data_required,
             )
 
     @property
     def io_mode(self) -> str:
         return self._io_mode
 
     @property
-    def names(self) -> list[str]:
-        return self._names
+    def filenames(self) -> list[str]:
+        return self._filenames
+
+    @property
+    def ranks(self) -> list[int]:
+        return self._ranks
+
+    @property
+    def ranks_unique(self) -> list[int]:
+        return self._ranks_unique
 
     @property
     def fontfamily(self) -> str:
-        return self._plot_core.fontfamily
+        return "Courier New, monospace"
 
     @property
     def fontsize(self) -> int:
-        return self._plot_core.size
+        return 17
 
     @property
     def width_figure(self) -> int:
         return self._plot_core.width
 
     @property
     def height_figure(self) -> int:
         return self._plot_core.height
 
     @property
-    def ranks(self) -> list[int]:
-        return self._ranks
-
-    @property
-    def file_data_by_file(self) -> dict[str, FileData]:
-        return self._file_data_by_file
+    def file_data_by_filename(self) -> dict[str, FileData]:
+        return self._file_data_by_filename
 
     @property
     def individual_is_selected(self) -> bool:
         return self._data.args.ind
 
     @property
     def n_shown_samples(self) -> int:
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/helper.py` & `ftio_hpc-0.0.4/ftio/plot/helper.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/plot_core.py` & `ftio_hpc-0.0.4/ftio/plot/plot_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from ftio.parse.metrics import Metrics
 from ftio.parse.scales import Scales
 from ftio.plot.dash_files.dash_app import IOAnalysisApp
 from ftio.plot.print_html import print_html
 from ftio.plot.helper import *  
 from ftio.plot.plot_error import plot_error_bar, plot_time_error_bar
 from ftio.plot.units import find_unit
+from ftio.freq.helper import MyConsole
+
+
+CONSOLE = MyConsole()
 
 def _find_free_port():
     sock = socket.socket()
     sock.bind(("", 0))
     return sock.getsockname()[1]
 
 
@@ -120,43 +124,45 @@
             for thread in t:
                 thread.start()
 
             for thread in t:
                 thread.join()
         else:
             if "stat" in args.render:
-                if "async_write" in args.mode:
-                    self.plot_io_mode("async write", self.data.df_wat, self.data.df_wab)
-                elif "async_read" in args.mode:
-                    self.plot_io_mode("async read", self.data.df_rat, self.data.df_rab)
-                elif "sync_write" in args.mode:
-                    self.plot_io_mode("sync write", self.data.df_wst)
-                elif "sync_read" in args.mode:
-                    self.plot_io_mode("sync read", self.data.df_rst)
+                if "async" in args.mode:
+                    if "write" in args.mode:
+                        self.plot_io_mode("async write", self.data.df_wat, self.data.df_wab)
+                    else:
+                        self.plot_io_mode("async read", self.data.df_rat, self.data.df_rab)
+                elif "sync" in args.mode:
+                    if "write" in args.mode:
+                        self.plot_io_mode("sync write", self.data.df_wst)
+                    else:
+                        self.plot_io_mode("sync read", self.data.df_rst)
                 else:
                     pass
                 exit(0)
             else:
                 self.plot_time()
                 out.generate_html_core("time.html", self.get_figure("time.html"))
                 self.plot_io_mode("async write", self.data.df_wat, self.data.df_wab)
                 out.generate_html_core(
-                    "async_write.html", self.get_figure("async_write.html")
+                    "write_async.html", self.get_figure("write_async.html")
                 )
                 self.plot_io_mode("async read", self.data.df_rat, self.data.df_rab)
                 out.generate_html_core(
-                    "async_read.html", self.get_figure("async_read.html")
+                    "read_async.html", self.get_figure("read_async.html")
                 )
                 self.plot_io_mode("sync write", self.data.df_wst)
                 out.generate_html_core(
-                    "sync_write.html", self.get_figure("sync_write.html")
+                    "write_sync.html", self.get_figure("write_sync.html")
                 )
                 self.plot_io_mode("sync read", self.data.df_rst)
                 out.generate_html_core(
-                    "sync_read.html", self.get_figure("sync_read.html")
+                    "read_sync.html", self.get_figure("read_sync.html")
                 )
 
         out.generate_html_end()
         print("\033[1;32m------------------- done -------------------\n\033[1;0m")
 
         return [*self.f_aw, *self.f_ar, *self.f_sr, *self.f_sr, *self.f_t]
 
@@ -164,31 +170,31 @@
     # *                       2. plot Multithreaded
     # **********************************************************************
     def plot_and_generate_html(self, mode, out):
         if "async" in mode:
             if "write" in mode:
                 self.plot_io_mode("async write", self.data.df_wat, self.data.df_wab)
                 out.generate_html_core(
-                    "async_write.html", self.get_figure("async_write.html")
+                    "write_async.html", self.get_figure("write_async.html")
                 )
             else:
                 self.plot_io_mode("async read", self.data.df_rat, self.data.df_rab)
                 out.generate_html_core(
-                    "async_read.html", self.get_figure("async_read.html")
+                    "read_async.html", self.get_figure("read_async.html")
                 )
         elif "sync" in mode:
             if "write" in mode:
                 self.plot_io_mode("sync write", self.data.df_wst)
                 out.generate_html_core(
-                    "sync_write.html", self.get_figure("sync_write.html")
+                    "write_sync.html", self.get_figure("write_sync.html")
                 )
             else:
                 self.plot_io_mode("sync read", self.data.df_rst)
                 out.generate_html_core(
-                    "sync_read.html", self.get_figure("sync_read.html")
+                    "read_sync.html", self.get_figure("read_sync.html")
                 )
         else:
             self.plot_time()
             out.generate_html_core("time.html", self.get_figure("time.html"))
 
     # **********************************************************************
     # *                       2. plot
@@ -460,64 +466,67 @@
                 for j in range(
                     int(df_t[1]["file_index"][index].min()),
                     int(df_t[1]["file_index"][index].max() + 1),
                 ):
                     f.append(go.Figure())
                     index2 = df_t[1]["file_index"][index].isin([j])
                     index2_ind = df_t[3]["file_index"][index_ind].isin([j])
-
                     # finder the order and unit of the plots on y-axis
                     unit, order = find_unit(df_t,index,index2,index_ind,index2_ind,args)
+                    # # compatibility mode with earlier version
+                    # CONSOLE.info(f"[yellow]WARNING:[/] Compatibility Mode")
+                    # unit, order = find_unit(df_t,index,index2,index_ind,index2_ind,args,pow(10,6)) 
+                    # order = order*pow(10,6)
                     # ? Avr plot
                     if args.avr:
                         if df_t:
                             f[-1].add_trace(
                                 go.Scatter(
                                     x=df_t[1]["t_overlap"][index][index2],
                                     y=df_t[1]["b_overlap_avr"][index][index2]*order,
                                     mode="lines",
-                                    name="$T_A$",
+                                    name="$T_A$", #name="$T$", # For BW limit paper
                                     line={"shape": "hv"},
                                     fill="tozeroy",
                                 )
                             )
-                            # f[-1].add_trace(go.Scatter(x=df_t[1]['t_overlap'][index][index2], y=df_t[1]['b_overlap_avr'][index][index2],  mode = 'lines',name = '$T$',line={"shape": 'hv'}, fill='tozeroy'))
+
                         if df_b:
                             f[-1].add_trace(
                                 go.Scatter(
                                     x=df_b[1]["t_overlap"][index][index2],
                                     y=df_b[1]["b_overlap_avr"][index][index2]*order,
                                     mode="lines",
-                                    name="$B_A$",
+                                    name="$B_A$", #name="$B_L$", # For BW limit paper
                                     line={"shape": "hv"},
                                     fill="tozeroy",
                                 )
-                            )  # , visible='legendonly'))#, "dash": "dash"}))
+                            )
 
                     # ? Sum plot
                     if args.sum:
                         if df_t:
                             f[-1].add_trace(
                                 go.Scatter(
                                     x=df_t[1]["t_overlap"][index][index2],
                                     y=df_t[1]["b_overlap_sum"][index][index2]*order,
                                     mode="lines",
                                     name="$T_S$",
                                     line={"shape": "hv"},
                                     fill="tozeroy",
-                                )
-                            )  # , visible='legendonly'))
-                            pass
+                                    )
+                                )  
+
                         if df_b:
                             f[-1].add_trace(
                                 go.Scatter(
                                     x=df_b[1]["t_overlap"][index][index2],
                                     y=df_b[1]["b_overlap_sum"][index][index2]*order,
                                     mode="lines",
-                                    name="$B_S$",
+                                    name="$B_S$",#name="$B$", # For BW limit paper
                                     line={"shape": "hv"},
                                     fill="tozeroy",
                                 )
                             )
 
                     # ? ind plot
                     if args.ind:
@@ -527,40 +536,42 @@
                                     x=df_t[3]["t_overlap_ind"][index_ind][index2_ind],
                                     y=df_t[3]["b_overlap_ind"][index_ind][index2_ind]*order,
                                     mode="lines",
                                     name="$T_E$",
                                     line={"shape": "hv"},
                                     fill="tozeroy",
                                 )
-                            )  # , visible='legendonly')),
-                            # f[-1].add_trace(go.Scatter(x=df_t_ind['t'], y=df_t_ind['b'],  mode = 'lines',name = '$T_E$',line={"shape": 'hv'}, fill='tozeroy' ))#, visible='legendonly')),
+                            ) 
+
                         if df_b:
                             f[-1].add_trace(
                                 go.Scatter(
                                     x=df_b[3]["t_overlap_ind"][index_ind][index2_ind],
                                     y=df_b[3]["b_overlap_ind"][index_ind][index2_ind]*order,
                                     mode="lines",
                                     name="$B_E$",
                                     line={"shape": "hv"},
                                     fill="tozeroy",
                                 )
-                            )  # , visible='legendonly' ))
+                            )  
+
                     f[-1].update_layout(
                         barmode="stack",
                         xaxis_title="Time (s)",
                         yaxis_title=f"Transfer Rate ({unit})",
                         width=self.width,
                         height=self.height,
+                        showlegend=True,
                         title=f"{i} Ranks (Run {j})",
                     )
                     f[-1] = format_plot(f[-1])
-
+                    
                     if self.names and (args.avr or args.sum or args.ind):
                         f[-1].update_layout(
-                            title=f"{i} Ranks (Run {j}: {self.names[j]})"
+                            title=f"{i} Ranks (Run {j}: {self.names[j]})",
                         )
 
                     if args.avr or args.sum or args.ind:
                         if args.zoom:
                             f[-1].update_layout(yaxis_range=[0, args.zoom])
                         else:
                             f[-1].update_layout(yaxis_rangemode="nonnegative")
@@ -2003,21 +2014,21 @@
         # print('%i figures'%len(self.f))
 
     # **********************************************************************
     # *                       6. Set and Get Functions
     # **********************************************************************
 
     def get_figure(self, mode):
-        if "async_write" in mode:
+        if "write_async" in mode:
             return self.f_aw
-        if "async_read" in mode:
+        if "read_async" in mode:
             return self.f_ar
-        if "sync_write" in mode:
+        if "write_sync" in mode:
             return self.f_sw
-        if "sync_read" in mode:
+        if "read_sync" in mode:
             return self.f_sr
         if "time" in mode:
             return self.f_t
 
     def set_figure(self, f, mode):
         # assign
         if "async" in mode:
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/plot_error.py` & `ftio_hpc-0.0.4/ftio/plot/plot_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -285,8 +285,8 @@
         hovermode="x",
         legend_tracegroupgap=1,
         width=990,
         height=640,
         title="I/O time with error bars (normed)",
     )
     f = format_plot(f)
-    return f
+    return f
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/print_html.py` & `ftio_hpc-0.0.4/ftio/plot/print_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 os.mkdir(self.path)
                 print(f" '-> Directory {self.outdir} created in {pwd}")
             else:
                 print(f" '-> Directory {self.outdir}  exists  in {pwd}")
         
             #?* create main HTML file
             #*-------------------------
-            # html_files = ["async_write.html","async_read.html","sync_write.html","sync_read.html","time.html"] 
+            # html_files = ["write_async.html","read_async.html","write_sync.html","read_sync.html","time.html"] 
             print(f"\n '-> To see intermediate result call: \n     open {self.path}/main.html \n")
             self.filename = os.path.join(self.path,self.filename)
             print(" '-> Generated main.html ")
             with open(self.filename, "w") as file:
                 file.write("<html><head></head><body>\n")
                 file.write("<center><h1 style=\"color:black;\"> Results </h1> </center><hr style=\"height:2px;border-width:0;color:gray;background-color:gray\">\n")
 
@@ -101,15 +101,15 @@
                 except:
                     os.system(f"powershell.exe start./{self.path}/main.html")
 
 
 #**********************************************************************
 #*                       1. figures_to_html
 #**********************************************************************
-def figures_to_html(figs, filename="async_write.html",names=[]) -> None:
+def figures_to_html(figs, filename="write_async.html",names=[]) -> None:
     # conf = {  "toImageButtonOptions": {     "format": "svg", "scale":1  }}
     conf = {  "toImageButtonOptions": {     "format": "png", "scale":2 }}
     template = """
     <!DOCTYPE html>
     <html lang="en">
     <head>
     <meta charset="utf-8"/>
```

### Comparing `ftio-hpc-0.0.3/ftio/plot/stack_plot.py` & `ftio_hpc-0.0.4/ftio/plot/stack_plot.py`

 * *Files identical despite different names*

### Comparing `ftio-hpc-0.0.3/ftio/plot/units.py` & `ftio_hpc-0.0.4/ftio/plot/units.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import numpy as np
 import pandas as pd
 
-def set_unit(arr:np.ndarray) -> tuple[str, float]:
+def set_unit(arr:np.ndarray|float, suffix = "B/s") -> tuple[str, float]:
     """set unit for the plots
 
     Args:
         arr (np.ndarray): array
+        unit (optional): default B/s
 
     Returns:
         unit (string): unit in GB/s, MB/s, KB/s or B/s
         arr: scaled array according to the unit
     """
-    unit = "B/s"
+    unit = suffix
     order = 1e-0
     if isinstance(arr, np.ndarray):
         pass
     elif isinstance(arr, pd.DataFrame):
         arr = arr.to_numpy()
+    elif isinstance(arr,float) or isinstance(arr,int):
+        arr = np.array(arr)
     
-    if arr.size > 0:
+    if arr.size > 0 and np.max(arr) > 0:
         order = np.log10(np.max(arr))
 
     if order > 9:
         order = 1e-9
-        unit = "GB/s"
+        unit = "G"+suffix
     elif order > 6:
         order = 1e-6
-        unit = "MB/s"
+        unit = "M"+suffix
     elif order > 3:
         order = 1e-3
-        unit = "KB/s"
+        unit = "K"+suffix
     else:
         pass
 
     return unit, order
 
 
 
-def find_unit(df_t,index,index2,index_ind,index2_ind,args):
+def find_unit(df_t,index,index2,index_ind,index2_ind,args, offset=1):
     unit = "B/s"
     order = 1e-0
     if args.avr:
-        tmp_unit, tmp_order = set_unit(df_t[1]["b_overlap_avr"][index][index2])
+        tmp_unit, tmp_order = set_unit(df_t[1]["b_overlap_avr"][index][index2]*offset)
         if tmp_order < order:
             order = tmp_order
             unit = tmp_unit
 
     if args.sum:
-        tmp_unit, tmp_order = set_unit(df_t[1]["b_overlap_sum"][index][index2])
+        tmp_unit, tmp_order = set_unit(df_t[1]["b_overlap_sum"][index][index2]*offset)
         if tmp_order < order:
             order = tmp_order
             unit = tmp_unit
 
     if args.ind:
-        tmp_unit, tmp_order = set_unit(df_t[3]["b_overlap_ind"][index_ind][index2_ind])
+        tmp_unit, tmp_order = set_unit(df_t[3]["b_overlap_ind"][index_ind][index2_ind]*offset)
         if tmp_order < order:
             order = tmp_order
             unit = tmp_unit
 
     return unit, order
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/analysis.py` & `ftio_hpc-0.0.4/ftio/prediction/analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,140 @@
-"""Performs the anylsis for prediction. This includes the calculation of ftio and parsing of the data into a queue """
+"""Performs the analysis for prediction. This includes the calculation of ftio and parsing of the data into a queue """
 from __future__ import annotations
 from multiprocessing import  Queue
-from ftio.cli import ftio_core
-from ftio.prediction.helper import get_dominant
 from rich.console import Console
 import numpy as np
+from ftio.cli import ftio_core
+from ftio.prediction.helper import get_dominant, get_hits
+from ftio.plot.units import set_unit
 
-
-def ftio_process(queue: Queue, count, hits, start_time, aggregated_bytes, args) -> None:
+def ftio_process(queue: Queue, count, hits, start_time, aggregated_bytes, args, msgs=None) -> None:
     """Perform a single prediction
 
     Args:
 
         queue (Manager().Queue): queue for FTIO data
         count (Manager().Value): number of prediction
-        hits (Manager().Value): hits indicating how often a dominant frequncy was found
+        hits (Manager().Value): hits indicating how often a dominant frequency was found
         start_time (Manager().Value): start time window for ftio
         aggregated_bytes (Manager().Value): total bytes transferred so far
         args (list[str]): additional arguments passed to ftio
     """
     console = Console()
-    console.print(f"[purple][PREDICTOR] (#{count.value}):[/]  Started")
+    console.print(f'[purple][PREDICTOR] (#{count.value}):[/]  Started')
     # Modify the arguments
-    args.extend(["-e", "no"])
-    args.extend(["-ts", f"{start_time.value:.2f}"])
+    args.extend(['-e', 'no'])
+    args.extend(['-ts', f'{start_time.value:.2f}'])
+    
     # perform prediction
-    prediction, args = ftio_core.main(args)
+    prediction, args = ftio_core.main(args,msgs)
+    
     # get data
-    t_s = prediction["t_start"]
-    t_e = prediction["t_end"]
-    total_bytes = prediction["total_bytes"]
     freq = get_dominant(prediction) #just get a single dominant value
     hits = get_hits(prediction,count.value,hits)
-    # save data
-    queue.put(
-        {
-            "phase": count.value,
-            "dominant_freq": prediction["dominant_freq"],
-            "conf": prediction["conf"],
-            "t_start": prediction["t_start"],
-            "t_end": prediction["t_end"],
-            "total_bytes": prediction["total_bytes"],
-            "ranks": prediction["ranks"],
-            "freq": prediction["freq"],
-            "hits": hits.value,
-        }
-    )
-    
-    text = ""
-    if not np.isnan(freq):
-        text = f"[purple][PREDICTOR] (#{count.value}):[/] Dominant freq {freq:.3f} \n"
 
-    text += (
-        f"[purple][PREDICTOR] (#{count.value}):[/] Time window {t_e-t_s:.3f} sec ([{t_s:.3f},{t_e:.3f}] sec)\n"
-        f"[purple][PREDICTOR] (#{count.value}):[/] Total bytes {total_bytes:.3f} B\n"
-        f"[purple][PREDICTOR] (#{count.value}):[/] Bytes transferred since last "
-        f"time {abs(total_bytes-aggregated_bytes.value):.3f} B\n"
-        )
-    # safe total transferred bytes
-    aggregated_bytes.value = total_bytes
-    
+    # save prediction results
+    save_data(queue, prediction, aggregated_bytes, count, hits)
+    # display results
+    text = display_result(freq ,prediction ,count, aggregated_bytes)
+    # data analysis to decrease window
+    text, start_time.value = data_analysis(args, prediction, freq, count, hits, text)
+    console.print(text)
+    count.value += 1
+
+
+def data_analysis(args, prediction, freq, count, hits, text:str) -> tuple[str, float]:
     # average data/data processing
+    t_s = prediction['t_start']
+    t_e = prediction['t_end']
+    total_bytes = prediction['total_bytes']
     if not np.isnan(freq):
         n_phases = (t_e-t_s)*freq
         avr_bytes = int(total_bytes/float(n_phases))
+        unit, order = set_unit(avr_bytes,'B')
+        avr_bytes = order *avr_bytes
+        
         #FIXME this needs to compensate for a smaller windows
         if not args.window_adaptation:
             text += (
-                f"[purple][PREDICTOR] (#{count.value}):[/] Estimated phases {n_phases:.2f}\n"
-                f"[purple][PREDICTOR] (#{count.value}):[/] Average transferred {avr_bytes:.3f} B\n"
+                f'[purple][PREDICTOR] (#{count.value}):[/] Estimated phases {n_phases:.2f}\n'
+                f'[purple][PREDICTOR] (#{count.value}):[/] Average transferred {avr_bytes:.0f} {unit}\n'
             )
         
         # adaptive time window
         if args.window_adaptation:
-            if hits.value > args.x_hits: 
+            if hits.value > args.frequency_hits: 
                 if True: #np.abs(avr_bytes - (total_bytes-aggregated_bytes.value)) < 100:
                     tmp = t_e - 3*1/freq
-                    start_time.value = tmp if tmp > 0 else 0
-                    aggregated_bytes.value = total_bytes
-                    text += f"[purple][PREDICTOR] (#{count.value}):[/][green] Adjsuting start time to {start_time.value} sec\n[/]"
+                    t_s = tmp if tmp > 0 else 0
+                    text += f'[purple][PREDICTOR] (#{count.value}):[/][green] Adjusting start time to {t_s} sec\n[/]'
             else:
-                start_time.value = 0
+                t_s = 0
                 if hits.value == 0:
-                    text += f"[purple][PREDICTOR] (#{count.value}):[/][red bold] Resetting start time to {start_time.value} sec\n[/]"
+                    text += f'[purple][PREDICTOR] (#{count.value}):[/][red bold] Resetting start time to {t_s} sec\n[/]'
                 
     # TODO 1: Make sanity check -- see if the same number of bytes was transferred
     # TODO 2: Train a model to validate the predictions?
-    text += f"[purple][PREDICTOR] (#{count.value}):[/] Ended"
-    console.print(text)
-    count.value += 1
+    text += f'[purple][PREDICTOR] (#{count.value}):[/] Ended'
 
+    return text, t_s
 
-def get_hits(prediction: dict, count: int, hits):
-    """Manges the hit variable. In case a dominant frequency is found, hits is increased. 
 
-    Args:
-        prediction (dict): predicition up till now
-        count (int): number of the predicition
-        hits (Value): how often a dominant frequency was found
+def save_data(queue, prediction, aggregated_bytes, count, hits) -> None:
+    """Put all data from `prediction` in a `queue`. The total bytes are as well saved here. 
 
-    Returns:
-        hits: increased value if a dominant frequncy was found, otherwise it is reset to 0
+    Args:
+        queue (Manager.queue): queue containing the data from the prediction 
+        prediction (dict): result from FTIO
+        aggregated_bytes (_type_): total bytes transferred over entire runtime 
+        count (_type_): prediction number
+        hits (_type_): home many times a dominant frequency was found
     """
-    console = Console()
-    text = ""
-    text += f"[purple][PREDICTOR] (#{count}):[/] Freq candidates: \n"
-    for i in range(0,len(prediction['dominant_freq'])):
-        text += (
-            f"[purple][PREDICTOR] (#{count}):[/]    {i}) "
-            f"{prediction['dominant_freq'][i]:.2f} Hz -- conf {prediction['conf'][i]:.2f}\n"
-        )
-    if  len(prediction["dominant_freq"]) == 1:
-        hits.value += 1
-        text += f"[purple][PREDICTOR] (#{count}):[/] Current hits {hits.value}\n"
-    else:
-        hits.value = 0
-        text += f"[purple][PREDICTOR] (#{count}):[/][red bold] Reseting hits {hits.value}[/]\n"
+    # safe total transferred bytes
+    aggregated_bytes.value += prediction['total_bytes']
+    
+    # save data
+    queue.put(
+        {
+            'phase': count.value,
+            'dominant_freq': prediction['dominant_freq'],
+            'conf': prediction['conf'],
+            'amp': prediction['amp'],
+            'phi': prediction['phi'],
+            't_start': prediction['t_start'],
+            't_end': prediction['t_end'],
+            'total_bytes': prediction['total_bytes'],
+            'ranks': prediction['ranks'],
+            'freq': prediction['freq'],
+            'hits': hits.value,
+        }
+    )
+
+
+def display_result(freq: float ,prediction: dict ,count, aggregated_bytes) -> str:
+    text = ''
+    if not np.isnan(freq):
+        text = f'[purple][PREDICTOR] (#{count.value}):[/] Dominant freq {freq:.3f} \n'
+
+    # time window
+    text += (
+        f'[purple][PREDICTOR] (#{count.value}):[/] Time window {prediction["t_end"]-prediction["t_start"]:.3f} sec ([{prediction["t_start"]:.3f},{prediction["t_end"]:.3f}] sec)\n')
+
+    # total bytes
+    total_bytes = aggregated_bytes.value
+    # total_bytes =  prediction["total_bytes"]
+    unit, order = set_unit(total_bytes,'B')
+    total_bytes = order*total_bytes
+    text += (
+        f'[purple][PREDICTOR] (#{count.value}):[/] Total bytes {total_bytes:.0f} {unit}\n')
 
-    console.print(text[:-1])
+    # Bytes since last time
+    # tmp = abs(prediction["total_bytes"] -aggregated_bytes.value)
+    tmp = abs(aggregated_bytes.value)
+    unit, order = set_unit(tmp,'B')
+    tmp = order *tmp
+    text += (
+        f'[purple][PREDICTOR] (#{count.value}):[/] Bytes transferred since last '
+        f'time {tmp:.0f} {unit}\n'
+        )
 
-    return hits
+    return text
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/async_process.py` & `ftio_hpc-0.0.4/ftio/prediction/async_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     # print(f'Process {process.name} (PID {os.getpid()}) started to execute {function}')
     process.start()
     # print(f'Process {process.name} (PID {os.getpid()}) ended')
     # print(f"Process {process} created")
     return process
 
 def join_procs(procs:list) -> list:
-    """joins procs by itterating over list and testing
+    """joins procs by iterating over list and testing
     that the process finished before joining
 
     Args:
         procs (list): list of procs to test
 
     Returns:
         list of new procs
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/group.py` & `ftio_hpc-0.0.4/ftio/prediction/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Groups predicitions according to frequency step
+"""Groups predictions according to frequency step
 """
 
 from __future__ import annotations
 import numpy as np
 from sklearn.cluster import DBSCAN
 from ftio.prediction.helper import get_dominant
 
 def group_step(data: list[dict]) -> tuple[list[dict], int]:
-    """generates dict contaiting predictions. Aditionally the entries are grouped according to the frequency resolution between the predicitions.
+    """generates dict contacting predictions. Additionally the entries are grouped according to the frequency resolution between the predictions.
 
     Args:
-        data (dict): predicitions
+        data (dict): predictions
 
     Returns:
         out (dict): data appended with a group field
         counter (int): Maximal number of groups
     """
     freq_new = 0
     freq_old = 0
@@ -40,18 +40,18 @@
             freq_old = freq_new
             old_window = time_window
 
     return out, counter
 
 
 def group_dbscan(data: list[dict]) -> tuple[list[dict], int]:
-    """generates dict contaiting predictions. Aditionally the entries are grouped according to dbscan with the frequency resolution as the eps distance.
+    """generates dict contacting predictions. Additionally the entries are grouped according to DBSCAN with the frequency resolution as the eps distance.
 
     Args:
-        data (dict): predicitions
+        data (dict): predictions
 
     Returns:
         out (dict): data appended with a group field
         counter (int): Maximal number of groups
     """
     freq = []
     window = []
@@ -69,15 +69,15 @@
             tol_max = max(abs(res), tol_max)
             # tol_min = min(abs(res), tol_min)
             freq.append(get_dominant(prediction))
             window.append(time_window)
             out.append(prediction)
             old_window = time_window
     
-    tol_min = 1/np.std(window) if np.std(window) != 0 else 1e-8
+    tol_min = 1/np.std(window) if window and np.std(window) != 0 else 1e-8
     tol = 2*tol_max if tol_max < 3*tol_min else np.abs(1-(tol_min/np.mean(window)))*tol_max#3 times std means 99 points
     tol = tol if tol > 0 and tol != np.inf else 1e-8 #dbscan expects tol > 0
     # print(f"tol_min is: {tol_min}\ntol_max is: {tol_max}\ntol is: {tol}")
 
     if out:
         if len(out) == 1:
             counter = 0
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/pools.py` & `ftio_hpc-0.0.4/ftio/prediction/pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Performs prediction with Pools (ProcessPoolExecutor) and a callback mechanism"""
 from __future__ import annotations
 from concurrent.futures import ProcessPoolExecutor
 import ftio.prediction.monitor as pm
-from ftio.prediction.probability import probability
+from ftio.prediction.probability_analysis import find_probability
 from ftio.prediction.helper import  print_data
 from ftio.prediction.analysis import ftio_process
 # from ftio.prediction.async_process import handle_in_process
 
 
 def predictor_with_pools(filename, data, queue, count, hits, start_time, aggregated_bytes, args):
     """performs prediction in ProcessPoolExecuter. FTIO is a submitted future and probability is calculated as a callback
 
     Args:
-        filenme (str): name of file
+        filename (str): name of file
         data (Manager().list): List of dicts with all predictions so far
         queue (Manager().Queue): queue for FTIO data
         count (Manager().Value): number of prediction
-        hits (Manager().Value): hits indicating how often a dominant frequncy was found
+        hits (Manager().Value): hits indicating how often a dominant frequency was found
         start_time (Manager().Value): start time window for ftio
         aggregated_bytes (Manager().Value): total bytes transferred so far
         args (list[str]): additional arguments passed to ftio
     """
-    # Init: Monitore a file
+    # Init: Monitor a file
     stamp, _ = pm.monitor(filename,"")
 
     # Loop and predict if changes occur
     try:
         while True:
             with ProcessPoolExecutor(max_workers=1) as executor:
-                # monitore
+                # monitor
                 stamp, _ = pm.monitor(filename, stamp)
                 future = executor.submit(ftio_future, data, queue, count, hits, start_time, aggregated_bytes, args)
                 future.add_done_callback(probability_callback)
     except KeyboardInterrupt:
         print_data(data)
         print("-- done -- ")
 
@@ -40,15 +40,15 @@
 def ftio_future(data, queue , count, hits, start_time, aggregated_bytes, args: list[str]) -> list[dict]:
     """Performs prediction made up of two part: (1) Executes FTIO and (2) appends to data the value
 
     Args:
         data (Manager().list): List of dicts with all predictions so far
         queue (Manager().Queue): queue for FTIO data
         count (Manager().Value): number of prediction
-        hits (Manager().Value): hits indicating how often a dominant frequncy was found
+        hits (Manager().Value): hits indicating how often a dominant frequency was found
         start_time (Manager().Value): start time window for ftio
         aggregated_bytes (Manager().Value): total bytes transferred so far
         args (list[str]): additional arguments passed to ftio
     """
     ftio_process(queue, count, hits, start_time, aggregated_bytes, args)
     while not queue.empty():
         data.append(queue.get())
@@ -57,8 +57,11 @@
 
 def probability_callback(future):
     """executes the probability calculation in a callback
 
     Args:
         future (Future): _description_
     """
-    probability(future.result()) #the queue
+    _ = find_probability(future.result()) #the queue
+
+
+
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/probability.py` & `ftio_hpc-0.0.4/ftio/prediction/probability_analysis.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-"""Module concerned with probability calculation
-"""
-from __future__ import annotations
 import numpy as np
-import ftio.prediction.group as gp
 from rich.console import Console
+import ftio.prediction.group as gp
 from ftio.prediction.helper import get_dominant
+from ftio.prediction.probability import Probability
 
-CONSOLE = Console()
 
-def probability(data: list[dict], method:str = "db") -> None:
+def find_probability(data: list[dict], method:str = "db") -> list:
     """Calculates the conditional probability that expresses
     how probable the frequency (event A) is given that the signal
-    is perodic occurred (prabability B).
+    is periodic occurred (probability B).
     According to Bayes' Theorem, P(A|B) = P(B|A)*P(A)/P(B)
-    P(B|A): Probability that the signal is perodic given that it has a frequency A --> 1
+    P(B|A): Probability that the signal is periodic given that it has a frequency A --> 1
     P(A): Probability that the signal has the frequency A
     P(B): Probability that the signal has is periodic
 
     Args:
-        data (dict): contating predicitions
+        data (dict): contacting predictions
 
     Returns:
         None
     """
     p_b = 0
     p_a = []
     p_a_given_b = 0
     p_b_given_a = 1
-    out = []
+    grouped_prediction = []
     counter = 0
+    out = []
 
     if data:
         if "step" in method:
-            out, counter = gp.group_step(data)
+            grouped_prediction, counter = gp.group_step(data)
         elif "db" in method:
-            out, counter = gp.group_dbscan(data)
+            grouped_prediction, counter = gp.group_dbscan(data)
 
         for prediction in data:
             if len(prediction["dominant_freq"]) >= 1:
                 p_b += 1
 
         p_b = p_b / len(data) 
+        CONSOLE = Console()
         CONSOLE.print(f"[purple][PREDICTOR]:[/] P(periodic) = {p_b*100:.3f}%")
 
-        if len(out) > 0:
+        if len(grouped_prediction) > 0:
             for group in range(0, counter + 1):
                 p_a = 0
                 f_min = np.inf
                 f_max = 0
-                for pred in out:
+                for pred in grouped_prediction:
                     # print(pred)
                     # print(f"index is {group}, group is {pred['group']}")
                     if group == pred["group"]:
                         f_min = min(get_dominant(pred), f_min)
                         f_max = max(get_dominant(pred), f_max)
                         # print(f"group: {group}, pred_group: {pred['group']}, freq: {get_dominant(pred):.3f}, f_min: {f_min:.3f}, f_max:{f_max:.3f}")
                         p_a += 1
+
                 p_a = p_a / len(data) if len(data) > 0 else 0
                 p_a_given_b = p_b_given_a * p_a / p_b if p_b > 0 else 0
-                CONSOLE.print(
-                    f"[purple][PREDICTOR]:[/] P([{f_min:.3f},{f_max:.3f}] Hz) = {p_a*100:.2f}%\n"
-                    f"[purple][PREDICTOR]:[/] |-> [{f_min:.3f},{f_max:.3f}] Hz = [{1/f_max if f_max != 0 else np.NaN:.3f},{1/f_min if f_min != 0 else np.NaN:.3f}] sec\n"
-                    f"[purple][PREDICTOR]:[/] '-> P([{f_min:.3f},{f_max:.3f}] Hz | perodic) = {p_a_given_b*100:.2f}%"
-                )
+
+                prob = Probability(f_min, f_max)
+                prob.set(p_b, p_a, p_a_given_b, p_b_given_a)
+                prob.display()
+                out.append(prob)
+
+    return out
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/processes.py` & `ftio_hpc-0.0.4/ftio/prediction/processes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Performs prediction with Pools (ProcessPoolExecutor) and a callback mechanism"""
 from __future__ import annotations
 import ftio.prediction.monitor as pm
-from ftio.prediction.probability import probability
+from ftio.prediction.probability_analysis import find_probability
 from ftio.prediction.helper import print_data, export_extrap
 from ftio.prediction.analysis import ftio_process
 from ftio.prediction.async_process import handle_in_process
 
 # from ftio.prediction.async_process import handle_in_process
 
 
 def predictor_with_processes(
     filename, data, queue, count, hits, start_time, aggregated_bytes, args
 ):
     """performs prediction in ProcessPoolExecuter. FTIO is a submitted future and probability is calculated as a callback
 
     Args:   
-        filenme (str): name of file
+        filename (str): name of file
         data (Manager().list): List of dicts with all predictions so far
         queue (Manager().Queue): queue for FTIO data
         count (Manager().Value): number of prediction
-        hits (Manager().Value): hits indicating how often a dominant frequncy was found
+        hits (Manager().Value): hits indicating how often a dominant frequency was found
         start_time (Manager().Value): start time window for ftio
         aggregated_bytes (Manager().Value): total bytes transferred so far
         args (list[str]): additional arguments passed to ftio
     """
     procs = []
-    # Init: Monitore a file
+    # Init: Monitor a file
     stamp,_ = pm.monitor(filename, "")
 
     # Loop and predict if changes occur
     try:
         while True:
-            # monitore
+            # monitor
             stamp, procs = pm.monitor(filename, stamp, procs)
             # launch prediction_process
             procs.append(
                 handle_in_process(
                     prediction_process,
                     args=(data, queue, count, hits, start_time, aggregated_bytes, args)
                 )
@@ -43,25 +43,24 @@
     except KeyboardInterrupt:
         print_data(data)
         export_extrap(data)
         print("-- done -- ")
 
 
 def prediction_process(
-    data, queue, count, hits, start_time, aggregated_bytes, args: list[str]
-) -> None:
+    data, queue, count, hits, start_time, aggregated_bytes, args: list[str], msgs=None) -> None:
     """Performs prediction made up of two part: (1) Executes FTIO and (2) appends to data the value
 
     Args:
         data (Manager().list): List of dicts with all predictions so far
         queue (Manager().Queue): queue for FTIO data
         count (Manager().Value): number of prediction
-        hits (Manager().Value): hits indicating how often a dominant frequncy was found
+        hits (Manager().Value): hits indicating how often a dominant frequency was found
         start_time (Manager().Value): start time window for ftio
         aggregated_bytes (Manager().Value): total bytes transferred so far
         args (list[str]): additional arguments passed to ftio.py
     """
-    ftio_process(queue, count, hits, start_time, aggregated_bytes, args)
+    ftio_process(queue, count, hits, start_time, aggregated_bytes, args, msgs)
     while not queue.empty():
         data.append(queue.get())
 
-    probability(data)
+    _ = find_probability(data)
```

### Comparing `ftio-hpc-0.0.3/ftio/prediction/unify_predictions.py` & `ftio_hpc-0.0.4/ftio/prediction/unify_predictions.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 CONSOLE = MyConsole()
 
 def merge_predictions(args, pred_dft:dict, pred_auto:dict)-> dict:
     """Merge prediction if both autocorrelation and freq. technique (dft/wavelet) are executed
 
     Args:
         args (_type_): _description_
-        pred_dft (dict): prediction frequency technqiue
+        pred_dft (dict): prediction frequency technique
         pred_auto (dict): prediction autocorrelation
 
     Returns:
         dict: merge prediction
     """
     CONSOLE.set(args.verbose)
     pred_merged = pred_dft.copy()
```

### Comparing `ftio-hpc-0.0.3/ftio_hpc.egg-info/PKG-INFO` & `ftio_hpc-0.0.4/ftio_hpc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftio-hpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Frequency Techniques for I/O
 Author-email: Ahmad Tarraf <ahmad.tarraf@tu-darmstadt.de>
 Maintainer-email: Ahmad Tarraf <ahmad.tarraf@tu-darmstadt.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Parallel Programming @ TU Darmstadt
         
@@ -54,14 +54,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
+Requires-Dist: zmq
 Requires-Dist: numba
 Requires-Dist: darshan
 Requires-Dist: fastdtw
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: jsonlines
 Requires-Dist: plotly
@@ -69,14 +70,15 @@
 Requires-Dist: kneed
 Requires-Dist: PyWavelets
 Requires-Dist: trace_updater
 Requires-Dist: plotly_resampler
 Requires-Dist: msgpack
 Requires-Dist: rich
 Requires-Dist: dash_extensions
+Requires-Dist: pytest
 
 <!-- # FTIO -->
 ![GitHub Release](https://img.shields.io/github/v/release/tuda-parallel/FTIO)
 ![GitHub Release Date](https://img.shields.io/github/release-date/tuda-parallel/FTIO)
 ![](https://img.shields.io/github/last-commit/tuda-parallel/FTIO)
 ![contributors](https://img.shields.io/github/contributors/tuda-parallel/FTIO)
 ![issues](https://img.shields.io/github/issues/tuda-parallel/FTIO)
@@ -233,15 +235,15 @@
 
 Several flags can be specified. The most relevant settings are:
 
 | Flag                        | Description|
 |---                          | --- |
 |file                         | file, file list (file 0 ... file n), folder, or folder list (folder 0.. folder n) containing traces  (positional argument)|
 |-h, --help                   | show this help message and exit|
-|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: async_write, async_read, sync_write, sync_read|
+|-m MODE, --mode MODE         | if the trace file contains several I/O modes, a specific mode can be selected. Supported modes are: write_async, read_async, write_sync, read_sync|
 |-r RENDER, --render RENDER   | specifies how the plots are rendered. Either dynamic (default) or static|
 |-f FREQ, --freq FREQ         | specifies the sampling rate with which the continuous signal is discretized (default=10Hz). This directly affects the highest captured frequency (Nyquist). The value is specified in Hz. In case this value is set to -1, the auto mode is launched which sets the sampling frequency automatically to the smallest change in the bandwidth detected. Note that the lowest allowed frequency in the auto mode is 2000 Hz|
 |-ts TS, --ts TS              | Modifies the start time of the examined time window
 |-te TE, --te TE              | Modifies the end time of the examined time window
 |-tr TRANSFORMATION, --transformation TRANSFORMATION| specifies the frequency technique to use. Supported modes are: dft (default), wave_disc, and wave_cont|
 |-e ENGINE, --engine ENGINE   | specifies the engine used to display the figures. Either plotly (default) or mathplotlib can be used. Plotly is used to generate interactive plots as HTML files. Set this value to no if you do not want to generate plots
 |-o OUTLIER, --outlier OUTLIER| outlier detection method: Z-score (default), DB-Scan, Isolation_forest, or LOF|
@@ -294,15 +296,15 @@
 
 <p align="right"><a href="#ftio">⬆</a></p>
 
 ## License
 
 ![license][license.bedge]
 
-Distributed under the BSD 3-Clause License. See [LISCENCE](./LICENSE) for more information.
+Distributed under the BSD 3-Clause License. See [LICENCE](./LICENSE) for more information.
 <p align="right"><a href="#ftio">⬆</a></p>
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
 
 Authors:
```

### Comparing `ftio-hpc-0.0.3/ftio_hpc.egg-info/SOURCES.txt` & `ftio_hpc-0.0.4/ftio_hpc.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
-examples/txt/custom_input.py
+examples/API/test_api.py
+examples/custom/txt/custom_input.py
 ftio/__init__.py
 ftio/__main__.py
+ftio/api/gekkoFs/ftio_gekko.py
+ftio/api/gekkoFs/parse_gekko.py
+ftio/api/gekkoFs/predictor_gekko.py
+ftio/api/gekkoFs/predictor_gekko_zmq.py
+ftio/api/metric_proxy/parse_proxy.py
+ftio/api/metric_proxy/proxy.py
 ftio/cli/__init__.py
 ftio/cli/ftio_core.py
 ftio/cli/predictor.py
 ftio/freq/__init__.py
 ftio/freq/_dft.py
 ftio/freq/_wavelet.py
 ftio/freq/anomaly_detection.py
@@ -15,39 +22,44 @@
 ftio/freq/autocorrelation.py
 ftio/freq/discretize.py
 ftio/freq/freq_data.py
 ftio/freq/freq_html.py
 ftio/freq/freq_plot_core.py
 ftio/freq/helper.py
 ftio/freq/perodicity_detection.py
+ftio/freq/time_window.py
 ftio/parse/__init__.py
 ftio/parse/args.py
 ftio/parse/bandwidth.py
 ftio/parse/custom_patterns.py
 ftio/parse/darshan_reader.py
 ftio/parse/extract.py
 ftio/parse/ftio_to_extrap.py
 ftio/parse/helper.py
 ftio/parse/input_template.py
 ftio/parse/metrics.py
 ftio/parse/msgpack_reader.py
 ftio/parse/overlap_thread.py
 ftio/parse/parse_custom.py
 ftio/parse/parse_darshan.py
+ftio/parse/parse_json.py
+ftio/parse/parse_jsonl.py
 ftio/parse/parse_msgpack.py
 ftio/parse/parse_recorder.py
 ftio/parse/parse_txt.py
+ftio/parse/parse_zmq.py
 ftio/parse/percent.py
 ftio/parse/print.py
 ftio/parse/recorder_reader.py
 ftio/parse/sample.py
 ftio/parse/scales.py
 ftio/parse/simrun.py
 ftio/parse/time_io.py
 ftio/parse/txt_reader.py
+ftio/parse/zmq_reader.py
 ftio/plot/__init__.py
 ftio/plot/helper.py
 ftio/plot/plot_core.py
 ftio/plot/plot_error.py
 ftio/plot/print_html.py
 ftio/plot/stack_plot.py
 ftio/plot/units.py
@@ -55,29 +67,33 @@
 ftio/plot/dash_files/data_source.py
 ftio/plot/dash_files/callback_files/callbacks.py
 ftio/plot/dash_files/callback_files/io_mode_callbacks.py
 ftio/plot/dash_files/constants/graph_mode.py
 ftio/plot/dash_files/constants/id.py
 ftio/plot/dash_files/constants/io_mode.py
 ftio/plot/dash_files/constants/legend_group.py
+ftio/post/processing.py
 ftio/prediction/__init__.py
 ftio/prediction/analysis.py
 ftio/prediction/async_process.py
 ftio/prediction/group.py
 ftio/prediction/helper.py
 ftio/prediction/monitor.py
 ftio/prediction/pools.py
 ftio/prediction/probability.py
+ftio/prediction/probability_analysis.py
 ftio/prediction/processes.py
+ftio/prediction/processes_zmq.py
 ftio/prediction/unify_predictions.py
 ftio/util/__init__.py
 ftio/util/ioparse.py
 ftio/util/ioplot.py
 ftio_hpc.egg-info/PKG-INFO
 ftio_hpc.egg-info/SOURCES.txt
 ftio_hpc.egg-info/dependency_links.txt
 ftio_hpc.egg-info/entry_points.txt
 ftio_hpc.egg-info/requires.txt
 ftio_hpc.egg-info/top_level.txt
+test/test_api.py
 test/test_ftio.py
 test/test_ioparse.py
 test/test_ioplot.py
```

### Comparing `ftio-hpc-0.0.3/pyproject.toml` & `ftio_hpc-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 [project]
 name = "ftio-hpc"
 dynamic = ["version"]
 dependencies = [
 	"scikit-learn",
+	"zmq",
 	"numba",
 	"darshan",
 	"fastdtw",
 	"scipy",
 	"pandas",
 	"jsonlines",
 	"plotly",
@@ -25,14 +26,15 @@
 	"kneed",
 	"PyWavelets",
 	"trace_updater",
 	"plotly_resampler",
 	"msgpack",
 	"rich",
 	"dash_extensions",
+	"pytest",
 ]
 requires-python = ">=3.8"
 authors = [
   {name = "Ahmad Tarraf", email = "ahmad.tarraf@tu-darmstadt.de"},
 ]
 maintainers = [
   {name = "Ahmad Tarraf", email = "ahmad.tarraf@tu-darmstadt.de"}
```

