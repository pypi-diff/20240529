# Comparing `tmp/pynxtools-0.3.1.tar.gz` & `tmp/pynxtools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynxtools-0.3.1.tar", last modified: Tue May 21 08:28:22 2024, max compression
+gzip compressed data, was "pynxtools-0.3.2.tar", last modified: Wed May 29 15:14:16 2024, max compression
```

## Comparing `pynxtools-0.3.1.tar` & `pynxtools-0.3.2.tar`

### file list

```diff
@@ -1,449 +1,452 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.334381 pynxtools-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-21 08:26:48.000000 pynxtools-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-21 08:28:22.334381 pynxtools-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-21 08:26:48.000000 pynxtools-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-21 08:26:48.000000 pynxtools-0.3.1/TROUBLESHOOTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-21 08:26:48.000000 pynxtools-0.3.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.262381 pynxtools-0.3.1/pynxtools/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/_build_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/file_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/hdfdict.py
--rw-r--r--   0 runner    (1001) docker     (127)    32762 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/nexus_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/readers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/base/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/readers/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/example/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_map/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_yml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_yml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/json_yml/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/readers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/dataconverter/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.266381 pynxtools-0.3.1/pynxtools/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/NXDL_VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.274381 pynxtools-0.3.1/pynxtools/definitions/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXarchive.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXarpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50852 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXcanSAS.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXdirecttof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXfluo.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXindirecttof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXiqproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXlauetof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXmonopd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50338 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXmx.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXrefscan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXreftof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXsas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXsastof.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXscan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXspe.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXsqom.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXstxm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtofnpd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtofraw.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtofsingle.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtomo.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtomophase.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXtomoproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxas.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxasproc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxbase.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxeuler.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxkappa.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxlaue.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxnb.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/applications/NXxrot.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.282381 pynxtools-0.3.1/pynxtools/definitions/base_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXaperture.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbeam.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcite.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcollection.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdata.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    40526 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXentry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfilter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXflipper.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXgrating.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXguide.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXlog.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmirror.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXnote.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXobject.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXorientation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXparameters.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpdb.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXprocess.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXreflections.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXroot.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsample.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsensor.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXshape.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXslit.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsource.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXuser.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.322381 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63644 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17894 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20415 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    62967 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    50568 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    24509 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28514 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44594 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    30066 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16465 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35845 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    59085 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    55436 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27543 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.322381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.322381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/dir_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/impatient_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/manual_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/nxclass_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/anchor_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27419 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/nxdl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/xsd_units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/ext/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/ext/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/ext/contrib_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_nxdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/nxdl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/impatient-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/impatient-guide/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.262381 pynxtools-0.3.1/pynxtools/definitions/manual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/manual/source/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5388 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.326381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/epics/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2538 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1706 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.262381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1827 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1979 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1490 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2816 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)      738 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/simple3D.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/verysimple.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51563 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/nxdl.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/nxdlTypes.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/definitions/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10003 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/utils/create_release_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/utils/dev_create_release_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-05-21 08:28:16.000000 pynxtools-0.3.1/pynxtools/definitions/utils/update_copyright_date.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/eln_mapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)      654 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/eln_mapper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5626 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/eln_mapper/eln.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/eln_mapper/eln_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/eln_mapper/scheme_eln.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30703 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pynxtools/nexus/nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 08:28:21.000000 pynxtools-0.3.1/pynxtools/nexus-version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:28:22.330381 pynxtools-0.3.1/pynxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-21 08:28:22.000000 pynxtools-0.3.1/pynxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-21 08:26:48.000000 pynxtools-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:28:22.334381 pynxtools-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.776825 pynxtools-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-29 15:13:01.000000 pynxtools-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-29 15:14:16.776825 pynxtools-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-29 15:13:01.000000 pynxtools-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-29 15:13:01.000000 pynxtools-0.3.2/TROUBLESHOOTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-29 15:13:01.000000 pynxtools-0.3.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.708825 pynxtools-0.3.2/pynxtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/_build_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14354 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/file_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/hdfdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32762 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24424 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/nexus_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/readers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/base/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/readers/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/example/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_map/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_yml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_yml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/json_yml/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/readers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/dataconverter/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.712825 pynxtools-0.3.2/pynxtools/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/NXDL_VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.716825 pynxtools-0.3.2/pynxtools/definitions/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXarchive.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXarpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50852 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXcanSAS.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXdirecttof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXfluo.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXindirecttof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXiqproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXlauetof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXmonopd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50338 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXmx.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXrefscan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXreftof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXsas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXsastof.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXscan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXspe.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXsqom.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXstxm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtofnpd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtofraw.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtofsingle.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtomo.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtomophase.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXtomoproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxas.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxasproc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxbase.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxeuler.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxkappa.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxlaue.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxnb.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/applications/NXxrot.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.728825 pynxtools-0.3.2/pynxtools/definitions/base_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXaperture.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbeam.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcite.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcollection.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15275 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdata.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    40526 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXentry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfilter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXflipper.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXgrating.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9448 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXguide.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXlog.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmirror.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXnote.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXobject.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXorientation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXparameters.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpdb.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXprocess.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXreflections.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXroot.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsample.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8793 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsensor.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXshape.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXslit.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsource.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXuser.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.764825 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63644 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17894 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12274 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20415 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15118 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13931 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62967 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    75728 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18235 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    29134 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19046 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50568 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    24509 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28514 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10719 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17556 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44594 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    30066 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16465 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18132 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35845 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    59085 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12586 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    55436 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15126 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27543 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.764825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/dir_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/impatient_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/manual_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/nxclass_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/anchor_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27419 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/nxdl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/xsd_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/ext/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1211 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/ext/contrib_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.768825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_nxdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6668 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/nxdl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/impatient-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/impatient-guide/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.704825 pynxtools-0.3.2/pynxtools/definitions/manual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5388 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/epics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2538 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1706 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.708825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1827 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      223 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1979 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1490 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2816 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      738 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/simple3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1087 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/verysimple.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51563 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/nxdl.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    17659 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/nxdlTypes.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.772825 pynxtools-0.3.2/pynxtools/definitions/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10003 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/utils/create_release_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/utils/dev_create_release_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-05-29 15:14:11.000000 pynxtools-0.3.2/pynxtools/definitions/utils/update_copyright_date.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.776825 pynxtools-0.3.2/pynxtools/eln_mapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      654 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/eln_mapper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5626 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/eln_mapper/eln.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/eln_mapper/eln_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/eln_mapper/scheme_eln.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.776825 pynxtools-0.3.2/pynxtools/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30703 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/nexus/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 15:14:16.000000 pynxtools-0.3.2/pynxtools/nexus-version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.776825 pynxtools-0.3.2/pynxtools/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pynxtools/testing/nexus_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:14:16.776825 pynxtools-0.3.2/pynxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-29 15:14:16.000000 pynxtools-0.3.2/pynxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-29 15:13:01.000000 pynxtools-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:14:16.776825 pynxtools-0.3.2/setup.cfg
```

### Comparing `pynxtools-0.3.1/LICENSE` & `pynxtools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/PKG-INFO` & `pynxtools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynxtools
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extend NeXus for experiments and characterization in Materials Science and Materials Engineering and serve as a NOMAD parser implementation for NeXus.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -245,24 +245,24 @@
 Requires-Dist: types-pyyaml; extra == "dev"
 Requires-Dist: types-pytz; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: convert
 Requires-Dist: pynxtools[apm,ellips,em,mpes,stm,xps,xrd]; extra == "convert"
