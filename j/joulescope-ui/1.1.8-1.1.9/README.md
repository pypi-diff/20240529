# Comparing `tmp/joulescope_ui-1.1.8.tar.gz` & `tmp/joulescope_ui-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope_ui-1.1.8.tar", last modified: Mon May 13 15:39:21 2024, max compression
+gzip compressed data, was "joulescope_ui-1.1.9.tar", last modified: Tue May 21 17:24:44 2024, max compression
```

## Comparing `joulescope_ui-1.1.8.tar` & `joulescope_ui-1.1.9.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-13 15:39:20.000000 joulescope_ui-1.1.8/joulescope.iss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.684787 joulescope_ui-1.1.8/joulescope_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    53673 2024-05-13 15:39:10.000000 joulescope_ui-1.1.8/joulescope_ui/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-13 15:39:10.000000 joulescope_ui-1.1.8/joulescope_ui/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/dev_signal_buffer_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/device_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js110.py
--rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/devices/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/devices/test/test_device_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/disk_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/entry_points/zip_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/error_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/error_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/expanding_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/filename_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/OFL.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui/fonts.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/getting_started.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/help_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/intel_graphics_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/jls_v2_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/json_plus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.688787 joulescope_ui-1.1.8/joulescope_ui/locale/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81702 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   112244 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71550 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102499 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    99351 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   130324 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   102570 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    73100 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104062 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    72339 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   103281 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.692787 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    75547 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105590 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)    68383 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/joulescope_ui.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70320 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)   100452 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.664788 joulescope_ui-1.1.8/joulescope_ui/locale/zh/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    61353 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
--rw-r--r--   0 runner    (1001) docker     (127)    91276 2024-05-13 15:39:11.000000 joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    42189 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/mem_leak_debugger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/index.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.696787 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p2/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/plugins/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/process_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    66497 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_callable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/pubsub_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.700787 joulescope_ui-1.1.8/joulescope_ui/range_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/cdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/max_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/plugin_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/range_tools/usb_inrush.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.700787 joulescope_ui-1.1.8/joulescope_ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.svg
--rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.704787 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/logo-large.png
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources/zoom.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-13 15:39:20.000000 joulescope_ui-1.1.8/joulescope_ui/resources.rcc
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/safe_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/shift_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/source_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.704787 joulescope_ui-1.1.8/joulescope_ui/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/fonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.708787 joulescope_ui-1.1.8/joulescope_ui/styles/js1/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/arrow_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_end.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_end_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_more.svg
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/branch_vline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/detach.svg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/hmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/hsepartoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/radio_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/radio_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.html
--rw-r--r--   0 runner    (1001) docker     (127)    19555 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/tabs_menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/transparent.svg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/vmovetoolbar.svg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/js1/vsepartoolbars.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.712787 joulescope_ui-1.1.8/joulescope_ui/styles/system/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/index.json
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/style.html
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.712787 joulescope_ui-1.1.8/joulescope_ui/styles/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_color_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/styles/test/test_parameter_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/anno1.anno.jls
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_annotation_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_disk_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_range_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_software_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_source_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/test/test_versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 15:39:12.000000 joulescope_ui-1.1.8/joulescope_ui/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/ui_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/versioned_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widget_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/accumulator_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.716787 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/clock/clock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.720787 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/log_view_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/profile_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/publish_spy_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.720787 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/current_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_control_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_info_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_update_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/active_checked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/doc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/info.svg
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/open.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/target_power_off.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/double_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/draggable_list_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/example/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/example_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/example/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/flyout_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/hamburger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.724787 joulescope_ui-1.1.8/joulescope_ui/widgets/help/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/help/help_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/jls_info_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/current_offset.png
--rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/voltage_offset.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/memory_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/notes/notes_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.728787 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/record_status_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/report_issue_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/settings_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/settings/unique_strings_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.732787 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/sidebar_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/device.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/memory.svg
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/misc.svg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/pause.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/play.svg
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/record.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/settings.svg
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/target_power.svg
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/disk_full_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/condition_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/active.svg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/continuous.svg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/inactive.svg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/searching.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/single.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/style.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.736787 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/trigger_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/value/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/value/value_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.740787 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/add.svg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/delete.svg
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/move.svg
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/view_manager_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/annotations.md
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/interval_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/line_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/quantities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/index.json
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_add1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_add2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/marker_clear.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/pin_left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/pin_right.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style.qss
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style_defines.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/trace.svg
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_in.svg
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_out.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/text_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_source_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)   174585 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/y_range_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/joulescope_ui/zip_inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:21.744787 joulescope_ui-1.1.8/joulescope_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:39:21.000000 joulescope_ui-1.1.8/joulescope_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 15:39:21.748786 joulescope_ui-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-13 15:38:44.000000 joulescope_ui-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.726230 joulescope_ui-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    54048 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-21 17:24:44.726230 joulescope_ui-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-21 17:24:42.000000 joulescope_ui-1.1.9/joulescope.iss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.662229 joulescope_ui-1.1.9/joulescope_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    54048 2024-05-21 17:24:20.000000 joulescope_ui-1.1.9/joulescope_ui/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-21 17:24:20.000000 joulescope_ui-1.1.9/joulescope_ui/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/dev_signal_buffer_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.662229 joulescope_ui-1.1.9/joulescope_ui/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/device_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.662229 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31966 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.662229 joulescope_ui-1.1.9/joulescope_ui/devices/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/devices/test/test_device_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/disk_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/entry_points/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/entry_points/zip_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/error_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/error_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/expanding_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/filename_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.634229 joulescope_ui-1.1.9/joulescope_ui/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/fonts/DSEG14-Modern/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/fonts/Hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/fonts/Hack/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/fonts/Lato/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/fonts/SourceCodePro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/fonts/SourceCodePro/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/fonts/SourceSerifPro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/fonts/SourceSerifPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  3102116 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui/fonts.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/help_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/intel_graphics_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/jls_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/jls_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/jls_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/jls_v2_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/json_plus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/locale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.634229 joulescope_ui-1.1.9/joulescope_ui/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81702 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   112244 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.634229 joulescope_ui-1.1.9/joulescope_ui/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71550 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102499 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.666229 joulescope_ui-1.1.9/joulescope_ui/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    99351 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   130324 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    71667 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   102570 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    73100 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104062 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    72339 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   103281 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    75547 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105590 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)    68383 2024-05-21 17:24:21.000000 joulescope_ui-1.1.9/joulescope_ui/locale/joulescope_ui.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70320 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   100452 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.638229 joulescope_ui-1.1.9/joulescope_ui/locale/zh/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.670230 joulescope_ui-1.1.9/joulescope_ui/locale/zh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    61353 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    91276 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42189 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/mem_leak_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p1/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p1/index.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p2/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p2/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/plugins/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/process_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66497 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/pubsub_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/pubsub_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.674229 joulescope_ui-1.1.9/joulescope_ui/range_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/cdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10544 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/max_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/plugin_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/range_tools/usb_inrush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.678229 joulescope_ui-1.1.9/joulescope_ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    48138 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100365 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.678229 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_128x128.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_128x128@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_16x16@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1510 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_256x256.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_256x256@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      550 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_32x32@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2980 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7537 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_512x512@2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      718 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_64x64.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_64x64@2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/logo-large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources/zoom.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22815 2024-05-21 17:24:42.000000 joulescope_ui-1.1.9/joulescope_ui/resources.rcc
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/safe_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/shift_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/source_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.682229 joulescope_ui-1.1.9/joulescope_ui/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/font_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/fonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.686230 joulescope_ui-1.1.9/joulescope_ui/styles/js1/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/arrow_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/arrow_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/arrow_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_end.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_end_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_more.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/branch_vline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/detach.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/hmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/hsepartoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/radio_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/radio_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/tabs_menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/transparent.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/vmovetoolbar.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/js1/vsepartoolbars.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.686230 joulescope_ui-1.1.9/joulescope_ui/styles/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/style.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/system/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.690230 joulescope_ui-1.1.9/joulescope_ui/styles/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/test/test_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/test/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/styles/test/test_parameter_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.690230 joulescope_ui-1.1.9/joulescope_ui/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/anno1.anno.jls
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_annotation_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_disk_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_range_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_software_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_source_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/test/test_versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 17:24:22.000000 joulescope_ui-1.1.9/joulescope_ui/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/ui_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/versioned_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14173 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widget_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.694229 joulescope_ui-1.1.9/joulescope_ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.694229 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/accumulator_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.694229 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.694229 joulescope_ui-1.1.9/joulescope_ui/widgets/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/clock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/clock/clock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.694229 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/log_view_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/profile_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/publish_spy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/developer/pubsub_explorer_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.698229 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/current_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_control_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_info_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_update_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/js220_ctrl_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.698229 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/active_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/active_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/device_close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/device_open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/doc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/info.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/target_power_off.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/double_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/draggable_list_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.698229 joulescope_ui-1.1.9/joulescope_ui/widgets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/example_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/example/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/flyout_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/hamburger/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/hamburger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/hamburger/hamburger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/help/help_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/jls_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/jls_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/jls_info/jls_info_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.702229 joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22114 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/current_offset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/js220_cal_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/voltage_offset.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/memory_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/notes/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/notes/notes_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/progress_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/progress_bar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/progress_bar/progress_bar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/record_status_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/report_issue/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/report_issue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/report_issue/report_issue_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.706230 joulescope_ui-1.1.9/joulescope_ui/widgets/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/settings/settings_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/settings/unique_strings_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.710229 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/sidebar_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.710229 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/device.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/memory.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/misc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/play.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/record.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/target_power.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/target_power_off.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.710229 joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/disk_full_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/signal_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/signal_record_config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.714229 joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/statistics_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.714229 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/condition_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.714229 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/active.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/continuous.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/inactive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/searching.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/single.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/style.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.714229 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48890 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/trigger_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.718229 joulescope_ui-1.1.9/joulescope_ui/widgets/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.718229 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)    27322 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/value/value_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.718229 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.718229 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/add.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/view_manager_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.722230 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/annotations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/interval_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/line_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/quantities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.722230 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/font_scheme_js1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/index.json
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/marker_add1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/marker_add2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/marker_clear.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/pin_left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/pin_right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/style.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/style_defines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/zoom_all.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/zoom_in.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/zoom_out.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.722230 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/test_axis_ticks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/test_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_source_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)   173406 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/y_range_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/joulescope_ui/zip_inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:24:44.722230 joulescope_ui-1.1.9/joulescope_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 17:24:44.000000 joulescope_ui-1.1.9/joulescope_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 17:24:44.726230 joulescope_ui-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-21 17:24:00.000000 joulescope_ui-1.1.9/setup.py
```

### Comparing `joulescope_ui-1.1.8/CHANGELOG.md` & `joulescope_ui-1.1.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
+## 1.1.9
+
+2024 May 21
+
+* Fixed Waveform widget issues. 
+  * Fixed OpenGL frame rendering corruption.
+  * Fixed "Save image to file" & "Copy image to clipboard".
+  * Added support for numpad 1 through 9 keys.
+  * Fixed control widget "Add single marker".
+* Fixed customary units display in Value widget.
+* Fixed QAbstractSpinBox styling.
+* Fixed QComboBox styling on macOS.
+
+
 ## 1.1.8
 
 2024 May 13
 
 * Added arbitrary divisor with optional units to Value widget  #265
 * Added Flyout widget click & drag right to resize   #267
 * Deferred data directory creation  #266
```

### Comparing `joulescope_ui-1.1.8/CREDITS.html` & `joulescope_ui-1.1.9/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/LICENSE.txt` & `joulescope_ui-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/PKG-INFO` & `joulescope_ui-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.8
+Version: 1.1.9
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.8/README.md` & `joulescope_ui-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope.iss` & `joulescope_ui-1.1.9/joulescope.iss`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "Joulescope"
-#define MyAppVersion "1.1.8"
-#define MyAppVersionUnderscores "1_1_8"
+#define MyAppVersion "1.1.9"
+#define MyAppVersionUnderscores "1_1_9"
 #define MyAppPublisher "Jetperch LLC"
 #define MyAppURL "https://www.joulescope.com"
 #define MyAppExeName "joulescope.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application.
 ; Do not use the same AppId value in installers for other applications.
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/CHANGELOG.md` & `joulescope_ui-1.1.9/joulescope_ui/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope_ui.
 
 ---
 
+## 1.1.9
+
+2024 May 21
+
+* Fixed Waveform widget issues. 
+  * Fixed OpenGL frame rendering corruption.
+  * Fixed "Save image to file" & "Copy image to clipboard".
+  * Added support for numpad 1 through 9 keys.
+  * Fixed control widget "Add single marker".
+* Fixed customary units display in Value widget.
+* Fixed QAbstractSpinBox styling.
+* Fixed QComboBox styling on macOS.
+
+
 ## 1.1.8
 
 2024 May 13
 
 * Added arbitrary divisor with optional units to Value widget  #265
 * Added Flyout widget click & drag right to resize   #267
 * Deferred data directory creation  #266
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/CREDITS.html` & `joulescope_ui-1.1.9/joulescope_ui/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/__main__.py` & `joulescope_ui-1.1.9/joulescope_ui/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/about.py` & `joulescope_ui-1.1.9/joulescope_ui/about.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/api.py` & `joulescope_ui-1.1.9/joulescope_ui/api.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/app.py` & `joulescope_ui-1.1.9/joulescope_ui/app.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/capabilities.py` & `joulescope_ui-1.1.9/joulescope_ui/capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/dev_signal_buffer_source.py` & `joulescope_ui-1.1.9/joulescope_ui/dev_signal_buffer_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/device_update.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/device.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/device.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js110.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_fuse.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220_fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/js220_updater.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/js220_updater.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/jsdrv_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/jsdrv/jsdrv_wrapper.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/devices/test/test_device_update.py` & `joulescope_ui-1.1.9/joulescope_ui/devices/test/test_device_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/disk_monitor.py` & `joulescope_ui-1.1.9/joulescope_ui/disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/entry_points/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/entry_points/ui.py` & `joulescope_ui-1.1.9/joulescope_ui/entry_points/ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/entry_points/zip_inspector.py` & `joulescope_ui-1.1.9/joulescope_ui/entry_points/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/error_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/error_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/error_window.py` & `joulescope_ui-1.1.9/joulescope_ui/error_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/expanding_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/expanding_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/exporter.py` & `joulescope_ui-1.1.9/joulescope_ui/exporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/file_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/filename_formatter.py` & `joulescope_ui-1.1.9/joulescope_ui/filename_formatter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt` & `joulescope_ui-1.1.9/joulescope_ui/fonts/DSEG14-Modern/DSEG-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts/Hack/LICENSE.md` & `joulescope_ui-1.1.9/joulescope_ui/fonts/Hack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts/Lato/OFL.txt` & `joulescope_ui-1.1.9/joulescope_ui/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts/SourceCodePro/LICENSE.md` & `joulescope_ui-1.1.9/joulescope_ui/fonts/SourceCodePro/LICENSE.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts/SourceSerifPro/OFL.txt` & `joulescope_ui-1.1.9/joulescope_ui/fonts/SourceSerifPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/fonts.rcc` & `joulescope_ui-1.1.9/joulescope_ui/fonts.rcc`

 * *Files 2% similar despite different names*

