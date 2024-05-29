# Comparing `tmp/eemeter-4.0.1.tar.gz` & `tmp/eemeter-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eemeter-4.0.1.tar", last modified: Mon Mar  4 19:25:15 2024, max compression
+gzip compressed data, was "eemeter-4.0.2.tar", last modified: Wed May 29 20:13:38 2024, max compression
```

## Comparing `eemeter-4.0.1.tar` & `eemeter-4.0.2.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.186370 eemeter-4.0.1/
--rw-rw-r--   0 root         (0) root         (0)    11359 2024-02-26 22:39:59.000000 eemeter-4.0.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      139 2024-02-26 22:39:59.000000 eemeter-4.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6603 2024-03-04 19:25:15.186370 eemeter-4.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5753 2024-02-26 22:39:59.000000 eemeter-4.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.146366 eemeter-4.0.1/eemeter/
--rw-rw-r--   0 root         (0) root         (0)     1065 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      950 2024-03-04 19:14:36.000000 eemeter-4.0.1/eemeter/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.146366 eemeter-4.0.1/eemeter/common/
--rw-rw-r--   0 root         (0) root         (0)      800 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1397 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/abstract_data_processor.py
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/abstract_data_settings.py
--rwxrwxr-x   0 root         (0) root         (0)    19117 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/adaptive_loss.py
--rw-rw-r--   0 root         (0) root         (0)    13893 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/adaptive_loss_tck.py
--rw-rw-r--   0 root         (0) root         (0)     2266 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/const.py
--rw-rw-r--   0 root         (0) root         (0)     1269 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/data_settings.py
--rw-rw-r--   0 root         (0) root         (0)     6388 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/test_data.py
--rw-rw-r--   0 root         (0) root         (0)     8498 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.146366 eemeter-4.0.1/eemeter/drmeter/
--rw-rw-r--   0 root         (0) root         (0)      728 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/drmeter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      790 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/drmeter/data.py
--rw-rw-r--   0 root         (0) root         (0)      840 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/drmeter/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.146366 eemeter-4.0.1/eemeter/eemeter/
--rw-rw-r--   0 root         (0) root         (0)      734 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.150367 eemeter-4.0.1/eemeter/eemeter/common/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    25309 2024-03-04 19:14:36.000000 eemeter-4.0.1/eemeter/eemeter/common/data_processor_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     1652 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/common/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)    32937 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/common/features.py
--rw-rw-r--   0 root         (0) root         (0)    37600 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/common/transform.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/common/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.150367 eemeter-4.0.1/eemeter/eemeter/models/
--rw-rw-r--   0 root         (0) root         (0)      723 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.150367 eemeter-4.0.1/eemeter/eemeter/models/billing/
--rw-rw-r--   0 root         (0) root         (0)      839 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/billing/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20985 2024-03-04 19:14:36.000000 eemeter-4.0.1/eemeter/eemeter/models/billing/data.py
--rw-rw-r--   0 root         (0) root         (0)     5778 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/billing/model.py
--rw-rw-r--   0 root         (0) root         (0)     5128 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/billing/plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.154367 eemeter-4.0.1/eemeter/eemeter/models/daily/
--rw-rw-r--   0 root         (0) root         (0)      827 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.154367 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    15510 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/c_hdd_tidd.py
--rw-rw-r--   0 root         (0) root         (0)     9173 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/full_model.py
--rwxrwxr-x   0 root         (0) root         (0)    11041 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/hdd_tidd_cdd.py
--rwxrwxr-x   0 root         (0) root         (0)     3082 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/tidd.py
--rw-rw-r--   0 root         (0) root         (0)    30973 2024-03-04 19:14:36.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/data.py
--rw-rw-r--   0 root         (0) root         (0)     6290 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/fit_base_models.py
--rw-rw-r--   0 root         (0) root         (0)    34810 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/model.py
--rw-rw-r--   0 root         (0) root         (0)    12919 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/objective_function.py
--rwxrwxr-x   0 root         (0) root         (0)    13059 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/optimize.py
--rwxrwxr-x   0 root         (0) root         (0)    15355 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/optimize_results.py
--rw-rw-r--   0 root         (0) root         (0)    13264 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/parameters.py
--rw-rw-r--   0 root         (0) root         (0)     6213 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/plot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.158367 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     3975 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/base_model.py
--rwxrwxr-x   0 root         (0) root         (0)    27046 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/config.py
--rw-rw-r--   0 root         (0) root         (0)     9152 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/ellipsoid_test.py
--rw-rw-r--   0 root         (0) root         (0)     5324 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/selection_criteria.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.162368 eemeter-4.0.1/eemeter/eemeter/models/hourly/
--rw-rw-r--   0 root         (0) root         (0)      835 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4566 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/data.py
--rw-rw-r--   0 root         (0) root         (0)    16061 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/derivatives.py
--rw-rw-r--   0 root         (0) root         (0)     7093 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/design_matrices.py
--rw-rw-r--   0 root         (0) root         (0)    20992 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/metrics.py
--rw-rw-r--   0 root         (0) root         (0)    22087 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/model.py
--rw-rw-r--   0 root         (0) root         (0)    18585 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/segmentation.py
--rw-rw-r--   0 root         (0) root         (0)    15087 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/usage_per_day.py
--rw-rw-r--   0 root         (0) root         (0)     8066 2024-03-04 19:14:36.000000 eemeter-4.0.1/eemeter/eemeter/models/hourly/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.170368 eemeter-4.0.1/eemeter/eemeter/samples/
--rw-rw-r--   0 root         (0) root         (0)      676 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      240 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-billing_bimonthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      333 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-billing_monthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)     4607 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-daily.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    84853 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-hourly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    97482 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-tempF.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      238 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-billing_bimonthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      338 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-billing_monthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)     4395 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-daily.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    81524 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-hourly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      223 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-billing_bimonthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      313 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-billing_monthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)     3855 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-daily.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    68596 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-hourly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      224 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-billing_bimonthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)      309 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-billing_monthly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)     3677 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-daily.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    70076 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-hourly.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    97462 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/il-tempF.csv.gz
--rw-rw-r--   0 root         (0) root         (0)     3422 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/load.py
--rw-rw-r--   0 root         (0) root         (0)    14407 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/metadata.json
--rw-rw-r--   0 root         (0) root         (0)   109572 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-0.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    78635 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-1.csv.gz
--rw-rw-r--   0 root         (0) root         (0)   128905 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-2.csv.gz
--rw-rw-r--   0 root         (0) root         (0)   107840 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-gas-hdd-only-hourly-sample-0.csv.gz
--rw-rw-r--   0 root         (0) root         (0)   219885 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-tempC-sample-0.csv.gz
--rw-rw-r--   0 root         (0) root         (0)    91509 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/samples/uk-tempC-sample-1_2.csv.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.174368 eemeter-4.0.1/eemeter/eemeter/utilities/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3999 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/utilities/cli.py
--rw-rw-r--   0 root         (0) root         (0)     9153 2024-02-26 22:39:59.000000 eemeter-4.0.1/eemeter/eemeter/utilities/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.182369 eemeter-4.0.1/eemeter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6603 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5257 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-04 19:25:15.000000 eemeter-4.0.1/eemeter.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      424 2024-02-26 22:39:59.000000 eemeter-4.0.1/pytest.ini
--rw-rw-r--   0 root         (0) root         (0)       63 2024-03-04 19:25:15.186370 eemeter-4.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3300 2024-02-26 22:39:59.000000 eemeter-4.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.178369 eemeter-4.0.1/tests/
--rw-rw-r--   0 root         (0) root         (0)     2181 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.182369 eemeter-4.0.1/tests/daily_model/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.182369 eemeter-4.0.1/tests/daily_model/base_models/
--rw-rw-r--   0 root         (0) root         (0)     3312 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/base_models/test_c_hdd_tidd_smooth.py
--rw-rw-r--   0 root         (0) root         (0)     1159 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/base_models/test_full_model_finder.py
--rw-rw-r--   0 root         (0) root         (0)    21690 2024-03-04 19:14:36.000000 eemeter-4.0.1/tests/daily_model/test_billing_data.py
--rw-rw-r--   0 root         (0) root         (0)    28243 2024-03-04 19:14:36.000000 eemeter-4.0.1/tests/daily_model/test_daily_data.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_daily_model.py
--rw-rw-r--   0 root         (0) root         (0)     6625 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_fit_base_models.py
--rw-rw-r--   0 root         (0) root         (0)     3501 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_fit_model.py
--rw-rw-r--   0 root         (0) root         (0)     5283 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_objective_function.py
--rw-rw-r--   0 root         (0) root         (0)     4389 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_optimize.py
--rw-rw-r--   0 root         (0) root         (0)     7747 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/test_optimize_results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.182369 eemeter-4.0.1/tests/daily_model/utilities/
--rw-rw-r--   0 root         (0) root         (0)     3821 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_adaptive_loss.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_base_model.py
--rw-rw-r--   0 root         (0) root         (0)     3554 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_config.py
--rw-rw-r--   0 root         (0) root         (0)     4033 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_ellipsoid_test.py
--rw-rw-r--   0 root         (0) root         (0)     6226 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_selection_criteria.py
--rw-rw-r--   0 root         (0) root         (0)     7649 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/daily_model/utilities/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 19:25:15.182369 eemeter-4.0.1/tests/snapshots/
--rw-rw-r--   0 root         (0) root         (0)      656 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/snapshots/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2522 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/snapshots/snap_test_features.py
--rw-rw-r--   0 root         (0) root         (0)     6440 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_caltrack_design_matrices.py
--rw-rw-r--   0 root         (0) root         (0)    15481 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_caltrack_hourly.py
--rw-rw-r--   0 root         (0) root         (0)     3086 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_cli.py
--rw-rw-r--   0 root         (0) root         (0)    20510 2024-03-04 19:14:36.000000 eemeter-4.0.1/tests/test_derivatives.py
--rw-rw-r--   0 root         (0) root         (0)     1707 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_exceptions.py
--rw-rw-r--   0 root         (0) root         (0)    40392 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_features.py
--rw-rw-r--   0 root         (0) root         (0)    10578 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_io.py
--rw-rw-r--   0 root         (0) root         (0)     5412 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_json_serialization.py
--rw-rw-r--   0 root         (0) root         (0)     3862 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_samples.py
--rw-rw-r--   0 root         (0) root         (0)     8968 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_segmentation.py
--rw-rw-r--   0 root         (0) root         (0)    39019 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_transform.py
--rw-rw-r--   0 root         (0) root         (0)      741 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_version.py
--rw-rw-r--   0 root         (0) root         (0)     1229 2024-02-26 22:39:59.000000 eemeter-4.0.1/tests/test_warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.258829 eemeter-4.0.2/
+-rw-rw-r--   0 root         (0) root         (0)    11359 2024-05-29 19:43:52.000000 eemeter-4.0.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      139 2024-05-29 19:43:52.000000 eemeter-4.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6603 2024-05-29 20:13:38.258829 eemeter-4.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5753 2024-05-29 19:43:52.000000 eemeter-4.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.218826 eemeter-4.0.2/eemeter/
+-rw-rw-r--   0 root         (0) root         (0)     1065 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      950 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.222826 eemeter-4.0.2/eemeter/common/
+-rw-rw-r--   0 root         (0) root         (0)      800 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1397 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/abstract_data_processor.py
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/abstract_data_settings.py
+-rwxrwxr-x   0 root         (0) root         (0)    19117 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/adaptive_loss.py
+-rw-rw-r--   0 root         (0) root         (0)    13893 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/adaptive_loss_tck.py
+-rw-rw-r--   0 root         (0) root         (0)     2266 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/const.py
+-rw-rw-r--   0 root         (0) root         (0)     1269 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/data_settings.py
+-rw-rw-r--   0 root         (0) root         (0)     6309 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/test_data.py
+-rw-rw-r--   0 root         (0) root         (0)     8498 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.226826 eemeter-4.0.2/eemeter/drmeter/
+-rw-rw-r--   0 root         (0) root         (0)      728 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/drmeter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      790 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/drmeter/data.py
+-rw-rw-r--   0 root         (0) root         (0)      840 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/drmeter/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.226826 eemeter-4.0.2/eemeter/eemeter/
+-rw-rw-r--   0 root         (0) root         (0)      734 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.226826 eemeter-4.0.2/eemeter/eemeter/common/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15421 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/data_processor_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)     1652 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)    32937 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/features.py
+-rw-rw-r--   0 root         (0) root         (0)    25222 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/sufficiency_criteria.py
+-rw-rw-r--   0 root         (0) root         (0)    37600 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/transform.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/common/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.226826 eemeter-4.0.2/eemeter/eemeter/models/
+-rw-rw-r--   0 root         (0) root         (0)      723 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.230826 eemeter-4.0.2/eemeter/eemeter/models/billing/
+-rw-rw-r--   0 root         (0) root         (0)      839 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/billing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21568 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/billing/data.py
+-rw-rw-r--   0 root         (0) root         (0)     5778 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/billing/model.py
+-rw-rw-r--   0 root         (0) root         (0)     5128 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/billing/plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.230826 eemeter-4.0.2/eemeter/eemeter/models/daily/
+-rw-rw-r--   0 root         (0) root         (0)      827 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.234827 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    15510 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/c_hdd_tidd.py
+-rw-rw-r--   0 root         (0) root         (0)     9173 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/full_model.py
+-rwxrwxr-x   0 root         (0) root         (0)    11041 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/hdd_tidd_cdd.py
+-rwxrwxr-x   0 root         (0) root         (0)     3082 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/tidd.py
+-rw-rw-r--   0 root         (0) root         (0)    31386 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/data.py
+-rw-rw-r--   0 root         (0) root         (0)     6290 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/fit_base_models.py
+-rw-rw-r--   0 root         (0) root         (0)    34810 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/model.py
+-rw-rw-r--   0 root         (0) root         (0)    12919 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/objective_function.py
+-rwxrwxr-x   0 root         (0) root         (0)    13059 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/optimize.py
+-rwxrwxr-x   0 root         (0) root         (0)    15355 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/optimize_results.py
+-rw-rw-r--   0 root         (0) root         (0)    13264 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/parameters.py
+-rw-rw-r--   0 root         (0) root         (0)     6213 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/plot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.234827 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     3975 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/base_model.py
+-rwxrwxr-x   0 root         (0) root         (0)    27046 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/config.py
+-rw-rw-r--   0 root         (0) root         (0)     9152 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/ellipsoid_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5324 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/selection_criteria.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.238827 eemeter-4.0.2/eemeter/eemeter/models/hourly/
+-rw-rw-r--   0 root         (0) root         (0)      835 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4566 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/data.py
+-rw-rw-r--   0 root         (0) root         (0)    16061 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/derivatives.py
+-rw-rw-r--   0 root         (0) root         (0)     7093 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/design_matrices.py
+-rw-rw-r--   0 root         (0) root         (0)    20992 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/metrics.py
+-rw-rw-r--   0 root         (0) root         (0)    22087 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/model.py
+-rw-rw-r--   0 root         (0) root         (0)    18585 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/segmentation.py
+-rw-rw-r--   0 root         (0) root         (0)    15087 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/usage_per_day.py
+-rw-rw-r--   0 root         (0) root         (0)     7981 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/models/hourly/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.246828 eemeter-4.0.2/eemeter/eemeter/samples/
+-rw-rw-r--   0 root         (0) root         (0)      676 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      240 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-billing_bimonthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      333 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-billing_monthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)     4607 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-daily.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    84853 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-hourly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    97482 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-tempF.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      238 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-billing_bimonthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      338 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-billing_monthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)     4395 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-daily.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    81524 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-hourly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      223 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-billing_bimonthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      313 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-billing_monthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)     3855 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-daily.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    68596 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-hourly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      224 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-billing_bimonthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)      309 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-billing_monthly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)     3677 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-daily.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    70076 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-hourly.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    97462 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/il-tempF.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/load.py
+-rw-rw-r--   0 root         (0) root         (0)    14407 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/metadata.json
+-rw-rw-r--   0 root         (0) root         (0)   109572 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-0.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    78635 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-1.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)   128905 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-2.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)   107840 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-gas-hdd-only-hourly-sample-0.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)   219885 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-tempC-sample-0.csv.gz
+-rw-rw-r--   0 root         (0) root         (0)    91509 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/samples/uk-tempC-sample-1_2.csv.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.250828 eemeter-4.0.2/eemeter/eemeter/utilities/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3999 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/utilities/cli.py
+-rw-rw-r--   0 root         (0) root         (0)     9153 2024-05-29 19:43:53.000000 eemeter-4.0.2/eemeter/eemeter/utilities/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.258829 eemeter-4.0.2/eemeter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6603 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5304 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-29 20:13:38.000000 eemeter-4.0.2/eemeter.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      424 2024-05-29 19:43:53.000000 eemeter-4.0.2/pytest.ini
+-rw-rw-r--   0 root         (0) root         (0)       63 2024-05-29 20:13:38.258829 eemeter-4.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3300 2024-05-29 19:43:53.000000 eemeter-4.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.254828 eemeter-4.0.2/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2181 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.254828 eemeter-4.0.2/tests/daily_model/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.254828 eemeter-4.0.2/tests/daily_model/base_models/
+-rw-rw-r--   0 root         (0) root         (0)     3312 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/base_models/test_c_hdd_tidd_smooth.py
+-rw-rw-r--   0 root         (0) root         (0)     1159 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/base_models/test_full_model_finder.py
+-rw-rw-r--   0 root         (0) root         (0)    21690 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_billing_data.py
+-rw-rw-r--   0 root         (0) root         (0)    29434 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_daily_data.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_daily_model.py
+-rw-rw-r--   0 root         (0) root         (0)     6625 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_fit_base_models.py
+-rw-rw-r--   0 root         (0) root         (0)     3501 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_fit_model.py
+-rw-rw-r--   0 root         (0) root         (0)     5283 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_objective_function.py
+-rw-rw-r--   0 root         (0) root         (0)     4389 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_optimize.py
+-rw-rw-r--   0 root         (0) root         (0)     7747 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/test_optimize_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.258829 eemeter-4.0.2/tests/daily_model/utilities/
+-rw-rw-r--   0 root         (0) root         (0)     3821 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_adaptive_loss.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_base_model.py
+-rw-rw-r--   0 root         (0) root         (0)     3554 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4033 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_ellipsoid_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6226 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_selection_criteria.py
+-rw-rw-r--   0 root         (0) root         (0)     7649 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/daily_model/utilities/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 20:13:38.258829 eemeter-4.0.2/tests/snapshots/
+-rw-rw-r--   0 root         (0) root         (0)      656 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/snapshots/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2522 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/snapshots/snap_test_features.py
+-rw-rw-r--   0 root         (0) root         (0)     6440 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_caltrack_design_matrices.py
+-rw-rw-r--   0 root         (0) root         (0)    15481 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_caltrack_hourly.py
+-rw-rw-r--   0 root         (0) root         (0)     3086 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_cli.py
+-rw-rw-r--   0 root         (0) root         (0)    20510 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_derivatives.py
+-rw-rw-r--   0 root         (0) root         (0)     1707 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)    40392 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_features.py
+-rw-rw-r--   0 root         (0) root         (0)    10578 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_io.py
+-rw-rw-r--   0 root         (0) root         (0)     5412 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_json_serialization.py
+-rw-rw-r--   0 root         (0) root         (0)     3862 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_samples.py
+-rw-rw-r--   0 root         (0) root         (0)     8968 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_segmentation.py
+-rw-rw-r--   0 root         (0) root         (0)    39019 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_transform.py
+-rw-rw-r--   0 root         (0) root         (0)      741 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_version.py
+-rw-rw-r--   0 root         (0) root         (0)     1229 2024-05-29 19:43:53.000000 eemeter-4.0.2/tests/test_warnings.py
```

### Comparing `eemeter-4.0.1/LICENSE` & `eemeter-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/PKG-INFO` & `eemeter-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eemeter
-Version: 4.0.1
+Version: 4.0.2
 Summary: Open Energy Efficiency Meter
 Home-page: http://github.com/openeemeter/eemeter
 Author: Phil Ngo
 Author-email: admin@openee.io
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `eemeter-4.0.1/README.rst` & `eemeter-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/__init__.py` & `eemeter-4.0.2/eemeter/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/__version__.py` & `eemeter-4.0.2/eemeter/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 __title__ = "eemeter"
 __description__ = "Open Energy Efficiency Meter"
 __url__ = "http://github.com/openeemeter/eemeter"
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 __author__ = "Phil Ngo"
 __author_email__ = "admin@openee.io"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2014-2024 OpenEEmeter contributors"
```

