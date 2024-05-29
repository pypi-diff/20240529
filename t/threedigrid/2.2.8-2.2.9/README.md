# Comparing `tmp/threedigrid-2.2.8.tar.gz` & `tmp/threedigrid-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedigrid-2.2.8.tar", last modified: Thu Apr 25 12:14:17 2024, max compression
+gzip compressed data, was "threedigrid-2.2.9.tar", last modified: Mon May 27 13:26:04 2024, max compression
```

## Comparing `threedigrid-2.2.8.tar` & `threedigrid-2.2.9.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-25 12:14:13.000000 threedigrid-2.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-25 12:14:13.000000 threedigrid-2.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-04-25 12:14:13.000000 threedigrid-2.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-25 12:14:13.000000 threedigrid-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-25 12:14:13.000000 threedigrid-2.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-25 12:14:17.452208 threedigrid-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-25 12:14:13.000000 threedigrid-2.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.436207 threedigrid-2.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/aggregate_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/functionalities.rst
--rw-r--r--   0 runner    (1001) docker     (127)    37537 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/gridadmin.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/structure_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-25 12:14:13.000000 threedigrid-2.2.8/docs/water_quality_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-25 12:14:17.456208 threedigrid-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-25 12:14:13.000000 threedigrid-2.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.440208 threedigrid-2.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-25 12:14:13.000000 threedigrid-2.2.8/tests/test_aggregateresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-25 12:14:13.000000 threedigrid-2.2.8/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21148 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_gridresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_id_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_prepare_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_structure_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-25 12:14:14.000000 threedigrid-2.2.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.440208 threedigrid-2.2.8/threedigrid/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/breaches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/breaches/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/crosssections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/crosssections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/crosssections/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporter_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/gridadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/gridresultadmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/h5py_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/h5py_swmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/idmapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.444208 threedigrid-2.2.8/threedigrid/admin/levees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/levees/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/lines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/lines/timeseries_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/nodes/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/prepare_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/pumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/pumps/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/rpc_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/admin/structure_controls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/structure_controls/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/admin/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/geo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.448208 threedigrid-2.2.8/threedigrid/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/commands/kick.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/management/help_texts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/numpy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid/orm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid/orm/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/timeseries_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-25 12:14:14.000000 threedigrid-2.2.8/threedigrid/orm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:14:17.452208 threedigrid-2.2.8/threedigrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 12:14:17.000000 threedigrid-2.2.8/threedigrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.865281 threedigrid-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 13:25:59.000000 threedigrid-2.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-27 13:25:59.000000 threedigrid-2.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18787 2024-05-27 13:25:59.000000 threedigrid-2.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-27 13:25:59.000000 threedigrid-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-27 13:25:59.000000 threedigrid-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24658 2024-05-27 13:26:04.865281 threedigrid-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-27 13:25:59.000000 threedigrid-2.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.849281 threedigrid-2.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/aggregate_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/functionalities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    37537 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/gridadmin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/structure_control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-27 13:25:59.000000 threedigrid-2.2.9/docs/water_quality_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-27 13:26:04.865281 threedigrid-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-27 13:25:59.000000 threedigrid-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.849281 threedigrid-2.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-05-27 13:25:59.000000 threedigrid-2.2.9/tests/test_aggregateresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-27 13:25:59.000000 threedigrid-2.2.9/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21148 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_gridresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_id_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_prepare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_structure_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-27 13:26:01.000000 threedigrid-2.2.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.853281 threedigrid-2.2.9/threedigrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/breaches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/breaches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/breaches/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/breaches/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/breaches/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/breaches/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/crosssections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/crosssections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/crosssections/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/exporter_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/gridadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20290 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/gridresultadmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/h5py_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/h5py_swmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/idmapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/levees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/levees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/levees/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/levees/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/levees/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.857281 threedigrid-2.2.9/threedigrid/admin/lines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/lines/timeseries_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/admin/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/nodes/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/prepare_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/admin/pumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/pumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/pumps/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/pumps/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/pumps/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/rpc_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/admin/structure_controls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/structure_controls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/structure_controls/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/structure_controls/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/admin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/geo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/management/commands/kick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/management/help_texts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/numpy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.861281 threedigrid-2.2.9/threedigrid/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.865281 threedigrid-2.2.9/threedigrid/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8744 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17964 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/timeseries_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-27 13:26:01.000000 threedigrid-2.2.9/threedigrid/orm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:26:04.865281 threedigrid-2.2.9/threedigrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24658 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 13:26:04.000000 threedigrid-2.2.9/threedigrid.egg-info/top_level.txt
```

### Comparing `threedigrid-2.2.8/CONTRIBUTING.rst` & `threedigrid-2.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/HISTORY.rst` & `threedigrid-2.2.9/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+2.2.9 (2024-05-27)
+------------------
+
+- Move _field_model_dict and its methods from GridH5ResultAdmin to GridH5Admin.
+
+
 2.2.8 (2024-04-25)
 ------------------
 
 - Add `group_by_grid_id` to structure control interface.
 
 
 2.2.7 (2024-04-22)