```diff
@@ -193814,70 +193814,70 @@
 002f5150: 0000 0000 0000 0000 0000 0080 0002 0000  ................
 002f5160: 000a 0000 0027 0000 0000 0000 0000 0000  .....'..........
 002f5170: 0050 0002 0000 000c 0000 001b 0000 0000  .P..............
 002f5180: 0000 0000 0000 0010 0002 0000 0006 0000  ................
 002f5190: 0015 0000 0000 0000 0000 0000 0030 0002  .............0..
 002f51a0: 0000 000e 0000 0007 0000 0000 0000 0000  ................
 002f51b0: 0000 071a 0004 0000 0001 0025 4f27 0000  ...........%O'..
-002f51c0: 018f 729b 2ff5 0000 07c4 0004 0000 0001  ..r./...........
-002f51d0: 0029 2537 0000 018f 729b 2ff1 0000 058c  .)%7....r./.....
-002f51e0: 0004 0000 0001 001c 6407 0000 018f 729b  ........d.....r.
-002f51f0: 2ff9 0000 05ba 0004 0000 0001 001d 95a3  /...............
-002f5200: 0000 018f 729b 3001 0000 0750 0004 0000  ....r.0....P....
-002f5210: 0001 0026 8517 0000 018f 729b 3001 0000  ...&......r.0...
+002f51c0: 018f 9c2e 70ba 0000 07c4 0004 0000 0001  ....p...........
+002f51d0: 0029 2537 0000 018f 9c2e 70ba 0000 058c  .)%7......p.....
+002f51e0: 0004 0000 0001 001c 6407 0000 018f 9c2e  ........d.......
+002f51f0: 70be 0000 05ba 0004 0000 0001 001d 95a3  p...............
+002f5200: 0000 018f 9c2e 70c6 0000 0750 0004 0000  ......p....P....
+002f5210: 0001 0026 8517 0000 018f 9c2e 70c6 0000  ...&........p...
 002f5220: 07fc 0004 0000 0001 002a 5802 0000 018f  .........*X.....
-002f5230: 729b 2ff5 0000 082e 0004 0000 0001 002b  r./............+
-002f5240: c4d1 0000 018f 729b 2ff9 0000 062c 0004  ......r./....,..
-002f5250: 0000 0001 0020 3160 0000 018f 729b 2ffd  ..... 1`....r./.
+002f5230: 9c2e 70ba 0000 082e 0004 0000 0001 002b  ..p............+
+002f5240: c4d1 0000 018f 9c2e 70c2 0000 062c 0004  ........p....,..
+002f5250: 0000 0001 0020 3160 0000 018f 9c2e 70c6  ..... 1`......p.
 002f5260: 0000 05f4 0004 0000 0001 001f 01ac 0000  ................
-002f5270: 018f 729b 2ffd 0000 078e 0004 0000 0001  ..r./...........
-002f5280: 0027 bab6 0000 018f 729b 2ffd 0000 0666  .'......r./....f
-002f5290: 0004 0000 0001 0021 6449 0000 018f 729b  .......!dI....r.
-002f52a0: 2ff9 0000 06e6 0004 0000 0001 0023 e72d  /............#.-
-002f52b0: 0000 018f 729b 2ff1 0000 0862 0004 0000  ....r./....b....
-002f52c0: 0001 002d 262d 0000 018f 729b 3001 0000  ...-&-....r.0...
+002f5270: 018f 9c2e 70c2 0000 078e 0004 0000 0001  ....p...........
+002f5280: 0027 bab6 0000 018f 9c2e 70c2 0000 0666  .'........p....f
+002f5290: 0004 0000 0001 0021 6449 0000 018f 9c2e  .......!dI......
+002f52a0: 70be 0000 06e6 0004 0000 0001 0023 e72d  p............#.-
+002f52b0: 0000 018f 9c2e 70b6 0000 0862 0004 0000  ......p....b....
+002f52c0: 0001 002d 262d 0000 018f 9c2e 70c6 0000  ...-&-......p...
 002f52d0: 06a8 0004 0000 0001 0022 8ce5 0000 018f  ........."......
-002f52e0: 729b 2ff9 0000 089a 0004 0000 0001 002e  r./.............
-002f52f0: 90bc 0000 018f 729b 2fe5 0000 08d0 0004  ......r./.......
-002f5300: 0000 0001 002e af00 0000 018f 729b 2fe5  ............r./.
+002f52e0: 9c2e 70be 0000 089a 0004 0000 0001 002e  ..p.............
+002f52f0: 90bc 0000 018f 9c2e 70aa 0000 08d0 0004  ........p.......
+002f5300: 0000 0001 002e af00 0000 018f 9c2e 70aa  ..............p.
 002f5310: 0000 097c 0004 0000 0001 002f 0ab2 0000  ...|......./....
-002f5320: 018f 729b 2fe5 0000 09b0 0004 0000 0001  ..r./...........
-002f5330: 002f 293e 0000 018f 729b 2fe5 0000 090c  ./)>....r./.....
-002f5340: 0004 0000 0001 002e cd3f 0000 018f 729b  .........?....r.
-002f5350: 2fe5 0000 094a 0004 0000 0001 002e ec32  /....J.........2
-002f5360: 0000 018f 729b 2fe5 0000 0544 0004 0000  ....r./....D....
-002f5370: 0001 001b 3ffe 0000 018f 729b 300d 0000  ....?.....r.0...
+002f5320: 018f 9c2e 70aa 0000 09b0 0004 0000 0001  ....p...........
+002f5330: 002f 293e 0000 018f 9c2e 70aa 0000 090c  ./)>......p.....
+002f5340: 0004 0000 0001 002e cd3f 0000 018f 9c2e  .........?......
+002f5350: 70aa 0000 094a 0004 0000 0001 002e ec32  p....J.........2
+002f5360: 0000 018f 9c2e 70aa 0000 0544 0004 0000  ......p....D....
+002f5370: 0001 001b 3ffe 0000 018f 9c2e 70d6 0000  ....?.......p...
 002f5380: 036a 0004 0000 0001 0010 f545 0000 018f  .j.........E....
-002f5390: 729b 3005 0000 041a 0004 0000 0001 0014  r.0.............
-002f53a0: f75f 0000 018f 729b 3009 0000 048c 0004  ._....r.0.......
-002f53b0: 0000 0001 0017 6f8d 0000 018f 729b 3009  ......o.....r.0.
+002f5390: 9c2e 70ca 0000 041a 0004 0000 0001 0014  ..p.............
+002f53a0: f75f 0000 018f 9c2e 70ce 0000 048c 0004  ._......p.......
+002f53b0: 0000 0001 0017 6f8d 0000 018f 9c2e 70d2  ......o.......p.
 002f53c0: 0000 04c2 0004 0000 0001 0018 d613 0000  ................
-002f53d0: 018f 729b 3009 0000 03aa 0004 0000 0001  ..r.0...........
-002f53e0: 0012 1971 0000 018f 729b 3005 0000 03de  ...q....r.0.....
-002f53f0: 0004 0000 0001 0013 8810 0000 018f 729b  ..............r.
-002f5400: 300d 0000 02dc 0004 0000 0001 000e c39f  0...............
-002f5410: 0000 018f 729b 3009 0000 0452 0004 0000  ....r.0....R....
-002f5420: 0001 0016 0ed3 0000 018f 729b 300d 0000  ..........r.0...
+002f53d0: 018f 9c2e 70ce 0000 03aa 0004 0000 0001  ....p...........
+002f53e0: 0012 1971 0000 018f 9c2e 70ca 0000 03de  ...q......p.....
+002f53f0: 0004 0000 0001 0013 8810 0000 018f 9c2e  ................
+002f5400: 70d2 0000 02dc 0004 0000 0001 000e c39f  p...............
+002f5410: 0000 018f 9c2e 70d2 0000 0452 0004 0000  ......p....R....
+002f5420: 0001 0016 0ed3 0000 018f 9c2e 70d2 0000  ............p...
 002f5430: 0502 0004 0000 0001 001a 2aab 0000 018f  ..........*.....
-002f5440: 729b 3005 0000 031e 0004 0000 0001 000f  r.0.............
-002f5450: e47b 0000 018f 729b 3009 0000 02a6 0004  .{....r.0.......
-002f5460: 0000 0001 000d 65a3 0000 018f 729b 3001  ......e.....r.0.
+002f5440: 9c2e 70ca 0000 031e 0004 0000 0001 000f  ..p.............
+002f5450: e47b 0000 018f 9c2e 70ce 0000 02a6 0004  .{......p.......
+002f5460: 0000 0001 000d 65a3 0000 018f 9c2e 70ca  ......e.......p.
 002f5470: 0000 01ae 0004 0000 0001 0003 6c6f 0000  ............lo..
-002f5480: 018f 729b 2fed 0000 008e 0004 0000 0001  ..r./...........
-002f5490: 0000 0000 0000 018f 729b 2fed 0000 018a  ........r./.....
-002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 729b  ..............r.
-002f54b0: 2fed 0000 010a 0004 0000 0001 0001 72aa  /.............r.
-002f54c0: 0000 018f 729b 2ff1 0000 00e8 0004 0000  ....r./.........
-002f54d0: 0001 0000 f2c6 0000 018f 729b 2fed 0000  ..........r./...
+002f5480: 018f 9c2e 70b2 0000 008e 0004 0000 0001  ....p...........
+002f5490: 0000 0000 0000 018f 9c2e 70b2 0000 018a  ..........p.....
+002f54a0: 0004 0000 0001 0002 e1fa 0000 018f 9c2e  ................
+002f54b0: 70b6 0000 010a 0004 0000 0001 0001 72aa  p.............r.
+002f54c0: 0000 018f 9c2e 70b6 0000 00e8 0004 0000  ......p.........
+002f54d0: 0001 0000 f2c6 0000 018f 9c2e 70b2 0000  ............p...
 002f54e0: 015e 0004 0000 0001 0002 7e0b 0000 018f  .^........~.....
-002f54f0: 729b 2ff1 0000 00ba 0004 0000 0001 0000  r./.............
-002f5500: 8b33 0000 018f 729b 2fed 0000 01f0 0004  .3....r./.......
-002f5510: 0000 0001 0004 74f0 0000 018f 729b 2ff1  ......t.....r./.
+002f54f0: 9c2e 70b6 0000 00ba 0004 0000 0001 0000  ..p.............
+002f5500: 8b33 0000 018f 9c2e 70b6 0000 01f0 0004  .3......p.......
+002f5510: 0000 0001 0004 74f0 0000 018f 9c2e 70b6  ......t.......p.
 002f5520: 0000 01ce 0004 0000 0001 0003 ee66 0000  .............f..
-002f5530: 018f 729b 2fed 0000 0130 0004 0000 0001  ..r./....0......
-002f5540: 0001 f768 0000 018f 729b 2fed 0000 0210  ...h....r./.....
-002f5550: 0004 0000 0001 0004 f353 0000 018f 729b  .........S....r.
-002f5560: 2fe9 0000 027a 0004 0000 0001 000b 366d  /....z........6m
-002f5570: 0000 018f 729b 2fe9 0000 0234 0004 0000  ....r./....4....
-002f5580: 0001 0007 158f 0000 018f 729b 2fe5 0000  ..........r./...
+002f5530: 018f 9c2e 70b6 0000 0130 0004 0000 0001  ....p....0......
+002f5540: 0001 f768 0000 018f 9c2e 70b2 0000 0210  ...h......p.....
+002f5550: 0004 0000 0001 0004 f353 0000 018f 9c2e  .........S......
+002f5560: 70b2 0000 027a 0004 0000 0001 000b 366d  p....z........6m
+002f5570: 0000 018f 9c2e 70ae 0000 0234 0004 0000  ......p....4....
+002f5580: 0001 0007 158f 0000 018f 9c2e 70ae 0000  ............p...
 002f5590: 0254 0004 0000 0001 0009 2ac5 0000 018f  .T........*.....
-002f55a0: 729b 2fed                                r./.
+002f55a0: 9c2e 70b2                                ..p.
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/getting_started.py` & `joulescope_ui-1.1.9/joulescope_ui/getting_started.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/help_ui.py` & `joulescope_ui-1.1.9/joulescope_ui/help_ui.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/intel_graphics_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/intel_graphics_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/jls_source.py` & `joulescope_ui-1.1.9/joulescope_ui/jls_source.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/jls_v1.py` & `joulescope_ui-1.1.9/joulescope_ui/jls_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/jls_v2.py` & `joulescope_ui-1.1.9/joulescope_ui/jls_v2.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/jls_v2_annotations.py` & `joulescope_ui-1.1.9/joulescope_ui/jls_v2_annotations.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/json_plus.py` & `joulescope_ui-1.1.9/joulescope_ui/json_plus.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/ar/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 msgid "Email"
 msgstr "البريد الإلكتروني"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "الوصف"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "تحرير"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "عرض كتخفيض"
 
@@ -610,15 +610,15 @@
 msgid "Do not show again"
 msgstr "لا تظهر مرة أخرى"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "تم الكشف عن رسومات إنتل"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "متعدد المقاييس"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "راسم الذبذبات"
 
@@ -761,15 +761,15 @@
 msgid "Manage"
 msgstr "إدارة"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "حدد الملف لفتحه"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "اسم هذه الأداة"
 
 #: paths.py:31
 msgid "Paths"
 msgstr "المسارات"
 
@@ -1058,15 +1058,15 @@
 "target device."
 msgstr ""
 "عند التمكين، يتدفق التيار بين طرفي التيار. عند تعطيله، لا يمكن للتيار أن "
 "يتدفق بين أطراف التيار. في إعدادات النظام الشائعة، يؤدي ذلك إلى تثبيط الطاقة"
 " المستهدفة، والتي يمكن استخدامها لإعادة ضبط دورة الطاقة للجهاز المستهدف."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "النطاق الحالي"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1206,33 +1206,33 @@
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "عدد العينات بعد نافذة النطاق الحالي المستخدمة لتحديد المتوسط. يتم تجاهل هذه "
 "القيمة لجميع أنواع IRF الأخرى."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "التيار"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "تمكين تدفق الإشارة الحالية."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "الجهد"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "تمكين تدفق إشارة الجهد."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "الطاقة"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "تمكين تدفق إشارة الطاقة."
 
@@ -1435,15 +1435,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "تمكين تدفق إشارة الإدخال 3 للأغراض العامة."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "مدخلات الزناد"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "تمكين تدفق إشارة إدخال الزناد."
 
@@ -1454,15 +1454,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "الاسم"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "مخزن جولسكوب للتيار"
 
@@ -1673,33 +1673,33 @@
 msgstr "افتراضي"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "نظام الخط الافتراضي لجولسكوب"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "مصدر تدفق البيانات الإحصائية."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "الإشارة المراد عرضها."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "الشحن"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "الطاقة"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "عرض عنوان قسم الإحصائيات لكل إشارة."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "المجمع"
 
@@ -1769,15 +1769,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "الموضوع"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "القيمة"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "نشر الجاسوس"
 
@@ -1807,15 +1807,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "تحديث"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "الجهاز"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "التقدم"
@@ -2359,15 +2359,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "إحصائياتالتسجيلالتكوين"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "تنسيق الوقت"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "حدد الجهاز المصدر"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "الجهاز المستخدم لحالة البدء وحالة التوقف."
 
@@ -2519,106 +2519,106 @@
 msgid "Stop Condition"
 msgstr "حالة التوقف"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "إجراءات الإيقاف"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "إظهار رأس اختيار الجهاز."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "عرض رأس الاستحقاق."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "عرض حقول الإحصائيات على اليمين."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "إظهار علامة + أو -."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "اقسم الكمية على هذه القيمة."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr "المقسوم عليه هو رقم عائم. قد يتبع الرقم اختياريًا وحدات."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "تأتي القيم التي تعرضها هذه الأداة من جهاز مصدر واحد. حدد الجهاز المصدر هنا."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "امسك الشاشة"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "عند تحديده، يمنع الشاشة من التحديث."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "تتضمن واجهة المستخدم أيضًا زر تعليق الإحصائيات العامة على الشريط الجانبي. "
 "عند تحديد زر تعليق الإحصائيات العامة، يتم تعطيل هذا الزر وليس له أي تأثير."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "يتم تحديث القيم المعروضة عادةً مع كل بيانات إحصائية جديدة يحسبها الجهاز. عند"
 " تحديد هذا الزر، لن يتم تحديث العرض. ومع ذلك، ستستمر الإحصائيات في التراكم "
 "والتراكم (إذا تم تحديده)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "تراكم القيم بمرور الوقت"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "عادةً ما يتم حساب التيار والجهد والطاقة على فاصل تردد إحصائي واحد. اضغط على "
 "هذا الزر لتجميع القيم إلى أجل غير مسمى. اضغط مرة أخرى للعودة إلى التشغيل "
 "العادي."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "لاحظ أن هذا الزر لا يؤثر على تراكم الشحن والطاقة. يتراكم كلاهما إلى أجل غير "
 "مسمى بغض النظر عن حالة هذا الزر."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "غير موجود"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "عقد"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "زيادة"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "عرض المدير"
@@ -2664,34 +2664,34 @@
 msgstr "المثلث الأيمن"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "المثلث الأيسر"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "دليل"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "المركز"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "النص"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "إظهار النص"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "الشكل"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "الوضع Y"
 
@@ -2878,317 +2878,317 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"افتراضي\" سيستخدم المصدر الافتراضي الذي يتم تكوينه عادةً باستخدام أداة "
 "التحكم في الجهاز."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "إيقاف"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "الشكل الموجي"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "مدخلات الأغراض العامة 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "مدخلات الأغراض العامة 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "مدخلات الأغراض العامة 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "مدخلات الأغراض العامة 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "سلسلة مرشح المصدر."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "عرض التتبع."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "الإطارات المستهدفة في الثانية."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "المزامنة"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 هرتز"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 هرتز"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 هرتز"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "الحد الأدنى للفاصل الزمني بين إعادة الطلاء بالمللي ثانية."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "إظهار الحد الأدنى والحد الأقصى لملء الحدود الدنيا والقصوى."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "الخطوط"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "ملء 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "ملء 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "عرض الإطارات في الثانية."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "عرض الإحصائيات عند تحريك الماوس."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "عرض إحصائيات الرسم على اليمين."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "عرض التردد للعلامات والإحصائيات المزدوجة."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "الكميات المراد عرضها افتراضيًا."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "دقة العرض بالأرقام."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "استخدم عرض OpenGL."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "تثبيت بيانات الجانب الأيسر (الأقدم) بحيث تبقى في العرض."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "تثبيت بيانات الجانب الأيمن (الأحدث) بحيث تبقى في العرض."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "حالة الشكل الموجي."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "الشروح"
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "موقع التحكم"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "أعلى"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "القاع"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "كمية الإشارة المراد إظهارها في الملخص."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "وضع التعليق التوضيحي للمحور X"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "المطلق"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "نسبي"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "المصادر الفرعية المتاحة."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "المصادر الفرعية المختارة لكل تتبع."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "أولوية التتبع: أعلى قيمة للتيار في الأعلى، لا شيء متوقف."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "حفظ الصورة في ملف"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "علامة واحدة"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "علامات مزدوجة"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "الوضع"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "مسح الكل"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "التعليقات التوضيحية"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "النطاق"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "تلقائي"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "دقيق"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "المقياس"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "الخطي"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "لوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "الصفر اللوغاريتمي"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "البادئة المفضلة"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "إضافة"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "إخفاء كل النص"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "إظهار كل النص"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "عمودي"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "أفقي"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "حفظ"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "النطاق التلقائي للمحور Y"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "نسخ الصورة إلى الحافظة"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "تصدير البيانات المرئية"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "تصدير جميع البيانات"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "التصدير"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "التحليل"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "الفاصل الزمني"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "تكبير"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "عرض الإحصائيات"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "يسار"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "صحيح"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "إيقاف التشغيل"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "إزالة"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "الوضع Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "الحد الأقصى"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/de/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
 msgid "Email"
 msgstr "E-Mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Beschreibung"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Bearbeiten"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Als Markdown anzeigen"
 
@@ -644,15 +644,15 @@
 msgid "Do not show again"
 msgstr "Nicht mehr anzeigen"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Intel-Grafik erkannt"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "Multimeter"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "Oszilloskop"
 
@@ -797,15 +797,15 @@
 msgid "Manage"
 msgstr "Verwalten Sie"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "Datei zum Öffnen auswählen"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "Der Name für dieses Widget."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "Pfade"
 
@@ -1102,15 +1102,15 @@
 "Wenn aktiviert, fließt Strom zwischen den Stromanschlüssen. Wenn er "
 "deaktiviert ist, kann kein Strom zwischen den Stromanschlüssen fließen. In "
 "gängigen Systemkonfigurationen wird dadurch die Stromversorgung des "
 "Zielgeräts unterbrochen, was zum Zurücksetzen des Zielgeräts durch einen "
 "Stromzyklus verwendet werden kann."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "Strombereich"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1259,33 +1259,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Die Anzahl der Abtastungen nach dem Strombereichsfenster, die zur Bestimmung"
 " des Mittelwerts verwendet wird. Dieser Wert wird für alle anderen IRF-Typen"
 " ignoriert."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "Strom"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Aktivieren Sie das Stromsignal-Streaming."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "Voltage"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Aktivieren Sie das Streaming von Spannungssignalen."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Strom"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Aktivieren Sie das Stromsignal-Streaming."
 
@@ -1503,15 +1503,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Aktivieren Sie den Allzweckeingang 3 Signalstreaming."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "Trigger-Eingang"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Aktivieren Sie das Streaming des Trigger-Eingangssignals."
 
@@ -1522,15 +1522,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "Name"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope Strompuffer"
 
@@ -1749,33 +1749,33 @@
 msgstr "Standard"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Joulescope Standard-Schriftschema"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "Die Statistik-Datenstromquelle."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "Das anzuzeigende Signal."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "Ladung"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "Energie"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "Zeigen Sie den Titel des Statistikabschnitts für jedes Signal an."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "Akkumulator"
 
@@ -1845,15 +1845,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Thema"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Wert"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Spion veröffentlichen"
 
@@ -1883,15 +1883,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "aktualisieren"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "Gerät"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Fortschritt"
@@ -2459,15 +2459,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatistikRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Zeitformat"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "Wählen Sie das Quellgerät"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Das Gerät, das für die Startbedingung und die Stoppbedingung zu verwenden "
@@ -2628,114 +2628,114 @@
 msgid "Stop Condition"
 msgstr "Stopp-Bedingung"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "Stopp-Aktionen"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "Zeigt die Kopfzeile der Geräteauswahl an."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "Zeigt die zugehörige Kopfzeile an."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "Zeigen Sie die Statistikfelder auf der rechten Seite an."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "Zeigt ein führendes + oder - Zeichen."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "Teilen Sie die Größe durch diesen Wert."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 "Der Divisor ist eine Gleitkommazahl. Die Zahl kann optional von Einheiten "
 "gefolgt werden."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Die von diesem Widget angezeigten Werte stammen von einem einzigen "
 "Quellgerät. Wählen Sie hier das Quellgerät aus."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "Halten Sie das Display"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "Wenn ausgewählt, wird die Aktualisierung der Anzeige verhindert."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "Die Benutzeroberfläche enthält auch eine Schaltfläche zum Halten globaler "
 "Statistiken in der Seitenleiste. Wenn die Schaltfläche \"Globale Statistik "
 "halten\" ausgewählt ist, ist diese Schaltfläche deaktiviert und hat keine "
 "Wirkung."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Die angezeigten Werte werden normalerweise mit jeder neuen, vom Gerät "
 "berechneten Statistik aktualisiert. Wenn diese Schaltfläche ausgewählt ist, "
 "wird die Anzeige nicht aktualisiert. Die Statistiken werden jedoch weiterhin"
 " akkumuliert und auflaufen (falls ausgewählt)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "Erfassen Sie Werte über die Zeit"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Strom, Spannung und Leistung werden normalerweise über ein einziges "
 "statistisches Frequenzintervall berechnet. Drücken Sie diese Taste, um die "
 "Werte auf unbestimmte Zeit zu akkumulieren. Drücken Sie erneut, um zum "
 "normalen Betrieb zurückzukehren."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Beachten Sie, dass diese Taste keinen Einfluss auf die Akkumulation von "
 "Ladung und Energie hat. Beide akkumulieren sich unabhängig vom Zustand "
 "dieser Taste auf unbestimmte Zeit."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "Nicht vorhanden"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Halten"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "Beschleunigt"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Ansicht Manager"
@@ -2781,34 +2781,34 @@
 msgstr "Dreieck rechts"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "Dreieck links"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "Handbuch"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Zentriert"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "Text"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "Text anzeigen"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "Form"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y Mode"
 
@@ -3009,323 +3009,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" verwendet die Standardquelle, die normalerweise über das Device "
 "Control Widget konfiguriert wird."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "aus"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Wellenform"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "Allzweck-Eingang 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "Allzweck-Eingang 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "Allzweck-Eingang 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "Allzweck-Eingang 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "Die Quellfilterkette."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "Die Leiterbahnbreite."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "Die angestrebten Bilder pro Sekunde."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 "Das minimale Intervall zwischen den Wiederholungsmessungen in Millisekunden."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "Zeigt die minimale und maximale Ausdehnung an."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "Zeilen"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "Füllung 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "Füllung 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "Zeigt die Bilder pro Sekunde an."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "Zeigen Sie die Statistik bei Mausbewegung an."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "Zeigen Sie die Plot-Statistiken auf der rechten Seite an."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "Zeigt die Frequenz für duale Marker und Statistiken an."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "Die Größen, die standardmäßig angezeigt werden."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "Die Genauigkeit der Anzeige in Ziffern."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "Verwenden Sie OpenGL-Rendering."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Pinnen Sie die (ältesten) Daten auf der linken Seite an, damit sie im "
 "Blickfeld bleiben."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Pinnen Sie die (neuesten) Daten auf der rechten Seite an, damit sie im "
 "Blickfeld bleiben."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "Der Zustand der Wellenform."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "Die Anmerkungen."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "Standort der Steuerung"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "oben"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "unten"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "Die Signalgröße, die in der Zusammenfassung angezeigt werden soll."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "X-Achsen-Anmerkungsmodus"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "Absolut"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "Relativ"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "Die verfügbaren Teilquellen."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "Die ausgewählten Teilquellen für jede Messkurve."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Die Priorität der Messkurve: Der höchste int-Wert steht oben, None ist aus."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "Bild in Datei speichern"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "Einzelner Marker"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "Zwei Marker"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "Modus"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "Alles löschen"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "Anmerkungen"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "Range"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "Genau"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "Skala"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "Linear"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "Logarithmisch"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "Logarithmischer Nullpunkt"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "Bevorzugte Vorsilbe"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "hinzufügen"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "Alle Texte ausblenden"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "Alle Texte anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "Vertikal"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "Speichern Sie"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Automatischer Bereich der Y-Achse"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "Bild in die Zwischenablage kopieren"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "Sichtbare Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "Alle Daten exportieren"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Exportieren"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "Statistik anzeigen"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "Links"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "Rechts"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Aus"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "entfernen"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Y-Modus"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/el/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 msgid "Email"
 msgstr "Email"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Περιγραφή"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Επεξεργασία"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Προβολή ως Markdown"
 
@@ -646,15 +646,15 @@
 msgid "Do not show again"
 msgstr "Μην εμφανίζετε ξανά"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Ανιχνεύονται γραφικά Intel"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "Πολύμετρο"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "Παλμογράφος"
 
@@ -800,15 +800,15 @@
 msgid "Manage"
 msgstr "Διαχείριση"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "Επιλέξτε αρχείο για άνοιγμα"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "Το όνομα για αυτό το widget."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "Διαδρομές"
 
@@ -1107,15 +1107,15 @@
 "Όταν είναι ενεργοποιημένο, το ρεύμα ρέει μεταξύ των ακροδεκτών ρεύματος. "
 "Όταν είναι απενεργοποιημένο, το ρεύμα δεν μπορεί να ρέει μεταξύ των "
 "ακροδεκτών ρεύματος. Στις συνήθεις ρυθμίσεις συστημάτων, αυτό αναστέλλει την"
 " τροφοδοσία του στόχου, η οποία μπορεί να χρησιμοποιηθεί για την επαναφορά "
 "της συσκευής στόχου σε κύκλο λειτουργίας."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "Εύρος ρεύματος"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1264,33 +1264,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Ο αριθμός των δειγμάτων μετά το παράθυρο εύρους ρεύματος που χρησιμοποιείται"
 " για τον προσδιορισμό του μέσου όρου. Αυτή η τιμή αγνοείται για όλους τους "
 "άλλους τύπους IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "Ρεύμα"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Ενεργοποίηση της ροής σημάτων ρεύματος."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "Τάση"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος τάσης."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Ισχύς"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος ισχύος."
 
@@ -1510,15 +1510,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Ενεργοποιήστε τη ροή σήματος εισόδου γενικού σκοπού 3."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "Είσοδος σκανδαλισμού"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Ενεργοποίηση της ροής σήματος εισόδου σκανδαλισμού."
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "Όνομα"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Απομονωτής ρεύματος Joulescope"
 
@@ -1757,33 +1757,33 @@
 msgstr "προεπιλογή"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Προεπιλεγμένο σχήμα γραμματοσειράς του Joulescope"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "Η πηγή ροής στατιστικών δεδομένων."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "Το σήμα προς απεικόνιση."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "φόρτιση"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "ενέργεια"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "Εμφάνιση του τίτλου της ενότητας στατιστικών για κάθε σήμα."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "Συσσωρευτής"
 
@@ -1854,15 +1854,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Θέμα"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Τιμή"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Δημοσίευση Spy"
 
@@ -1892,15 +1892,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Ενημέρωση"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "Συσκευή"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progress"
@@ -2467,15 +2467,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Μορφή χρόνου"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "Επιλέξτε τη συσκευή προέλευσης"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Η συσκευή που θα χρησιμοποιηθεί για τη συνθήκη εκκίνησης και τη συνθήκη "
@@ -2638,114 +2638,114 @@
 msgid "Stop Condition"
 msgstr "Κατάσταση διακοπής"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "Ενέργειες διακοπής"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "Εμφάνιση της επικεφαλίδας επιλογής συσκευής."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "Εμφάνιση της επικεφαλίδας accrue."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "Εμφανίστε τα πεδία στατιστικών στοιχείων στα δεξιά."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "Εμφανίζει ένα πρόσημο + ή -."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "Διαιρέστε την ποσότητα με αυτή την τιμή."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 "Ο διαιρέτης είναι ένας αριθμός κινητής υποδιαστολής. Ο αριθμός μπορεί "
 "προαιρετικά να ακολουθείται από μονάδες."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Οι τιμές που εμφανίζονται από αυτό το widget προέρχονται από μία μόνο "
 "συσκευή προέλευσης. Επιλέξτε τη συσκευή προέλευσης εδώ."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "Κρατήστε την οθόνη"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "Όταν είναι επιλεγμένο, εμποδίζει την ενημέρωση της οθόνης."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "Το UI περιλαμβάνει επίσης ένα κουμπί κράτησης συνολικών στατιστικών "
 "στοιχείων στην πλευρική γραμμή. Όταν είναι επιλεγμένο το κουμπί global "
 "statistics hold, αυτό το κουμπί είναι απενεργοποιημένο και δεν έχει καμία "
 "επίδραση."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Οι εμφανιζόμενες τιμές ενημερώνονται κανονικά με κάθε νέο στατιστικό "
 "δεδομένο που υπολογίζεται από τη συσκευή. Όταν είναι επιλεγμένο αυτό το "
 "κουμπί, η οθόνη δεν θα ενημερώνεται. Ωστόσο, τα στατιστικά στοιχεία θα "
 "συνεχίσουν να συσσωρεύονται και να συσσωρεύονται (εάν επιλεγεί)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "Συγκέντρωση τιμών με την πάροδο του χρόνου"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Το ρεύμα, η τάση και η ισχύς υπολογίζονται συνήθως σε ένα ενιαίο διάστημα "
 "στατιστικής συχνότητας. Πατήστε αυτό το κουμπί για να συγκεντρώσετε τις "
 "τιμές επ' αόριστον. Πατήστε το ξανά για να επιστρέψετε στην κανονική "
 "λειτουργία."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Σημειώστε ότι αυτό το κουμπί δεν επηρεάζει τη φόρτιση και τη συσσώρευση "
 "ενέργειας. Και τα δύο συσσωρεύονται επ' αόριστον ανεξάρτητα από την "
 "κατάσταση αυτού του κουμπιού."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "Δεν υπάρχει"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Hold"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "Αυξημένο"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Διαχείριση προβολής"
@@ -2791,34 +2791,34 @@
 msgstr "τρίγωνο δεξιά"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "τρίγωνο αριστερά"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "Εγχειρίδιο"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centered"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "Κείμενο"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "Εμφάνιση κειμένου"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "Σχήμα"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Λειτουργία Y"
 
@@ -3016,325 +3016,325 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" θα χρησιμοποιήσει την προεπιλεγμένη πηγή, η οποία κανονικά "
 "διαμορφώνεται χρησιμοποιώντας το widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "off"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Κυματομορφή"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "Είσοδος γενικού σκοπού 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "Είσοδος γενικού σκοπού 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "Είσοδος γενικού σκοπού 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "Είσοδος γενικού σκοπού 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "Η συμβολοσειρά φίλτρων πηγής."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "Το πλάτος του ίχνους."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "Τα καρέ ανά δευτερόλεπτο που είναι ο στόχος."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 "Το ελάχιστο χρονικό διάστημα μεταξύ επανεκτύπωσης σε χιλιοστά του "
 "δευτερολέπτου."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "Εμφανίζει την ελάχιστη και τη μέγιστη έκταση πλήρωσης."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "γραμμές"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "γέμισμα 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "γέμισμα 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "Εμφάνιση των καρέ ανά δευτερόλεπτο."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "Εμφάνιση των στατιστικών στοιχείων κατά το πέρασμα του ποντικιού."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "Εμφάνιση των στατιστικών στοιχείων της γραφικής παράστασης στα δεξιά."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "Εμφάνιση συχνότητας για διπλούς δείκτες και στατιστικά στοιχεία."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "Οι ποσότητες που θα εμφανίζονται από προεπιλογή."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "Η ακρίβεια για την εμφάνιση σε ψηφία."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "Χρησιμοποιήστε απόδοση OpenGL."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Καρφιτσώστε τα δεδομένα της αριστερής πλευράς (παλαιότερα) ώστε να "
 "παραμένουν σε προβολή."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Καρφιτσώστε τα δεδομένα της δεξιάς πλευράς (τα νεότερα), ώστε να παραμένουν "
 "σε προβολή."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "Η κατάσταση της κυματομορφής."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "Οι επισημάνσεις."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "Θέση ελέγχου"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "κάτω"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "Η ποσότητα σήματος που θα εμφανίζεται στη σύνοψη."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "Λειτουργία σχολιασμού του άξονα Χ"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "Απόλυτο"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "Σχετική"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "Οι διαθέσιμες υποπηγές."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "Οι επιλεγμένες υποπηγές για κάθε ίχνος."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "Η προτεραιότητα του ίχνους: η υψηλότερη τιμή int στην κορυφή, το None είναι "
 "απενεργοποιημένο."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "Αποθήκευση εικόνας σε αρχείο"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "Ενιαίος δείκτης"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "Διπλοί δείκτες"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "Λειτουργία"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "Εκκαθάριση όλων"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "Σημειώσεις"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "Εύρος"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "Ακριβές"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "Κλίμακα"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "Γραμμική"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "Λογαριθμική"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "Λογαριθμικό μηδέν"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "Προτιμώμενο πρόθεμα"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "Προσθήκη"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "Απόκρυψη όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "Εμφάνιση όλου του κειμένου"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "Κατακόρυφο"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "Οριζόντια"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "Αποθήκευση"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Αυτόματο εύρος του άξονα Y"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "Αντιγραφή εικόνας στο πρόχειρο"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "Εξαγωγή ορατών δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "Εξαγωγή όλων των δεδομένων"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Εξαγωγή"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "Ανάλυση"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Διάστημα"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "Ζουμ"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "Εμφάνιση στατιστικών στοιχείων"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "Αριστερά"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "Σωστό"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "Αφαίρεση"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Λειτουργία Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/es/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
 msgid "Email"
 msgstr "Correo electrónico"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descripción"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Editar"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Ver como Markdown"
 
@@ -646,15 +646,15 @@
 msgid "Do not show again"
 msgstr "No volver a mostrar"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Gráficos Intel detectados"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "Multímetro"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "Osciloscopio"
 
@@ -800,15 +800,15 @@
 msgid "Manage"
 msgstr "Gestione"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "Seleccionar archivo para abrir"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "El nombre de este widget."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "Caminos"
 
@@ -1103,15 +1103,15 @@
 "Cuando está activado, la corriente fluye entre los terminales de corriente. "
 "Cuando está desactivado, la corriente no puede fluir entre los terminales de"
 " corriente. En configuraciones de sistema comunes, esto inhibe la "
 "alimentación del objetivo, que puede utilizarse para reiniciar el "
 "dispositivo objetivo."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "Rango de corriente"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1259,33 +1259,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "El número de muestras después de la ventana de rango de corriente utilizada "
 "para determinar la media. Este valor se ignora para todos los demás tipos de"
 " IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "Corriente"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Habilita la transmisión de la señal de corriente."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "Tensión"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Habilita la transmisión de señales de tensión."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Potencia"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Habilita la transmisión de señales de potencia."
 
@@ -1501,15 +1501,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Habilita el flujo de señales de entrada 3 de propósito general."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "Entrada de disparo"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Habilita la transmisión de la señal de entrada de disparo."
 
@@ -1520,15 +1520,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "Nombre"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Búfer de corriente de Joulescope"
 
@@ -1747,33 +1747,33 @@
 msgstr "por defecto"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Esquema de fuentes por defecto de Joulescope"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "La fuente de flujo de datos estadísticos."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "La señal a visualizar."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "carga"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "energía"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "Muestra el título de la sección de estadísticas para cada señal."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "Acumulador"
 
@@ -1844,15 +1844,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Tema"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Valor"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Publicar Espía"
 
@@ -1882,15 +1882,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Actualización"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "Dispositivo"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progreso"
@@ -2451,15 +2451,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "EstadísticasRegistroConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Formato de tiempo"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "Seleccione el dispositivo fuente"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "El dispositivo a utilizar para la condición de arranque y la condición de "
@@ -2617,113 +2617,113 @@
 msgid "Stop Condition"
 msgstr "Condición de parada"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "Acciones de parada"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "Muestra la cabecera de selección de dispositivos."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "Muestra la cabecera de acumulación."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "Muestra los campos de estadísticas a la derecha."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "Muestra un signo + o - inicial."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "Divida la cantidad por este valor."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 "El divisor es un número de coma flotante. Opcionalmente, el número puede ir "
 "seguido de unidades."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Los valores mostrados por este widget proceden de un único dispositivo "
 "fuente. Seleccione aquí el dispositivo de origen."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "Mantener la pantalla"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "Cuando se selecciona, evita que la pantalla se actualice."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "La interfaz de usuario también incluye un botón de retención de estadísticas"
 " globales en la barra lateral. Cuando se selecciona el botón de retención de"
 " estadísticas globales, este botón se desactiva y no tiene ningún efecto."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Los valores mostrados normalmente se actualizan con cada nuevo dato "
 "estadístico calculado por el dispositivo. Cuando se selecciona este botón, "
 "la pantalla no se actualiza. Sin embargo, las estadísticas seguirán "
 "acumulándose y acumulándose (si está seleccionado)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "Acumula valores a lo largo del tiempo"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "La corriente, la tensión y la potencia se calculan normalmente en un único "
 "intervalo de frecuencia estadística. Pulse este botón para acumular los "
 "valores indefinidamente. Pulse de nuevo para volver al funcionamiento "
 "normal."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Tenga en cuenta que este botón no afecta a la acumulación de carga y "
 "energía. Ambas se acumulan indefinidamente independientemente del estado de "
 "este botón."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "No presente"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Mantenga"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "Aumento de"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Administrador de vistas"
@@ -2769,34 +2769,34 @@
 msgstr "triángulo derecho"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triángulo izquierdo"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "Manual"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrado"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "Texto"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "Mostrar texto"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modo Y"
 
@@ -2994,323 +2994,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"por defecto\" utilizará la fuente por defecto que normalmente se configura"
 " utilizando el widget de Control de Dispositivos."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "off"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forma de onda"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "Entrada de propósito general 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "Entrada de propósito general 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "Entrada de propósito general 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "Entrada de propósito general 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "La cadena de filtros de la fuente."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "La anchura de la traza."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "El objetivo de imágenes por segundo."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "El intervalo mínimo entre repintados en milisegundos."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "Muestra las extensiones mínima y máxima de llenado."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "líneas"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "llenar 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "llenar 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "Muestra las imágenes por segundo."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "Muestra las estadísticas al pasar el ratón por encima."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "Muestra las estadísticas del gráfico a la derecha."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "Muestra la frecuencia para marcadores duales y estadísticas."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "Las cantidades a mostrar por defecto."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "La precisión a mostrar en dígitos."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "Utilice el renderizado OpenGL."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Fije los datos del lado izquierdo (más antiguos) para que permanezcan a la "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Fija los datos del lado derecho (los más nuevos) para que permanezcan a la "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "El estado de la forma de onda."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "Las anotaciones."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "Lugar de control"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "inferior"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "La cantidad de señal a mostrar en el resumen."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "Modo de anotación en el eje X"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "Absoluto"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "Relativa"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "Las subfuentes disponibles."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "Las subfuentes seleccionadas para cada traza."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La prioridad de la traza: el valor int más alto en la parte superior, "
 "Ninguno está desactivado."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "Guardar imagen en archivo"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "Marcador único"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "Marcadores duales"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "Modo"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "Borrar todo"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "Anotaciones"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "Gama"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "Exacto"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "Escala"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "Lineal"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "Logarítmica"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "Cero logarítmico"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "Prefijo preferido"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "Añadir"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "Ocultar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "Mostrar todo el texto"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "Guardar"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Rango automático del eje Y"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "Copiar imagen al portapapeles"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "Exportación de datos visibles"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "Exportar todos los datos"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Exportar"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "Análisis"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Intervalo"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "Mostrar estadísticas"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "Izquierda"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "Derecha"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Apagado"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "Eliminar"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Modo Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "máx"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/fr/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 msgid "Email"
 msgstr "Courriel"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Description"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Editer"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Voir comme Markdown"
 
@@ -649,15 +649,15 @@
 msgid "Do not show again"
 msgstr "Ne plus afficher"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Graphique Intel détecté"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "Multimètre"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "Oscilloscope"
 
@@ -803,15 +803,15 @@
 msgid "Manage"
 msgstr "Gérer"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "Sélectionner le fichier à ouvrir"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "Le nom de ce widget."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "Chemins d'accès"
 
@@ -1111,15 +1111,15 @@
 "Lorsqu'il est activé, le courant circule entre les bornes de courant. "
 "Lorsqu'il est désactivé, le courant ne peut pas circuler entre les bornes de"
 " courant. Dans les configurations de système courantes, cela inhibe "
 "l'alimentation de la cible, ce qui peut être utilisé pour réinitialiser le "
 "dispositif cible par cycle d'alimentation."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "Gamme de courant"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1267,33 +1267,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Le nombre d'échantillons après la fenêtre de la plage de courant utilisée "
 "pour déterminer la moyenne. Cette valeur est ignorée pour tous les autres "
 "types d'IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "Courant"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Active le flux de signaux de courant."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "Tension"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Active le flux de signaux de tension."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Puissance"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Active le flux de signaux d'alimentation."
 
@@ -1514,15 +1514,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Active le flux de signaux de l'entrée générale 3."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "Entrée de déclenchement"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Active le flux de signaux d'entrée de déclenchement."
 
@@ -1533,15 +1533,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "Nom"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope stream buffer"
 
@@ -1761,33 +1761,33 @@
 msgstr "par défaut"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Police de caractères par défaut du Joulescope"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "La source du flux de données statistiques."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "Le signal à afficher."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "charge"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "énergie"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "Affiche le titre de la section des statistiques pour chaque signal."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "Accumulateur"
 
@@ -1857,15 +1857,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Sujet"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Valeur"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Publier l'espion"
 
@@ -1895,15 +1895,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Mise à jour"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "Dispositif"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progrès"
@@ -2466,15 +2466,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Format de l'heure"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "Sélectionner l'appareil source"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 "Le dispositif à utiliser pour la condition de démarrage et la condition "
@@ -2633,115 +2633,115 @@
 msgid "Stop Condition"
 msgstr "Condition d'arrêt"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "Arrêter les actions"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "Affiche l'en-tête de sélection de l'appareil."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "Affiche l'en-tête d'accumulation."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "Afficher les champs de statistiques à droite."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "Afficher un signe + ou -."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "Divisez la quantité par cette valeur."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 "Le diviseur est un nombre à virgule flottante. Le nombre peut éventuellement"
 " être suivi d'unités."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "Les valeurs affichées par ce widget proviennent d'un seul appareil source. "
 "Sélectionnez l'appareil source ici."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "Tenir l'écran"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr ""
 "Lorsque cette option est sélectionnée, elle empêche la mise à jour de "
 "l'affichage."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "L'interface utilisateur comprend également un bouton de maintien des "
 "statistiques globales dans la barre latérale. Lorsque le bouton de maintien "
 "des statistiques globales est sélectionné, ce bouton est désactivé et n'a "
 "aucun effet."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "Les valeurs affichées sont normalement mises à jour avec chaque nouvelle "
 "donnée statistique calculée par l'appareil. Lorsque ce bouton est "
 "sélectionné, l'affichage n'est pas mis à jour. Cependant, les statistiques "
 "continueront à s'accumuler et à se cumuler (si sélectionné)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "Accumuler des valeurs au fil du temps"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "Le courant, la tension et la puissance sont normalement calculés sur un seul"
 " intervalle de fréquence statistique. Appuyez sur ce bouton pour accumuler "
 "les valeurs indéfiniment. Appuyez à nouveau sur ce bouton pour revenir au "
 "fonctionnement normal."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Notez que ce bouton n'affecte pas l'accumulation de charge et d'énergie. Les"
 " deux s'accumulent indéfiniment quel que soit l'état de ce bouton."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "Non présent"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Tenir"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "Accrue"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Gestionnaire d'affichage"
@@ -2787,34 +2787,34 @@
 msgstr "triangle droit"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangle gauche"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "Manuel"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centré"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "Texte"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "Afficher le texte"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "Forme"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Mode Y"
 
@@ -3014,323 +3014,323 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" utilisera la source par défaut qui est normalement configurée à "
 "l'aide du widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "off"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forme d'onde"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "Entrée générale 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "Entrée d'usage général 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "Entrée d'usage général 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "Entrée à usage général 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "La chaîne de filtrage de la source."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "La largeur de la trace."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "L'objectif en termes d'images par seconde."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "Intervalle minimum entre deux repeints en millisecondes."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "Affiche les remplissages minimum et maximum des étendues."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "lignes"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "remplir 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "remplir 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "Indique le nombre d'images par seconde."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "Afficher les statistiques au passage de la souris."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "Afficher les statistiques du tracé à droite."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "Fréquence d'affichage pour les marqueurs doubles et les statistiques."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "Les quantités à afficher par défaut."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "La précision à afficher en chiffres."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "Utiliser le rendu OpenGL."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Épingler les données de gauche (les plus anciennes) pour qu'elles restent "
 "visibles."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Épingler les données de droite (les plus récentes) pour qu'elles restent "
 "visibles."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "L'état de la forme d'onde."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "Les annotations."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "Emplacement de contrôle"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "haut"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "fond"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "La quantité de signal à afficher dans le résumé."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "Mode d'annotation de l'axe X"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "Absolu"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "Relatif"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "Les sous-sources disponibles."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "Les sous-sources sélectionnées pour chaque trace."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorité de la trace : la valeur int la plus élevée est en haut, None est"
 " désactivé."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "Enregistrer l'image dans un fichier"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "Marqueur unique"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "Double marqueur"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "Mode de fonctionnement"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "Tout effacer"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "Annotations"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "Gamme"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "Exact"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "Échelle"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "Linéaire"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "Logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "Zéro logarithmique"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "Préfixe préféré"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "Ajouter"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "Cacher tout le texte"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "Afficher tous les textes"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "Vertical"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "Horizontal"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "Sauvegarder"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Plage automatique de l'axe Y"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "Copier l'image dans le presse-papiers"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "Export visible data"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "Exporter toutes les données"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Exportation"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "Analyse"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Intervalle"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "Afficher les statistiques"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "Gauche"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "Droit"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "Enlever"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Mode Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/it/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 msgid "Email"
 msgstr "E-mail"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "Descrizione"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Modifica"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "Visualizza come Markdown"
 
@@ -647,15 +647,15 @@
 msgid "Do not show again"
 msgstr "Non mostrare di nuovo"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "Rilevata la grafica Intel"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "Multimetro"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "Oscilloscope"
 
@@ -802,15 +802,15 @@
 msgid "Manage"
 msgstr "Gestire"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "Selezionare il file da aprire"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "Il nome di questo widget."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "Percorsi"
 
@@ -1107,15 +1107,15 @@
 "Quando è abilitata, la corrente scorre tra i terminali di corrente. Quando è"
 " disabilitata, la corrente non può scorrere tra i terminali di corrente. "
 "Nelle comuni configurazioni di sistema, questo inibisce l'alimentazione del "
 "target, che può essere utilizzata per resettare il dispositivo di "
 "destinazione."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "Intervallo di corrente"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1263,33 +1263,33 @@
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 "Il numero di campioni dopo la finestra dell'intervallo di corrente viene "
 "utilizzato per determinare la media. Questo valore viene ignorato per tutti "
 "gli altri tipi di IRF."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "Corrente"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "Abilitare lo streaming del segnale di corrente."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "Tensione"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "Abilitare lo streaming del segnale di tensione."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Potenza"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "Abilitare lo streaming del segnale di potenza."
 
@@ -1510,15 +1510,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "Abilitare lo streaming del segnale dell'ingresso 3 per uso generale."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "Ingresso di trigger"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "Abilitare lo streaming del segnale di ingresso di trigger."
 
@@ -1529,15 +1529,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "Nome"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Buffer di flusso Joulescope"
 
@@ -1758,33 +1758,33 @@
 msgstr "predefinito"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Schema di caratteri predefinito di Joulescope"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "La fonte del flusso di dati statistici."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "Il segnale da visualizzare."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "carica"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "energia"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "Mostra il titolo della sezione statistiche per ogni segnale."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "Accumulatore"
 
@@ -1854,15 +1854,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "Argomento"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Valore"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "Pubblicare la spia"
 
@@ -1892,15 +1892,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "Aggiornamento"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "Dispositivo"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "Progressi"
@@ -2468,15 +2468,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticheRegistrazioneConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "Formato temporale"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "Selezionare il dispositivo sorgente"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "Il dispositivo da utilizzare per la condizione di avvio e di arresto."
 
@@ -2632,114 +2632,114 @@
 msgid "Stop Condition"
 msgstr "Condizione di arresto"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "Azioni di arresto"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "Mostra l'intestazione di selezione del dispositivo."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "Mostra l'intestazione di accumulo."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "Mostrare i campi delle statistiche a destra."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "Mostrare un segno + o - iniziale."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "Dividere la quantità per questo valore."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 "Il divisore è un numero in virgola mobile. Il numero può essere "
 "facoltativamente seguito da unità."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 "I valori visualizzati da questo widget provengono da un unico dispositivo "
 "sorgente. Selezionare qui il dispositivo sorgente."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "Tenere il display"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "Se selezionato, impedisce l'aggiornamento del display."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "L'interfaccia utente comprende anche un pulsante di mantenimento delle "
 "statistiche globali nella barra laterale. Quando il pulsante di mantenimento"
 " delle statistiche globali è selezionato, questo pulsante è disabilitato e "
 "non ha alcun effetto."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "I valori visualizzati si aggiornano normalmente con ogni nuovo dato "
 "statistico calcolato dal dispositivo. Quando si seleziona questo pulsante, "
 "il display non viene aggiornato. Tuttavia, le statistiche continueranno ad "
 "accumularsi (se selezionato)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "Accumulare valori nel tempo"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "La corrente, la tensione e la potenza sono normalmente calcolate su un "
 "singolo intervallo di frequenza statistica. Premere questo pulsante per "
 "accumulare i valori a tempo indeterminato. Premere nuovamente per tornare al"
 " funzionamento normale."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 "Si noti che questo pulsante non influisce sull'accumulo di carica e di "
 "energia. Entrambi si accumulano indefinitamente indipendentemente dallo "
 "stato di questo pulsante."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "Non presente"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Tenere"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "Accumulare"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "Visualizza Manager"
@@ -2785,34 +2785,34 @@
 msgstr "triangolo destro"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "triangolo a sinistra"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "Manuale"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "Centrato"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "Testo"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "Mostra testo"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "Forma"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Modalità Y"
 
@@ -3008,322 +3008,322 @@
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 "\"default\" utilizzerà la sorgente predefinita, normalmente configurata "
 "tramite il widget Device Control."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "off"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "Forma d'onda"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "Ingresso generico 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "Ingresso generico 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "Ingresso generico 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "Ingresso generico 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "La stringa del filtro sorgente."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "La larghezza della traccia."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "I fotogrammi al secondo di riferimento."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "L'intervallo minimo tra un repaint e l'altro, in millisecondi."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "Mostra il riempimento delle estensioni minime e massime."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "linee"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "riempimento 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "riempimento 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "Mostra i fotogrammi al secondo."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "Mostra le statistiche al passaggio del mouse."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "Mostrare le statistiche del grafico a destra."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "Mostra la frequenza per i doppi marcatori e le statistiche."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "Le quantità da visualizzare per impostazione predefinita."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "La precisione di visualizzazione in cifre."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "Utilizzare il rendering OpenGL."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 "Appuntate i dati di sinistra (i più vecchi) in modo che rimangano in vista."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 "Appuntate i dati sul lato destro (i più recenti) in modo che rimangano in "
 "vista."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "Lo stato della forma d'onda."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "Le annotazioni."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "Posizione di controllo"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "bottom"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "La quantità di segnale da mostrare nel riepilogo."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "Modalità di annotazione sull'asse X"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "Assoluta"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "Relativo"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "Le sotto-sorgenti disponibili."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "Le sottosorgenti selezionate per ogni traccia."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 "La priorità della traccia: il valore int più alto è in cima, nessuno è "
 "spento."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "Salva l'immagine su file"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "Marcatore singolo"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "Doppio marcatore"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "Modalità"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "Cancella tutto"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "Annotazioni"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "Gamma"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "Esatta"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "Scale"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "Lineare"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "Logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "Zero logaritmico"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "Prefisso preferito"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "Aggiungere"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "Nascondi tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "Mostra tutto il testo"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "Verticale"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "Orizzontale"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "Risparmiare"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Gamma automatica dell'asse Y"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "Copia l'immagine negli appunti"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "Esportazione di dati visibili"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "Esportazione di tutti i dati"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Esportazione"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "Analisi"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Intervallo"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "Zoom"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "Mostra le statistiche"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "A sinistra"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "A destra"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Spento"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "Rimuovere"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Modalità Y"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "max"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/ja/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
 msgid "Email"
 msgstr "電子メール"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "商品概要"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "編集"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "マークダウンで表示"
 
@@ -562,15 +562,15 @@
 msgid "Do not show again"
 msgstr "再表示しない"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "インテル・グラフィックス検出"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "マルチメーター"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "オシロスコープ"
 
@@ -707,15 +707,15 @@
 msgid "Manage"
 msgstr "管理"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "ファイルを選択して開く"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "このウィジェットの名称。"
 
 #: paths.py:31
 msgid "Paths"
 msgstr "経路"
 
@@ -991,15 +991,15 @@
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 "有効にすると、電流端子間に電流が流れます。無効にすると、電流端子間に電流が流れなくなります。一般的なシステム・セットアップでは、これによってターゲット電源が抑制され、ターゲット・デバイスのパワー・サイクル・リセットに使用できます。"
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "電流レンジ"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1123,33 +1123,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "平均を決定するために使用される電流範囲ウィンドウの後のサンプル数。他のIRFタイプではこの値は無視されます。"
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "電流"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "電流信号ストリーミングを有効にします。"
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "電圧"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "電圧信号ストリーミングを有効にします。"
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "パワー"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "電源信号ストリーミングを有効にします。"
 
@@ -1333,15 +1333,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "汎用入力 3 信号ストリーミングを有効にします。"
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "トリガー入力"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "トリガー入力信号ストリーミングを有効にします。"
 
@@ -1352,15 +1352,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope ストリームバッファ"
 
@@ -1563,33 +1563,33 @@
 msgstr "デフォルト"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Joulescopeデフォルトのフォントスキーム"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "統計データ・ストリーム・ソース。"
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "表示する信号。"
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "チャージ"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "エネルギー"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "各信号の統計セクションタイトルを表示します。"
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "アキュムレータ"
 
@@ -1659,15 +1659,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "トピック"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "値"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "スパイを公表する"
 
@@ -1697,15 +1697,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "更新"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "デバイス"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "進捗状況"
@@ -2230,15 +2230,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "統計レコードコンフィグ"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "時間フォーマット"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "ソースデバイスを選択"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "開始条件および停止条件に使用するデバイス。"
 
@@ -2386,98 +2386,98 @@
 msgid "Stop Condition"
 msgstr "停止条件"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "動作停止"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "デバイス選択ヘッダーを表示します。"
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "accrueヘッダを表示します。"
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "右側の統計フィールドを表示します。"
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "先頭の+または-記号を表示します。"
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "この値で量を割る。"
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr "除数は浮動小数点数です。数値の後に単位を付けることもできます。"
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "このウィジェットで表示される値は、単一のソース・デバイスからのものです。ここでソース・デバイスを選択してください。"
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "ディスプレイを保持する"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "選択すると、ディスプレイが更新されないようにします。"
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "UIには、サイドバーにグローバル統計ホールドボタンがあります。グローバル統計ホールドボタンが選択されている場合、このボタンは無効になり、何の効果もありません。"
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "表示値は通常、デバイスによって計算された新しい統計データごとに更新されます。このボタンを選択すると、表示は更新されません。ただし、統計値は蓄積され続けます（選択されている場合）。"
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "時間の経過とともに値を蓄積"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "電流、電圧、電力は通常、1つの統計周波数間隔にわたって計算されます。このボタンを押すと、値が無期限に累積されます。もう一度押すと通常動作に戻ります。"
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "このボタンは電荷とエネルギーの蓄積には影響しません。このボタンの状態に関係なく、どちらも無期限に蓄積されます。"
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "存在しない"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "ホールド"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "増加"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "ビュー・マネージャー"
@@ -2523,34 +2523,34 @@
 msgstr "トライアングルライト"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "マニュアル"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "中心"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "テキスト"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "テキストを表示"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Yモード"
 
@@ -2718,317 +2718,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "「default \"は、通常デバイス制御ウィジェットを使用して設定されるデフォルトのソースを使用します。"
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "オフ"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "波形"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "汎用入力 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "汎用入力 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "汎用入力 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "汎用入力 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "ソース・フィルター・ストリング。"
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "トレース幅。"
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "目標フレーム/秒。"
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "再描画の最小間隔（ミリ秒）。"
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "最小および最大エクステントを表示します。"
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "ライン"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "充填 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "フィル 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "フレーム/秒を表示します。"
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "マウスホバーで統計を表示します。"
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "右側にプロット統計を表示します。"
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "デュアルマーカーと統計のために周波数を表示します。"
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "デフォルトで表示する量。"
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "桁で表示する精度。"
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "OpenGLレンダリングを使用します。"
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "左側（最も古い）のデータをピン留めして、表示されたままにします。"
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "右側（最新）のデータをピン留めして、表示されたままにします。"
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "波形の状態。"
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "注釈"
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "制御位置"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "トップ"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "ボトム"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "サマリーに表示する信号量。"
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "X軸注釈モード"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "絶対値"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "相対"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "利用可能なサブソース"
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "各トレースで選択されたサブソース。"
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "トレースの優先順位：最高 int 値が一番上、None はオフ。"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "画像をファイルに保存"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "シングルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "デュアルマーカー"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "モード"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "すべてクリア"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "注釈"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "測定範囲"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "オート"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "正確"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "スケール"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "リニア"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "対数"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "対数ゼロ"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "優先接頭辞"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "追加"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "すべてのテキストを隠す"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "すべてのテキストを表示"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "節約"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Y軸オートレンジ"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "画像をクリップボードにコピー"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "可視データをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "すべてのデータをエクスポート"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "輸出"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "解析"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "インターバル"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "ズーム"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "統計を表示"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "左"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "右"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "オフ"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "削除"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Yモード"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/joulescope_ui.pot` & `joulescope_ui-1.1.9/joulescope_ui/locale/joulescope_ui.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) 2024 Jetperch LLC
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PROJECT 1.1.8\n"
+"Project-Id-Version: PROJECT 1.1.9\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2024-05-06 17:27-0400\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -284,15 +284,15 @@
 msgid "Email"
 msgstr ""
 
 #: error_window.py:103
 msgid "Description"
 msgstr ""
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr ""
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr ""
 
@@ -542,15 +542,15 @@
 msgid "Do not show again"
 msgstr ""
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr ""
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr ""
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr ""
 
@@ -685,15 +685,15 @@
 msgid "Manage"
 msgstr ""
 
 #: main.py:747
 msgid "Select file to open"
 msgstr ""
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr ""
 
 #: paths.py:31
 msgid "Paths"
 msgstr ""
 
@@ -962,15 +962,15 @@
 "When enabled, current flows between the current terminals. When disabled, "
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr ""
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1086,33 +1086,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr ""
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr ""
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr ""
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr ""
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr ""
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr ""
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr ""
 
@@ -1289,15 +1289,15 @@
 msgid "GPI 3"
 msgstr ""
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr ""
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr ""
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr ""
 
@@ -1308,15 +1308,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr ""
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr ""
 
@@ -1517,33 +1517,33 @@
 msgstr ""
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr ""
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr ""
 
@@ -1613,15 +1613,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr ""
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr ""
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr ""
 
@@ -1651,15 +1651,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr ""
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr ""
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr ""
@@ -2171,15 +2171,15 @@
 msgid "StatisticsRecordConfig"
 msgstr ""
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr ""
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr ""
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr ""
 
@@ -2326,95 +2326,95 @@
 msgid "Stop Condition"
 msgstr ""
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr ""
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr ""
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr ""
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr ""
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr ""
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr ""
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr ""
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr ""
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr ""
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr ""
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr ""
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr ""
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr ""
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr ""
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr ""
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr ""
@@ -2460,34 +2460,34 @@
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr ""
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr ""
 
@@ -2654,317 +2654,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr ""
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr ""
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr ""
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr ""
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr ""
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/ko/LC_MESSAGES/joulescope_ui.po`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 msgid "Email"
 msgstr "이메일"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "설명"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "Edit"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "마크다운으로 보기"
 
