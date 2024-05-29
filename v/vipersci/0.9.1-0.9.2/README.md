# Comparing `tmp/vipersci-0.9.1.tar.gz` & `tmp/vipersci-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipersci-0.9.1.tar", last modified: Wed Apr 10 22:45:32 2024, max compression
+gzip compressed data, was "vipersci-0.9.2.tar", last modified: Mon Apr 15 17:01:05 2024, max compression
```

## Comparing `vipersci-0.9.1.tar` & `vipersci-0.9.2.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.982906 vipersci-0.9.1/
--rw-r--r--   0 rbeyer     (503) staff       (20)      614 2023-09-25 00:36:59.000000 vipersci-0.9.1/AUTHORS.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)    13230 2024-04-10 21:40:40.000000 vipersci-0.9.1/CHANGELOG.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)     7942 2024-02-07 01:56:52.000000 vipersci-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.9.1/LICENSE
--rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.9.1/MANIFEST.in
--rw-r--r--   0 rbeyer     (503) staff       (20)    17658 2024-04-10 22:45:31.981184 vipersci-0.9.1/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     3295 2023-07-26 18:46:41.000000 vipersci-0.9.1/README.rst
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.576628 vipersci-0.9.1/docs/
--rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.9.1/docs/Makefile
--rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.9.1/docs/authors.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.9.1/docs/changelog.rst
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.9.1/docs/conf.py
--rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.9.1/docs/contributing.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.9.1/docs/index.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.9.1/docs/installation.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.9.1/docs/make.bat
--rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.9.1/docs/modules.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.9.1/docs/readme.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.9.1/docs/usage.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.9.1/docs/vipersci.pds.data.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.9.1/docs/vipersci.pds.data.template.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.9.1/docs/vipersci.pds.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.9.1/docs/vipersci.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.9.1/docs/vipersci.vis.rst
--rw-r--r--   0 rbeyer     (503) staff       (20)      356 2023-05-05 04:04:23.000000 vipersci-0.9.1/pyproject.toml
--rw-r--r--   0 rbeyer     (503) staff       (20)     3070 2024-04-10 22:45:31.992473 vipersci-0.9.1/setup.cfg
--rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.9.1/setup.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.489529 vipersci-0.9.1/src/
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.587010 vipersci-0.9.1/src/vipersci/
--rw-r--r--   0 rbeyer     (503) staff       (20)      130 2024-04-10 21:40:52.000000 vipersci-0.9.1/src/vipersci/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.650926 vipersci-0.9.1/src/vipersci/carto/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.9.1/src/vipersci/carto/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3731 2023-04-11 20:22:14.000000 vipersci-0.9.1/src/vipersci/carto/accrual.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.9.1/src/vipersci/carto/bounds.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    12418 2024-02-07 01:56:52.000000 vipersci-0.9.1/src/vipersci/carto/colorforge.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.9.1/src/vipersci/carto/dice_buffer.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.9.1/src/vipersci/carto/dissolve_dice.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.9.1/src/vipersci/carto/dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6244 2024-04-10 21:24:13.000000 vipersci-0.9.1/src/vipersci/carto/get_position.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    20383 2023-07-26 18:42:09.000000 vipersci-0.9.1/src/vipersci/carto/heatmap.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.9.1/src/vipersci/carto/msolo_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.9.1/src/vipersci/carto/nirvss_simulator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3061 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/carto/nss_modeler.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     7540 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/carto/nss_simulator.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.658564 vipersci-0.9.1/src/vipersci/carto/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:01:47.000000 vipersci-0.9.1/src/vipersci/carto/pds/__init__.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.661489 vipersci-0.9.1/src/vipersci/carto/pds/data/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:03:38.000000 vipersci-0.9.1/src/vipersci/carto/pds/data/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     3733 2024-02-07 01:56:52.000000 vipersci-0.9.1/src/vipersci/carto/traverse_interpolator.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    11429 2024-04-01 23:27:57.000000 vipersci-0.9.1/src/vipersci/carto/tri2gpkg.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.9.1/src/vipersci/msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.9.1/src/vipersci/nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    10898 2023-06-06 20:26:52.000000 vipersci-0.9.1/src/vipersci/nss.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.676445 vipersci-0.9.1/src/vipersci/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)     2035 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5234 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/bundle_install.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2023-10-27 17:08:28.000000 vipersci-0.9.1/src/vipersci/pds/datetime.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.698411 vipersci-0.9.1/src/vipersci/pds/labelmaker/
--rw-r--r--   0 rbeyer     (503) staff       (20)     9858 2024-02-07 01:56:52.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4267 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/bundle.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1755 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/cli.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4747 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/collection.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1975 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/generic.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2290 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/labelmaker/inventory.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)    16452 2024-02-21 21:07:21.000000 vipersci-0.9.1/src/vipersci/pds/pid.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2030 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/pds/xml.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2566 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/util.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.741621 vipersci-0.9.1/src/vipersci/vis/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.1/src/vipersci/vis/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5376 2024-04-10 21:51:15.000000 vipersci-0.9.1/src/vipersci/vis/anaglyph.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2537 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/anom_pixel.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    12800 2024-02-21 03:54:05.000000 vipersci-0.9.1/src/vipersci/vis/create_image.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     7817 2024-04-10 21:24:13.000000 vipersci-0.9.1/src/vipersci/vis/create_mmgis_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11737 2024-01-31 17:28:33.000000 vipersci-0.9.1/src/vipersci/vis/create_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2031 2023-08-09 00:22:12.000000 vipersci-0.9.1/src/vipersci/vis/create_tif.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.794519 vipersci-0.9.1/src/vipersci/vis/db/
--rw-r--r--   0 rbeyer     (503) staff       (20)     1093 2023-07-26 18:42:09.000000 vipersci-0.9.1/src/vipersci/vis/db/__init__.py
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     5674 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/create_vis_dbs.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    29400 2024-04-10 21:24:13.000000 vipersci-0.9.1/src/vipersci/vis/db/image_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    10446 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/image_requests.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1888 2023-08-09 00:22:12.000000 vipersci-0.9.1/src/vipersci/vis/db/image_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2148 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/image_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1877 2023-10-24 18:52:44.000000 vipersci-0.9.1/src/vipersci/vis/db/junc_image_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2045 2023-09-21 04:19:35.000000 vipersci-0.9.1/src/vipersci/vis/db/junc_image_record_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2704 2023-10-24 18:52:44.000000 vipersci-0.9.1/src/vipersci/vis/db/junc_image_req_ldst.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1680 2023-09-23 17:38:22.000000 vipersci-0.9.1/src/vipersci/vis/db/ldst.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3752 2023-10-24 18:52:44.000000 vipersci-0.9.1/src/vipersci/vis/db/light_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9404 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/pano_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3291 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/ptu_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1951 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/db/validators.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3192 2023-08-09 00:22:12.000000 vipersci-0.9.1/src/vipersci/vis/header.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4322 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/image_statistics.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9073 2024-04-10 21:24:13.000000 vipersci-0.9.1/src/vipersci/vis/pano_check.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.813753 vipersci-0.9.1/src/vipersci/vis/pds/
--rw-r--r--   0 rbeyer     (503) staff       (20)     2701 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/pds/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5178 2024-02-07 01:56:52.000000 vipersci-0.9.1/src/vipersci/vis/pds/create_browse.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     7341 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/pds/create_pano_product.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    12865 2024-04-10 21:24:13.000000 vipersci-0.9.1/src/vipersci/vis/pds/create_raw.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.817050 vipersci-0.9.1/src/vipersci/vis/pds/data/
--rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.1/src/vipersci/vis/pds/data/__init__.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5342 2024-01-26 00:56:09.000000 vipersci-0.9.1/src/vipersci/vis/viseer.py
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.977800 vipersci-0.9.1/src/vipersci.egg-info/
--rw-r--r--   0 rbeyer     (503) staff       (20)    17658 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/PKG-INFO
--rw-r--r--   0 rbeyer     (503) staff       (20)     3897 2024-04-10 22:45:31.000000 vipersci-0.9.1/src/vipersci.egg-info/SOURCES.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/dependency_links.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)     1344 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/entry_points.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/not-zip-safe
--rw-r--r--   0 rbeyer     (503) staff       (20)      121 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/requires.txt
--rw-r--r--   0 rbeyer     (503) staff       (20)        9 2024-04-10 22:45:29.000000 vipersci-0.9.1/src/vipersci.egg-info/top_level.txt
-drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-10 22:45:31.974599 vipersci-0.9.1/tests/
--rwxr-xr-x   0 rbeyer     (503) staff       (20)     2301 2023-08-09 00:22:12.000000 vipersci-0.9.1/tests/datetime_sqlite.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6112 2023-09-06 15:17:57.000000 vipersci-0.9.1/tests/test_anaglyph.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.9.1/tests/test_area_bin.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    14596 2024-04-10 21:24:13.000000 vipersci-0.9.1/tests/test_bundle_install.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11820 2023-05-05 04:04:23.000000 vipersci-0.9.1/tests/test_colorforge.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11937 2024-02-21 21:07:21.000000 vipersci-0.9.1/tests/test_create_image.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5015 2024-04-10 21:24:13.000000 vipersci-0.9.1/tests/test_create_mmgis_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     9001 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_create_pano.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8441 2024-02-21 21:07:21.000000 vipersci-0.9.1/tests/test_create_pano_product.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6123 2024-02-21 21:07:21.000000 vipersci-0.9.1/tests/test_create_raw.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1636 2023-08-09 00:22:12.000000 vipersci-0.9.1/tests/test_create_tif.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2848 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_create_vis_dbs.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.9.1/tests/test_datetime.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     8388 2023-07-26 18:42:09.000000 vipersci-0.9.1/tests/test_density_heatmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.9.1/tests/test_dotmap.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.9.1/tests/test_heatmap_helpers.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    22535 2024-04-10 21:24:13.000000 vipersci-0.9.1/tests/test_image_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3835 2023-09-23 17:38:22.000000 vipersci-0.9.1/tests/test_image_requests.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2602 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_image_statistics.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1300 2023-08-09 00:22:12.000000 vipersci-0.9.1/tests/test_image_stats.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1192 2023-09-21 04:19:35.000000 vipersci-0.9.1/tests/test_image_tags.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    11202 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     5619 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker_bundle.py
--rw-r--r--   0 rbeyer     (503) staff       (20)      571 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker_cli.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     6289 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker_collection.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1588 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker_generic.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1549 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_labelmaker_inventory.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1773 2023-10-24 18:52:44.000000 vipersci-0.9.1/tests/test_light_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.9.1/tests/test_msolo.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.9.1/tests/test_msolo_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.9.1/tests/test_nirvss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.9.1/tests/test_nirvss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3737 2022-11-01 14:54:30.000000 vipersci-0.9.1/tests/test_nss.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.9.1/tests/test_nss_modeler.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.9.1/tests/test_nss_simulator.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     4591 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_pano_check.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     3807 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_pano_records.py
--rw-r--r--   0 rbeyer     (503) staff       (20)    13805 2024-02-21 21:07:21.000000 vipersci-0.9.1/tests/test_pid.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     1589 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_util.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2333 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_validators.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2588 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_vis_pds.py
--rw-r--r--   0 rbeyer     (503) staff       (20)     2826 2024-01-26 00:56:09.000000 vipersci-0.9.1/tests/test_xml.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.073245 vipersci-0.9.2/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      614 2023-09-25 00:36:59.000000 vipersci-0.9.2/AUTHORS.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)    13502 2024-04-15 16:33:52.000000 vipersci-0.9.2/CHANGELOG.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7942 2024-02-07 01:56:52.000000 vipersci-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11357 2021-10-25 21:26:36.000000 vipersci-0.9.2/LICENSE
+-rw-r--r--   0 rbeyer     (503) staff       (20)      264 2021-10-25 21:34:05.000000 vipersci-0.9.2/MANIFEST.in
+-rw-r--r--   0 rbeyer     (503) staff       (20)    17930 2024-04-15 17:01:05.072977 vipersci-0.9.2/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3295 2023-07-26 18:46:41.000000 vipersci-0.9.2/README.rst
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.966338 vipersci-0.9.2/docs/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      609 2021-10-25 21:48:39.000000 vipersci-0.9.2/docs/Makefile
+-rw-r--r--   0 rbeyer     (503) staff       (20)       28 2021-03-28 21:36:13.000000 vipersci-0.9.2/docs/authors.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       30 2022-10-06 00:17:46.000000 vipersci-0.9.2/docs/changelog.rst
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     4895 2022-11-01 14:54:30.000000 vipersci-0.9.2/docs/conf.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)       33 2021-03-28 21:36:13.000000 vipersci-0.9.2/docs/contributing.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      307 2022-10-06 00:17:46.000000 vipersci-0.9.2/docs/index.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      716 2022-10-06 00:17:46.000000 vipersci-0.9.2/docs/installation.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      770 2021-10-25 21:48:14.000000 vipersci-0.9.2/docs/make.bat
+-rw-r--r--   0 rbeyer     (503) staff       (20)       61 2022-10-05 23:23:34.000000 vipersci-0.9.2/docs/modules.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       27 2021-03-28 21:36:13.000000 vipersci-0.9.2/docs/readme.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)       71 2021-10-25 21:48:27.000000 vipersci-0.9.2/docs/usage.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      260 2022-10-05 23:15:23.000000 vipersci-0.9.2/docs/vipersci.pds.data.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      201 2022-10-05 23:15:23.000000 vipersci-0.9.2/docs/vipersci.pds.data.template.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      927 2022-10-05 23:15:23.000000 vipersci-0.9.2/docs/vipersci.pds.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      511 2022-10-05 23:23:34.000000 vipersci-0.9.2/docs/vipersci.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      465 2022-10-05 23:15:23.000000 vipersci-0.9.2/docs/vipersci.vis.rst
+-rw-r--r--   0 rbeyer     (503) staff       (20)      356 2023-05-05 04:04:23.000000 vipersci-0.9.2/pyproject.toml
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3070 2024-04-15 17:01:05.074211 vipersci-0.9.2/setup.cfg
+-rw-r--r--   0 rbeyer     (503) staff       (20)       86 2022-11-08 00:15:45.000000 vipersci-0.9.2/setup.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.941303 vipersci-0.9.2/src/
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.970443 vipersci-0.9.2/src/vipersci/
+-rw-r--r--   0 rbeyer     (503) staff       (20)      130 2024-04-15 16:33:52.000000 vipersci-0.9.2/src/vipersci/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.997003 vipersci-0.9.2/src/vipersci/carto/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-11-14 18:58:15.000000 vipersci-0.9.2/src/vipersci/carto/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3731 2023-04-11 20:22:14.000000 vipersci-0.9.2/src/vipersci/carto/accrual.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3454 2023-03-01 16:59:24.000000 vipersci-0.9.2/src/vipersci/carto/bounds.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    12418 2024-02-07 01:56:52.000000 vipersci-0.9.2/src/vipersci/carto/colorforge.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3718 2022-11-10 16:51:53.000000 vipersci-0.9.2/src/vipersci/carto/dice_buffer.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2325 2022-11-10 16:51:53.000000 vipersci-0.9.2/src/vipersci/carto/dissolve_dice.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3463 2023-03-01 16:59:24.000000 vipersci-0.9.2/src/vipersci/carto/dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6244 2024-04-10 21:24:13.000000 vipersci-0.9.2/src/vipersci/carto/get_position.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    20383 2023-07-26 18:42:09.000000 vipersci-0.9.2/src/vipersci/carto/heatmap.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5959 2022-11-10 16:51:53.000000 vipersci-0.9.2/src/vipersci/carto/msolo_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     6644 2022-11-10 16:51:53.000000 vipersci-0.9.2/src/vipersci/carto/nirvss_simulator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3061 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/carto/nss_modeler.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     7540 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/carto/nss_simulator.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.998036 vipersci-0.9.2/src/vipersci/carto/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:01:47.000000 vipersci-0.9.2/src/vipersci/carto/pds/__init__.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:04.998784 vipersci-0.9.2/src/vipersci/carto/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2023-04-23 00:03:38.000000 vipersci-0.9.2/src/vipersci/carto/pds/data/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     3733 2024-02-07 01:56:52.000000 vipersci-0.9.2/src/vipersci/carto/traverse_interpolator.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    11429 2024-04-01 23:27:57.000000 vipersci-0.9.2/src/vipersci/carto/tri2gpkg.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1434 2022-11-01 14:54:30.000000 vipersci-0.9.2/src/vipersci/msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1382 2022-11-01 14:54:30.000000 vipersci-0.9.2/src/vipersci/nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11369 2024-04-15 16:33:52.000000 vipersci-0.9.2/src/vipersci/nss.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.004455 vipersci-0.9.2/src/vipersci/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2035 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5234 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/bundle_install.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2901 2023-10-27 17:08:28.000000 vipersci-0.9.2/src/vipersci/pds/datetime.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.011018 vipersci-0.9.2/src/vipersci/pds/labelmaker/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9858 2024-02-07 01:56:52.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4267 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/bundle.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1755 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/cli.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4747 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/collection.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1975 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/generic.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2290 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/labelmaker/inventory.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)    16452 2024-02-21 21:07:21.000000 vipersci-0.9.2/src/vipersci/pds/pid.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2030 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/pds/xml.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2566 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/util.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.022673 vipersci-0.9.2/src/vipersci/vis/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.2/src/vipersci/vis/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5376 2024-04-10 21:51:15.000000 vipersci-0.9.2/src/vipersci/vis/anaglyph.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2537 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/anom_pixel.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    12800 2024-02-21 03:54:05.000000 vipersci-0.9.2/src/vipersci/vis/create_image.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7817 2024-04-10 21:24:13.000000 vipersci-0.9.2/src/vipersci/vis/create_mmgis_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11737 2024-01-31 17:28:33.000000 vipersci-0.9.2/src/vipersci/vis/create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2031 2023-08-09 00:22:12.000000 vipersci-0.9.2/src/vipersci/vis/create_tif.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.034335 vipersci-0.9.2/src/vipersci/vis/db/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1093 2023-07-26 18:42:09.000000 vipersci-0.9.2/src/vipersci/vis/db/__init__.py
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     5674 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/create_vis_dbs.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    29400 2024-04-10 21:24:13.000000 vipersci-0.9.2/src/vipersci/vis/db/image_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    10446 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/image_requests.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1888 2023-08-09 00:22:12.000000 vipersci-0.9.2/src/vipersci/vis/db/image_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2148 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/image_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1877 2023-10-24 18:52:44.000000 vipersci-0.9.2/src/vipersci/vis/db/junc_image_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2045 2023-09-21 04:19:35.000000 vipersci-0.9.2/src/vipersci/vis/db/junc_image_record_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2704 2023-10-24 18:52:44.000000 vipersci-0.9.2/src/vipersci/vis/db/junc_image_req_ldst.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1680 2023-09-23 17:38:22.000000 vipersci-0.9.2/src/vipersci/vis/db/ldst.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3752 2023-10-24 18:52:44.000000 vipersci-0.9.2/src/vipersci/vis/db/light_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9404 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/pano_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3291 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/ptu_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1951 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/db/validators.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3192 2023-08-09 00:22:12.000000 vipersci-0.9.2/src/vipersci/vis/header.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4322 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/image_statistics.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9073 2024-04-10 21:24:13.000000 vipersci-0.9.2/src/vipersci/vis/pano_check.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.036972 vipersci-0.9.2/src/vipersci/vis/pds/
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2701 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/pds/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5178 2024-02-07 01:56:52.000000 vipersci-0.9.2/src/vipersci/vis/pds/create_browse.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     7341 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/pds/create_pano_product.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    12865 2024-04-10 21:24:13.000000 vipersci-0.9.2/src/vipersci/vis/pds/create_raw.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.037716 vipersci-0.9.2/src/vipersci/vis/pds/data/
+-rw-r--r--   0 rbeyer     (503) staff       (20)        0 2022-10-24 16:37:05.000000 vipersci-0.9.2/src/vipersci/vis/pds/data/__init__.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5342 2024-01-26 00:56:09.000000 vipersci-0.9.2/src/vipersci/vis/viseer.py
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.072221 vipersci-0.9.2/src/vipersci.egg-info/
+-rw-r--r--   0 rbeyer     (503) staff       (20)    17930 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/PKG-INFO
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3897 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/SOURCES.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/dependency_links.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1344 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/entry_points.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        1 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/not-zip-safe
+-rw-r--r--   0 rbeyer     (503) staff       (20)      121 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/requires.txt
+-rw-r--r--   0 rbeyer     (503) staff       (20)        9 2024-04-15 17:01:04.000000 vipersci-0.9.2/src/vipersci.egg-info/top_level.txt
+drwxr-xr-x   0 rbeyer     (503) staff       (20)        0 2024-04-15 17:01:05.071403 vipersci-0.9.2/tests/
+-rwxr-xr-x   0 rbeyer     (503) staff       (20)     2301 2023-08-09 00:22:12.000000 vipersci-0.9.2/tests/datetime_sqlite.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6112 2023-09-06 15:17:57.000000 vipersci-0.9.2/tests/test_anaglyph.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1682 2022-11-30 20:55:10.000000 vipersci-0.9.2/tests/test_area_bin.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    14596 2024-04-10 21:24:13.000000 vipersci-0.9.2/tests/test_bundle_install.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11820 2023-05-05 04:04:23.000000 vipersci-0.9.2/tests/test_colorforge.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11937 2024-02-21 21:07:21.000000 vipersci-0.9.2/tests/test_create_image.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5015 2024-04-10 21:24:13.000000 vipersci-0.9.2/tests/test_create_mmgis_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     9001 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_create_pano.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8441 2024-02-21 21:07:21.000000 vipersci-0.9.2/tests/test_create_pano_product.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6123 2024-02-21 21:07:21.000000 vipersci-0.9.2/tests/test_create_raw.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1636 2023-08-09 00:22:12.000000 vipersci-0.9.2/tests/test_create_tif.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2848 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_create_vis_dbs.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1644 2022-11-30 20:55:10.000000 vipersci-0.9.2/tests/test_datetime.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     8388 2023-07-26 18:42:09.000000 vipersci-0.9.2/tests/test_density_heatmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3895 2023-02-24 03:28:58.000000 vipersci-0.9.2/tests/test_dotmap.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2526 2023-02-24 03:28:58.000000 vipersci-0.9.2/tests/test_heatmap_helpers.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    22535 2024-04-13 18:37:20.000000 vipersci-0.9.2/tests/test_image_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3835 2023-09-23 17:38:22.000000 vipersci-0.9.2/tests/test_image_requests.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2602 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_image_statistics.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1300 2023-08-09 00:22:12.000000 vipersci-0.9.2/tests/test_image_stats.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1192 2023-09-21 04:19:35.000000 vipersci-0.9.2/tests/test_image_tags.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    11202 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     5619 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker_bundle.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)      571 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker_cli.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6289 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker_collection.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1588 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker_generic.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1549 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_labelmaker_inventory.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1773 2023-10-24 18:52:44.000000 vipersci-0.9.2/tests/test_light_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1646 2022-11-01 14:54:30.000000 vipersci-0.9.2/tests/test_msolo.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2278 2023-02-24 03:28:58.000000 vipersci-0.9.2/tests/test_msolo_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1649 2022-11-01 14:54:30.000000 vipersci-0.9.2/tests/test_nirvss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2387 2023-02-24 03:28:58.000000 vipersci-0.9.2/tests/test_nirvss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     6183 2024-04-15 16:33:52.000000 vipersci-0.9.2/tests/test_nss.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1782 2022-11-30 20:55:10.000000 vipersci-0.9.2/tests/test_nss_modeler.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2727 2022-11-30 20:55:10.000000 vipersci-0.9.2/tests/test_nss_simulator.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     4591 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_pano_check.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     3807 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_pano_records.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)    13805 2024-02-21 21:07:21.000000 vipersci-0.9.2/tests/test_pid.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     1589 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_util.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2333 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_validators.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2588 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_vis_pds.py
+-rw-r--r--   0 rbeyer     (503) staff       (20)     2826 2024-01-26 00:56:09.000000 vipersci-0.9.2/tests/test_xml.py
```

### Comparing `vipersci-0.9.1/AUTHORS.rst` & `vipersci-0.9.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/CHANGELOG.rst` & `vipersci-0.9.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,23 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.2 (2024-04-15)
+------------------
+
+Fixed
+^^^^^
+- nss.py - The DataModeler class would incorrectly always return a weh_arr of all-NaN
+  values.  This bug has been fixed, and additional safeguards and error reporting have
+  been placed in the class, and tests written.
+
 0.9.1 (2024-04-10)
 ------------------
 
 Fixed
 ^^^^^
 - anaglyph.py - when used with scikit-image versions greater than 0.21 changed the
   argument signature for phase_cross_correlation().  Fixed call, and should now