### Comparing `eemeter-4.0.1/eemeter/common/__init__.py` & `eemeter-4.0.2/eemeter/common/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/abstract_data_processor.py` & `eemeter-4.0.2/eemeter/common/abstract_data_processor.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/abstract_data_settings.py` & `eemeter-4.0.2/eemeter/common/abstract_data_settings.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/adaptive_loss.py` & `eemeter-4.0.2/eemeter/common/adaptive_loss.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/adaptive_loss_tck.py` & `eemeter-4.0.2/eemeter/common/adaptive_loss_tck.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/const.py` & `eemeter-4.0.2/eemeter/common/const.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/data_settings.py` & `eemeter-4.0.2/eemeter/common/data_settings.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/common/test_data.py` & `eemeter-4.0.2/eemeter/common/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 from eemeter.common.const import TutorialDataChoice
 
 # Define the current directory
 current_dir = Path(__file__).resolve().parent
 data_dir = current_dir.parents[1] / "data"
 
 # Set download branch
-## TODO: THIS BRANCH MUST BE UPDATED TO THE CURRENT BRANCH
-branch = "feature/caltrack-2.1-daily"
+branch = "master"
 
 
 comparison_group_time_series = [
     TutorialDataChoice.HOURLY_COMPARISON_GROUP_DATA,
     TutorialDataChoice.DAILY_COMPARISON_GROUP_DATA,
     TutorialDataChoice.MONTHLY_COMPARISON_GROUP_DATA,
 ]