@@ -570,15 +570,15 @@
 msgid "Do not show again"
 msgstr "다시 표시하지 않음"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "인텔 그래픽 감지"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "멀티미터"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "오실로스코프"
 
@@ -715,15 +715,15 @@
 msgid "Manage"
 msgstr "관리"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "열 파일 선택"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "이 위젯의 이름입니다."
 
 #: paths.py:31
 msgid "Paths"
 msgstr "경로"
 
@@ -1004,15 +1004,15 @@
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr ""
 "활성화되면 전류 단자 간에 전류가 흐릅니다. 비활성화하면 전류 단자 사이에 전류가 흐르지 않습니다. 일반적인 시스템 설정에서 이 기능은 "
 "목표 전력을 억제하여 목표 장치의 전원 사이클을 리셋하는 데 사용할 수 있습니다."
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "전류 범위"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1139,33 +1139,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "평균을 결정하는 데 사용되는 전류 범위 창 이후의 샘플 수입니다. 다른 모든 IRF 유형에서는 이 값이 무시됩니다."
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "전류"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "전류 신호 스트리밍을 활성화합니다."
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "전압"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "전압 신호 스트리밍을 활성화합니다."
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "Power"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "전원 신호 스트리밍을 활성화합니다."
 
@@ -1354,15 +1354,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "범용 입력 3 신호 스트리밍을 활성화합니다."
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "트리거 입력"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "트리거 입력 신호 스트리밍을 활성화합니다."
 