```

### Comparing `vipersci-0.9.1/CONTRIBUTING.rst` & `vipersci-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/LICENSE` & `vipersci-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/PKG-INFO` & `vipersci-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.9.1
+Version: 0.9.2
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -150,14 +150,23 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.2 (2024-04-15)
+------------------
+
+Fixed
+^^^^^
+- nss.py - The DataModeler class would incorrectly always return a weh_arr of all-NaN
+  values.  This bug has been fixed, and additional safeguards and error reporting have
+  been placed in the class, and tests written.
+
 0.9.1 (2024-04-10)
 ------------------
 
 Fixed
 ^^^^^
 - anaglyph.py - when used with scikit-image versions greater than 0.21 changed the
   argument signature for phase_cross_correlation().  Fixed call, and should now
```

### Comparing `vipersci-0.9.1/README.rst` & `vipersci-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/docs/Makefile` & `vipersci-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/docs/conf.py` & `vipersci-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/docs/installation.rst` & `vipersci-0.9.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/docs/make.bat` & `vipersci-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/docs/vipersci.pds.rst` & `vipersci-0.9.2/docs/vipersci.pds.rst`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/setup.cfg` & `vipersci-0.9.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.1
+current_version = 0.9.2
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `vipersci-0.9.1/src/vipersci/carto/accrual.py` & `vipersci-0.9.2/src/vipersci/carto/accrual.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/bounds.py` & `vipersci-0.9.2/src/vipersci/carto/bounds.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/colorforge.py` & `vipersci-0.9.2/src/vipersci/carto/colorforge.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/dice_buffer.py` & `vipersci-0.9.2/src/vipersci/carto/dice_buffer.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/dissolve_dice.py` & `vipersci-0.9.2/src/vipersci/carto/dissolve_dice.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/dotmap.py` & `vipersci-0.9.2/src/vipersci/carto/dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/get_position.py` & `vipersci-0.9.2/src/vipersci/carto/get_position.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/heatmap.py` & `vipersci-0.9.2/src/vipersci/carto/heatmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/msolo_simulator.py` & `vipersci-0.9.2/src/vipersci/carto/msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/nirvss_simulator.py` & `vipersci-0.9.2/src/vipersci/carto/nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/nss_modeler.py` & `vipersci-0.9.2/src/vipersci/carto/nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/nss_simulator.py` & `vipersci-0.9.2/src/vipersci/carto/nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/traverse_interpolator.py` & `vipersci-0.9.2/src/vipersci/carto/traverse_interpolator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/carto/tri2gpkg.py` & `vipersci-0.9.2/src/vipersci/carto/tri2gpkg.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/msolo.py` & `vipersci-0.9.2/src/vipersci/msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/nirvss.py` & `vipersci-0.9.2/src/vipersci/nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/nss.py` & `vipersci-0.9.2/src/vipersci/nss.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,28 +153,40 @@
         :returns: A three-tuple of values or np.arrays.  If *det1* and *det2* are
         singular elements, then a three-tuple is returned of the BD, WEH, and UWEH
         values at that location.  If *det1* and *det2* contain more than
         one value each, then the returned three-tuple will be a numpy array
         of BD values, a numpy array of WEH values, and a numpy array of UWEH values.
         """
         is_arraylike = True if hasattr(det1, "__iter__") else False
-        d1 = det1 if isinstance(det1, np.ma.MaskedArray) else np.ma.array(det1)
-        d2 = det2 if isinstance(det2, np.ma.MaskedArray) else np.ma.array(det2)
 
-        bd_arr = np.full_like(d1, self.fill_value, dtype=np.double)
-        weh_arr = np.full_like(d2, self.fill_value, dtype=np.double)
+        if isinstance(det1, np.ma.MaskedArray) or isinstance(det2, np.ma.MaskedArray):
+            d1 = det1 if isinstance(det1, np.ma.MaskedArray) else np.ma.array(det1)
+            d2 = det2 if isinstance(det2, np.ma.MaskedArray) else np.ma.array(det2)
+
+            if not np.array_equal(d1.mask, d2.mask):
+                raise ValueError(
+                    "The masks for the two masked arrays are not symmetric."
+                )
+
+            bd_arr = np.full_like(det1, self.fill_value, dtype=np.double)
+            weh_arr = np.full_like(det2, self.fill_value, dtype=np.double)
+
+            stacked = np.column_stack((d1.compressed(), d2.compressed()))
+            bd_arr[~d1.mask] = self.det1_model(stacked)
+            weh_arr[~d1.mask] = self.det2_model(stacked)
+            d1_for_uweh = d1.filled(self.fill_value)
+
+        else:
+            stacked = np.column_stack((det1, det2))
+            bd_arr = self.det1_model(stacked)
+            weh_arr = self.det2_model(stacked)
+            d1_for_uweh = det1
 
-        bd_arr[~d1.mask] = self.det1_model(
-            np.column_stack((d1.compressed(), d2.compressed()))
-        )
-        weh_arr[~d1.mask] = self.det2_model(
-            np.column_stack((d2.compressed(), d2.compressed()))
-        )
         uweh_arr = uniform_weh(
-            d1.filled(self.fill_value), fill_value=self.fill_value, bounds_error=False
+            d1_for_uweh, fill_value=self.fill_value, bounds_error=False
         )
 
         if not is_arraylike:
             return bd_arr.item(), weh_arr.item(), uweh_arr.item()
 
         return bd_arr, weh_arr, uweh_arr
```

### Comparing `vipersci-0.9.1/src/vipersci/pds/__init__.py` & `vipersci-0.9.2/src/vipersci/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/bundle_install.py` & `vipersci-0.9.2/src/vipersci/pds/bundle_install.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/datetime.py` & `vipersci-0.9.2/src/vipersci/pds/datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/__init__.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/bundle.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/bundle.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/cli.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/cli.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/collection.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/collection.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/generic.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/generic.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/labelmaker/inventory.py` & `vipersci-0.9.2/src/vipersci/pds/labelmaker/inventory.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/pid.py` & `vipersci-0.9.2/src/vipersci/pds/pid.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/pds/xml.py` & `vipersci-0.9.2/src/vipersci/pds/xml.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/util.py` & `vipersci-0.9.2/src/vipersci/util.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/anaglyph.py` & `vipersci-0.9.2/src/vipersci/vis/anaglyph.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/anom_pixel.py` & `vipersci-0.9.2/src/vipersci/vis/anom_pixel.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/create_image.py` & `vipersci-0.9.2/src/vipersci/vis/create_image.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/create_mmgis_pano.py` & `vipersci-0.9.2/src/vipersci/vis/create_mmgis_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/create_pano.py` & `vipersci-0.9.2/src/vipersci/vis/create_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/create_tif.py` & `vipersci-0.9.2/src/vipersci/vis/create_tif.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/__init__.py` & `vipersci-0.9.2/src/vipersci/vis/db/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/create_vis_dbs.py` & `vipersci-0.9.2/src/vipersci/vis/db/create_vis_dbs.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/image_records.py` & `vipersci-0.9.2/src/vipersci/vis/db/image_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/image_requests.py` & `vipersci-0.9.2/src/vipersci/vis/db/image_requests.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/image_stats.py` & `vipersci-0.9.2/src/vipersci/vis/db/image_stats.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/image_tags.py` & `vipersci-0.9.2/src/vipersci/vis/db/image_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/junc_image_pano.py` & `vipersci-0.9.2/src/vipersci/vis/db/junc_image_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/junc_image_record_tags.py` & `vipersci-0.9.2/src/vipersci/vis/db/junc_image_record_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/junc_image_req_ldst.py` & `vipersci-0.9.2/src/vipersci/vis/db/junc_image_req_ldst.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/ldst.py` & `vipersci-0.9.2/src/vipersci/vis/db/ldst.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/light_records.py` & `vipersci-0.9.2/src/vipersci/vis/db/light_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/pano_records.py` & `vipersci-0.9.2/src/vipersci/vis/db/pano_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/ptu_records.py` & `vipersci-0.9.2/src/vipersci/vis/db/ptu_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/db/validators.py` & `vipersci-0.9.2/src/vipersci/vis/db/validators.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/header.py` & `vipersci-0.9.2/src/vipersci/vis/header.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/image_statistics.py` & `vipersci-0.9.2/src/vipersci/vis/image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/pano_check.py` & `vipersci-0.9.2/src/vipersci/vis/pano_check.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/pds/__init__.py` & `vipersci-0.9.2/src/vipersci/vis/pds/__init__.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/pds/create_browse.py` & `vipersci-0.9.2/src/vipersci/vis/pds/create_browse.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/pds/create_pano_product.py` & `vipersci-0.9.2/src/vipersci/vis/pds/create_pano_product.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/pds/create_raw.py` & `vipersci-0.9.2/src/vipersci/vis/pds/create_raw.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci/vis/viseer.py` & `vipersci-0.9.2/src/vipersci/vis/viseer.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci.egg-info/PKG-INFO` & `vipersci-0.9.2/src/vipersci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vipersci
-Version: 0.9.1
+Version: 0.9.2
 Summary: The VIPER Science package is software to support the activities of the Volatiles Investigating Polar Exploration Rover (VIPER) Science Team.
 Home-page: https://github.com/NeoGeographyToolkit/vipersci
 Author: vipersci Developers
 Author-email: Ross.A.Beyer@nasa.gov
 License: Apache 2
 Keywords: VIPER
 Classifier: Programming Language :: Python :: 3.7
@@ -150,14 +150,23 @@
 underlined with dashes under Unreleased_ with the version number
 and the release date, in year-month-day format (see examples below).
 
 
 Unreleased
 ----------
 
+0.9.2 (2024-04-15)
+------------------
+
+Fixed
+^^^^^
+- nss.py - The DataModeler class would incorrectly always return a weh_arr of all-NaN
+  values.  This bug has been fixed, and additional safeguards and error reporting have
+  been placed in the class, and tests written.
+
 0.9.1 (2024-04-10)
 ------------------
 
 Fixed
 ^^^^^
 - anaglyph.py - when used with scikit-image versions greater than 0.21 changed the
   argument signature for phase_cross_correlation().  Fixed call, and should now
```

### Comparing `vipersci-0.9.1/src/vipersci.egg-info/SOURCES.txt` & `vipersci-0.9.2/src/vipersci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/src/vipersci.egg-info/entry_points.txt` & `vipersci-0.9.2/src/vipersci.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/datetime_sqlite.py` & `vipersci-0.9.2/tests/datetime_sqlite.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_anaglyph.py` & `vipersci-0.9.2/tests/test_anaglyph.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_area_bin.py` & `vipersci-0.9.2/tests/test_area_bin.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_bundle_install.py` & `vipersci-0.9.2/tests/test_bundle_install.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_colorforge.py` & `vipersci-0.9.2/tests/test_colorforge.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_image.py` & `vipersci-0.9.2/tests/test_create_image.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_mmgis_pano.py` & `vipersci-0.9.2/tests/test_create_mmgis_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_pano.py` & `vipersci-0.9.2/tests/test_create_pano.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_pano_product.py` & `vipersci-0.9.2/tests/test_create_pano_product.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_raw.py` & `vipersci-0.9.2/tests/test_create_raw.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_tif.py` & `vipersci-0.9.2/tests/test_create_tif.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_create_vis_dbs.py` & `vipersci-0.9.2/tests/test_create_vis_dbs.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_datetime.py` & `vipersci-0.9.2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_density_heatmap.py` & `vipersci-0.9.2/tests/test_density_heatmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_dotmap.py` & `vipersci-0.9.2/tests/test_dotmap.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_heatmap_helpers.py` & `vipersci-0.9.2/tests/test_heatmap_helpers.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_image_records.py` & `vipersci-0.9.2/tests/test_image_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_image_requests.py` & `vipersci-0.9.2/tests/test_image_requests.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_image_statistics.py` & `vipersci-0.9.2/tests/test_image_statistics.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_image_stats.py` & `vipersci-0.9.2/tests/test_image_stats.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_image_tags.py` & `vipersci-0.9.2/tests/test_image_tags.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker.py` & `vipersci-0.9.2/tests/test_labelmaker.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker_bundle.py` & `vipersci-0.9.2/tests/test_labelmaker_bundle.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker_cli.py` & `vipersci-0.9.2/tests/test_labelmaker_cli.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker_collection.py` & `vipersci-0.9.2/tests/test_labelmaker_collection.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker_generic.py` & `vipersci-0.9.2/tests/test_labelmaker_generic.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_labelmaker_inventory.py` & `vipersci-0.9.2/tests/test_labelmaker_inventory.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_light_records.py` & `vipersci-0.9.2/tests/test_light_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_msolo.py` & `vipersci-0.9.2/tests/test_msolo.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_msolo_simulator.py` & `vipersci-0.9.2/tests/test_msolo_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_nirvss.py` & `vipersci-0.9.2/tests/test_nirvss.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_nirvss_simulator.py` & `vipersci-0.9.2/tests/test_nirvss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_nss_modeler.py` & `vipersci-0.9.2/tests/test_nss_modeler.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_nss_simulator.py` & `vipersci-0.9.2/tests/test_nss_simulator.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_pano_check.py` & `vipersci-0.9.2/tests/test_pano_check.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_pano_records.py` & `vipersci-0.9.2/tests/test_pano_records.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_pid.py` & `vipersci-0.9.2/tests/test_pid.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_util.py` & `vipersci-0.9.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_validators.py` & `vipersci-0.9.2/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_vis_pds.py` & `vipersci-0.9.2/tests/test_vis_pds.py`

 * *Files identical despite different names*

### Comparing `vipersci-0.9.1/tests/test_xml.py` & `vipersci-0.9.2/tests/test_xml.py`

 * *Files identical despite different names*