```

### Comparing `eemeter-4.0.1/eemeter/common/utils.py` & `eemeter-4.0.2/eemeter/common/utils.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/drmeter/__init__.py` & `eemeter-4.0.2/eemeter/drmeter/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/drmeter/data.py` & `eemeter-4.0.2/eemeter/drmeter/data.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/drmeter/model.py` & `eemeter-4.0.2/eemeter/drmeter/model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/common/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/data_processor_utilities.py` & `eemeter-4.0.2/eemeter/eemeter/common/sufficiency_criteria.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,116 +14,557 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 
 """
 from math import ceil
-from typing import Optional
 
+import dataclasses
 import numpy as np
 import pandas as pd
 import pytz
-from pandas.tseries.offsets import MonthBegin, MonthEnd
 
 from eemeter.eemeter.common.warnings import EEMeterWarning
+from eemeter.eemeter.common.data_processor_utilities import day_counts
 
 
-def remove_duplicates(df_or_series):
-    """Remove duplicate rows or values by keeping the first of each duplicate.
+@dataclasses.dataclass
+class SufficiencyCriteria:
+    data: pd.DataFrame
+    requested_start: pd.Timestamp = None
+    requested_end: pd.Timestamp = None
+    num_days: int = 365
+    min_fraction_daily_coverage: float = 0.9
+    min_fraction_hourly_temperature_coverage_per_period: float = 0.9
+    is_reporting_data: bool = False
+    is_electricity_data: bool = True
+    disqualification: list = dataclasses.field(default_factory=list)
+    warnings: list = dataclasses.field(default_factory=list)
+    n_days_total: int = None
+
+    def __post_init__(self):
+        self._compute_n_days_total()
+        self._compute_valid_meter_temperature_days()
+
+    def _check_no_data(self):
+        if self.data.dropna().empty:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.no_data",
+                    description=("No data available."),
+                    data={},
+                )
+            )
+            return False
+        return True
 
-    Parameters
-    ----------
-    df_or_series : :any:`pandas.DataFrame` or :any:`pandas.Series`
-        Pandas object from which to drop duplicate index values.
-
-    Returns
-    -------
-    deduplicated : :any:`pandas.DataFrame` or :any:`pandas.Series`
-        The deduplicated pandas object.
-    """
-    # CalTrack 2.3.2.2
-    return df_or_series[~df_or_series.index.duplicated(keep="first")]
+    def _check_n_days_end_gap(self):
+        data_end = self.data.dropna().index.max()
 
+        if self.requested_end is not None:
+            # check for gap at end
+            self.requested_end = self.requested_end.astimezone(pytz.UTC)
+            n_days_end_gap = (self.requested_end - data_end).days
+        else:
+            n_days_end_gap = 0
 
-def day_counts(index):
-    """Days between DatetimeIndex values as a :any:`pandas.Series`.
+        if n_days_end_gap < 0:
+            # CalTRACK 2.2.4
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria"
+                        ".extra_data_after_requested_end_date"
+                    ),
+                    description=("Extra data found after requested end date."),
+                    data={
+                        "requested_end": self.requested_end.isoformat(),
+                        "data_end": data_end.isoformat(),
+                    },
+                )
+            )
+        n_days_end_gap = 0
 
