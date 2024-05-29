# Comparing `tmp/adafruit-circuitpython-ov5640-1.1.9.tar.gz` & `tmp/adafruit_circuitpython_ov5640-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ov5640-1.1.9.tar", last modified: Fri Aug 26 02:27:09 2022, max compression
+gzip compressed data, was "adafruit_circuitpython_ov5640-1.2.0.tar", last modified: Wed May 29 16:04:16 2024, max compression
```

## Comparing `adafruit-circuitpython-ov5640-1.1.9.tar` & `adafruit_circuitpython_ov5640-1.2.0.tar`

### file list

```diff
@@ -1,51 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.304962 adafruit-circuitpython-ov5640-1.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:27:09.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41909 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/adafruit_ov5640.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.308962 adafruit-circuitpython-ov5640-1.1.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6081 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     6247 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_directio_kaluga1_3_ili9341.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3_boot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3544 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_sdcard_kaluga_1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_stopmotion_kaluga1_3.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-08-26 02:27:00.000000 adafruit-circuitpython-ov5640-1.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:26:50.000000 adafruit-circuitpython-ov5640-1.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:27:09.312962 adafruit-circuitpython-ov5640-1.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.211452 adafruit_circuitpython_ov5640-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.199452 adafruit_circuitpython_ov5640-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.203452 adafruit_circuitpython_ov5640-1.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.203452 adafruit_circuitpython_ov5640-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.207452 adafruit_circuitpython_ov5640-1.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/LICENSES/GPL-2.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-29 16:04:16.211452 adafruit_circuitpython_ov5640-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.211452 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-29 16:04:16.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-29 16:04:16.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 16:04:16.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 16:04:16.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 16:04:16.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.207452 adafruit_circuitpython_ov5640-1.2.0/adafruit_ov5640/
+-rw-r--r--   0 runner    (1001) docker     (127)    46757 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_ov5640/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_ov5640/ov5640_autofocus.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/adafruit_ov5640/ov5640_autofocus.bin.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.207452 adafruit_circuitpython_ov5640-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.207452 adafruit_circuitpython_ov5640-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 16:04:16.211452 adafruit_circuitpython_ov5640-1.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_directio_kaluga1_3_ili9341.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_capture_af.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_capture_manual_focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_kaluga1_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_kaluga1_3_boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_pico_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_pico_st7789.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_sdcard_kaluga_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_stopmotion_kaluga1_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-29 16:04:13.000000 adafruit_circuitpython_ov5640-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 16:04:05.000000 adafruit_circuitpython_ov5640-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 16:04:16.211452 adafruit_circuitpython_ov5640-1.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_ov5640-1.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/.gitignore` & `adafruit_circuitpython_ov5640-1.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/.pre-commit-config.yaml` & `adafruit_circuitpython_ov5640-1.2.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/.pylintrc` & `adafruit_circuitpython_ov5640-1.2.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_ov5640-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/LICENSE` & `adafruit_circuitpython_ov5640-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_ov5640-1.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/LICENSES/MIT.txt` & `adafruit_circuitpython_ov5640-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_ov5640-1.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/PKG-INFO` & `adafruit_circuitpython_ov5640-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov5640
-Version: 1.1.9
+Version: 1.2.0
 Summary: CircuitPython driver for OV5640 Camera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OV5640
 Keywords: adafruit,ov5640,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ov5640/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ov5640/en/latest/
@@ -53,15 +55,15 @@
     pip3 install circup
 
 With ``circup`` installed and your CircuitPython device connected use the
 following command to install:
 
 .. code-block:: shell
 
-    circup install ov5640
+    circup install adafruit_ov5640
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/README.rst` & `adafruit_circuitpython_ov5640-1.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     pip3 install circup
 
 With ``circup`` installed and your CircuitPython device connected use the
 following command to install:
 
 .. code-block:: shell
 
-    circup install ov5640
+    circup install adafruit_ov5640
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/PKG-INFO` & `adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ov5640
-Version: 1.1.9
+Version: 1.2.0
 Summary: CircuitPython driver for OV5640 Camera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OV5640
 Keywords: adafruit,ov5640,camera,breakout,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ov5640/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ov5640/en/latest/
@@ -53,15 +55,15 @@
     pip3 install circup
 
 With ``circup`` installed and your CircuitPython device connected use the
 following command to install:
 
 .. code-block:: shell
 
-    circup install ov5640
+    circup install adafruit_ov5640
 
 Or the following command to update an existing version:
 
 .. code-block:: shell
 
     circup update
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt` & `adafruit_circuitpython_ov5640-1.2.0/adafruit_circuitpython_ov5640.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,47 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
-adafruit_ov5640.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
+LICENSES/GPL-2.0-only.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ov5640.egg-info/PKG-INFO
 adafruit_circuitpython_ov5640.egg-info/SOURCES.txt
 adafruit_circuitpython_ov5640.egg-info/dependency_links.txt
 adafruit_circuitpython_ov5640.egg-info/requires.txt
 adafruit_circuitpython_ov5640.egg-info/top_level.txt