```

### Comparing `threedigrid-2.2.8/LICENSE` & `threedigrid-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/PKG-INFO` & `threedigrid-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Classifier: Development Status :: 4 - Beta
@@ -194,14 +194,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.2.9 (2024-05-27)
+------------------
+
+- Move _field_model_dict and its methods from GridH5ResultAdmin to GridH5Admin.
+
+
 2.2.8 (2024-04-25)
 ------------------
 
 - Add `group_by_grid_id` to structure control interface.
 
 
 2.2.7 (2024-04-22)
```

### Comparing `threedigrid-2.2.8/README.rst` & `threedigrid-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/Makefile` & `threedigrid-2.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/aggregate_results.rst` & `threedigrid-2.2.9/docs/aggregate_results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/conf.py` & `threedigrid-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/functionalities.rst` & `threedigrid-2.2.9/docs/functionalities.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/gridadmin.rst` & `threedigrid-2.2.9/docs/gridadmin.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/introduction.rst` & `threedigrid-2.2.9/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/make.bat` & `threedigrid-2.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/results.rst` & `threedigrid-2.2.9/docs/results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/structure_control.rst` & `threedigrid-2.2.9/docs/structure_control.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/docs/water_quality_results.rst` & `threedigrid-2.2.9/docs/water_quality_results.rst`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/setup.cfg` & `threedigrid-2.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/setup.py` & `threedigrid-2.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_aggregateresultadmin.py` & `threedigrid-2.2.9/tests/test_aggregateresultadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_exporter.py` & `threedigrid-2.2.9/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_filters.py` & `threedigrid-2.2.9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_gridadmin.py` & `threedigrid-2.2.9/tests/test_gridadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_gridresultadmin.py` & `threedigrid-2.2.9/tests/test_gridresultadmin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_id_mapper.py` & `threedigrid-2.2.9/tests/test_id_mapper.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_management.py` & `threedigrid-2.2.9/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_meta.py` & `threedigrid-2.2.9/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_options.py` & `threedigrid-2.2.9/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_prepare.py` & `threedigrid-2.2.9/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_prepare_utils.py` & `threedigrid-2.2.9/tests/test_prepare_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_structure_controls.py` & `threedigrid-2.2.9/tests/test_structure_controls.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/tests/test_utils.py` & `threedigrid-2.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/breaches/exporters.py` & `threedigrid-2.2.9/threedigrid/admin/breaches/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/breaches/models.py` & `threedigrid-2.2.9/threedigrid/admin/breaches/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/breaches/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/breaches/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/breaches/timeseries_mixin.py` & `threedigrid-2.2.9/threedigrid/admin/breaches/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/constants.py` & `threedigrid-2.2.9/threedigrid/admin/constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/crosssections/models.py` & `threedigrid-2.2.9/threedigrid/admin/crosssections/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/exporter_constants.py` & `threedigrid-2.2.9/threedigrid/admin/exporter_constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/default.py` & `threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/default.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/exporters/geopackage/exporter.py` & `threedigrid-2.2.9/threedigrid/admin/exporters/geopackage/exporter.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/gridadmin.py` & `threedigrid-2.2.9/threedigrid/admin/gridadmin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # (c) Nelen & Schuurmans.  GPL licensed, see LICENSE.rst.
 """
 Main entry point for threedigrid applications.
 """
 
 import logging
+from collections import defaultdict
 
 import h5py
 import numpy as np
 
 from threedigrid.admin.breaches.models import Breaches
 from threedigrid.admin.crosssections.models import CrossSections
 from threedigrid.admin.h5py_datasource import H5pyGroup
 from threedigrid.admin.levees.models import Levees
 from threedigrid.admin.lines.models import Lines
 from threedigrid.admin.nodes.models import Cells, EmbeddedNodes, Grid, Nodes
 from threedigrid.admin.pumps.models import Pumps
 from threedigrid.geo_utils import raise_import_exception, transform_bbox
+from threedigrid.orm.models import Model
 
 try:
     import pyproj
 except ImportError:
     pyproj = None
 
 try:
@@ -49,15 +51,15 @@
 
     def __init__(self, h5_file_path, file_modus="r", set_props=False):
         """
         :param h5_file_path: path to the gridadmin file
         :param file_modus: mode with which to open the file
             (defaults to r=READ)
         """
-
+        self._field_model_dict = defaultdict(list)
         self.grid_file = h5_file_path
         self.datasource_class = H5pyGroup
         self.is_rpc = False
 
         if type(h5_file_path) in (str, bytes) and h5_file_path.startswith("rpc://"):
             if not asyncio_rpc_support:
                 raise Exception("Please reinstall this package with threedigrid[rpc]")
@@ -185,14 +187,58 @@
 
     @property
     def has_levees(self):
         if not hasattr(self, "levees"):
             return False
         return bool(self.levees.id.size)
 
+    @property
+    def _field_model_map(self):
+        """
+        :return: a dict of {<field name>: [model name, ...]}
+        """
+        if self._field_model_dict:
+            return self._field_model_dict
+
+        model_names = set()
+        for attr_name in dir(self):
+            # skip private attrs
+            if any([attr_name.startswith("__"), attr_name.startswith("_")]):
+                continue
+            try:
+                attr = getattr(self, attr_name)
+            except AttributeError:
+                logger.warning(
+                    "Attribute: '{}' does not " "exist in h5py_file.".format(attr_name)
+                )
+                continue
+            if not issubclass(type(attr), Model):
+                continue
+            model_names.add(attr_name)
+
+        for model_name in model_names:
+            for x in getattr(self, model_name)._field_names:
+                self._field_model_dict[x].append(model_name)
+        return self._field_model_dict
+
+    def get_model_instance_by_field_name(self, field_name):
+        """
+        :param field_name: name of a models field
+        :return: instance of the model the field belongs to
+        :raises IndexError if the field name is not unique across models
+        """
+        model_name = self._field_model_map.get(field_name)
+        if not model_name or len(model_name) != 1:
+            raise IndexError(
+                "Ambiguous result. Field name {} yields {} model(s)".format(
+                    field_name, len(model_name) if model_name else 0
+                )
+            )
+        return getattr(self, model_name[0])
+
     def get_extent_subset(self, subset_name, target_epsg_code=""):
         """
 
         :param subset_name: name of the node subset for which the extent
             should be calculated.
             Valid input: '1D_all', '2D_groundwater'
         :param target_epsg_code: string representation of the desired
```