-    Parameters
-    ----------
-    index : :any:`pandas.DatetimeIndex`
-        The index for which to get day counts.
-
-    Returns
-    -------
-    day_counts : :any:`pandas.Series`
-        A :any:`pandas.Series` with counts of days between periods. Counts are
-        given on start dates of periods.
-    """
-    # dont affect the original data
-    index = index.copy()
+    def _check_n_days_start_gap(self):
+        data_start = self.data.dropna().index.min()
 
-    if len(index) == 0:
-        return pd.Series([], index=index)
+        if self.requested_start is not None:
+            # check for gap at beginning
+            self.requested_start = self.requested_start.astimezone(pytz.UTC)
+            n_days_start_gap = (data_start - self.requested_start).days
+        else:
+            n_days_start_gap = 0
 
-    timedeltas = (index[1:] - index[:-1]).append(pd.TimedeltaIndex([pd.NaT]))
-    timedelta_days = timedeltas.total_seconds() / (60 * 60 * 24)
+        if n_days_start_gap < 0:
+            # CalTRACK 2.2.4
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria"
+                        ".extra_data_before_requested_start_date"
+                    ),
+                    description=("Extra data found before requested start date."),
+                    data={
+                        "requested_start": self.requested_start.isoformat(),
+                        "data_start": data_start.isoformat(),
+                    },
+                )
+            )
+            n_days_start_gap = 0
 
-    return pd.Series(timedelta_days, index=index)
+    def _check_negative_meter_values(self):
+        if not self.is_reporting_data and not self.is_electricity_data:
+            n_negative_meter_values = self.data.observed[self.data.observed < 0].shape[
+                0
+            ]
+
+            if n_negative_meter_values > 0:
+                # CalTrack 2.3.5
+                self.disqualification.append(
+                    EEMeterWarning(
+                        qualified_name=(
+                            "eemeter.sufficiency_criteria" ".negative_meter_values"
+                        ),
+                        description=("Found negative meter data values"),
+                        data={"n_negative_meter_values": n_negative_meter_values},
+                    )
+                )
 
+    def _compute_n_days_total(self):
+        data_end = self.data.dropna().index.max()
+        data_start = self.data.dropna().index.min()
+        n_days_data = (
+            data_end - data_start
+        ).days + 1  # TODO confirm. no longer using last row nan
+
+        if self.requested_start is not None:
+            # check for gap at beginning
+            self.requested_start = self.requested_start.astimezone(pytz.UTC)
+            n_days_start_gap = (data_start - self.requested_start).days
+        else:
+            n_days_start_gap = 0
 
-def clean_billing_data(data, source_interval, warnings):
-    # check for empty data
-    if data["value"].dropna().empty:
-        return data[:0]
+        if self.requested_end is not None:
+            # check for gap at end
+            self.requested_end = self.requested_end.astimezone(pytz.UTC)
+            n_days_end_gap = (self.requested_end - data_end).days
+        else:
+            n_days_end_gap = 0
 
-    if source_interval.startswith("billing"):
-        diff = list((data.index[1:] - data.index[:-1]).days)
-        filter_ = pd.Series(diff + [np.nan], index=data.index)
+        n_days_total = n_days_data + n_days_start_gap + n_days_end_gap
 
-        # CalTRACK 2.2.3.4, 2.2.3.5
-        if source_interval == "billing_monthly":
-            data = data[
-                (filter_ <= 35) & (filter_ >= 25)  # keep these, inclusive
-            ].reindex(data.index)
+        self.n_days_total = n_days_total
+
+    def _check_baseline_length_daily_billing_model(self):
+        
+
+        MAX_BASELINE_LENGTH = 365
+        MIN_BASELINE_LENGTH = ceil(0.9 * MAX_BASELINE_LENGTH)
+        if (
+            not self.is_reporting_data
+            and self.n_days_total > MAX_BASELINE_LENGTH
+            or self.n_days_total < MIN_BASELINE_LENGTH
+        ):
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria" ".incorrect_number_of_total_days"
+                    ),
+                    description=(
+                        f"Baseline length is not within the expected range of {MIN_BASELINE_LENGTH}-{MAX_BASELINE_LENGTH} days."
+                    ),
+                    data={"num_days": self.num_days, "n_days_total": self.n_days_total},
+                )
+            )
+
+    def _compute_valid_meter_temperature_days(self):
+        if not self.is_reporting_data:
+            valid_meter_value_rows = self.data.observed.notnull()
+        valid_temperature_rows = (
+            self.data.temperature_not_null
+            / (self.data.temperature_not_null + self.data.temperature_null)
+        ) > self.min_fraction_hourly_temperature_coverage_per_period
+
+        if not self.is_reporting_data:
+            valid_rows = valid_meter_value_rows & valid_temperature_rows
+        else:
+            valid_rows = valid_temperature_rows
+
+        # get number of days per period - for daily this should be a series of ones
+        row_day_counts = day_counts(self.data.index)
+
+        # apply masks, giving total
+        if not self.is_reporting_data:
+            self.n_valid_meter_value_days = int(
+                (valid_meter_value_rows * row_day_counts).sum()
+            )
+        n_valid_temperature_days = int((valid_temperature_rows * row_day_counts).sum())
+        n_valid_days = int((valid_rows * row_day_counts).sum())
+
+        self.n_valid_days = n_valid_days
+        self.n_valid_temperature_days = n_valid_temperature_days
+
+
+    def _check_valid_days_percentage(self):
+
+        if self.n_days_total > 0:
+            fraction_valid_days = self.n_valid_days / float(self.n_days_total)
+        else:
+            fraction_valid_days = 0
+        
+
+        if fraction_valid_days < self.min_fraction_daily_coverage:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria"
+                        ".too_many_days_with_missing_data"
+                    ),
+                    description=(
+                        "Too many days in data have missing meter data or"
+                        " temperature data."
+                    ),
+                    data={
+                        "n_valid_days": self.n_valid_days,
+                        "n_days_total": self.n_days_total,
+                    },
+                )
+            )
 
-            if len(data[(filter_ > 35) | (filter_ < 25)]) > 0:
-                warnings.append(
+    def _check_valid_meter_readings_percentage(self):
+
+        if self.n_days_total > 0:
+            if not self.is_reporting_data:
+                fraction_valid_meter_value_days = self.n_valid_meter_value_days / float(
+                    self.n_days_total
+                )
+        else:
+            fraction_valid_meter_value_days = 0
+
+
+        if (
+            not self.is_reporting_data
+            and fraction_valid_meter_value_days < self.min_fraction_daily_coverage
+        ):
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria"
+                        ".too_many_days_with_missing_meter_data"
+                    ),
+                    description=("Too many days in data have missing meter data."),
+                    data={
+                        "n_valid_meter_data_days": self.n_valid_meter_value_days,
+                        "n_days_total": self.n_days_total,
+                    },
+                )
+            )
+
+    def _check_valid_temperature_values_percentage(self):
+
+        if self.n_days_total > 0:
+            fraction_valid_temperature_days = self.n_valid_temperature_days / float(
+                self.n_days_total
+            )
+        else:
+            fraction_valid_temperature_days = 0
+
+        if fraction_valid_temperature_days < self.min_fraction_daily_coverage:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name=(
+                        "eemeter.sufficiency_criteria"
+                        ".too_many_days_with_missing_temperature_data"
+                    ),
+                    description=(
+                        "Too many days in data have missing temperature data."
+                    ),
+                    data={
+                        "n_valid_temperature_data_days": self.n_valid_temperature_days,
+                        "n_days_total": self.n_days_total,
+                    },
+                )
+            )
+
+    def _check_monthly_temperature_values_percentage(self):
+        non_null_temp_percentage_per_month = (
+            self.data["temperature"]
+            .groupby(self.data.index.month)
+            .apply(lambda x: x.notna().mean())
+        )
+        if (
+            non_null_temp_percentage_per_month < self.min_fraction_daily_coverage
+        ).any():
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.missing_monthly_temperature_data",
+                    description=(
+                        "More than 10% of the monthly temperature data is missing."
+                    ),
+                    data={
+                        # TODO report percentage
+                    },
+                )
+            )
+
+    def _check_season_weekday_weekend_availability(self):
+        raise NotImplementedError(
+            "90% of season and weekday/weekend check not implemented yet"
+        )
+
+    def _check_extreme_values(self):
+        if not self.is_reporting_data:
+            median = self.data.observed.median()
+            upper_quantile = self.data.observed.quantile(0.75)
+            lower_quantile = self.data.observed.quantile(0.25)
+            iqr = upper_quantile - lower_quantile
+            extreme_value_limit = median + (3 * iqr)
+            n_extreme_values = self.data.observed[
+                self.data.observed > extreme_value_limit
+            ].shape[0]
+            max_value = float(self.data.observed.max())
+
+            if n_extreme_values > 0:
+                # CalTRACK 2.3.6
+                self.warnings.append(
                     EEMeterWarning(
-                        qualified_name="eemeter.sufficiency_criteria.offcycle_reads_in_billing_monthly_data",
+                        qualified_name=(
+                            "eemeter.sufficiency_criteria" ".extreme_values_detected"
+                        ),
                         description=(
-                            "Off-cycle reads found in billing monthly data having a duration of less than 25 days"
+                            "Extreme values (greater than (median + (3 * IQR)),"
+                            " must be flagged for manual review."
                         ),
-                        data=[
-                            timestamp.isoformat()
-                            for timestamp in data[(filter_ > 35) | (filter_ < 25)].index
-                        ],
+                        data={
+                            "n_extreme_values": n_extreme_values,
+                            "median": median,
+                            "upper_quantile": upper_quantile,
+                            "lower_quantile": lower_quantile,
+                            "extreme_value_limit": extreme_value_limit,
+                            "max_value": max_value,
+                        },
                     )
                 )
 
-        # CalTRACK 2.2.3.4, 2.2.3.5
-        if source_interval == "billing_bimonthly":
-            data = data[
-                (filter_ <= 70) & (filter_ >= 25)  # keep these, inclusive
-            ].reindex(data.index)
+    def _check_high_frequency_temperature_values(self):
+        # If high frequency data check for 50% data coverage in rollup
+        if len(temperature_features[temperature_features.coverage <= 0.5]) > 0:
+            self.warnings.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.missing_high_frequency_temperature_data",
+                    description=(
+                        "More than 50% of the high frequency Temperature data is missing."
+                    ),
+                    data={
+                        "high_frequency_data_missing_count": len(
+                            temperature_features[
+                                temperature_features.coverage <= 0.5
+                            ].index.to_list()
+                        )
+                    },
+                )
+            )
+
+        # Set missing high frequency data to NaN
+        temperature_features.value[temperature_features.coverage > 0.5] = (
+            temperature_features[temperature_features.coverage > 0.5].value
+            / temperature_features[temperature_features.coverage > 0.5].coverage
+        )
+
+        temperature_features = (
+            temperature_features[temperature_features.coverage > 0.5]
+            .reindex(temperature_features.index)[["value"]]
+            .rename(columns={"value": "temperature_mean"})
+        )
+
+        if "coverage" in temperature_features.columns:
+            temperature_features = temperature_features.drop(columns=["coverage"])
+
+    def _check_high_frequency_meter_values(self):
+        if not self.data[self.data.coverage <= 0.5].empty:
+            self.warnings.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.missing_high_frequency_meter_data",
+                    description=(
+                        "More than 50% of the high frequency Meter data is missing."
+                    ),
+                    data=(self.data[self.data.coverage <= 0.5].index.to_list()),
+                )
+            )
+
+        # CalTRACK 2.2.2.1 - interpolate with average of non-null values
+        self.data.value[self.data.coverage > 0.5] = (
+            self.data[self.data.coverage > 0.5].value
+            / self.data[self.data.coverage > 0.5].coverage
+        )
 
-            if len(data[(filter_ > 70) | (filter_ < 25)]) > 0:
-                warnings.append(
+    def check_sufficiency_baseline(self):
+        raise NotImplementedError("Use Hourly / Daily / Billing SufficiencyCriteria class for concrete implementation")
+
+    def check_sufficiency_reporting(self):
+        raise NotImplementedError("Use Hourly / Daily / Billing SufficiencyCriteria class for concrete implementation")
+
+
+class HourlySufficiencyCriteria(SufficiencyCriteria):
+    """
+        Sufficiency Criteria class for hourly models
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _check_baseline_length_hourly_model(self):
+        # TODO : Implement this
+        raise NotImplementedError("Hourly Baseline length check not implemented yet")
+
+    def _check_monthly_meter_readings_percentage(self):
+        if not self.is_reporting_data:
+            non_null_meter_percentage_per_month = (
+                self.data["observed"]
+                .groupby(self.data.index.month)
+                .apply(lambda x: x.notna().mean())
+            )
+            if (
+                non_null_meter_percentage_per_month < self.min_fraction_daily_coverage
+            ).any():
+                self.disqualification.append(
                     EEMeterWarning(
-                        qualified_name="eemeter.sufficiency_criteria.offcycle_reads_in_billing_monthly_data",
+                        qualified_name="eemeter.sufficiency_criteria.missing_monthly_meter_data",
                         description=(
-                            "Off-cycle reads found in billing monthly data having a duration of less than 25 days"
+                            "More than 10% of the monthly meter data is missing."
                         ),
-                        data=[
-                            timestamp.isoformat()
-                            for timestamp in data[(filter_ > 70) | (filter_ < 25)].index
-                        ],
+                        data={
+                            # TODO report percentage
+                        },
                     )
                 )
 