@@ -1373,15 +1373,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "이름"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "줄스코프 스트림 버퍼"
 
@@ -1586,33 +1586,33 @@
 msgstr "기본값"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "줄스코프 기본 글꼴 체계"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "통계 데이터 스트림 소스."
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "표시할 신호."
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "charge"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "에너지"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "각 신호에 대한 통계 섹션 제목을 표시합니다."
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "어큐뮬레이터"
 
@@ -1682,15 +1682,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "주제"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "Value"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "스파이 게시"
 
@@ -1720,15 +1720,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "업데이트"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "디바이스"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "진행"
@@ -2251,15 +2251,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "StatisticsRecordConfig"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "시간 형식"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "소스 디바이스 선택"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "시작 조건 및 중지 조건에 사용할 장치입니다."
 
@@ -2409,100 +2409,100 @@
 msgid "Stop Condition"
 msgstr "정지 조건"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "동작 중지"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "장치 선택 헤더를 표시합니다."
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "발생 헤더를 표시합니다."
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "오른쪽에 통계 필드가 표시됩니다."
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "선행 + 또는 - 기호를 표시합니다."
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "수량을 이 값으로 나눕니다."
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr "제수는 부동 소수점 숫자입니다. 숫자 뒤에 선택적으로 단위를 붙일 수 있습니다."
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "이 위젯에 표시되는 값은 단일 소스 장치에서 가져온 것입니다. 여기에서 소스 장치를 선택하세요."
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "디스플레이 잡기"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "이 옵션을 선택하면 디스플레이가 업데이트되지 않습니다."
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr ""
 "UI에는 사이드바에 글로벌 통계 보류 버튼도 있습니다. 글로벌 통계 보류 버튼을 선택하면 이 버튼은 비활성화되며 아무런 효과가 없습니다."
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr ""
 "표시된 값은 일반적으로 장치에서 계산된 새로운 통계 데이터에 따라 업데이트됩니다. 이 버튼을 선택하면 디스플레이가 업데이트되지 않습니다."
 " 그러나 통계는 계속 누적되어 누적됩니다(선택한 경우)."
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "시간에 따른 값 누적"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr ""
 "전류, 전압 및 전력은 일반적으로 단일 통계 주파수 간격에 걸쳐 계산됩니다. 이 버튼을 누르면 값이 무한정 누적됩니다. 다시 누르면 정상"
 " 작동으로 돌아갑니다."
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "이 버튼은 충전 및 에너지 축적에 영향을 주지 않습니다. 둘 다 이 버튼 상태에 관계없이 무기한으로 누적됩니다."
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "현재 없음"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "Hold"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "증가"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "뷰 관리자"
@@ -2548,34 +2548,34 @@
 msgstr "삼각형 오른쪽"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "왼쪽 삼각형"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "매뉴얼"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "중심"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "텍스트"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "텍스트 표시"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "모양"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 모드"
 