### Comparing `threedigrid-2.2.8/threedigrid/admin/gridresultadmin.py` & `threedigrid-2.2.9/threedigrid/admin/gridresultadmin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # (c) Nelen & Schuurmans.  GPL licensed, see LICENSE.rst.
 
 
 import logging
 import re
-from collections import defaultdict
 from typing import List, Optional, Union
 
 import h5py
 import numpy as np
 
 from threedigrid.admin.breaches.models import Breaches
 from threedigrid.admin.breaches.timeseries_mixin import (
@@ -34,15 +33,14 @@
     PumpsAggregateResultsMixin,
     PumpsResultsMixin,
 )
 from threedigrid.admin.structure_controls.models import (
     StructureControl,
     StructureControlTypes,
 )
-from threedigrid.orm.models import Model
 
 logger = logging.getLogger(__name__)
 
 try:
     import asyncio_rpc  # noqa
 
     asyncio_rpc_support = True
@@ -59,15 +57,14 @@
         """
 
         :param h5_file_path: path to the hdf5 gridadmin file
         :param netcdf_file_path: path to the netcdf result file (usually
             called subgrid_map.nc)
         :param file_modus: modus in which to open the files
         """
-        self._field_model_dict = defaultdict(list)
         self._netcdf_file_path = netcdf_file_path
         super().__init__(h5_file_path, file_modus)
 
         self.result_datasource_class = H5pyResultGroup
 
         if h5_file_path.startswith("rpc://"):
             if not asyncio_rpc_support:
@@ -154,58 +151,14 @@
                 "Version result file has been created with: %s\n"
                 "Version gridadmin file has been created with: %s",
                 self.threedicore_result_version,
                 self.threedicore_version,
             )
 
     @property
-    def _field_model_map(self):
-        """
-        :return: a dict of {<field name>: [model name, ...]}
-        """
-        if self._field_model_dict:
-            return self._field_model_dict
-
-        model_names = set()
-        for attr_name in dir(self):
-            # skip private attrs
-            if any([attr_name.startswith("__"), attr_name.startswith("_")]):
-                continue
-            try:
-                attr = getattr(self, attr_name)
-            except AttributeError:
-                logger.warning(
-                    "Attribute: '{}' does not " "exist in h5py_file.".format(attr_name)
-                )
-                continue
-            if not issubclass(type(attr), Model):
-                continue
-            model_names.add(attr_name)
-
-        for model_name in model_names:
-            for x in getattr(self, model_name)._field_names:
-                self._field_model_dict[x].append(model_name)
-        return self._field_model_dict
-
-    def get_model_instance_by_field_name(self, field_name):
-        """
-        :param field_name: name of a models field
-        :return: instance of the model the field belongs to
-        :raises IndexError if the field name is not unique across models
-        """
-        model_name = self._field_model_map.get(field_name)
-        if not model_name or len(model_name) != 1:
-            raise IndexError(
-                "Ambiguous result. Field name {} yields {} model(s)".format(
-                    field_name, len(model_name) if model_name else 0
-                )
-            )
-        return getattr(self, model_name[0])
-
-    @property
     def threedicore_result_version(self):
         """
         :return: version of the grid result file (if found), an empty
         string otherwise
         """
         try:
             return self.netcdf_file.attrs.get("threedicore_version")