+    def _check_hourly_consecutive_temperature_data(self):
+        # TODO : Check implementation wrt Caltrack 2.2.4.1
+        # Resample to hourly by taking the first non NaN value
+        hourly_data = self.data['temperature'].resample('H').first()
+        mask = hourly_data.isna().any(axis=1)
+        grouped = mask.groupby((mask != mask.shift()).cumsum())
+        max_consecutive_nans = grouped.sum().max()
+        if max_consecutive_nans > 6:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.too_many_consecutive_hours_temperature_data_missing",
+                    description=("More than 6 hours of consecutive hourly data is missing."),
+                    data={'Max_consecutive_hours_missing': int(max_consecutive_nans)},
+                )
+            )
+
+    def check_sufficiency_baseline(self):
+        # TODO : add caltrack check number on top of each method
+        self._check_no_data()
+        self._check_negative_meter_values()
+        self._check_baseline_length_hourly_model()
+        self._check_valid_days_percentage()
+        self._check_valid_meter_readings_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        self._check_monthly_meter_readings_percentage()
+        self._check_extreme_values()
+        self._check_high_frequency_meter_values()
+        self._check_high_frequency_temperature_values()
+        self._check_hourly_consecutive_temperature_data()
+
+
+    def check_sufficiency_reporting(self):
+        self._check_no_data()
+        self._check_valid_days_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        # self._check_high_frequency_temperature_values()
+
+    
+class DailySufficiencyCriteria(SufficiencyCriteria):
+    """
+        Sufficiency Criteria class for daily models
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def check_sufficiency_baseline(self):
+        self._check_no_data()
+        self._check_negative_meter_values()
+        self._check_baseline_length_daily_billing_model()
+        self._check_valid_days_percentage()
+        self._check_valid_meter_readings_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        self._check_extreme_values()
+        # TODO : Maybe make these checks static? To work with the current data class
+        # self._check_high_frequency_meter_values()
+        # self._check_high_frequency_temperature_values()
+
+    def check_sufficiency_reporting(self):
+        self._check_no_data()
+        self._check_valid_days_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        # self._check_high_frequency_temperature_values()
+
+
+class BillingSufficiencyCriteria(SufficiencyCriteria):
+    """
+        Sufficiency Criteria class for billing models - monthly / bimonthly
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def _check_meter_data_billing_monthly(self):
+        if self.data["value"].dropna().empty:
+            return
+
+        diff = list((data.index[1:] - data.index[:-1]).days)
+        filter_ = pd.Series(diff + [np.nan], index=data.index)
+
+        # CalTRACK 2.2.3.4, 2.2.3.5
+        # Billing Monthly data frequency check
+        data = data[(filter_ <= 35) & (filter_ >= 25)].reindex(  # keep these, inclusive
+            data.index
+        )
+
+        if len(data[(filter_ > 35) | (filter_ < 25)]) > 0:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.offcycle_reads_in_billing_monthly_data",
+                    description=(
+                        "Off-cycle reads found in billing monthly data having a duration of less than 25 days"
+                    ),
+                    data=(data[(filter_ > 35) | (filter_ < 25)].index.to_list()),
+                )
+            )
+
+    def _check_meter_data_billing_bimonthly(self):
+        if self.data["value"].dropna().empty:
+            return
+
+        diff = list((data.index[1:] - data.index[:-1]).days)
+        filter_ = pd.Series(diff + [np.nan], index=data.index)
+
+        # CalTRACK 2.2.3.4, 2.2.3.5
+        data = data[(filter_ <= 70) & (filter_ >= 25)].reindex(  # keep these, inclusive
+            data.index
+        )
+
+        if len(data[(filter_ > 70) | (filter_ < 25)]) > 0:
+            self.disqualification.append(
+                EEMeterWarning(
+                    qualified_name="eemeter.sufficiency_criteria.offcycle_reads_in_billing_monthly_data",
+                    description=(
+                        "Off-cycle reads found in billing monthly data having a duration of less than 25 days"
+                    ),
+                    data=(data[(filter_ > 70) | (filter_ < 25)].index.to_list()),
+                )
+            )
+
+    def _check_estimated_meter_values(self):
         # CalTRACK 2.2.3.1
         """
         Adds estimate to subsequent read if there aren't more than one estimate in a row
         and then removes the estimated row.
 
         Input:
         index   value   estimated
@@ -143,15 +584,15 @@
         4       9
         5       NaN
         7       7
         8       NaN
         """
         add_estimated = []
         remove_estimated_fixed_rows = []
-        orig_data = data.copy()
+        data = self.data
         if "estimated" in data.columns:
             data["unestimated_value"] = (
                 data[:-1].value[(data[:-1].estimated == False)].reindex(data.index)
             )
             data["estimated_value"] = (
                 data[:-1].value[(data[:-1].estimated)].reindex(data.index)
             )
@@ -170,481 +611,29 @@
                 prev_row = row
                 prev_index = index
             add_estimated.append(np.nan)
             data["value"] = data["unestimated_value"] + add_estimated
             data = data[~data.index.isin(remove_estimated_fixed_rows)]
             data = data[["value"]]  # remove the estimated column
 