@@ -2744,317 +2744,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "\"기본\"은 일반적으로 장치 제어 위젯을 사용하여 구성되는 기본 소스를 사용합니다."
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "off"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "파형"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "범용 입력 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "범용 입력 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "범용 입력 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "범용 입력 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "소스 필터 문자열입니다."
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "트레이스 폭."
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "초당 목표 프레임."
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 Hz"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 Hz"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 Hz"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "밀리초 단위의 최소 재도장 간격입니다."
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "최소 및 최대 범위 채우기를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "lines"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "채우기 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "채우기 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "초당 프레임을 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "마우스 호버에 대한 통계를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "오른쪽에 플롯 통계가 표시됩니다."
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "듀얼 마커 및 통계에 대한 주파수를 표시합니다."
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "기본적으로 표시되는 수량입니다."
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "숫자로 표시되는 정밀도."
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "OpenGL 렌더링을 사용합니다."
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "왼쪽(가장 오래된) 데이터를 고정하여 계속 볼 수 있도록 합니다."
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "오른쪽(최신) 데이터를 고정하여 계속 볼 수 있도록 합니다."
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "파형 상태."
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "주석."
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "제어 위치"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "top"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "bottom"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "요약에 표시할 신호 양입니다."
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "X축 주석 모드"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "절대"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "상대"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "사용 가능한 하위 소스."
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "각 트레이스에 대해 선택된 하위 소스."
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "트레이스 우선순위: 가장 높은 int 값이 위에 있고 없음은 꺼져 있습니다."
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "파일에 이미지 저장"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "단일 마커"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "듀얼 마커"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "모드"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "모두 지우기"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "주석"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "범위"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "Auto"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "정확한"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "스케일"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "선형"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "로그"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "로그 제로"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "기본 접두사"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "추가"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "모든 텍스트 숨기기"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "모든 텍스트 표시"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "수직"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "수평"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "저장"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Y축 자동 범위"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "이미지를 클립보드에 복사"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "가시 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "모든 데이터 내보내기"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "Export"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "분석"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "Interval"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "줌"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "통계 보기"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "왼쪽"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "Right"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "Off"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "제거"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Y 모드"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "최대"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo` & `joulescope_ui-1.1.9/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.mo`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po` & `joulescope_ui-1.1.9/joulescope_ui/locale/zh/LC_MESSAGES/joulescope_ui.po`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
 msgid "Email"
 msgstr "电子邮件"
 
 #: error_window.py:103
 msgid "Description"
 msgstr "描述"
 
-#: error_window.py:112 widgets/waveform/waveform_widget.py:3403
+#: error_window.py:112 widgets/waveform/waveform_widget.py:3367
 msgid "Edit"
 msgstr "编辑"
 
 #: error_window.py:113
 msgid "View as Markdown"
 msgstr "以 Markdown 格式查看"
 
@@ -551,15 +551,15 @@
 msgid "Do not show again"
 msgstr "不再显示"
 
 #: intel_graphics_dialog.py:91
 msgid "Intel graphics detected"
 msgstr "检测到英特尔显卡"
 
-#: main.py:69 widgets/value/value_widget.py:660
+#: main.py:69 widgets/value/value_widget.py:664
 msgid "Multimeter"
 msgstr "万用表"
 
 #: main.py:70
 msgid "Oscilloscope"
 msgstr "示波器"
 
@@ -694,15 +694,15 @@
 msgid "Manage"
 msgstr "管理"
 
 #: main.py:747
 msgid "Select file to open"
 msgstr "选择要打开的文件"
 
-#: paths.py:30 styles/manager.py:46
+#: paths.py:30 styles/manager.py:52
 msgid "The name for this widget."
 msgstr "该部件的名称。"
 
 #: paths.py:31
 msgid "Paths"
 msgstr "路径"
 
@@ -971,15 +971,15 @@
 "When enabled, current flows between the current terminals. When disabled, "
 "current cannot flow between the current terminals. In common system setups, "
 "this inhibits target power, which can be used to power cycle reset the "
 "target device."
 msgstr "启用时，电流在电流端子之间流动。禁用时，电流不会在电流端之间流动。在常见的系统设置中，这会抑制目标电源，可用于对目标设备进行电源循环复位。"
 
 #: devices/jsdrv/js110.py:147 devices/jsdrv/js220.py:163
-#: widgets/waveform/waveform_widget.py:109
+#: widgets/waveform/waveform_widget.py:110
 msgid "Current range"
 msgstr "电流范围"
 
 #: devices/jsdrv/js110.py:149
 msgid ""
 "Configure the J110's current range. Most applications should use the "
 "default, \"auto\"."
@@ -1098,33 +1098,33 @@
 #: devices/jsdrv/js110.py:255
 msgid ""
 "The number of samples after the current range window used to determine the "
 "mean. This value is ignored for all other IRF types."
 msgstr "用于确定平均值的电流范围窗口后的采样数目。对于所有其他 IRF 类型，该值将被忽略。"
 
 #: devices/jsdrv/js110.py:269 devices/jsdrv/js220.py:332
-#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:104
+#: widgets/device_control/fuse.py:103 widgets/waveform/waveform_widget.py:105
 msgid "Current"
 msgstr "电流"
 
 #: devices/jsdrv/js110.py:270 devices/jsdrv/js220.py:333
 msgid "Enable the current signal streaming."
 msgstr "启用电流信号流。"
 
 #: devices/jsdrv/js110.py:278 devices/jsdrv/js220.py:341
-#: widgets/waveform/waveform_widget.py:105
+#: widgets/waveform/waveform_widget.py:106
 msgid "Voltage"
 msgstr "电压"
 
 #: devices/jsdrv/js110.py:279 devices/jsdrv/js220.py:342
 msgid "Enable the voltage signal streaming."
 msgstr "启用电压信号流。"
 
 #: devices/jsdrv/js110.py:287 devices/jsdrv/js220.py:350
-#: widgets/waveform/waveform_widget.py:106
+#: widgets/waveform/waveform_widget.py:107
 msgid "Power"
 msgstr "功率"
 
 #: devices/jsdrv/js110.py:288 devices/jsdrv/js220.py:351
 msgid "Enable the power signal streaming."
 msgstr "启用电源信号流。"
 
@@ -1303,15 +1303,15 @@
 msgid "GPI 3"
 msgstr "GPI 3"
 
 #: devices/jsdrv/js220.py:402
 msgid "Enable the general purpose input 3 signal streaming."
 msgstr "启用通用输入 3 信号流。"
 
-#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:123
+#: devices/jsdrv/js220.py:410 widgets/waveform/waveform_widget.py:124
 msgid "Trigger input"
 msgstr "触发输入"
 
 #: devices/jsdrv/js220.py:411
 msgid "Enable the trigger input signal streaming."
 msgstr "启用触发输入信号流。"
 
@@ -1322,15 +1322,15 @@
 #: devices/jsdrv/jsdrv_stream_buffer.py:44
 #: devices/jsdrv/jsdrv_stream_buffer.py:93
 #: devices/jsdrv/jsdrv_stream_buffer.py:107 plugins/selector.py:58
 #: widgets/settings/settings_widget.py:85
 #: widgets/settings/settings_widget.py:266
 #: widgets/settings/settings_widget.py:364
 #: widgets/settings/settings_widget.py:431
-#: widgets/waveform/waveform_widget.py:3110
+#: widgets/waveform/waveform_widget.py:3074
 msgid "Name"
 msgstr "名称"
 
 #: devices/jsdrv/jsdrv_stream_buffer.py:45
 msgid "Joulescope stream buffer"
 msgstr "Joulescope 数据流缓冲器"
 
@@ -1532,33 +1532,33 @@
 msgstr "默认值"
 
 #: styles/font_scheme.py:22
 msgid "Joulescope default font scheme"
 msgstr "Joulescope 默认字体方案"
 
 #: widgets/accumulator/accumulator_widget.py:27
-#: widgets/value/value_widget.py:31
+#: widgets/value/value_widget.py:32
 msgid "The statistics data stream source."
 msgstr "统计数据流源。"
 
 #: widgets/accumulator/accumulator_widget.py:32
-#: widgets/value/value_widget.py:81
+#: widgets/value/value_widget.py:82
 msgid "The signal to display."
 msgstr "要显示的信号。"
 
 #: widgets/accumulator/accumulator_widget.py:34
 msgid "charge"
 msgstr "电荷"
 
 #: widgets/accumulator/accumulator_widget.py:35
 msgid "energy"
 msgstr "能量"
 
 #: widgets/accumulator/accumulator_widget.py:41
-#: widgets/value/value_widget.py:56
+#: widgets/value/value_widget.py:57
 msgid "Show the statistics section title for each signal."
 msgstr "显示每个信号的统计部分标题。"
 
 #: widgets/accumulator/accumulator_widget.py:48
 msgid "Accumulator"
 msgstr "累加器"
 
@@ -1628,15 +1628,15 @@
 
 #: widgets/developer/publish_spy_widget.py:20
 #: widgets/developer/publish_spy_widget.py:21
 msgid "Topic"
 msgstr "主题"
 
 #: widgets/developer/publish_spy_widget.py:21
-#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:669
+#: widgets/settings/settings_widget.py:87 widgets/value/value_widget.py:673
 msgid "Value"
 msgstr "值"
 
 #: widgets/developer/publish_spy_widget.py:24
 msgid "Publish Spy"
 msgstr "发布间谍"
 
@@ -1666,15 +1666,15 @@
 
 #: widgets/device_control/device_update_dialog.py:24
 #: widgets/device_control/device_update_dialog.py:45
 msgid "Update"
 msgstr "更新"
 
 #: widgets/device_control/device_update_dialog.py:25