+adafruit_ov5640/__init__.py
+adafruit_ov5640/ov5640_autofocus.bin
+adafruit_ov5640/ov5640_autofocus.bin.license
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/ov5640_directio_kaluga1_3_ili9341.py
+examples/ov5640_jpeg_capture_af.py
+examples/ov5640_jpeg_capture_manual_focus.py
 examples/ov5640_jpeg_kaluga1_3.py
 examples/ov5640_jpeg_kaluga1_3_boot.py
+examples/ov5640_pico_simpletest.py
+examples/ov5640_pico_st7789.py
 examples/ov5640_sdcard_kaluga_1_3.py
 examples/ov5640_simpletest.py
 examples/ov5640_stopmotion_kaluga1_3.py
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/adafruit_ov5640.py` & `adafruit_circuitpython_ov5640-1.2.0/adafruit_ov5640/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
 # pylint: disable=too-many-lines
-
+# pylint: disable=too-many-public-methods
 # imports
 import time
 import imagecapture
 import pwmio
 from adafruit_bus_device.i2c_device import I2CDevice
 
 try:
     from typing import Optional, Sequence, List, Union
     from busio import I2C
     from microcontroller import Pin
     from digitalio import DigitalInOut
 except ImportError:
     pass
 
-__version__ = "1.1.9"
+__version__ = "1.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ov5640.git"
 
 from micropython import const
 
 OV5640_COLOR_RGB = 0
 OV5640_COLOR_YUV = 1
 OV5640_COLOR_GRAYSCALE = 2
@@ -410,14 +410,36 @@
 
 _pll_pre_div2x_factors = [1, 1, 2, 3, 4, 1.5, 6, 2.5, 8]
 _pll_pclk_root_div_factors = [1,2,4,8]
 
 _REG_DLY = const(0xFFFF)
 _REGLIST_TAIL = const(0x0000)
 
+_OV5640_STAT_FIRMWAREBAD = const(0x7F)
+_OV5640_STAT_STARTUP = const(0x7E)
+_OV5640_STAT_IDLE = const(0x70)
+_OV5640_STAT_FOCUSING = const(0x00)
+_OV5640_STAT_FOCUSED = const(0x10)
+
+_OV5640_CMD_TRIGGER_AUTOFOCUS = const(0x03)
+_OV5640_CMD_AUTO_AUTOFOCUS = const(0x04)
+_OV5640_CMD_RELEASE_FOCUS = const(0x08)
+_OV5640_CMD_AF_SET_VCM_STEP = const(0x1A)
+_OV5640_CMD_AF_GET_VCM_STEP = const(0x1B)
+
+_OV5640_CMD_MAIN = const(0x3022)
+_OV5640_CMD_ACK = const(0x3023)
+_OV5640_CMD_PARA0 = const(0x3024)
+_OV5640_CMD_PARA1 = const(0x3025)
+_OV5640_CMD_PARA2 = const(0x3026)
+_OV5640_CMD_PARA3 = const(0x3027)
+_OV5640_CMD_PARA4 = const(0x3028)
+_OV5640_CMD_FW_STATUS = const(0x3029)
+
+
 _sensor_default_regs = [
     _SYSTEM_CTROL0, 0x82,  # software reset
     _REG_DLY, 10,  # delay 10ms
     _SYSTEM_CTROL0, 0x42,  # power down
     # enable pll
     0x3103, 0x13,
     # io direction
@@ -932,14 +954,35 @@
         reg_value = obj._read_register16(self.reg)
         reg_value &= ~(self.mask << self.shift)
         reg_value |= value << self.shift
         obj._write_register16(self.reg, reg_value)
 
 
 class _SCCB16CameraBase:  # pylint: disable=too-few-public-methods
+    _finalize_firmware_load = (
+        0x3022,
+        0x00,
+        0x3023,
+        0x00,
+        0x3024,
+        0x00,
+        0x3025,
+        0x00,
+        0x3026,
+        0x00,
+        0x3027,
+        0x00,
+        0x3028,
+        0x00,
+        0x3029,
+        0x7F,
+        0x3000,
+        0x00,
+    )
+
     def __init__(self, i2c_bus: I2C, i2c_address: int) -> None:
         self._i2c_device = I2CDevice(i2c_bus, i2c_address)
         self._bank = None
 
     def _write_register(self, reg: int, value: int) -> None:
         b = bytearray(3)
         b[0] = reg >> 8
@@ -1000,14 +1043,15 @@
         href: Pin,
         shutdown: Optional[DigitalInOut] = None,
         reset: Optional[DigitalInOut] = None,
         mclk: Optional[Pin] = None,
         mclk_frequency: int = 20_000_000,
         i2c_address: int = 0x3C,
         size: int = OV5640_SIZE_QQVGA,
+        init_autofocus: bool = True,
     ):  # pylint: disable=too-many-arguments
         """
         Args:
             i2c_bus (busio.I2C): The I2C bus used to configure the OV5640
             data_pins (List[microcontroller.Pin]): A list of 8 data pins, in order.
             clock (microcontroller.Pin): The pixel clock from the OV5640.
             vsync (microcontroller.Pin): The vsync signal from the OV5640.
@@ -1024,14 +1068,15 @@
                 ignored if mclk is None, requred if it is specified.
                 Note that the OV5640 requires a very low jitter clock,
                 so only specific (microcontroller-dependent) values may
                 work reliably.  On the ESP32-S2, a 20MHz clock can be generated
                 with sufficiently low jitter.
             i2c_address (int): The I2C address of the camera.
             size (int): The captured image size
+            init_autofocus (bool): initialize autofocus
         """
 
         # Initialize the master clock
         if mclk:
             self._mclk_pwm = pwmio.PWMOut(mclk, frequency=mclk_frequency)
             self._mclk_pwm.duty_cycle = 32768
         else:
@@ -1074,16 +1119,108 @@
         self._test_pattern = False
         self._binning = False
         self._scale = False
         self._ev = 0
         self._white_balance = 0
         self.size = size
 
+        if init_autofocus:
+            self.autofocus_init()
+
     chip_id = _RegBits16(_CHIP_ID_HIGH, 0, 0xFFFF)
 
+    def autofocus_init_from_file(self, filename):
+        """Initialize the autofocus engine from a .bin file"""
+        with open(filename, mode="rb") as file:
+            firmware = file.read()
+        self.autofocus_init_from_bitstream(firmware)
+
+    def autofocus_init_from_bitstream(self, firmware: bytes):
+        """Initialize the autofocus engine from a bytestring"""
+        self._write_register(0x3000, 0x20)  # reset autofocus coprocessor
+        time.sleep(0.01)
+
+        arr = bytearray(256)
+        with self._i2c_device as i2c:
+            for offset in range(0, len(firmware), 254):
+                num_firmware_bytes = min(254, len(firmware) - offset)
+                reg = offset + 0x8000
+                arr[0] = reg >> 8
+                arr[1] = reg & 0xFF
+                arr[2 : 2 + num_firmware_bytes] = firmware[
+                    offset : offset + num_firmware_bytes
+                ]
+                i2c.write(arr, end=2 + num_firmware_bytes)
+
+        self._write_list(self._finalize_firmware_load)
+        for _ in range(100):
+            if self.autofocus_status == _OV5640_STAT_IDLE:
+                break
+            time.sleep(0.01)
+        else:
+            raise RuntimeError("Timed out after trying to load autofocus firmware")
+
+    def autofocus_init(self):
+        """Initialize the autofocus engine from ov5640_autofocus.bin"""
+        if "/" in __file__:
+            binfile = (
+                __file__.rsplit("/", 1)[0].rsplit(".", 1)[0] + "/ov5640_autofocus.bin"
+            )
+        else:
+            binfile = "ov5640_autofocus.bin"
+        print(binfile)
+        return self.autofocus_init_from_file(binfile)
+
+    @property
+    def autofocus_status(self):
+        """Read the camera autofocus status register"""
+        return self._read_register(_OV5640_CMD_FW_STATUS)
+
+    def _send_autofocus_command(self, command, msg):  # pylint: disable=unused-argument
+        self._write_register(_OV5640_CMD_ACK, 0x01)  # clear command ack
+        self._write_register(_OV5640_CMD_MAIN, command)  # send command
+        for _ in range(1000):
+            if self._read_register(_OV5640_CMD_ACK) == 0x0:  # command is finished
+                return True
+            time.sleep(0.01)
+        return False
+
+    def autofocus(self) -> list[int]:
+        """Perform an autofocus operation.
+
+        If all elements of the list are 0, the autofocus operation failed. Otherwise,
+        if at least one element is nonzero, the operation succeeded.
+
+        In principle the elements correspond to 5 autofocus regions, if configured."""
+        if not self._send_autofocus_command(_OV5640_CMD_RELEASE_FOCUS, "release focus"):
+            return [False] * 5
+        if not self._send_autofocus_command(_OV5640_CMD_TRIGGER_AUTOFOCUS, "autofocus"):
+            return [False] * 5
+        zone_focus = [self._read_register(_OV5640_CMD_PARA0 + i) for i in range(5)]
+        print(f"zones focused: {zone_focus}")
+        return zone_focus
+
+    @property
+    def autofocus_vcm_step(self):
+        """Get the voice coil motor step location"""
+        if not self._send_autofocus_command(
+            _OV5640_CMD_AF_GET_VCM_STEP, "get vcm step"
+        ):
+            return None
+        return self._read_register(_OV5640_CMD_PARA4)
+
+    @autofocus_vcm_step.setter
+    def autofocus_vcm_step(self, step):
+        """Get the voice coil motor step location, from 0 to 255"""
+        if not 0 <= step <= 255:
+            raise RuntimeError("VCM step must be 0 to 255")
+        self._write_register(_OV5640_CMD_PARA3, 0x00)
+        self._write_register(_OV5640_CMD_PARA4, step)
+        self._send_autofocus_command(_OV5640_CMD_AF_SET_VCM_STEP, "set vcm step")
+
     def capture(self, buf: Union[bytearray, memoryview]) -> None:
         """Capture an image into the buffer.
 
         Args:
             buf (Union[bytearray, memoryview]): A WritableBuffer to contain the \
                 captured image.  Note that this can be a ulab array or a displayio Bitmap.
         """
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/docs/_static/favicon.ico` & `adafruit_circuitpython_ov5640-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/docs/conf.py` & `adafruit_circuitpython_ov5640-1.2.0/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
@@ -116,27 +117,18 @@
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/docs/examples.rst` & `adafruit_circuitpython_ov5640-1.2.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/docs/index.rst` & `adafruit_circuitpython_ov5640-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_directio_kaluga1_3_ili9341.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_directio_kaluga1_3_ili9341.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,17 @@
         yield from brightness_modes(cam_obj)
         # These don't work right (yet)
         # yield from exposure_value_modes(cam_obj)  # Issue #8
         # yield from nite_modes(cam_obj) # Issue #6
 
 
 def main():