-    # check again for empty data
-    if data.dropna().empty:
-        return data[:0]
-
-    return data["value"].to_frame()
-
-
-def as_freq(
-    data_series,
-    freq,
-    atomic_freq="1 Min",
-    series_type="cumulative",
-    include_coverage=False,
-):
-    """Resample data to a different frequency.
-
-    This method can be used to upsample or downsample meter data. The
-    assumption it makes to do so is that meter data is constant and averaged
-    over the given periods. For instance, to convert billing-period data to
-    daily data, this method first upsamples to the atomic frequency
-    (1 minute freqency, by default), "spreading" usage evenly across all
-    minutes in each period. Then it downsamples to hourly frequency and
-    returns that result. With instantaneous series, the data is copied to all
-    contiguous time intervals and the mean over `freq` is returned.
-
-    **Caveats**:
-
-     - This method gives a fair amount of flexibility in
-       resampling as long as you are OK with the assumption that usage is
-       constant over the period (this assumption is generally broken in
-       observed data at large enough frequencies, so this caveat should not be
-       taken lightly).
-
-    Parameters
-    ----------
-    data_series : :any:`pandas.Series`
-        Data to resample. Should have a :any:`pandas.DatetimeIndex`.
-    freq : :any:`str`
-        The frequency to resample to. This should be given in a form recognized
-        by the :any:`pandas.Series.resample` method.
-    atomic_freq : :any:`str`, optional
-        The "atomic" frequency of the intermediate data form. This can be
-        adjusted to a higher atomic frequency to increase speed or memory
-        performance.
-    series_type : :any:`str`, {'cumulative', ‘instantaneous’},
-        default 'cumulative'
-        Type of data sampling. 'cumulative' data can be spread over smaller
-        time intervals and is aggregated using addition (e.g. meter data).
-        'instantaneous' data is copied (not spread) over smaller time intervals
-        and is aggregated by averaging (e.g. weather data).
-    include_coverage: :any:`bool`,
-        default `False`
-        Option of whether to return a series with just the resampled values
-        or a dataframe with a column that includes percent coverage of source data
-        used for each sample.
-
-    Returns
-    -------
-    resampled_data : :any:`pandas.Series` or :any:`pandas.DataFrame`
-        Data resampled to the given frequency (optionally as a dataframe with a coverage column if `include_coverage` is used.
-    """
-    # TODO(philngo): make sure this complies with CalTRACK 2.2.2.1
-    if not isinstance(data_series, pd.Series):
-        raise ValueError(
-            "expected series, got object with class {}".format(data_series.__class__)
-        )
-    if data_series.empty:
-        return data_series
-    series = remove_duplicates(data_series)
-    target_freq = pd.Timedelta(atomic_freq)
-    timedeltas = (series.index[1:] - series.index[:-1]).append(
-        pd.TimedeltaIndex([pd.NaT])
-    )
-
-    if series_type == "cumulative":
-        spread_factor = target_freq.total_seconds() / timedeltas.total_seconds()
-        series_spread = series * spread_factor
-        atomic_series = series_spread.asfreq(atomic_freq, method="ffill")
-        resampled = atomic_series.resample(freq, origin=series.index[0]).sum()
-        resampled_with_nans = atomic_series.resample(
-            freq, origin=series.index[0]
-        ).first()
-        n_coverage = atomic_series.resample(freq, origin=series.index[0]).count()
-        resampled = resampled[resampled_with_nans.notnull()].reindex(resampled.index)
-
-    elif series_type == "instantaneous":
-        # ffill on series.asfreq can produce unintuitive results if resampling a sparse matrix.
-        # for example, attempting to resample 2 months of hourly data to daily with a month of
-        # absent rows (not NaN, but missing from the dataframe) will ffill that month with the previous read.
-        #
-        # a similar effect can happen if you have NaNs at a different frequency appended to the end
-        # of a series. this could happen if you concat a monthly series with an hourly one at an offset.
-        # the call to asfreq() could erroneously fill in a month of data, followed by NaNs
-        atomic_series = series.asfreq(atomic_freq, method="ffill")
-        resampled = atomic_series.resample(freq, origin=series.index[0]).mean()
-        n_coverage = atomic_series.resample(freq, origin=series.index[0]).count()
-
-    # Edit : Added a check so that hourly and daily frequencies don't have a null value at the end
-    if freq not in ["H", "D"] and resampled.index[-1] < series.index[-1]:
-        # this adds a null at the end using the target frequency
-        last_index = pd.date_range(resampled.index[-1], freq=freq, periods=2)[1:]
-        resampled = (
-            pd.concat([resampled, pd.Series(np.nan, index=last_index)])
-            .resample(freq)
-            .mean()
-        )
-    if include_coverage:
-        n_total = resampled.resample(atomic_freq).count().resample(freq).count()
-        resampled = resampled.to_frame("value")
-        resampled["coverage"] = n_coverage / n_total
-
-        # TODO : hacky fix to account all occurences of last hour not being counted due to the NaN appended above.
-        # Due to above issue number of median granularity periods would end up being 1 rather than the entire 720(24 * 30), thus squashing the
-        # reported value to 1/720th the actual. Set it back to 1 like the other usual periods. Might break if the last period is uneven.
-        if resampled.coverage[-1] > 1:
-            resampled.coverage[-1] = 1
-        return resampled
-    else:
-        return resampled
-
-
-def downsample_and_clean_daily_data(dataset, warnings):
-    dataset = as_freq(dataset, "D", include_coverage=True)
-
-    if not dataset[dataset.coverage <= 0.5].empty:
-        warnings.append(
-            EEMeterWarning(
-                qualified_name="eemeter.sufficiency_criteria.missing_high_frequency_meter_data",
-                description=(
-                    "More than 50% of the high frequency Meter data is missing."
-                ),
-                data=[
-                    timestamp.isoformat()
-                    for timestamp in dataset[dataset.coverage <= 0.5].index
-                ],
-            )
-        )
-
-    # CalTRACK 2.2.2.1 - interpolate with average of non-null values
-    dataset.value[dataset.coverage > 0.5] = (
-        dataset[dataset.coverage > 0.5].value / dataset[dataset.coverage > 0.5].coverage
-    )
-
-    return dataset[dataset.coverage > 0.5].reindex(dataset.index)[["value"]]
-
-
-def clean_billing_daily_data(data, source_interval, warnings):
-    # billing data is cleaned but not resampled
-    if source_interval.startswith("billing"):
-        # CalTRACK 2.2.3.4, 2.2.3.5
-        return clean_billing_data(data, source_interval, warnings)
-
-    # higher intervals like daily, hourly, 30min, 15min are
-    # resampled (daily) or downsampled (hourly, 30min, 15min)
-    elif source_interval == "daily":
-        return data.to_frame("value")
-    else:
-        return downsample_and_clean_daily_data(data, warnings)
-
-
-# TODO : requires more testing
-def compute_minimum_granularity(index: pd.Series, default_granularity: Optional[str]):
-    # Inferred frequency returns None if frequency can't be autodetected
-    index.freq = index.inferred_freq
-    if index.freq is None:
-        # max_difference = day_counts(index).max()
-        # min_difference = day_counts(index).min()
-        median_difference = day_counts(index).median()
-        # if max_difference == 1 and min_difference == 1:
-        #     min_granularity = 'daily'
-        # elif max_difference < 1:
-        #     min_granularity = 'hourly'
-        # elif max_difference >= 60:
-        #     min_granularity = 'billing_bimonthly'
-        # elif max_difference >= 30:
-        #     min_granularity = 'billing_monthly'
-        # else:
-        #     min_granularity = default_granularity
-
-        granularity_dict = {
-            median_difference < 1: "hourly",
-            median_difference == 1: "daily",
-            1 < median_difference <= 35: "billing_monthly",
-            35 < median_difference <= 70: "billing_bimonthly",
-        }
-        min_granularity = granularity_dict.get(True, default_granularity)
-        return min_granularity
-    # The other cases still result in granularity being unknown so this causes the frequency to be resampled to daily
-    if isinstance(index.freq, MonthEnd) or isinstance(
-        index.freq, MonthBegin
-    ):  # Can be MonthEnd or MonthBegin instance
-        if index.freq.n == 1:
-            min_granularity = "billing_monthly"
-        else:
-            min_granularity = "billing_bimonthly"
-    elif index.freq <= pd.Timedelta(hours=1):
-        min_granularity = "hourly"
-    elif index.freq <= pd.Timedelta(days=1):
-        min_granularity = "daily"
-    elif index.freq <= pd.Timedelta(days=30):
-        min_granularity = "billing_monthly"
-    else:
-        min_granularity = "billing_bimonthly"
-
-    return min_granularity
-
-
-def sufficiency_criteria_baseline(
-    data,
-    requested_start=None,
-    requested_end=None,
-    num_days=365,
-    min_fraction_daily_coverage=0.9,
-    min_fraction_hourly_temperature_coverage_per_period=0.9,
-    is_reporting_data=False,
-    is_electricity_data=True,
-):
-    """
-    Refer to usage_per_day.py in eemeter/caltrack/ folder
-    """
-    warnings = []
-    if data.dropna().empty:
-        warnings.append(
-            EEMeterWarning(
-                qualified_name="eemeter.sufficiency_criteria.no_data",
-                description=("No data available."),
-                data={},
-            )
-        )
-        return data, warnings, []
-
-    data_start = data.dropna().index.min()
-    data_end = data.dropna().index.max()
-    n_days_data = (
-        data_end - data_start
-    ).days + 1  # TODO confirm. no longer using last row nan
-
-    if requested_start is not None:
-        # check for gap at beginning
-        requested_start = requested_start.astimezone(pytz.UTC)
-        n_days_start_gap = (data_start - requested_start).days
-    else:
-        n_days_start_gap = 0
-
-    if requested_end is not None:
-        # check for gap at end
-        requested_end = requested_end.astimezone(pytz.UTC)
-        n_days_end_gap = (requested_end - data_end).days
-    else:
-        n_days_end_gap = 0
-
-    critical_warnings = []
-    non_critical_warnings = []
-
-    if n_days_end_gap < 0:
-        # CalTRACK 2.2.4
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria"
-                    ".extra_data_after_requested_end_date"
-                ),
-                description=("Extra data found after requested end date."),
-                data={
-                    "requested_end": requested_end.isoformat(),
-                    "data_end": data_end.isoformat(),
-                },
-            )
-        )
-        n_days_end_gap = 0
-
-    if n_days_start_gap < 0:
-        # CalTRACK 2.2.4
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria"
-                    ".extra_data_before_requested_start_date"
-                ),
-                description=("Extra data found before requested start date."),
-                data={
-                    "requested_start": requested_start.isoformat(),
-                    "data_start": data_start.isoformat(),
-                },
-            )
-        )
-        n_days_start_gap = 0
-
-    n_days_total = n_days_data + n_days_start_gap + n_days_end_gap
-
-    if not is_reporting_data and not is_electricity_data:
-        n_negative_meter_values = data.observed[data.observed < 0].shape[0]
-
-        # TODO : This check should only be done for non electric data
-        if n_negative_meter_values > 0:
-            # CalTrack 2.3.5
-            critical_warnings.append(
-                EEMeterWarning(
-                    qualified_name=(
-                        "eemeter.sufficiency_criteria" ".negative_meter_values"
-                    ),
-                    description=("Found negative meter data values"),
-                    data={"n_negative_meter_values": n_negative_meter_values},
-                )
-            )
-
-    # TODO(philngo): detect and report unsorted or repeated values.
-
-    # create masks showing which daily or billing periods meet criteria
-
-    # TODO : How to handle temperature if already rolled up in the dataframe?
-    if not is_reporting_data:
-        valid_meter_value_rows = data.observed.notnull()
-    valid_temperature_rows = (
-        data.temperature_not_null / (data.temperature_not_null + data.temperature_null)
-    ) > min_fraction_hourly_temperature_coverage_per_period
-
-    if not is_reporting_data:
-        valid_rows = valid_meter_value_rows & valid_temperature_rows
-    else:
-        valid_rows = valid_temperature_rows
-
-    # get number of days per period - for daily this should be a series of ones
-    row_day_counts = day_counts(data.index)
-
-    # apply masks, giving total
-    if not is_reporting_data:
-        n_valid_meter_value_days = int((valid_meter_value_rows * row_day_counts).sum())
-    n_valid_temperature_days = int((valid_temperature_rows * row_day_counts).sum())
-    n_valid_days = int((valid_rows * row_day_counts).sum())
-
-    if not is_reporting_data:
-        median = data.observed.median()
-        upper_quantile = data.observed.quantile(0.75)
-        lower_quantile = data.observed.quantile(0.25)
-        iqr = upper_quantile - lower_quantile
-        extreme_value_limit = median + (3 * iqr)
-        n_extreme_values = data.observed[data.observed > extreme_value_limit].shape[0]
-        max_value = float(data.observed.max())
-
-    if n_days_total > 0:
-        if not is_reporting_data:
-            fraction_valid_meter_value_days = n_valid_meter_value_days / float(
-                n_days_total
-            )
-        fraction_valid_temperature_days = n_valid_temperature_days / float(n_days_total)
-        fraction_valid_days = n_valid_days / float(n_days_total)
-    else:
-        # unreachable, I think.
-        fraction_valid_meter_value_days = 0
-        fraction_valid_temperature_days = 0
-        fraction_valid_days = 0
-
-    MAX_BASELINE_LENGTH = 365
-    MIN_BASELINE_LENGTH = ceil(0.9 * MAX_BASELINE_LENGTH)
-    if (
-        not is_reporting_data
-        and n_days_total > MAX_BASELINE_LENGTH
-        or n_days_total < MIN_BASELINE_LENGTH
-    ):
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria" ".incorrect_number_of_total_days"
-                ),
-                description=(
-                    f"Baseline length is not within the expected range of {MIN_BASELINE_LENGTH}-{MAX_BASELINE_LENGTH} days."
-                ),
-                data={"num_days": num_days, "n_days_total": n_days_total},
-            )
-        )
-
-    if fraction_valid_days < min_fraction_daily_coverage:
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria" ".too_many_days_with_missing_data"
-                ),
-                description=(
-                    "Too many days in data have missing meter data or"
-                    " temperature data."
-                ),
-                data={"n_valid_days": n_valid_days, "n_days_total": n_days_total},
-            )
-        )
-
-    if (
-        not is_reporting_data
-        and fraction_valid_meter_value_days < min_fraction_daily_coverage
-    ):
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria"
-                    ".too_many_days_with_missing_meter_data"
-                ),
-                description=("Too many days in data have missing meter data."),
-                data={
-                    "n_valid_meter_data_days": n_valid_meter_value_days,
-                    "n_days_total": n_days_total,
-                },
-            )
-        )
-
-    if fraction_valid_temperature_days < min_fraction_daily_coverage:
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria"
-                    ".too_many_days_with_missing_temperature_data"
-                ),
-                description=("Too many days in data have missing temperature data."),
-                data={
-                    "n_valid_temperature_data_days": n_valid_temperature_days,
-                    "n_days_total": n_days_total,
-                },
-            )
-        )
-
-    # Check for 90% for individual months present:
-    non_null_temp_percentage_per_month = (
-        data["temperature"].groupby(data.index.month).apply(lambda x: x.notna().mean())
-    )
-    if (non_null_temp_percentage_per_month < min_fraction_daily_coverage).any():
-        critical_warnings.append(
-            EEMeterWarning(
-                qualified_name="eemeter.sufficiency_criteria.missing_monthly_temperature_data",
-                description=(
-                    "More than 10% of the monthly temperature data is missing."
-                ),
-                data={
-                    # TODO report percentage
-                },
-            )
-        )
-
-    # if not is_reporting_data:
-    #     non_null_meter_percentage_per_month = data['observed'].groupby(data.index.month).apply(lambda x: x.notna().mean())
-    #     if (non_null_meter_percentage_per_month < min_fraction_daily_coverage).any():
-    #         critical_warnings.append(
-    #             EEMeterWarning(
-    #                 qualified_name="eemeter.sufficiency_criteria.missing_monthly_meter_data",
-    #                 description=("More than 10% of the monthly meter data is missing."),
-    #                 data={
-    #                     #TODO report percentage
-    #                 },
-    #             )
-    #         )
-
-    # TODO : Check 90% of seasons & weekday/weekend available?
-
-    if not is_reporting_data and n_extreme_values > 0:
-        # CalTRACK 2.3.6
-        non_critical_warnings.append(
-            EEMeterWarning(
-                qualified_name=(
-                    "eemeter.sufficiency_criteria" ".extreme_values_detected"
-                ),
-                description=(
-                    "Extreme values (greater than (median + (3 * IQR)),"
-                    " must be flagged for manual review."
-                ),
-                data={
-                    "n_extreme_values": n_extreme_values,
-                    "median": median,
-                    "upper_quantile": upper_quantile,
-                    "lower_quantile": lower_quantile,
-                    "extreme_value_limit": extreme_value_limit,
-                    "max_value": max_value,
-                },
-            )
-        )
-
-    return data, critical_warnings, non_critical_warnings
+    def check_sufficiency_baseline(self):
+        self._check_no_data()
+        self._check_negative_meter_values()
+        # if self.median_granularity == "billing_monthly":
+        #     self._check_meter_data_billing_monthly()
+        # else :
+        #     self._check_meter_data_billing_bimonthly()
+        self._check_baseline_length_daily_billing_model()
+        self._check_valid_days_percentage()
+        self._check_valid_meter_readings_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        self._check_extreme_values()
+        self._check_estimated_meter_values()
+        # self._check_high_frequency_temperature_values()
+
+    def check_sufficiency_reporting(self):
+        self._check_no_data()
+        self._check_valid_days_percentage()
+        self._check_valid_temperature_values_percentage()
+        self._check_monthly_temperature_values_percentage()
+        # self._check_high_frequency_temperature_values()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/exceptions.py` & `eemeter-4.0.2/eemeter/eemeter/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/features.py` & `eemeter-4.0.2/eemeter/eemeter/common/features.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/transform.py` & `eemeter-4.0.2/eemeter/eemeter/common/transform.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/common/warnings.py` & `eemeter-4.0.2/eemeter/eemeter/common/warnings.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/billing/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/billing/data.py` & `eemeter-4.0.2/eemeter/eemeter/models/billing/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 import pandas as pd
 from pandas.tseries.offsets import MonthBegin, MonthEnd
 
 from eemeter.eemeter.common.data_processor_utilities import (
     as_freq,
     clean_billing_daily_data,
     compute_minimum_granularity,
-    sufficiency_criteria_baseline,
 )
 from eemeter.eemeter.common.features import compute_temperature_features
 from eemeter.eemeter.common.warnings import EEMeterWarning