-#: widgets/value/value_widget.py:155
+#: widgets/value/value_widget.py:156
 msgid "Device"
 msgstr "器件"
 
 #: widgets/device_control/device_update_dialog.py:27
 #: widgets/progress_bar/progress_bar_widget.py:59
 msgid "Progress"
 msgstr "进展"
@@ -2188,15 +2188,15 @@
 msgid "StatisticsRecordConfig"
 msgstr "统计记录配置"
 
 #: widgets/statistics_record/statistics_record_config_widget.py:123
 msgid "Time Format"
 msgstr "时间格式"
 
-#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:94
+#: widgets/trigger/trigger_widget.py:41 widgets/value/value_widget.py:95
 msgid "Select the source device"
 msgstr "选择源器件"
 
 #: widgets/trigger/trigger_widget.py:42
 msgid "The device to use for the start condition and stop condition."
 msgstr "用于启动条件和停止条件的设备。"
 
@@ -2343,95 +2343,95 @@
 msgid "Stop Condition"
 msgstr "停止条件"
 
 #: widgets/trigger/trigger_widget.py:860
 msgid "Stop Actions"
 msgstr "停止操作"
 
-#: widgets/value/value_widget.py:36
+#: widgets/value/value_widget.py:37
 msgid "Show the device selection header."
 msgstr "显示设备选择标题。"
 
-#: widgets/value/value_widget.py:41
+#: widgets/value/value_widget.py:42
 msgid "Show the accrue header."
 msgstr "显示累加标题。"
 
-#: widgets/value/value_widget.py:46
+#: widgets/value/value_widget.py:47
 msgid "Show the statistics fields at the right."
 msgstr "显示右侧的统计字段。"
 
-#: widgets/value/value_widget.py:51
+#: widgets/value/value_widget.py:52
 msgid "Show a leading + or - sign."
 msgstr "显示前导 + 或 - 符号。"
 
-#: widgets/value/value_widget.py:62
+#: widgets/value/value_widget.py:63
 msgid "Divide the quantity by this value."
 msgstr "用这个值除以数量。"
 
-#: widgets/value/value_widget.py:63
+#: widgets/value/value_widget.py:64
 msgid ""
 "The divisor is a floating point number. The number may optionally be "
 "followed by units."
 msgstr "除数是浮点数。数字后面可以选择单位。"
 
-#: widgets/value/value_widget.py:95
+#: widgets/value/value_widget.py:96
 msgid ""
 "The values displayed by this widget come from a single source device. Select"
 " the source device here."
 msgstr "此 widget 显示的值来自单个源器件。在此选择源设备。"
 
-#: widgets/value/value_widget.py:101
+#: widgets/value/value_widget.py:102
 msgid "Hold the display"
 msgstr "保持显示"
 
-#: widgets/value/value_widget.py:103
+#: widgets/value/value_widget.py:104
 msgid "When selected, prevent the display from updating."
 msgstr "选中时，防止显示更新。"
 
-#: widgets/value/value_widget.py:104
+#: widgets/value/value_widget.py:105
 msgid ""
 "The UI also includes a global statistics hold button on the sidebar. When "
 "the global statistics hold button is selected, this button is disabled and "
 "has no effect."
 msgstr "用户界面侧边栏上还有一个全局统计保持按钮。选择全局统计保持按钮后，该按钮将被禁用，没有任何作用。"
 
-#: widgets/value/value_widget.py:107
+#: widgets/value/value_widget.py:108
 msgid ""
 "The displayed values normally update with each new statistics data computed "
 "by the device. When this button is selected, the display will not be "
 "updated. However, the statistics will continue accumulate and accrue (if "
 "selected)."
 msgstr "显示值通常随设备计算的每个新统计数据更新。选择此按钮后，显示值将不会更新。但是，统计数据将继续累积（如果选择）。"
 
-#: widgets/value/value_widget.py:114
+#: widgets/value/value_widget.py:115
 msgid "Accrue values over time"
 msgstr "随时间累积值"
 
-#: widgets/value/value_widget.py:116
+#: widgets/value/value_widget.py:117
 msgid ""
 "Current, voltage, and power are normally computed over a single statistics "
 "frequency interval. Press this button to accrue the values indefinitely. "
 "Press again to return to normal operation."
 msgstr "电流、电压和功率通常在单个统计频率间隔内计算。按下此按钮可无限累积数值。再次按下则返回正常操作。"
 
-#: widgets/value/value_widget.py:120
+#: widgets/value/value_widget.py:121
 msgid ""
 "Note that this button does not affect the charge and energy accumulation. "
 "Both accumulate indefinitely regardless of this button state."
 msgstr "请注意，该按钮不会影响电荷和能量的累积。无论按钮状态如何，两者都会无限累积。"
 
-#: widgets/value/value_widget.py:203
+#: widgets/value/value_widget.py:204
 msgid "Not present"
 msgstr "不存在"
 
-#: widgets/value/value_widget.py:223
+#: widgets/value/value_widget.py:224
 msgid "Hold"
 msgstr "保持"
 
-#: widgets/value/value_widget.py:231
+#: widgets/value/value_widget.py:232
 msgid "Accrue"
 msgstr "增加"
 
 #: widgets/view_manager/view_manager_widget.py:108
 #: widgets/view_manager/view_manager_widget.py:174
 msgid "View Manager"
 msgstr "查看管理器"
@@ -2477,34 +2477,34 @@
 msgstr "右三角"
 
 #: widgets/waveform/text_annotation.py:62
 msgid "triangle left"
 msgstr "左三角形"
 
 #: widgets/waveform/text_annotation.py:66
-#: widgets/waveform/waveform_widget.py:3056
+#: widgets/waveform/waveform_widget.py:3020
 msgid "Manual"
 msgstr "手册"
 
 #: widgets/waveform/text_annotation.py:67
 msgid "Centered"
 msgstr "居中"
 
 #: widgets/waveform/text_annotation.py:99
-#: widgets/waveform/waveform_widget.py:3173
+#: widgets/waveform/waveform_widget.py:3137
 msgid "Text"
 msgstr "文本"
 
 #: widgets/waveform/text_annotation.py:107
-#: widgets/waveform/waveform_widget.py:3404
+#: widgets/waveform/waveform_widget.py:3368
 msgid "Show text"
 msgstr "显示文本"
 
 #: widgets/waveform/text_annotation.py:116
-#: widgets/waveform/waveform_widget.py:3416
+#: widgets/waveform/waveform_widget.py:3380
 msgid "Shape"
 msgstr "形状"
 
 #: widgets/waveform/text_annotation.py:126
 msgid "Y Mode"
 msgstr "Y 模式"
 
@@ -2671,317 +2671,317 @@
 #: widgets/waveform/waveform_source_widget.py:40
 msgid ""
 "\"default\" will use the default source which is normally configured using "
 "the Device Control widget."
 msgstr "\"默认 \"将使用默认源，该源通常使用设备控制 widget 进行配置。"
 
 #: widgets/waveform/waveform_source_widget.py:104
-#: widgets/waveform/waveform_widget.py:401
-#: widgets/waveform/waveform_widget.py:478
+#: widgets/waveform/waveform_widget.py:375
+#: widgets/waveform/waveform_widget.py:452
 msgid "off"
 msgstr "关闭"
 
 #: widgets/waveform/waveform_widget.py:43
 msgid "Waveform"
 msgstr "波形"
 
-#: widgets/waveform/waveform_widget.py:119
+#: widgets/waveform/waveform_widget.py:120
 msgid "General purpose input 0"
 msgstr "通用输入 0"
 
-#: widgets/waveform/waveform_widget.py:120
+#: widgets/waveform/waveform_widget.py:121
 msgid "General purpose input 1"
 msgstr "通用输入 1"
 
-#: widgets/waveform/waveform_widget.py:121
+#: widgets/waveform/waveform_widget.py:122
 msgid "General purpose input 2"
 msgstr "通用输入 2"
 
-#: widgets/waveform/waveform_widget.py:122
+#: widgets/waveform/waveform_widget.py:123
 msgid "General purpose input 3"
 msgstr "通用输入 3"
 
-#: widgets/waveform/waveform_widget.py:357
+#: widgets/waveform/waveform_widget.py:331
 msgid "The source filter string."
 msgstr "源滤波器串。"
 
-#: widgets/waveform/waveform_widget.py:368
+#: widgets/waveform/waveform_widget.py:342
 msgid "The trace width."
 msgstr "轨迹宽度。"
 
-#: widgets/waveform/waveform_widget.py:383
+#: widgets/waveform/waveform_widget.py:357
 msgid "The target frames per second."
 msgstr "目标帧/秒。"
 
-#: widgets/waveform/waveform_widget.py:385
+#: widgets/waveform/waveform_widget.py:359
 msgid "vsync"
 msgstr "vsync"
 
-#: widgets/waveform/waveform_widget.py:386
+#: widgets/waveform/waveform_widget.py:360
 msgid "20 Hz"
 msgstr "20 赫兹"
 
-#: widgets/waveform/waveform_widget.py:387
+#: widgets/waveform/waveform_widget.py:361
 msgid "10 Hz"
 msgstr "10 赫兹"
 
-#: widgets/waveform/waveform_widget.py:388
+#: widgets/waveform/waveform_widget.py:362
 msgid "5 Hz"
 msgstr "5 赫兹"
 
-#: widgets/waveform/waveform_widget.py:394
+#: widgets/waveform/waveform_widget.py:368
 msgid "The minimum interval between repaint in milliseconds."
 msgstr "以毫秒为单位的最小重绘间隔。"
 
-#: widgets/waveform/waveform_widget.py:399
+#: widgets/waveform/waveform_widget.py:373
 msgid "Show the minimum and maximum extents fill."
 msgstr "显示填充的最小和最大范围。"
 
-#: widgets/waveform/waveform_widget.py:402
+#: widgets/waveform/waveform_widget.py:376
 msgid "lines"
 msgstr "线路"
 
-#: widgets/waveform/waveform_widget.py:403
+#: widgets/waveform/waveform_widget.py:377
 msgid "fill 1"
 msgstr "填充 1"
 
-#: widgets/waveform/waveform_widget.py:404
+#: widgets/waveform/waveform_widget.py:378
 msgid "fill 2"
 msgstr "填充 2"
 
-#: widgets/waveform/waveform_widget.py:410
+#: widgets/waveform/waveform_widget.py:384
 msgid "Show the frames per second."
 msgstr "显示每秒帧数。"
 
-#: widgets/waveform/waveform_widget.py:415
+#: widgets/waveform/waveform_widget.py:389
 msgid "Show the statistics on mouse hover."
 msgstr "鼠标悬停时显示统计数据。"
 
-#: widgets/waveform/waveform_widget.py:420
+#: widgets/waveform/waveform_widget.py:394
 msgid "Show the plot statistics on the right."
 msgstr "在右侧显示绘图统计数据。"
 
-#: widgets/waveform/waveform_widget.py:425
+#: widgets/waveform/waveform_widget.py:399
 msgid "Show frequency for dual markers and statistics."
 msgstr "显示频率，用于双重标记和统计。"
 
-#: widgets/waveform/waveform_widget.py:430
+#: widgets/waveform/waveform_widget.py:404
 msgid "The quantities to display by default."
 msgstr "默认显示的量。"
 
-#: widgets/waveform/waveform_widget.py:436
+#: widgets/waveform/waveform_widget.py:410
 msgid "The precision to display in digits."
 msgstr "以位数显示的精度。"
 
-#: widgets/waveform/waveform_widget.py:442
+#: widgets/waveform/waveform_widget.py:416
 msgid "Use OpenGL rendering."
 msgstr "使用 OpenGL 渲染。"
 
-#: widgets/waveform/waveform_widget.py:453
+#: widgets/waveform/waveform_widget.py:427
 msgid "Pin the left side (oldest) data so that it stays in view."
 msgstr "钉住左侧（最旧）数据，使其保持在视图中。"
 
-#: widgets/waveform/waveform_widget.py:458
+#: widgets/waveform/waveform_widget.py:432
 msgid "Pin the right side (newest) data so that it stays in view."
 msgstr "钉住右侧（最新）数据，使其保持在视图中。"
 
-#: widgets/waveform/waveform_widget.py:463
+#: widgets/waveform/waveform_widget.py:437
 msgid "The waveform state."
 msgstr "波形状态。"
 
-#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:443
 msgid "The annotations."
 msgstr "注释。"
 
-#: widgets/waveform/waveform_widget.py:475
+#: widgets/waveform/waveform_widget.py:449
 msgid "Control location"
 msgstr "控制位置"
 
-#: widgets/waveform/waveform_widget.py:479
+#: widgets/waveform/waveform_widget.py:453
 msgid "top"
 msgstr "顶部"
 
-#: widgets/waveform/waveform_widget.py:480
+#: widgets/waveform/waveform_widget.py:454
 msgid "bottom"
 msgstr "底部"
 
-#: widgets/waveform/waveform_widget.py:485
+#: widgets/waveform/waveform_widget.py:459
 msgid "The signal quantity to show in the summary."
 msgstr "要在摘要中显示的信号量。"
 
-#: widgets/waveform/waveform_widget.py:491
+#: widgets/waveform/waveform_widget.py:465
 msgid "X-axis annotation mode"
 msgstr "X 轴注释模式"
 
-#: widgets/waveform/waveform_widget.py:494
-#: widgets/waveform/waveform_widget.py:2936
+#: widgets/waveform/waveform_widget.py:468
+#: widgets/waveform/waveform_widget.py:2900
 msgid "Absolute"
 msgstr "绝对值"
 
-#: widgets/waveform/waveform_widget.py:495
-#: widgets/waveform/waveform_widget.py:2941
+#: widgets/waveform/waveform_widget.py:469
+#: widgets/waveform/waveform_widget.py:2905
 msgid "Relative"
 msgstr "相对值"
 
-#: widgets/waveform/waveform_widget.py:501
+#: widgets/waveform/waveform_widget.py:475
 msgid "The available subsources."
 msgstr "可用的子源。"
 
-#: widgets/waveform/waveform_widget.py:507
+#: widgets/waveform/waveform_widget.py:481
 msgid "The selected subsources for each trace."
 msgstr "每个跟踪所选的子源。"
 
-#: widgets/waveform/waveform_widget.py:513
+#: widgets/waveform/waveform_widget.py:487
 msgid "The trace priority: highest int value on top, None is off."
 msgstr "跟踪优先级：最高 int 值在顶部，无则关闭。"
 
-#: widgets/waveform/waveform_widget.py:2883
-#: widgets/waveform/waveform_widget.py:3185
+#: widgets/waveform/waveform_widget.py:2847
+#: widgets/waveform/waveform_widget.py:3149
 msgid "Save image to file"
 msgstr "将图像保存到文件"
 
-#: widgets/waveform/waveform_widget.py:2930
-#: widgets/waveform/waveform_widget.py:2999
+#: widgets/waveform/waveform_widget.py:2894
+#: widgets/waveform/waveform_widget.py:2963
 msgid "Single marker"
 msgstr "单标记"
 
-#: widgets/waveform/waveform_widget.py:2931
-#: widgets/waveform/waveform_widget.py:3000
+#: widgets/waveform/waveform_widget.py:2895
+#: widgets/waveform/waveform_widget.py:2964
 msgid "Dual markers"
 msgstr "双标记"
 
-#: widgets/waveform/waveform_widget.py:2933
+#: widgets/waveform/waveform_widget.py:2897
 msgid "Mode"
 msgstr "模式"
 
-#: widgets/waveform/waveform_widget.py:2946
-#: widgets/waveform/waveform_widget.py:3001
-#: widgets/waveform/waveform_widget.py:3161
-#: widgets/waveform/waveform_widget.py:3179
+#: widgets/waveform/waveform_widget.py:2910
+#: widgets/waveform/waveform_widget.py:2965
+#: widgets/waveform/waveform_widget.py:3125
+#: widgets/waveform/waveform_widget.py:3143
 msgid "Clear all"
 msgstr "全部清除"
 
-#: widgets/waveform/waveform_widget.py:2957
-#: widgets/waveform/waveform_widget.py:3046
-#: widgets/waveform/waveform_widget.py:3167
+#: widgets/waveform/waveform_widget.py:2921
+#: widgets/waveform/waveform_widget.py:3010
+#: widgets/waveform/waveform_widget.py:3131
 msgid "Annotations"
 msgstr "注释"
 
-#: widgets/waveform/waveform_widget.py:3049
+#: widgets/waveform/waveform_widget.py:3013
 msgid "Range"
 msgstr "范围"
 
-#: widgets/waveform/waveform_widget.py:3053
-#: widgets/waveform/waveform_widget.py:3384
+#: widgets/waveform/waveform_widget.py:3017
+#: widgets/waveform/waveform_widget.py:3348
 msgid "Auto"
 msgstr "自动"
 
-#: widgets/waveform/waveform_widget.py:3059
+#: widgets/waveform/waveform_widget.py:3023
 msgid "Exact"
 msgstr "精确"
 
-#: widgets/waveform/waveform_widget.py:3068
+#: widgets/waveform/waveform_widget.py:3032
 msgid "Scale"
 msgstr "规模"
 
-#: widgets/waveform/waveform_widget.py:3071
+#: widgets/waveform/waveform_widget.py:3035
 msgid "Linear"
 msgstr "线性"
 
-#: widgets/waveform/waveform_widget.py:3076
+#: widgets/waveform/waveform_widget.py:3040
 msgid "Logarithmic"
 msgstr "对数"
 
-#: widgets/waveform/waveform_widget.py:3084
+#: widgets/waveform/waveform_widget.py:3048
 msgid "Logarithmic zero"
 msgstr "对数零"
 
-#: widgets/waveform/waveform_widget.py:3098
+#: widgets/waveform/waveform_widget.py:3062
 msgid "Preferred prefix"
 msgstr "首选前缀"
 
-#: widgets/waveform/waveform_widget.py:3158
+#: widgets/waveform/waveform_widget.py:3122
 msgid "Add"
 msgstr "添加"
 
-#: widgets/waveform/waveform_widget.py:3159
+#: widgets/waveform/waveform_widget.py:3123
 msgid "Hide all text"
 msgstr "隐藏所有文本"
 
-#: widgets/waveform/waveform_widget.py:3160
+#: widgets/waveform/waveform_widget.py:3124
 msgid "Show all text"
 msgstr "显示所有文本"
 
-#: widgets/waveform/waveform_widget.py:3168
+#: widgets/waveform/waveform_widget.py:3132
 msgid "Vertical"
 msgstr "垂直"
 
-#: widgets/waveform/waveform_widget.py:3171
+#: widgets/waveform/waveform_widget.py:3135
 msgid "Horizontal"
 msgstr "水平"
 