+Provides-Extra: mpes
+Requires-Dist: pynxtools-mpes; extra == "mpes"
 Provides-Extra: apm
 Requires-Dist: pynxtools-apm; extra == "apm"
 Provides-Extra: em
 Requires-Dist: pynxtools-em; extra == "em"
-Provides-Extra: mpes
-Requires-Dist: pynxtools-mpes; extra == "mpes"
-Provides-Extra: xps
-Requires-Dist: pynxtools-xps; extra == "xps"
 Provides-Extra: stm
 Requires-Dist: pynxtools-stm; extra == "stm"
+Provides-Extra: xps
+Requires-Dist: pynxtools-xps; extra == "xps"
 Provides-Extra: xrd
 Requires-Dist: pynxtools-xrd; extra == "xrd"
 Provides-Extra: ellips
 Requires-Dist: pynxtools-ellips; extra == "ellips"
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![](https://github.com/FAIRmat-NFDI/pynxtools/actions/workflows/pytest.yml/badge.svg)
```

### Comparing `pynxtools-0.3.1/README.md` & `pynxtools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/TROUBLESHOOTING.md` & `pynxtools-0.3.2/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/dev-requirements.txt` & `pynxtools-0.3.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/__init__.py` & `pynxtools-0.3.2/pynxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/_build_wrapper.py` & `pynxtools-0.3.2/pynxtools/_build_wrapper.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/convert.py` & `pynxtools-0.3.2/pynxtools/dataconverter/convert.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/exceptions.py` & `pynxtools-0.3.2/pynxtools/dataconverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/file_hashing.py` & `pynxtools-0.3.2/pynxtools/dataconverter/file_hashing.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/hdfdict.py` & `pynxtools-0.3.2/pynxtools/dataconverter/hdfdict.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/helpers.py` & `pynxtools-0.3.2/pynxtools/dataconverter/helpers.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/nexus_tree.py` & `pynxtools-0.3.2/pynxtools/dataconverter/nexus_tree.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/readers/base/reader.py` & `pynxtools-0.3.2/pynxtools/dataconverter/readers/base/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/readers/example/reader.py` & `pynxtools-0.3.2/pynxtools/dataconverter/readers/example/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/readers/json_map/reader.py` & `pynxtools-0.3.2/pynxtools/dataconverter/readers/json_map/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/readers/json_yml/reader.py` & `pynxtools-0.3.2/pynxtools/dataconverter/readers/json_yml/reader.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/readers/utils.py` & `pynxtools-0.3.2/pynxtools/dataconverter/readers/utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/template.py` & `pynxtools-0.3.2/pynxtools/dataconverter/template.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/validation.py` & `pynxtools-0.3.2/pynxtools/dataconverter/validation.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/dataconverter/writer.py` & `pynxtools-0.3.2/pynxtools/dataconverter/writer.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXarchive.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXarchive.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXarpes.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXarpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXcanSAS.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXcanSAS.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXdirecttof.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXdirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXfluo.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXfluo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXindirecttof.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXindirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXiqproc.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXiqproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXlauetof.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXlauetof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXmonopd.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXmonopd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXmx.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXmx.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXrefscan.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXrefscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXreftof.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXreftof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXsas.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXsas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXsastof.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXsastof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXscan.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXspe.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXspe.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXsqom.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXsqom.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXstxm.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXstxm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtas.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtofnpd.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtofnpd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtofraw.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtofraw.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtofsingle.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtofsingle.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtomo.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtomo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtomophase.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtomophase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXtomoproc.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXtomoproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxas.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxasproc.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxasproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxbase.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxbase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxeuler.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxeuler.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxkappa.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxkappa.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxlaue.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxlaue.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxlaueplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxnb.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxnb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/applications/NXxrot.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/applications/NXxrot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXaperture.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXaperture.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXattenuator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbeam.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbeam.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbeam_stop.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXbending_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcapillary.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcite.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcite.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcollection.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcollection.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcollimator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcrystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXcylindrical_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdata.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector_group.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdetector_module.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXdisk_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXentry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXenvironment.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXevent_data.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfermi_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfilter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfilter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXflipper.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXflipper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXgeometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXgrating.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXgrating.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXguide.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXguide.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXinsertion_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXinstrument.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXlog.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXlog.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmirror.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmirror.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmoderator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmonitor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXmonochromator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXnote.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXnote.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXobject.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXobject.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXoff_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXorientation.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXorientation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXparameters.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXparameters.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpdb.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpdb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpinhole.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpolarizer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXpositioner.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXprocess.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXprocess.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXreflections.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXreflections.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXroot.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXroot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsample.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsample.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsample_component.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsensor.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsensor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXshape.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXshape.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXslit.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXslit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsource.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsource.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXsubentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXtransformations.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXtranslation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXuser.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXuser.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXvelocity_selector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/base_classes/NXxraylens.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model_ceos.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaberration_model_nion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXactivity.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXactuator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXadc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXamplifier.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXaperture_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_charge_state_analysis.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_composition_space_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_compositionspace_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_hit_finding.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_msr.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_clusterer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_distancer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_intersector_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_nanochem_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_ranger_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_selector_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_spatstat_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_surfacer_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tessellator_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_common.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_tool_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_paraprobe_transcoder_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_ranging.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_reconstruction.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_sim.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXapm_volt_and_bowl.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_path.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_splitter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbeam_transfer_matrix_table.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXbias_spectroscopy.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcalibration.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_alpha_complex.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_cylinder_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_ellipsoid_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_face_list_data_structure.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_geodesic_mesh.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_grid.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_half_edge_data_structure.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_hexahedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_marching_cubes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_parallelogram_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_point_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polygon_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polyhedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_polyline_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_primitive_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_roi_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_sphere_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_tetrahedron_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_triangle_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_triangulated_surface_mesh.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcg_unit_normal_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchamber.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchemical_composition.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXchemical_process.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcircuit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcircuit_board.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcollectioncolumn.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcomponent_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcontainer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcoordinate_system.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcoordinate_system_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcorrector_cs.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcrystal_structure.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_computer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_cpu_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_filter_boolean_mask.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_gpu_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_io_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_io_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_mm_obj.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_mm_sys.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_prng.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_profiling.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcs_profiling_event.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcsg.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdac.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdata_mpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdata_mpes_detector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdeflector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdelocalization.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_function.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_repeated_parameter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_single_parameter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersion_table.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdispersive_material.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXdistortion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXebeam_column.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectron_level.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectronanalyser.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXellipsometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_adf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_conventions.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_conventions_ebsd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_correlation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_ebsd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_eds.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_eels.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_img.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_method.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_msr.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXem_sim.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXenergydispersion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_apm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_apm_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXevent_data_em_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXfabrication.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXfiber.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_edge_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_node_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXgraph_root.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXhistory.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXibeam_column.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXidentifier.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_c_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_r_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_r_set_diff.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXimage_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXinteraction_vol_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXisocontour.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXiv_bias.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXiv_temp.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlab_electro_chemo_mechanical_preparation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlab_sample_mounting.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlens_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlens_opt.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXlockin.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmanipulator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmatch_filter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXmpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_feature_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_ipf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_ipf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_mtex_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_odf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_odf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_pf.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_pf_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_recon.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_score_config.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_score_results.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_snapshot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXms_snapshot_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXopt.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXopt_window.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXoptical_system_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpeak.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXphysical_process.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpid.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpolarizer_opt.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpositioner_sts.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXprocess_mpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXprogram.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpulser_apm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXpump.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXquadric.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXraman.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXreflectron.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXregion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXregistration.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXresolution.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXroi.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXrotation_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsample_component_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXscanbox_em.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsensor_scan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsensor_sts.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXseparator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXserialized.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsimilarity_grouping.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsingle_crystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXslip_system_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsnsevent.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsnshisto.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspatial_filter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspectrum_set.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspin_rotator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXspindispersion.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXstage_lab.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsts.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsubsampling_filter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXsubstance.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXtransmission.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXunit_cell.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXwaveplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxpcs.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxrd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml` & `pynxtools-0.3.2/pynxtools/definitions/contributed_definitions/NXxrd_pan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/__main__.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/__main__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/dir_app.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/dir_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/manual_app.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/manual_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/apps/nxclass_app.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/apps/nxclass_app.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/anchor_list.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/anchor_list.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/nxdl.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/nxdl_index.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/nxdl_index.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/xsd.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/xsd.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/docs/xsd_units.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/docs/xsd_units.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/ext/contrib_ext.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/ext/contrib_ext.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/directories.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/directories.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/globals/nxdl.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/globals/nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/discover.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/discover.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/nxdl/syntax.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/nxdl/syntax.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_docs.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_nxdl.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_nxdl.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/tests/test_nxdl_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/copy.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/copy.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/diff.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/diff.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/github.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/github.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/dev_tools/utils/nxdl_utils.py` & `pynxtools-0.3.2/pynxtools/definitions/dev_tools/utils/nxdl_utils.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/impatient-guide/conf.py` & `pynxtools-0.3.2/pynxtools/definitions/impatient-guide/conf.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/conf.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/conf.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/epics/write_nexus_file.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/epics/write_nexus_file2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/external_example_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/external_example_write/nexusformat/external_example_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/nexusformat/reader_attributes_trail.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/plotting/reader_attributes_trail.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/nexusformat/simple_example_basic_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_basic/simple_example_basic_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_read.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_test/simple_example_test_write.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/nexusformat/simple_example_write1.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write1/simple_example_write1.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/nexusformat/simple_example_write2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/python/simple_example_write2/simple_example_write2.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/simple3D.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/simple3D.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/manual/source/examples/verysimple.py` & `pynxtools-0.3.2/pynxtools/definitions/manual/source/examples/verysimple.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/nxdl.xsd` & `pynxtools-0.3.2/pynxtools/definitions/nxdl.xsd`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/nxdlTypes.xsd` & `pynxtools-0.3.2/pynxtools/definitions/nxdlTypes.xsd`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/utils/create_release_notes.py` & `pynxtools-0.3.2/pynxtools/definitions/utils/create_release_notes.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/definitions/utils/update_copyright_date.py` & `pynxtools-0.3.2/pynxtools/definitions/utils/update_copyright_date.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/eln_mapper/__init__.py` & `pynxtools-0.3.2/pynxtools/eln_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/eln_mapper/eln.py` & `pynxtools-0.3.2/pynxtools/eln_mapper/eln.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/eln_mapper/eln_mapper.py` & `pynxtools-0.3.2/pynxtools/eln_mapper/eln_mapper.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/eln_mapper/scheme_eln.py` & `pynxtools-0.3.2/pynxtools/eln_mapper/scheme_eln.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/nexus/__init__.py` & `pynxtools-0.3.2/pynxtools/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools/nexus/nexus.py` & `pynxtools-0.3.2/pynxtools/nexus/nexus.py`

 * *Files identical despite different names*

### Comparing `pynxtools-0.3.1/pynxtools.egg-info/SOURCES.txt` & `pynxtools-0.3.2/pynxtools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -398,8 +398,10 @@
 pynxtools/definitions/utils/dev_create_release_notes.py
 pynxtools/definitions/utils/update_copyright_date.py
 pynxtools/eln_mapper/__init__.py
 pynxtools/eln_mapper/eln.py
 pynxtools/eln_mapper/eln_mapper.py
 pynxtools/eln_mapper/scheme_eln.py
 pynxtools/nexus/__init__.py
-pynxtools/nexus/nexus.py
+pynxtools/nexus/nexus.py
+pynxtools/testing/__init__.py
+pynxtools/testing/nexus_conversion.py
```

### Comparing `pynxtools-0.3.1/pyproject.toml` & `pynxtools-0.3.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,29 +60,29 @@
     "types-requests",
     "pip-tools",
     "pre-commit",
 ]
 convert = [
     "pynxtools[apm,em,mpes,xps,stm,xrd,ellips]",
 ]
+mpes = [
+    "pynxtools-mpes",
+]
 apm = [
     "pynxtools-apm",
 ]
 em = [
     "pynxtools-em",
 ]
-mpes = [
-    "pynxtools-mpes",
+stm = [
+    "pynxtools-stm",
 ]
 xps = [
     "pynxtools-xps",
 ]
-stm = [
-    "pynxtools-stm",
-]
 xrd = [
     "pynxtools-xrd",
 ]
 ellips = [
     "pynxtools-ellips",
 ]
```