```

### Comparing `threedigrid-2.2.8/threedigrid/admin/h5py_datasource.py` & `threedigrid-2.2.9/threedigrid/admin/h5py_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/h5py_swmr.py` & `threedigrid-2.2.9/threedigrid/admin/h5py_swmr.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/idmapper.py` & `threedigrid-2.2.9/threedigrid/admin/idmapper.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/levees/exporters.py` & `threedigrid-2.2.9/threedigrid/admin/levees/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/levees/models.py` & `threedigrid-2.2.9/threedigrid/admin/levees/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/levees/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/levees/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/lines/exporters.py` & `threedigrid-2.2.9/threedigrid/admin/lines/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/lines/models.py` & `threedigrid-2.2.9/threedigrid/admin/lines/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/lines/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/lines/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/lines/subsets.py` & `threedigrid-2.2.9/threedigrid/admin/lines/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/lines/timeseries_mixin.py` & `threedigrid-2.2.9/threedigrid/admin/lines/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/nodes/exporters.py` & `threedigrid-2.2.9/threedigrid/admin/nodes/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/nodes/models.py` & `threedigrid-2.2.9/threedigrid/admin/nodes/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/nodes/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/nodes/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/nodes/subsets.py` & `threedigrid-2.2.9/threedigrid/admin/nodes/subsets.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/nodes/timeseries_mixin.py` & `threedigrid-2.2.9/threedigrid/admin/nodes/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/prepare_utils.py` & `threedigrid-2.2.9/threedigrid/admin/prepare_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/pumps/models.py` & `threedigrid-2.2.9/threedigrid/admin/pumps/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/pumps/prepare.py` & `threedigrid-2.2.9/threedigrid/admin/pumps/prepare.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/pumps/timeseries_mixin.py` & `threedigrid-2.2.9/threedigrid/admin/pumps/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/rpc_datasource.py` & `threedigrid-2.2.9/threedigrid/admin/rpc_datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/serializers.py` & `threedigrid-2.2.9/threedigrid/admin/serializers.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/structure_controls/exporters.py` & `threedigrid-2.2.9/threedigrid/admin/structure_controls/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/structure_controls/models.py` & `threedigrid-2.2.9/threedigrid/admin/structure_controls/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/admin/utils.py` & `threedigrid-2.2.9/threedigrid/admin/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/geo_utils.py` & `threedigrid-2.2.9/threedigrid/geo_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/management/commands/kick.py` & `threedigrid-2.2.9/threedigrid/management/commands/kick.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/management/help_texts.py` & `threedigrid-2.2.9/threedigrid/management/help_texts.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/numpy_utils.py` & `threedigrid-2.2.9/threedigrid/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/datasource.py` & `threedigrid-2.2.9/threedigrid/orm/base/datasource.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/encoder.py` & `threedigrid-2.2.9/threedigrid/orm/base/encoder.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/exporters.py` & `threedigrid-2.2.9/threedigrid/orm/base/exporters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/fields.py` & `threedigrid-2.2.9/threedigrid/orm/base/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/filters.py` & `threedigrid-2.2.9/threedigrid/orm/base/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/models.py` & `threedigrid-2.2.9/threedigrid/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/options.py` & `threedigrid-2.2.9/threedigrid/orm/base/options.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/timeseries_mixin.py` & `threedigrid-2.2.9/threedigrid/orm/base/timeseries_mixin.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/base/utils.py` & `threedigrid-2.2.9/threedigrid/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/constants.py` & `threedigrid-2.2.9/threedigrid/orm/constants.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/fields.py` & `threedigrid-2.2.9/threedigrid/orm/fields.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/filters.py` & `threedigrid-2.2.9/threedigrid/orm/filters.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid/orm/models.py` & `threedigrid-2.2.9/threedigrid/orm/models.py`

 * *Files identical despite different names*

### Comparing `threedigrid-2.2.8/threedigrid.egg-info/PKG-INFO` & `threedigrid-2.2.9/threedigrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedigrid
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python package for the threedigrid administration
 Home-page: https://github.com/nens/threedigrid
 Author: Lars Claussen
 Author-email: info@nelen-schuurmans.nl
 License: BSD license
 Keywords: threedigrid
 Classifier: Development Status :: 4 - Beta
@@ -194,14 +194,20 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 History
 =======
 
+2.2.9 (2024-05-27)
+------------------
+
+- Move _field_model_dict and its methods from GridH5ResultAdmin to GridH5Admin.
+
+
 2.2.8 (2024-04-25)
 ------------------
 
 - Add `group_by_grid_id` to structure control interface.
 
 
 2.2.7 (2024-04-22)
```

### Comparing `threedigrid-2.2.8/threedigrid.egg-info/SOURCES.txt` & `threedigrid-2.2.9/threedigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