-#: widgets/waveform/waveform_widget.py:3177
+#: widgets/waveform/waveform_widget.py:3141
 msgid "Save"
 msgstr "保存"
 
-#: widgets/waveform/waveform_widget.py:3182
+#: widgets/waveform/waveform_widget.py:3146
 msgid "Y-axis auto range"
 msgstr "Y 轴自动量程"
 
-#: widgets/waveform/waveform_widget.py:3186
+#: widgets/waveform/waveform_widget.py:3150
 msgid "Copy image to clipboard"
 msgstr "将图像复制到剪贴板"
 
-#: widgets/waveform/waveform_widget.py:3187
+#: widgets/waveform/waveform_widget.py:3151
 msgid "Export visible data"
 msgstr "导出可见数据"
 
-#: widgets/waveform/waveform_widget.py:3188
+#: widgets/waveform/waveform_widget.py:3152
 msgid "Export all data"
 msgstr "导出所有数据"
 
-#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3324
 msgid "Export"
 msgstr "出口"
 
-#: widgets/waveform/waveform_widget.py:3361
+#: widgets/waveform/waveform_widget.py:3325
 msgid "Analysis"
 msgstr "分析"
 
-#: widgets/waveform/waveform_widget.py:3369
+#: widgets/waveform/waveform_widget.py:3333
 msgid "Interval"
 msgstr "间隔"
 
-#: widgets/waveform/waveform_widget.py:3378
+#: widgets/waveform/waveform_widget.py:3342
 msgid "Zoom"
 msgstr "放大"
 
-#: widgets/waveform/waveform_widget.py:3382
+#: widgets/waveform/waveform_widget.py:3346
 msgid "Show statistics"
 msgstr "显示统计数据"
 
-#: widgets/waveform/waveform_widget.py:3387
+#: widgets/waveform/waveform_widget.py:3351
 msgid "Left"
 msgstr "左侧"
 
-#: widgets/waveform/waveform_widget.py:3390
+#: widgets/waveform/waveform_widget.py:3354
 msgid "Right"
 msgstr "正确"
 
-#: widgets/waveform/waveform_widget.py:3393
+#: widgets/waveform/waveform_widget.py:3357
 msgid "Off"
 msgstr "关闭"
 
-#: widgets/waveform/waveform_widget.py:3396
-#: widgets/waveform/waveform_widget.py:3424
-#: widgets/waveform/waveform_widget.py:3454
+#: widgets/waveform/waveform_widget.py:3360
+#: widgets/waveform/waveform_widget.py:3388
+#: widgets/waveform/waveform_widget.py:3418
 msgid "Remove"
 msgstr "删除"
 
-#: widgets/waveform/waveform_widget.py:3407
+#: widgets/waveform/waveform_widget.py:3371
 msgid "Y mode"
 msgstr "Y 模式"
 
 #: widgets/waveform/y_range_widget.py:67
 msgid "max"
 msgstr "最大值"
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/logging_util.py` & `joulescope_ui-1.1.9/joulescope_ui/logging_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/main.py` & `joulescope_ui-1.1.9/joulescope_ui/main.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/mem_leak_debugger.py` & `joulescope_ui-1.1.9/joulescope_ui/mem_leak_debugger.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/metadata.py` & `joulescope_ui-1.1.9/joulescope_ui/metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/paths.py` & `joulescope_ui-1.1.9/joulescope_ui/paths.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/plugins/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/plugins/manager.py` & `joulescope_ui-1.1.9/joulescope_ui/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/plugins/selector.py` & `joulescope_ui-1.1.9/joulescope_ui/plugins/selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/plugins/test/plugins/p1/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/plugins/test/plugins/p1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/plugins/test/test_manager.py` & `joulescope_ui-1.1.9/joulescope_ui/plugins/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/process_monitor.py` & `joulescope_ui-1.1.9/joulescope_ui/process_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/profile.py` & `joulescope_ui-1.1.9/joulescope_ui/profile.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/pubsub.py` & `joulescope_ui-1.1.9/joulescope_ui/pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/pubsub_aggregator.py` & `joulescope_ui-1.1.9/joulescope_ui/pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/pubsub_callable.py` & `joulescope_ui-1.1.9/joulescope_ui/pubsub_callable.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/pubsub_proxy.py` & `joulescope_ui-1.1.9/joulescope_ui/pubsub_proxy.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tool.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/cdf.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/cdf.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/frequency.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/frequency.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/histogram.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/histogram.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/max_window.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/max_window.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/plugin_helpers.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/range_tools/usb_inrush.py` & `joulescope_ui-1.1.9/joulescope_ui/range_tools/usb_inrush.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/reporter.py` & `joulescope_ui-1.1.9/joulescope_ui/reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background.svg` & `joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/dmg_background@2x.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/dmg_background@2x.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.ico` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.ico`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_128x128@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_128x128@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_16x16@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_16x16@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_256x256@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_256x256@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_32x32@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_32x32@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_512x512@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_512x512@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icon.iconset/icon_64x64@2.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/icon.iconset/icon_64x64@2.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/icons.svg` & `joulescope_ui-1.1.9/joulescope_ui/resources/icons.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/logo-large.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/logo-large.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/logo-small.png` & `joulescope_ui-1.1.9/joulescope_ui/resources/logo-small.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources/zoom.svg` & `joulescope_ui-1.1.9/joulescope_ui/resources/zoom.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources.py` & `joulescope_ui-1.1.9/joulescope_ui/resources.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/resources.rcc` & `joulescope_ui-1.1.9/joulescope_ui/resources.rcc`

 * *Files 1% similar despite different names*

```diff
@@ -1416,11 +1416,11 @@
 00005870: 5f00 3600 3400 7800 3600 3400 2e00 6900  _.6.4.x.6.4...i.
 00005880: 6300 6f00 0e03 14ce 8700 6c00 6f00 6700  c.o.......l.o.g.
 00005890: 6f00 2d00 6c00 6100 7200 6700 6500 2e00  o.-.l.a.r.g.e...
 000058a0: 7000 6e00 6700 0e0f ebc7 e700 6c00 6f00  p.n.g.......l.o.
 000058b0: 6700 6f00 2d00 7300 6d00 6100 6c00 6c00  g.o.-.s.m.a.l.l.
 000058c0: 2e00 7000 6e00 6700 0000 0000 0200 0000  ..p.n.g.........
 000058d0: 0300 0000 0100 0000 0000 0000 0000 0000  ................
-000058e0: 2200 0000 0000 0100 0001 9900 0001 8f72  "..............r
-000058f0: 9b30 1500 0000 0000 0400 0000 0100 0000  .0..............
-00005900: 0000 0001 8f72 9b30 1500 0000 4400 0000  .....r.0....D...
-00005910: 0000 0100 0043 f800 0001 8f72 9b30 15    .....C.....r.0.
+000058e0: 2200 0000 0000 0100 0001 9900 0001 8f9c  "...............
+000058f0: 2e70 de00 0000 0000 0400 0000 0100 0000  .p..............
+00005900: 0000 0001 8f9c 2e70 de00 0000 4400 0000  .......p....D...
+00005910: 0000 0100 0043 f800 0001 8f9c 2e70 de    .....C.......p.
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/safe_mode.py` & `joulescope_ui-1.1.9/joulescope_ui/safe_mode.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/sanitize.py` & `joulescope_ui-1.1.9/joulescope_ui/sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/shift_key.py` & `joulescope_ui-1.1.9/joulescope_ui/shift_key.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/software_update.py` & `joulescope_ui-1.1.9/joulescope_ui/software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/source_selector.py` & `joulescope_ui-1.1.9/joulescope_ui/source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/README.md` & `joulescope_ui-1.1.9/joulescope_ui/styles/README.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_editor.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_editor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_file.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_picker.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_picker.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/color_scheme_light.txt` & `joulescope_ui-1.1.9/joulescope_ui/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/font_scheme.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/font_scheme.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/fonts.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/fonts.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/js1/detach.svg` & `joulescope_ui-1.1.9/joulescope_ui/styles/js1/detach.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/js1/index.json` & `joulescope_ui-1.1.9/joulescope_ui/styles/js1/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/js1/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/styles/js1/style.qss`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 QPlainTextEdit:!read-only
 {
     background-color: {% js1.input_background %};
     border-color: {% js1.input_border %};
 }
 
 QAbstractSpinBox {
-    padding-right: 20px; /* make room for the arrows */
     background-color: {% js1.input_background %};
     border-color: {% js1.input_border %};
+    min-width: 3em;
 }
 
 QAbstractSpinBox::up-button {
-    subcontrol-origin: border;
+    subcontrol-origin: padding;
     subcontrol-position: top right;
     width: 18px;
 }
 
 QAbstractSpinBox::down-button {
-    subcontrol-origin: border;
+    subcontrol-origin: padding;
     subcontrol-position: bottom right;
     width: 18px;
 }
 
 QHeaderView::section,
 QTableCornerButton::section
 {
@@ -205,28 +205,31 @@
 }
 
 
 /****************************************************************************/
 /* QComboBox                                                                */
 /****************************************************************************/
 
+
 QComboBox
 {
     background: {% js1.input_background %};
     selection-background-color: {% js1.clickable_hover %};
     padding-left: 0.5ex;
     padding-right: 0.5ex;
+    ~macos combobox-popup: 0;  /* unofficial Qt feature to hide checkmark on macOS */
 }
 
 QComboBox QAbstractItemView  /* The popup */
 {
     background: {% js1.input_background %};
     selection-background-color: {% js1.clickable_hover %};
     padding-left: 0.1ex;
     padding-right: 0.1ex;
+    ~macos min-width: 4em;  /* macOS does not size correctly */
 }
 
 QComboBox::drop-down
 {
     background: {% js1.input_background %};
     subcontrol-origin: padding;
     subcontrol-position: top right;
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/js1/vmovetoolbar.svg` & `joulescope_ui-1.1.9/joulescope_ui/styles/js1/vmovetoolbar.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/js1/vsepartoolbars.svg` & `joulescope_ui-1.1.9/joulescope_ui/styles/js1/vsepartoolbars.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/manager.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,27 @@
 from joulescope_ui import json_plus as json
 from joulescope_ui.sanitize import str_to_filename
 from . import color_file, parameter_file
 from .color_scheme import COLOR_SCHEMES
 from .font_scheme import FONT_SCHEMES
 import copy
 import pkgutil
+import sys
 import time
 
 
 _template_replace = re.compile(r'{%\s*([a-zA-Z0-9_\.]+)\s*%}')
 RENDER_TOPIC = f'registry/style/actions/!render'
 _ENABLE_TEMPLATE_DEBUG = False
 _log = logging.getLogger(__name__)
+_PLATFORM_MAP = {
+    'darwin': '~macos',
+    'win32': '~windows',
+    'linux': '~linux',
+}
 
 
 def name_setting(name):
     """Generate the name setting metadata.
 
     :param name: The translated name.
     :return: The name setting metadata.
@@ -231,16 +237,30 @@
         v = style_vars[varname]
         if v.startswith('#') and len(v) == 9:
             r, g, b, a = int(v[1:3], 16), int(v[3:5], 16), int(v[5:7], 16), int(v[7:9], 16)
             a = a / 255.0
             v = f'rgba({r},{g},{b},{a})'
         return v
 
+    include_prefix = _PLATFORM_MAP.get(sys.platform, '~none')
     for name, template in style_cls['load']['templates'].items():
         s = _template_replace.sub(replace, template)
+
+        # Conditional line include using prefix.
+        lines = []
+        for line in s.split('\n'):
+            sline = line.strip()
+            if sline.startswith('~'):
+                if sline.startswith(include_prefix):
+                    line = line.replace(include_prefix, '')
+                else:
+                    continue
+            lines.append(line)
+        s = '\n'.join(lines)
+
         obj.style_obj['templates'][name] = s
         if _ENABLE_TEMPLATE_DEBUG:
             template_path = os.path.join(path, name)
             with open(template_path, 'wt') as f:
                 f.write(s)
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/parameter_file.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/system/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/styles/system/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/system/zoom_all.svg` & `joulescope_ui-1.1.9/joulescope_ui/styles/system/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_color_file.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/test/test_color_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_manager.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/styles/test/test_parameter_file.py` & `joulescope_ui-1.1.9/joulescope_ui/styles/test/test_parameter_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/anno1.anno.jls` & `joulescope_ui-1.1.9/joulescope_ui/test/anno1.anno.jls`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_annotation_load.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_annotation_load.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_capabilities.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_disk_monitor.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_disk_monitor.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_metadata.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_aggregator.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub_aggregator.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_pubsub_registry.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_pubsub_registry.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_range_tool.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_range_tool.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_reporter.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_reporter.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_sanitize.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_software_update.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_software_update.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_source_selector.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_source_selector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_time_map.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_tooltip.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_units.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/test/test_versioned_file.py` & `joulescope_ui-1.1.9/joulescope_ui/test/test_versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/time_map.py` & `joulescope_ui-1.1.9/joulescope_ui/time_map.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/tokens.py` & `joulescope_ui-1.1.9/joulescope_ui/tokens.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/tooltip.py` & `joulescope_ui-1.1.9/joulescope_ui/tooltip.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/ui_util.py` & `joulescope_ui-1.1.9/joulescope_ui/ui_util.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/units.py` & `joulescope_ui-1.1.9/joulescope_ui/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,19 +159,24 @@
         if v is not None:
             if v >= 1:
                 v = int(v)
             number *= v
     return number
 
 
+def effective_units(unit_setting=None):
+    if unit_setting in [None, 'default']:
+        unit_setting = pubsub_singleton.query('registry/app/settings/units', default='SI')
+    return unit_setting
+
+
 def convert_units(x, x_units, unit_setting):
     if x_units not in ['C', 'J']:
         return x, x_units
-    if unit_setting == 'default':
-        unit_setting = pubsub_singleton.query('registry/app/settings/units', default='SI')
+    unit_setting = effective_units(unit_setting)
     if unit_setting == 'Xh':
         x /= 3600
         y_units = 'Wh' if x_units == 'J' else 'Ah'
     else:
         y_units = x_units
     return x, y_units
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/urls.py` & `joulescope_ui-1.1.9/joulescope_ui/urls.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/versioned_file.py` & `joulescope_ui-1.1.9/joulescope_ui/versioned_file.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/view.py` & `joulescope_ui-1.1.9/joulescope_ui/view.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widget_tools.py` & `joulescope_ui-1.1.9/joulescope_ui/widget_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/accumulator_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/accumulator_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/accumulator/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/accumulator/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/clock/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/clock/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/clock/clock_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/clock/clock_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/developer/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/log_view_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/developer/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/profile_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/developer/profile_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/publish_spy_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/developer/publish_spy_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/developer/pubsub_explorer_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/developer/pubsub_explorer_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/current_limits.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/current_limits.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_control_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_control_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_info_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_info_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/device_update_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/device_update_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/fuse.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/fuse.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/js220_ctrl_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/js220_ctrl_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/device_open.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/device_open.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/fuse_normal.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/index.json` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/info.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/info.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/device_control/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/device_control/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/double_slider.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/double_slider.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/draggable_list_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/draggable_list_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/example/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/example/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/example/example_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/example/example_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/flyout_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/flyout_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/flyout/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/flyout/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/hamburger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/hamburger/hamburger_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/hamburger/hamburger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/help/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/help/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/help/help_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/help/help_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/jls_info/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/jls_info/jls_info_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/jls_info/jls_info_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/current_offset.png` & `joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/current_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/js220_cal_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/js220_cal_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/js220_cal/voltage_offset.png` & `joulescope_ui-1.1.9/joulescope_ui/widgets/js220_cal/voltage_offset.png`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/memory_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/memory/memory_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/memory/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/memory/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/notes/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/notes/notes_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/notes/notes_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/progress_bar/progress_bar_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/progress_bar/progress_bar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/record_status_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/record_status_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/index.json` & `joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/record_status/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/record_status/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/report_issue/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/report_issue/report_issue_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/report_issue/report_issue_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/settings_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/settings/settings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/settings/unique_strings_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/settings/unique_strings_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/sidebar_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/sidebar_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/fuse_engaged.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/fuse_normal.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/index.json` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/sidebar/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/sidebar/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/disk_full_dialog.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/disk_full_dialog.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/signal_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/signal_record/signal_record_config_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/signal_record/signal_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/statistics_record.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/statistics_record/statistics_record_config_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/switch.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/condition_detector.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/condition_detector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/continuous.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/continuous.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/index.json` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/searching.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/searching.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_const.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_const.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_duration.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/test/test_edge.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/test/test_edge.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/trigger/trigger_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/trigger/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/value/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/value/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/value/value_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/value/value_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from PySide6 import QtWidgets, QtGui, QtCore
 from joulescope_ui import CAPABILITIES, register, N_, P_, get_topic_name, tooltip_format
 from joulescope_ui.widget_tools import settings_action_create, context_menu_show
 from joulescope_ui.styles import styled_widget, color_as_qcolor, font_as_qfont
-from joulescope_ui.units import RE_IS_NUMBER, UNITS_SETTING, convert_units, unit_prefix, three_sig_figs
+from joulescope_ui.units import RE_IS_NUMBER, UNITS_SETTING, \
+    convert_units, effective_units, unit_prefix, three_sig_figs
 from joulescope_ui.ui_util import comboBoxConfig, comboBoxSelectItemByText
 from joulescope_ui.source_selector import SourceSelector
 import datetime
 import numpy as np
 import copy
 import logging
 
@@ -298,14 +299,15 @@
     def _on_statistics(self, value):
         self._statistics = copy.deepcopy(value)
         self.repaint()
 
     def paintEvent(self, event):
         fields = [field for field in self._fields if field != self._main]
         parent: ValueWidget = self.parent()
+        unit_setting = effective_units(parent.units)
         resolved = parent.source_selector.resolved()
         if resolved is None or parent.style_obj is None:
             return
 
         self._geometry = {}
         painter = QtGui.QPainter(self)
         v = parent.style_obj['vars']
@@ -336,14 +338,16 @@
         main_color = color_as_qcolor(v['value.main_color'])
         main_font = font_as_qfont(v['value.main_font'])
         main_font_metrics = QtGui.QFontMetrics(main_font)
         main_number_width = main_font_metrics.boundingRect(number_example).width()
         main_num_char_width = _width(main_font_metrics)
         main_txt_char_width = main_font_metrics.boundingRect('W').width()
         main_units_width = main_font_metrics.boundingRect('W').width()