+    deadline = 0
+    effects = iter((None,))
+
     display.auto_refresh = False
     display_bus.send(42, struct.pack(">hh", 0, bitmap.width - 1))
     display_bus.send(43, struct.pack(">hh", 0, bitmap.height - 1))
 
     if test_effects:
         time_per_effect = 1500
         deadline = ticks_ms() + time_per_effect
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_kaluga1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_jpeg_kaluga1_3_boot.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_jpeg_kaluga1_3_boot.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_sdcard_kaluga_1_3.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_sdcard_kaluga_1_3.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_simpletest.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ov5640-1.1.9/examples/ov5640_stopmotion_kaluga1_3.py` & `adafruit_circuitpython_ov5640-1.2.0/examples/ov5640_stopmotion_kaluga1_3.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 
 # Pre-cache the next image number
 next_filename("gif")
 
 # Blank the whole display, we'll draw what we want with directio
 empty_group = displayio.Group()
-display.show(empty_group)
+display.root_group = empty_group
 display.auto_refresh = False
 display.refresh()
 
 
 def open_next_image(extension="jpg"):
     while True:
         filename = next_filename(extension)
@@ -231,15 +231,34 @@
         frame = wait_record_pressed_update_display(True, cap)
         with open_next_image("gif") as f, gifio.GifWriter(
             f, cam.width, cam.height, displayio.Colorspace.RGB565_SWAPPED, dither=True
         ) as g:
             g.add_frame(frame, replay_frame_time)
             for i in range(1, n_frames):
                 print(f"{i}/{n_frames}")
-                old_frame.blit(0, 0, frame, x1=0, y1=0, x2=frame.width, y2=frame.height)
+
+                # CircuitPython Versions <= 8.2.0
+                if hasattr(old_frame, "blit"):
+                    old_frame.blit(
+                        0, 0, frame, x1=0, y1=0, x2=frame.width, y2=frame.height
+                    )
+
+                # CircuitPython Versions >= 9.0.0
+                else:
+                    bitmaptools.blit(
+                        old_frame,
+                        frame,
+                        0,
+                        0,
+                        x1=0,
+                        y1=0,
+                        x2=frame.width,
+                        y2=frame.height,
+                    )
+
                 frame = wait_record_pressed_update_display(False, cap)
                 g.add_frame(frame, replay_frame_time)
             print("done")
 
 
 est_frame_size = cam.width * cam.height * 128 // 126 + 1
 est_hdr_size = 1000
```

### Comparing `adafruit-circuitpython-ov5640-1.1.9/pyproject.toml` & `adafruit_circuitpython_ov5640-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ov5640"
 description = "CircuitPython driver for OV5640 Camera"
-version = "1.1.9"
+version = "1.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_OV5640"}
 keywords = [
     "adafruit",
@@ -34,12 +34,12 @@
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["adafruit_ov5640"]
+packages = ["adafruit_ov5640"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = {optional = {file = ["optional_requirements.txt"]}}
```