+from eemeter.eemeter.common.sufficiency_criteria import BillingSufficiencyCriteria
 from eemeter.eemeter.models.daily.data import _DailyData
 
 """TODO there is still a ton of unecessarily duplicated code between billing+daily.
     we should be able to perform a few transforms within the billing baseclass, and then call super() for the rest
 
     unsure whether we should inherit from the public classes because we'll have to take care to use type(data)
     instead of isinstance(data,  _) when doing the checks in the model/wrapper to avoid unintentionally allowing a mix of data/model type
@@ -321,19 +321,27 @@
             temperature_not_null: number of temperature non null periods in each aggregation step
 
         Returns:
             disqualification (List): List of disqualifications
             warnings (list): List of warnings
 
         """
-        _, disqualification, warnings = sufficiency_criteria_baseline(
-            sufficiency_df,
-            is_reporting_data=False,
-            is_electricity_data=self.is_electricity_data,
+        bsc = BillingSufficiencyCriteria(
+            data = sufficiency_df,
+            is_electricity_data = self.is_electricity_data
         )
+        bsc.check_sufficiency_baseline()
+        disqualification = bsc.disqualification
+        warnings = bsc.warnings
+
+        # _, disqualification, warnings = sufficiency_criteria_baseline(
+        #     sufficiency_df,
+        #     is_reporting_data=False,
+        #     is_electricity_data=self.is_electricity_data,
+        # )
         return disqualification, warnings
 
 
 class BillingReportingData(_BillingData):
     """
     Data class to represent Billing Reporting Data. Only reporting data should go into the dataframe input, no blackout data should be input.
     Checks sufficiency for the data provided as input depending on OpenEEMeter specifications and populates disqualifications and warnings based on it.
@@ -442,13 +450,21 @@
 
         Returns
         -------
             disqualification (List): List of disqualifications
             warnings (list): List of warnings
 
         """
-        _, disqualification, warnings = sufficiency_criteria_baseline(
-            sufficiency_df,
-            is_reporting_data=True,
-            is_electricity_data=self.is_electricity_data,
+        bsc = BillingSufficiencyCriteria(
+            data = sufficiency_df,
+            is_reporting_data = True
         )
+        bsc.check_sufficiency_reporting()
+        disqualification = bsc.disqualification
+        warnings = bsc.warnings
+
+        # _, disqualification, warnings = sufficiency_criteria_baseline(
+        #     sufficiency_df,
+        #     is_reporting_data=True,
+        #     is_electricity_data=self.is_electricity_data,
+        # )
         return disqualification, warnings
```

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/billing/model.py` & `eemeter-4.0.2/eemeter/eemeter/models/billing/model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/billing/plot.py` & `eemeter-4.0.2/eemeter/eemeter/models/billing/plot.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/c_hdd_tidd.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/c_hdd_tidd.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/full_model.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/full_model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/hdd_tidd_cdd.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/hdd_tidd_cdd.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/base_models/tidd.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/base_models/tidd.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/data.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 import pandas as pd
 
 import eemeter.common.const as _const
 from eemeter.eemeter.common.data_processor_utilities import (
     as_freq,
     clean_billing_daily_data,
     compute_minimum_granularity,
-    remove_duplicates,
-    sufficiency_criteria_baseline,
+    remove_duplicates
 )
 from eemeter.eemeter.common.features import compute_temperature_features
 from eemeter.eemeter.common.warnings import EEMeterWarning
+from eemeter.eemeter.common.sufficiency_criteria import DailySufficiencyCriteria
 
 
 class _DailyData:
     """Private base class for daily baseline and reporting data.
 
     Will raise exception during data sufficiency check if instantiated
     """
@@ -503,14 +503,21 @@
                         "Datetime index is in UTC. Use tz_localize() with the local timezone to ensure correct aggregations"
                     ),
                     data={},
                 )
             )
         self.tz = df.index.tz
 
+        # prevent later issues when merging on generated datetimes, which default to ns precision
+        # there is almost certainly a smoother way to accomplish this conversion, but this works
+        if df.index.dtype.unit != "ns":
+            utc_index = df.index.tz_convert("UTC")
+            ns_index = utc_index.astype("datetime64[ns, UTC]")
+            df.index = ns_index.tz_convert(self.tz)
+
         # Convert electricity data having 0 meter values to NaNs
         if self.is_electricity_data:
             df.loc[df["observed"] == 0, "observed"] = np.nan
 
         # Caltrack 2.3.2 - Drop duplicates
         df = remove_duplicates(df)
 
@@ -567,20 +574,22 @@
 
         Returns:
             disqualification (List): List of disqualifications
             warnings (list): List of warnings
 
         """
         # 90% coverage per period only required for billing models
-        _, disqualification, warnings = sufficiency_criteria_baseline(
-            sufficiency_df,
-            min_fraction_hourly_temperature_coverage_per_period=0.5,
-            is_reporting_data=False,
-            is_electricity_data=self.is_electricity_data,
-        )
+        dsc = DailySufficiencyCriteria(
+            data = sufficiency_df,
+            is_electricity_data = self.is_electricity_data
+        )
+        dsc.check_sufficiency_baseline()
+        disqualification = dsc.disqualification
+        warnings = dsc.warnings
+
         return disqualification, warnings
 
 
 class DailyReportingData(_DailyData):
     """
     Data class to represent Daily Reporting Data. Only reporting data should go into the dataframe input, no blackout data should be input.
     Checks sufficiency for the data provided as input depending on OpenEEMeter specifications and populates disqualifications and warnings based on it.
@@ -690,14 +699,16 @@
         Returns
         -------
             disqualification (List): List of disqualifications
             warnings (list): List of warnings
 
         """
         # 90% coverage per period only required for billing models
-        _, disqualification, warnings = sufficiency_criteria_baseline(
-            sufficiency_df,
-            min_fraction_hourly_temperature_coverage_per_period=0.5,
-            is_reporting_data=True,
-            is_electricity_data=self.is_electricity_data,
-        )
+        dsc = DailySufficiencyCriteria(
+            data = sufficiency_df,
+            is_reporting_data = True
+        )
+        dsc.check_sufficiency_reporting()
+        disqualification = dsc.disqualification
+        warnings = dsc.warnings
+
         return disqualification, warnings
```

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/fit_base_models.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/fit_base_models.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/model.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/objective_function.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/objective_function.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/optimize.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/optimize.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/optimize_results.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/optimize_results.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/parameters.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/parameters.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/plot.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/plot.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/base_model.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/base_model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/config.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/config.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/ellipsoid_test.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/ellipsoid_test.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/daily/utilities/selection_criteria.py` & `eemeter-4.0.2/eemeter/eemeter/models/daily/utilities/selection_criteria.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/data.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/data.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/derivatives.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/derivatives.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/design_matrices.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/design_matrices.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/metrics.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/metrics.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/model.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/segmentation.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/segmentation.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/usage_per_day.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/usage_per_day.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/models/hourly/wrapper.py` & `eemeter-4.0.2/eemeter/eemeter/models/hourly/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,17 +60,15 @@
     occupied_temperature_bins = None
     unoccupied_temperature_bins = None
     segmented_design_matrices = None
 
 
 class HourlyModel:
     def __init__(self, settings=None):
-        if settings is None:
-            settings = {}
-        self.segment_type = settings.get("segment_type", "three_month_weighted")
+        self.segment_type = "three_month_weighted"
         self.alpha = 0.1
 
     def fit(self, data):
         meter_data = data.df["observed"].to_frame("value")
         temperature_data = data.df["temperature"]
 
         self.model_process_variables = IntermediateModelVariables()
```

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-daily.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-daily.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-hourly.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-hourly.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-hdd-tempF.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-hdd-tempF.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-daily.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-daily.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-electricity-cdd-only-hourly.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-electricity-cdd-only-hourly.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-daily.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-daily.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-gas-hdd-only-hourly.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-gas-hdd-only-hourly.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-daily.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-daily.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-gas-intercept-only-hourly.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-gas-intercept-only-hourly.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/il-tempF.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/il-tempF.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/load.py` & `eemeter-4.0.2/eemeter/eemeter/samples/load.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/metadata.json` & `eemeter-4.0.2/eemeter/eemeter/samples/metadata.json`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-0.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-0.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-1.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-1.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-2.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-electricity-hdd-only-hourly-sample-2.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-gas-hdd-only-hourly-sample-0.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-gas-hdd-only-hourly-sample-0.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-tempC-sample-0.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-tempC-sample-0.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/samples/uk-tempC-sample-1_2.csv.gz` & `eemeter-4.0.2/eemeter/eemeter/samples/uk-tempC-sample-1_2.csv.gz`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/utilities/__init__.py` & `eemeter-4.0.2/eemeter/eemeter/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/utilities/cli.py` & `eemeter-4.0.2/eemeter/eemeter/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter/eemeter/utilities/io.py` & `eemeter-4.0.2/eemeter/eemeter/utilities/io.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/eemeter.egg-info/PKG-INFO` & `eemeter-4.0.2/eemeter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eemeter
-Version: 4.0.1
+Version: 4.0.2
 Summary: Open Energy Efficiency Meter
 Home-page: http://github.com/openeemeter/eemeter
 Author: Phil Ngo
 Author-email: admin@openee.io
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `eemeter-4.0.1/eemeter.egg-info/SOURCES.txt` & `eemeter-4.0.2/eemeter.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 eemeter/drmeter/data.py
 eemeter/drmeter/model.py
 eemeter/eemeter/__init__.py
 eemeter/eemeter/common/__init__.py
 eemeter/eemeter/common/data_processor_utilities.py
 eemeter/eemeter/common/exceptions.py
 eemeter/eemeter/common/features.py
+eemeter/eemeter/common/sufficiency_criteria.py
 eemeter/eemeter/common/transform.py
 eemeter/eemeter/common/warnings.py
 eemeter/eemeter/models/__init__.py
 eemeter/eemeter/models/billing/__init__.py
 eemeter/eemeter/models/billing/data.py
 eemeter/eemeter/models/billing/model.py
 eemeter/eemeter/models/billing/plot.py
```

### Comparing `eemeter-4.0.1/setup.py` & `eemeter-4.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/conftest.py` & `eemeter-4.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/base_models/test_c_hdd_tidd_smooth.py` & `eemeter-4.0.2/tests/daily_model/base_models/test_c_hdd_tidd_smooth.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/base_models/test_full_model_finder.py` & `eemeter-4.0.2/tests/daily_model/base_models/test_full_model_finder.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_billing_data.py` & `eemeter-4.0.2/tests/daily_model/test_billing_data.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_daily_data.py` & `eemeter-4.0.2/tests/daily_model/test_daily_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -785,8 +785,33 @@
     baseline_meter_data, temp_series = baseline_data_daily_params(tz=tz, hour=hour)
     baseline = DailyBaselineData.from_series(baseline_meter_data, temp_series, is_electricity_data=True)
     tz = baseline_meter_data.index.tz
 
     abs_diff = 0
     for day in baseline.df.index:
         abs_diff += abs(temp_series[day:day+pd.Timedelta(hours=23)].mean() - baseline.df.temperature.loc[day].squeeze())
-    assert abs_diff < 0.000001
+    assert abs_diff < 0.000001
+
+def test_non_ns_datetime_index():
+    meter, temperature, _ = load_sample("il-electricity-cdd-hdd-hourly")
+    meter = meter[meter.index.year == 2017]
+    temperature = temperature[temperature.index.year == 2017]
+
+    # convert to microseconds
+    meter.index = meter.index.astype("datetime64[us, UTC]")
+    temperature.index = temperature.index.astype("datetime64[us, UTC]")
+    cls = DailyBaselineData.from_series(meter, temperature, is_electricity_data=True)
+
+    assert cls.df is not None
+    assert len(cls.df) == NUM_DAYS_IN_YEAR
+
+def test_offset_aggregations_hourly(il_electricity_cdd_hdd_hourly):
+    meter_data = il_electricity_cdd_hdd_hourly["meter_data"]
+    temperature_data = il_electricity_cdd_hdd_hourly["temperature_data"]
+    blackout_start_date = il_electricity_cdd_hdd_hourly["blackout_start_date"]
+    baseline_meter_data, warnings = get_baseline_data(
+        meter_data, end=blackout_start_date
+    )
+    baseline_meter_data = baseline_meter_data.iloc[3:]  # begin from 3AM UTC
+    baseline = DailyBaselineData.from_series(baseline_meter_data, temperature_data, is_electricity_data=True)
+    assert baseline is not None
+    assert len(baseline.df) == NUM_DAYS_IN_YEAR
```

### Comparing `eemeter-4.0.1/tests/daily_model/test_daily_model.py` & `eemeter-4.0.2/tests/daily_model/test_daily_model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_fit_base_models.py` & `eemeter-4.0.2/tests/daily_model/test_fit_base_models.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_fit_model.py` & `eemeter-4.0.2/tests/daily_model/test_fit_model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_objective_function.py` & `eemeter-4.0.2/tests/daily_model/test_objective_function.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_optimize.py` & `eemeter-4.0.2/tests/daily_model/test_optimize.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/test_optimize_results.py` & `eemeter-4.0.2/tests/daily_model/test_optimize_results.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_adaptive_loss.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_adaptive_loss.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_base_model.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_base_model.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_config.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_config.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_ellipsoid_test.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_ellipsoid_test.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_selection_criteria.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_selection_criteria.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/daily_model/utilities/test_utils.py` & `eemeter-4.0.2/tests/daily_model/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/snapshots/__init__.py` & `eemeter-4.0.2/tests/snapshots/__init__.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/snapshots/snap_test_features.py` & `eemeter-4.0.2/tests/snapshots/snap_test_features.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_caltrack_design_matrices.py` & `eemeter-4.0.2/tests/test_caltrack_design_matrices.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_caltrack_hourly.py` & `eemeter-4.0.2/tests/test_caltrack_hourly.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_cli.py` & `eemeter-4.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_derivatives.py` & `eemeter-4.0.2/tests/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_exceptions.py` & `eemeter-4.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_features.py` & `eemeter-4.0.2/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_io.py` & `eemeter-4.0.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_json_serialization.py` & `eemeter-4.0.2/tests/test_json_serialization.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_samples.py` & `eemeter-4.0.2/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_segmentation.py` & `eemeter-4.0.2/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_transform.py` & `eemeter-4.0.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_version.py` & `eemeter-4.0.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `eemeter-4.0.1/tests/test_warnings.py` & `eemeter-4.0.2/tests/test_warnings.py`

 * *Files identical despite different names*