+        if unit_setting == 'Xh':
+            main_units_width *= 2
         main_divisor_width = main_font_metrics.boundingRect(divisor_units).width()
 
         stats_color = color_as_qcolor(v['value.stats_color'])
         stats_font = font_as_qfont(v['value.stats_font'])
         stats_font_metrics = QtGui.QFontMetrics(stats_font)
         stats_number_width = stats_font_metrics.boundingRect(number_example).width()
         stats_char_width = _width(stats_font_metrics)
@@ -431,15 +435,15 @@
 
             painter.setPen(main_color)
             painter.setFont(main_font)
             y += main_font_metrics.ascent() + (y_signal - title_height - main_font_metrics.height()) // 2
 
             if signal_name in self._statistics['accumulators']:
                 signal = self._statistics['accumulators'][signal_name]
-                fields = ['accumulate_duration']
+                fields = ['accumulate_duration'] if parent.show_fields else []
                 signal_value, signal_units = convert_units(signal['value'] / divisor, signal['units'], parent.units)
                 _, prefix, scale = unit_prefix(signal_value)
                 scale *= divisor
             else:
                 signal = self._statistics['signals'][signal_name]
                 fields = fields if parent.show_fields else []
                 fields_all = [self._main] + fields
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/view_manager/view_manager_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/view_manager/view_manager_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/__init__.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/annotations.md` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/annotations.md`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/axis_ticks.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/interval_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/interval_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/line_segments.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/line_segments.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/quantities.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/color_scheme_dark.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/color_scheme_light.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/index.json` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/index.json`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/style.qss` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/style.qss`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/y_zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/styles/zoom_all.svg` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/styles/zoom_all.svg`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_axis_ticks.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/test_axis_ticks.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/test/test_quantities.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/test/test_quantities.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/text_annotation.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/text_annotation.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_control.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_control.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_source_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_source_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/waveform_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/waveform_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 _TEXT_ANNOTATION_X_POS_ALLOC = 64
 _ANNOTATION_TEXT_MOD = (1 << 48)
 _ANNOTATION_Y_MOD = ((1 << 16) + 2)   # must be multiple of plot colors
 _MARKER_SELECT_DISTANCE_PIXELS = 5
 _EXPORT_WHILE_STREAMING_START_OFFSET = time64.SECOND  # not sure of any better way...
 _X_MARKER_ZOOM_LEVELS = [100, 90, 75, 50, 33, 25, 10]
 _DOT_RADIUS = 3
+_ANTIALIASING = QtGui.QPainter.RenderHint.Antialiasing
 
 
 def _analog_plot(quantity, show, units, name, integral=None, range_bounds=None):
     return {
         'quantity': quantity,
         'name': name,
         'units': units,
@@ -232,45 +233,40 @@
 
 
 class _PlotOpenGLWidget(QtOpenGLWidgets.QOpenGLWidget):
     """The inner plot widget that simply calls back to the Waveform widget."""
 
     def __init__(self, parent):
         self._log = logging.getLogger(__name__ + '.plot')
-        self._antialiasing = QtGui.QPainter.RenderHint.Antialiasing
-        self._render_cbk = None
         super().__init__(parent)
         self.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         self.setMouseTracking(True)
 
     def initializeGL(self) -> None:
         functions = QtGui.QOpenGLFunctions(self.context())
         functions.initializeOpenGLFunctions()
         vendor = _gl_get_string(gl.GL_VENDOR)
         self._log.info(f"""OpenGL information:
             Vendor: {vendor}
             Renderer: {_gl_get_string(gl.GL_RENDERER)}
             OpenGL Version: {_gl_get_string(gl.GL_VERSION)}
             Shader Version: {_gl_get_string(gl.GL_SHADING_LANGUAGE_VERSION)}""")
+
         if 'Intel' in vendor:
             self.parent().on_intel_graphics()
 
     def paintGL(self):
         size = self.width(), self.height()
         painter = QtGui.QPainter(self)
-        painter.setRenderHint(self._antialiasing)
         painter.beginNativePainting()
         try:
             self.parent().plot_paint(painter, size)
         finally:
             painter.endNativePainting()
         painter.end()
-        render_cbk, self._render_cbk = self._render_cbk, None
-        if callable(render_cbk):
-            render_cbk(self.render_to_image())
 
     def resizeEvent(self, event):
         self.parent().plot_resizeEvent(event)
         return super().resizeEvent(event)
 
     def mousePressEvent(self, event):
         self.parent().plot_mousePressEvent(event)
@@ -280,40 +276,29 @@
 
     def mouseMoveEvent(self, event):
         self.parent().plot_mouseMoveEvent(event)
 
     def wheelEvent(self, event):
         self.parent().plot_wheelEvent(event)
 
-    def render_callback(self, fn):
-        self._render_cbk = fn
-
-    def render_to_image(self) -> QtGui.QImage:
-        return self.grabFramebuffer()
-
 
 class _PlotWidget(QtWidgets.QWidget):
     """The inner plot widget that simply calls back to the Waveform widget."""
 
     def __init__(self, parent):
         self._log = logging.getLogger(__name__ + '.plot')
-        self._render_cbk = None
         super().__init__(parent)
         self.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         self.setMouseTracking(True)
 
     def paintEvent(self, ev):
         size = self.width(), self.height()
         painter = QtGui.QPainter(self)
-        painter.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing)
         self.parent().plot_paint(painter, size)
         painter.end()
-        render_cbk, self._render_cbk = self._render_cbk, None
-        if callable(render_cbk):
-            render_cbk(self.render_to_image())
 
     def resizeEvent(self, event):
         self.parent().plot_resizeEvent(event)
         return super().resizeEvent(event)
 
     def mousePressEvent(self, event):
         self.parent().plot_mousePressEvent(event)
@@ -323,25 +308,14 @@
 
     def mouseMoveEvent(self, event):
         self.parent().plot_mouseMoveEvent(event)
 
     def wheelEvent(self, event):
         self.parent().plot_wheelEvent(event)
 
-    def render_callback(self, fn):
-        self._render_cbk = fn
-
-    def render_to_image(self) -> QtGui.QImage:
-        sz = self.size()
-        sz = QtCore.QSize(sz.width() * 2, sz.height() * 2)
-        pixmap = QtGui.QPixmap(sz)
-        pixmap.setDevicePixelRatio(2)
-        self.render(pixmap)
-        return pixmap.toImage()
-
 
 class PaintState:
     IDLE = 0
     READY = 1
     PROCESSING = 2
     WAIT = 3
 
@@ -531,19 +505,18 @@
         self._default_source = None
 
         super().__init__(parent)
         self.setFocusPolicy(QtGui.Qt.FocusPolicy.StrongFocus)
 
         # manage repainting
         self.__repaint_request = False
-        self._paint_state = PaintState.IDLE
         self._paint_timer = QtCore.QTimer(self)
         self._paint_timer.setTimerType(QtGui.Qt.PreciseTimer)
-        self._paint_timer.setSingleShot(True)
         self._paint_timer.timeout.connect(self._on_paint_timer)
+        self._paint_duration_ns = 0
 
         # Cache Qt default instances to prevent memory leak in Pyside6 6.4.2
         self._NO_PEN = QtGui.QPen(QtGui.Qt.NoPen)  # prevent memory leak
         self._NO_BRUSH = QtGui.QBrush(QtGui.Qt.NoBrush)  # prevent memory leak
         self._CURSOR_ARROW = QtGui.QCursor(QtGui.Qt.ArrowCursor)
         self._CURSOR_SIZE_VER = QtGui.QCursor(QtGui.Qt.SizeVerCursor)
         self._CURSOR_SIZE_HOR = QtGui.QCursor(QtGui.Qt.SizeHorCursor)
@@ -808,22 +781,21 @@
         topic = get_topic_name(self)
         self._control.on_pubsub_register(self.pubsub, topic, source_filter)
         self.pubsub.subscribe('registry/app/settings/units', self._update_on_publish, ['pub'])
         self.pubsub.subscribe('registry/app/settings/defaults/signal_buffer_source',
                               self._on_default_signal_buffer_source, ['pub', 'retain'])
         self._keymap_load()
         self._repaint_request = True
-        self._paint_state = PaintState.READY
-        self._paint_timer.start(1)
 
     def _keymap_load(self):
         _any = None
         _no = QtCore.Qt.KeyboardModifier.NoModifier
         shift = QtCore.Qt.KeyboardModifier.ShiftModifier
         ctrl = QtCore.Qt.KeyboardModifier.ControlModifier
+        num = QtCore.Qt.KeyboardModifier.KeypadModifier
         self._keymap = {
             (QtCore.Qt.Key_Asterisk, _any): (f'{self.topic}/actions/!x_zoom_all', None),
             (QtCore.Qt.Key_Left, _any): (f'{self.topic}/actions/!x_pan', -1),
             (QtCore.Qt.Key_Right, _any): (f'{self.topic}/actions/!x_pan', 1),
             (QtCore.Qt.Key_Up, _any): (f'{self.topic}/actions/!x_zoom', [1, -1]),
             (QtCore.Qt.Key_Down, _any): (f'{self.topic}/actions/!x_zoom', [-1, -1]),
             (QtCore.Qt.Key_Plus, _any): (f'{self.topic}/actions/!x_zoom', [1, -1]),
@@ -840,14 +812,17 @@
             (QtCore.Qt.Key_5, _no): (f'{self.topic}/actions/!x_markers', ['select', 4]),
             (QtCore.Qt.Key_6, _no): (f'{self.topic}/actions/!x_markers', ['select', 5]),
             (QtCore.Qt.Key_7, _no): (f'{self.topic}/actions/!x_markers', ['select', 6]),
             (QtCore.Qt.Key_8, _no): (f'{self.topic}/actions/!x_markers', ['select', 7]),
             (QtCore.Qt.Key_9, _no): (f'{self.topic}/actions/!x_markers', ['select', 8]),
             (QtCore.Qt.Key_Space, shift): (f'{self.topic}/actions/!viewport', ['toggle']),
         }
+        for key in [QtCore.Qt.Key_1, QtCore.Qt.Key_2, QtCore.Qt.Key_3, QtCore.Qt.Key_4, QtCore.Qt.Key_5,
+                    QtCore.Qt.Key_6, QtCore.Qt.Key_7, QtCore.Qt.Key_8, QtCore.Qt.Key_9]:
+            self._keymap[(key, num)] = self._keymap[(key, _no)]
 
     def on_action_viewport(self, topic, value):
         cmd = value[0]
         t1 = f'{self.topic}/settings/pin_right'
         t2 = f'{self.topic}/settings/pin_left'
         v1 = self.pubsub.query(t1)
         v2 = self.pubsub.query(t2)
@@ -881,15 +856,14 @@
                 super().keyPressEvent(event)
                 return
         self._log.info(f'key {(key, modifiers)} -> publish {v}')
         self.pubsub.publish(*v)
 
     def on_pubsub_unregister(self):
         self._paint_timer.stop()
-        self._paint_state = PaintState.IDLE
 
     def on_pubsub_delete(self):
         for topic, value in self.pubsub.query(f'{self.topic}/settings/close_actions', default=[]):
             self._log.info('waveform close: %s %s', topic, value)
             self.pubsub.publish(topic, value)
 
     def _update_fps(self, thread_duration, time_duration):
@@ -952,24 +926,20 @@
     @property
     def _repaint_request(self):
         return self.__repaint_request
 
     @_repaint_request.setter
     def _repaint_request(self, value):
         self.__repaint_request |= value
-        if self.__repaint_request and self._paint_state == PaintState.READY:
-            self._graphics.update()
 
     @QtCore.Slot()
     def _on_paint_timer(self):
-        if self._paint_state != PaintState.WAIT:
-            self._log.warning('Unexpected paint state: %s', self._paint_state)
-        self._paint_state = PaintState.READY
-        if self.__repaint_request:
+        if self.__repaint_request and self._paint_duration_ns < (1e6 * self.fps / 2):
             self._graphics.update()
+        self._paint_duration_ns = 0
 
     def _extents(self):
         x_min = []
         x_max = []
         for signal_id, signal in self._signals.items():
             if self.is_signal_active(signal_id):
                 x_range = signal['range']
@@ -1462,30 +1432,22 @@
 
     def plot_resizeEvent(self, event):
         event.accept()
         self._repaint_request = True
         self._plots_height_adjust()
 
     def plot_paint(self, p, size):
-        if self._paint_state != PaintState.READY:
-            return
-        self._paint_state = PaintState.PROCESSING
-        t_time_start = time.time_ns()
+        t_start = time.time_ns()
         try:
             self._plot_paint(p, size)
         except Exception:
             self._log.exception('Exception during drawing')
-
         self._request_data()
-
-        t_time_end = time.time_ns()
-        t_duration_ms = np.ceil(1e-6 * (t_time_end - t_time_start) + 0.5)
-        self._paint_state = PaintState.WAIT
-        wait = max(self.paint_delay, int(self.fps - t_duration_ms))
-        self._paint_timer.start(wait)
+        t_end = time.time_ns()
+        self._paint_duration_ns = t_end - t_start
 
     def _compute_geometry(self, size=None):
         s = self._style
         if s is None:
             self._x_geometry_info = {}
             self._y_geometry_info = {}
             return
@@ -1553,23 +1515,25 @@
         """
         s = self._style
         if s is None:
             return
         t_thread_start = time.thread_time_ns()
         t_time_start = time.time_ns()
 
+        p.setRenderHint(_ANTIALIASING)
         resize = not len(self._y_geometry_info)
         self._compute_geometry(size)
         if resize:
             self._plots_height_adjust()
         self._draw_background(p, size)
         self._draw_summary(p)
+        self.__repaint_request = False
+
         if not self._draw_x_axis(p):
             return  # plot is not valid
-        self.__repaint_request = False
         self._annotations_remove_expired()
         self._draw_update_markers()
         self._draw_markers_background(p)
 
         # Draw each plot
         for plot in self.state['plots']:
             if plot['enabled']:
@@ -2837,50 +2801,50 @@
                 if x_name.startswith('plot'):
                     self._menu_x_axis(event)
                 elif x_name.startswith('statistics'):
                     self._menu_dt(event)
             elif y_name == 'summary':
                 self._menu_summary(event)
 
-    def _render_to_image(self, cbk) -> QtGui.QImage:
-        return self._graphics.render_callback(cbk)
-        self._repaint_request = True
+    def _render_to_image(self):
+        width, height = self._graphics.width(), self._graphics.height()
+        image = QtGui.QImage(width, height, QtGui.QImage.Format.Format_ARGB32)
+        p = QtGui.QPainter(image)
+        self._plot_paint(p, (width, height))
+        return image
 
     def _action_copy_image_to_clipboard(self, checked=False):
-        def on_image(img: QtGui.QImage):
-            self._clipboard_image = img
-            QtWidgets.QApplication.clipboard().setImage(self._clipboard_image)
-        self._render_to_image(on_image)
+        self._clipboard_image = self._render_to_image()
+        QtWidgets.QApplication.clipboard().setImage(self._clipboard_image)
 
     @QtCore.Slot(int)
     def _action_save_image_dialog_finish(self, value):
         self._log.info('finished: %d', value)
         if value == QtWidgets.QDialog.DialogCode.Accepted:
             filenames = self._dialog.selectedFiles()
             if len(filenames) == 1:
                 filename = filenames[0]
                 _, ext = os.path.splitext(filename)
                 if ext in [None, '']:
                     filename += '.png'
                 elif ext[1:].lower() not in ['bmp', 'jpg', 'jpeg', 'png', 'ppm', 'xbm', 'xpm']:
                     filename += '.png'
                 self._log.info('finished: accept - save: %s', filename)
-                def on_image(img: QtGui.QImage):
-                    if not img.save(filename):
-                        self._log.warning('Could not save image: %s', filename)
-                self._render_to_image(on_image)
+                img = self._render_to_image()
+                if not img.save(filename):
+                    self._log.warning('Could not save image: %s', filename)
             else:
                 self._log.info('finished: accept - but no file selected, ignore')
         else:
             self._log.info('finished: reject - abort recording')
         self._dialog.close()
         self._dialog = None
 
     def _action_save_image(self, checked=False):
-        filter_str = 'png (*.png)'
+        filter_str = 'PNG (*.png)'
         filename = time64.filename('.png')
         path = self.pubsub.query('registry/paths/settings/path')
         path = os.path.join(path, filename)
         dialog = QtWidgets.QFileDialog(self, N_('Save image to file'), path, filter_str)
         dialog.setFileMode(QtWidgets.QFileDialog.AnyFile)
         dialog.setAcceptMode(QtWidgets.QFileDialog.AcceptSave)
         dialog.finished.connect(self._action_save_image_dialog_finish)
@@ -3516,15 +3480,15 @@
             marker = self.annotations['x'].pop(marker['id'])
             return marker
         else:
             raise ValueError('unsupported remove')
 
     def _x_marker_add_single(self, pos1=None):
         x0, x1 = self.x_range
-        if pos1 < 0:
+        if pos1 is not None and pos1 < 0:
             if self._mouse_pos is not None:
                 pos1 = self._x_map.counter_to_time64(self._mouse_pos[0])
             else:
                 pos1 = None
         if pos1 is None:
             xc = (x1 + x0) // 2
             pos1 = self._x_marker_position(xc)
@@ -4250,14 +4214,16 @@
         self._plot_data_invalidate()
 
     def on_setting_show_min_max(self):
         self._repaint_request = True
 
     def on_setting_fps(self, value):
         self._log.info('fps: period = %s ms', value)
+        self._paint_timer.stop()
+        self._paint_timer.start(int(value))
 
     def on_setting_summary_quantity(self):
         self._plot_data_invalidate()
 
     def on_setting_trace_subsources(self):
         self._plot_data_invalidate()
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui/widgets/waveform/y_range_widget.py` & `joulescope_ui-1.1.9/joulescope_ui/widgets/waveform/y_range_widget.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui/zip_inspector.py` & `joulescope_ui-1.1.9/joulescope_ui/zip_inspector.py`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/joulescope_ui.egg-info/PKG-INFO` & `joulescope_ui-1.1.9/joulescope_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope_ui
-Version: 1.1.8
+Version: 1.1.9
 Summary: Joulescope™ graphical user interface
 Home-page: https://www.joulescope.com
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope_ui/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope_ui-1.1.8/joulescope_ui.egg-info/SOURCES.txt` & `joulescope_ui-1.1.9/joulescope_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/pyproject.toml` & `joulescope_ui-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope_ui-1.1.8/setup.py` & `joulescope_ui-1.1.9/setup.py`

 * *Files identical despite different names*

