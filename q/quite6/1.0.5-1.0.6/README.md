# Comparing `tmp/quite6-1.0.5.tar.gz` & `tmp/quite6-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quite6-1.0.5.tar", last modified: Sat May 25 14:54:43 2024, max compression
+gzip compressed data, was "quite6-1.0.6.tar", last modified: Wed May 29 16:46:46 2024, max compression
```

## Comparing `quite6-1.0.5.tar` & `quite6-1.0.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.339669 quite6-1.0.5/
--rw-r--r--   0 wangcong   (502) staff       (20)     1074 2024-05-14 10:15:26.000000 quite6-1.0.5/LICENSE
--rw-r--r--   0 wangcong   (502) staff       (20)      104 2024-05-14 10:15:26.000000 quite6-1.0.5/MANIFEST.in
--rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-25 14:54:43.339455 quite6-1.0.5/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2936 2024-05-14 10:15:26.000000 quite6-1.0.5/README.rst
--rw-r--r--   0 wangcong   (502) staff       (20)        6 2024-05-25 14:54:10.000000 quite6-1.0.5/RELEASE-VERSION
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.243157 quite6-1.0.5/quite6/
--rw-r--r--   0 wangcong   (502) staff       (20)      272 2024-05-14 11:46:55.000000 quite6-1.0.5/quite6/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.253900 quite6-1.0.5/quite6/controller/
--rw-r--r--   0 wangcong   (502) staff       (20)      211 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/controller/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      606 2024-05-14 14:24:17.000000 quite6-1.0.5/quite6/controller/dialog_ui_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2634 2024-05-14 14:24:17.000000 quite6-1.0.5/quite6/controller/file_dialog_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1616 2024-05-14 14:24:17.000000 quite6-1.0.5/quite6/controller/widget_controller.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3617 2024-05-25 14:49:48.000000 quite6-1.0.5/quite6/controller/widget_ui_controller.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.257072 quite6-1.0.5/quite6/core/
--rw-r--r--   0 wangcong   (502) staff       (20)      203 2024-05-14 10:47:48.000000 quite6-1.0.5/quite6/core/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 10:43:54.000000 quite6-1.0.5/quite6/core/event_loop.py
--rw-r--r--   0 wangcong   (502) staff       (20)      281 2024-05-14 10:43:54.000000 quite6-1.0.5/quite6/core/timer.py
--rw-r--r--   0 wangcong   (502) staff       (20)     3712 2024-05-14 15:04:01.000000 quite6-1.0.5/quite6/deferred_function.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.260964 quite6-1.0.5/quite6/gui/
--rw-r--r--   0 wangcong   (502) staff       (20)     1129 2024-05-25 13:12:30.000000 quite6-1.0.5/quite6/gui/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.276833 quite6-1.0.5/quite6/gui/interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      554 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/interfaces/__init__.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.281571 quite6-1.0.5/quite6/gui/interfaces/ability_interfaces/
--rw-r--r--   0 wangcong   (502) staff       (20)      120 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/interfaces/ability_interfaces/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      188 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1092 2024-05-14 10:57:04.000000 quite6-1.0.5/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      539 2024-05-14 03:20:46.000000 quite6-1.0.5/quite6/gui/interfaces/base_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      303 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/interfaces/changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      470 2024-05-14 08:19:12.000000 quite6-1.0.5/quite6/gui/interfaces/closed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      307 2024-05-14 10:57:04.000000 quite6-1.0.5/quite6/gui/interfaces/excited_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      199 2024-05-14 10:57:04.000000 quite6-1.0.5/quite6/gui/interfaces/focus_in_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      201 2024-05-14 10:57:04.000000 quite6-1.0.5/quite6/gui/interfaces/focus_out_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      322 2024-05-14 10:57:04.000000 quite6-1.0.5/quite6/gui/interfaces/row_changed_signal_interface.py
--rw-r--r--   0 wangcong   (502) staff       (20)      298 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/interfaces/showed_signal_interface.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.285343 quite6-1.0.5/quite6/gui/layouts/
--rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/layouts/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2712 2024-05-14 14:37:29.000000 quite6-1.0.5/quite6/gui/layouts/square_layout.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.293989 quite6-1.0.5/quite6/gui/paint/
--rw-r--r--   0 wangcong   (502) staff       (20)      129 2024-05-13 08:52:57.000000 quite6-1.0.5/quite6/gui/paint/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     5084 2024-05-17 03:34:53.000000 quite6-1.0.5/quite6/gui/paint/painter.py
--rw-r--r--   0 wangcong   (502) staff       (20)      502 2024-05-14 11:03:11.000000 quite6-1.0.5/quite6/gui/paint/pen.py
--rw-r--r--   0 wangcong   (502) staff       (20)      904 2024-05-14 11:03:11.000000 quite6-1.0.5/quite6/gui/paint/point.py
--rw-r--r--   0 wangcong   (502) staff       (20)      280 2024-05-14 11:03:11.000000 quite6-1.0.5/quite6/gui/paint/scaling.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1471 2024-05-14 11:03:11.000000 quite6-1.0.5/quite6/gui/paint/size.py
--rw-r--r--   0 wangcong   (502) staff       (20)      398 2024-05-14 10:17:44.000000 quite6-1.0.5/quite6/gui/qt_gui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      311 2024-05-14 10:15:26.000000 quite6-1.0.5/quite6/gui/ui_extension.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.333430 quite6-1.0.5/quite6/gui/widgets/
--rw-r--r--   0 wangcong   (502) staff       (20)      832 2024-05-25 13:12:30.000000 quite6-1.0.5/quite6/gui/widgets/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)      383 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/action.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2454 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/combo_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/date_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      683 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/date_time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      780 2024-05-14 11:51:50.000000 quite6-1.0.5/quite6/gui/widgets/dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      195 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/dock_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      721 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/double_spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)      189 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/group_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1627 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/input_dialog.py
--rw-r--r--   0 wangcong   (502) staff       (20)      736 2024-05-14 14:37:29.000000 quite6-1.0.5/quite6/gui/widgets/label.py
--rw-r--r--   0 wangcong   (502) staff       (20)      183 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/layout.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1004 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/line_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2347 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/list_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      697 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/main_window.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2904 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/plot_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      676 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/push_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      680 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/radio_button.py
--rw-r--r--   0 wangcong   (502) staff       (20)      582 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/shortcut.py
--rw-r--r--   0 wangcong   (502) staff       (20)      693 2024-05-14 11:54:28.000000 quite6-1.0.5/quite6/gui/widgets/spin_box.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1663 2024-05-25 14:51:37.000000 quite6-1.0.5/quite6/gui/widgets/tab_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)     6529 2024-05-14 11:32:31.000000 quite6-1.0.5/quite6/gui/widgets/table_view.py
--rw-r--r--   0 wangcong   (502) staff       (20)     9397 2024-05-14 14:37:29.000000 quite6-1.0.5/quite6/gui/widgets/table_widget.py
--rw-r--r--   0 wangcong   (502) staff       (20)      720 2024-05-14 11:37:12.000000 quite6-1.0.5/quite6/gui/widgets/text_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)      926 2024-05-14 11:37:12.000000 quite6-1.0.5/quite6/gui/widgets/time_edit.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1326 2024-05-14 14:37:29.000000 quite6-1.0.5/quite6/gui/widgets/widget.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.336810 quite6-1.0.5/quite6/tools/
--rw-r--r--   0 wangcong   (502) staff       (20)      110 2024-05-14 11:51:08.000000 quite6-1.0.5/quite6/tools/__init__.py
--rw-r--r--   0 wangcong   (502) staff       (20)     1207 2024-05-15 06:35:06.000000 quite6-1.0.5/quite6/tools/load_qrc.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2461 2024-05-14 15:28:56.000000 quite6-1.0.5/quite6/tools/load_ui.py
--rw-r--r--   0 wangcong   (502) staff       (20)      315 2024-05-14 14:37:29.000000 quite6-1.0.5/quite6/tools/process.py
-drwxr-xr-x   0 wangcong   (502) staff       (20)        0 2024-05-25 14:54:43.338085 quite6-1.0.5/quite6.egg-info/
--rw-r--r--   0 wangcong   (502) staff       (20)     3749 2024-05-25 14:54:43.000000 quite6-1.0.5/quite6.egg-info/PKG-INFO
--rw-r--r--   0 wangcong   (502) staff       (20)     2427 2024-05-25 14:54:43.000000 quite6-1.0.5/quite6.egg-info/SOURCES.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        1 2024-05-25 14:54:43.000000 quite6-1.0.5/quite6.egg-info/dependency_links.txt
--rw-r--r--   0 wangcong   (502) staff       (20)       41 2024-05-25 14:54:43.000000 quite6-1.0.5/quite6.egg-info/requires.txt
--rw-r--r--   0 wangcong   (502) staff       (20)        7 2024-05-25 14:54:43.000000 quite6-1.0.5/quite6.egg-info/top_level.txt
--rw-r--r--   0 wangcong   (502) staff       (20)     2557 2024-05-14 10:15:26.000000 quite6-1.0.5/readme.md
--rw-r--r--   0 wangcong   (502) staff       (20)       40 2024-05-16 14:15:45.000000 quite6-1.0.5/requirements.txt
--rw-r--r--   0 wangcong   (502) staff       (20)      154 2024-05-25 14:54:43.340234 quite6-1.0.5/setup.cfg
--rw-r--r--   0 wangcong   (502) staff       (20)     1633 2024-05-14 10:15:26.000000 quite6-1.0.5/setup.py
--rw-r--r--   0 wangcong   (502) staff       (20)     2173 2024-05-14 10:15:26.000000 quite6-1.0.5/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.213080 quite6-1.0.6/
+-rw-rw-rw-   0        0        0     1095 2024-05-29 16:01:54.000000 quite6-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      108 2024-05-29 16:01:54.000000 quite6-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3887 2024-05-29 16:46:46.212084 quite6-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2024-05-29 16:01:54.000000 quite6-1.0.6/README.rst
+-rw-rw-rw-   0        0        0        7 2024-05-29 16:44:19.000000 quite6-1.0.6/RELEASE-VERSION
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.166237 quite6-1.0.6/quite6/
+-rw-rw-rw-   0        0        0      276 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.172217 quite6-1.0.6/quite6/controller/
+-rw-rw-rw-   0        0        0      215 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/controller/__init__.py
+-rw-rw-rw-   0        0        0      627 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/controller/dialog_ui_controller.py
+-rw-rw-rw-   0        0        0     2693 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/controller/file_dialog_controller.py
+-rw-rw-rw-   0        0        0     1672 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/controller/widget_controller.py
+-rw-rw-rw-   0        0        0     3726 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/controller/widget_ui_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.174211 quite6-1.0.6/quite6/core/
+-rw-rw-rw-   0        0        0      210 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/core/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/core/event_loop.py
+-rw-rw-rw-   0        0        0      292 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/core/timer.py
+-rw-rw-rw-   0        0        0     3827 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/deferred_function.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.176204 quite6-1.0.6/quite6/gui/
+-rw-rw-rw-   0        0        0     1156 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.182184 quite6-1.0.6/quite6/gui/interfaces/
+-rw-rw-rw-   0        0        0      563 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.183181 quite6-1.0.6/quite6/gui/interfaces/ability_interfaces/
+-rw-rw-rw-   0        0        0      122 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/ability_interfaces/__init__.py
+-rw-rw-rw-   0        0        0      198 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/ability_interfaces/class_exec_interface.py
+-rw-rw-rw-   0        0        0     1119 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py
+-rw-rw-rw-   0        0        0      559 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/base_interface.py
+-rw-rw-rw-   0        0        0      313 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/changed_signal_interface.py
+-rw-rw-rw-   0        0        0      490 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/closed_signal_interface.py
+-rw-rw-rw-   0        0        0      318 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/excited_signal_interface.py
+-rw-rw-rw-   0        0        0      207 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/focus_in_signal_interface.py
+-rw-rw-rw-   0        0        0      209 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/focus_out_signal_interface.py
+-rw-rw-rw-   0        0        0      333 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/row_changed_signal_interface.py
+-rw-rw-rw-   0        0        0      308 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/interfaces/showed_signal_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.185174 quite6-1.0.6/quite6/gui/layouts/
+-rw-rw-rw-   0        0        0       41 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/layouts/__init__.py
+-rw-rw-rw-   0        0        0     2797 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/layouts/square_layout.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.189160 quite6-1.0.6/quite6/gui/paint/
+-rw-rw-rw-   0        0        0      134 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/__init__.py
+-rw-rw-rw-   0        0        0     5199 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/painter.py
+-rw-rw-rw-   0        0        0      520 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/pen.py
+-rw-rw-rw-   0        0        0      934 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/point.py
+-rw-rw-rw-   0        0        0      293 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/scaling.py
+-rw-rw-rw-   0        0        0     1530 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/paint/size.py
+-rw-rw-rw-   0        0        0      576 2024-05-29 16:42:41.000000 quite6-1.0.6/quite6/gui/qt_gui.py
+-rw-rw-rw-   0        0        0      327 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/ui_extension.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.208097 quite6-1.0.6/quite6/gui/widgets/
+-rw-rw-rw-   0        0        0      857 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      398 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/action.py
+-rw-rw-rw-   0        0        0     2529 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/combo_box.py
+-rw-rw-rw-   0        0        0      954 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/date_edit.py
+-rw-rw-rw-   0        0        0      706 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/date_time_edit.py
+-rw-rw-rw-   0        0        0      810 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/dialog.py
+-rw-rw-rw-   0        0        0      204 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/dock_widget.py
+-rw-rw-rw-   0        0        0      744 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/double_spin_box.py
+-rw-rw-rw-   0        0        0      198 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/group_box.py
+-rw-rw-rw-   0        0        0     1668 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/input_dialog.py
+-rw-rw-rw-   0        0        0      760 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/label.py
+-rw-rw-rw-   0        0        0      192 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/layout.py
+-rw-rw-rw-   0        0        0     1036 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     2419 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/list_widget.py
+-rw-rw-rw-   0        0        0      721 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/main_window.py
+-rw-rw-rw-   0        0        0     2995 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/plot_widget.py
+-rw-rw-rw-   0        0        0      699 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/push_button.py
+-rw-rw-rw-   0        0        0      703 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/radio_button.py
+-rw-rw-rw-   0        0        0      601 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/shortcut.py
+-rw-rw-rw-   0        0        0      716 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     1714 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/tab_widget.py
+-rw-rw-rw-   0        0        0     6717 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/table_view.py
+-rw-rw-rw-   0        0        0     9627 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/table_widget.py
+-rw-rw-rw-   0        0        0      744 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/text_edit.py
+-rw-rw-rw-   0        0        0      954 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/time_edit.py
+-rw-rw-rw-   0        0        0     1372 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/gui/widgets/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.211087 quite6-1.0.6/quite6/tools/
+-rw-rw-rw-   0        0        0      113 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/tools/__init__.py
+-rw-rw-rw-   0        0        0     1832 2024-05-29 16:41:27.000000 quite6-1.0.6/quite6/tools/load_qrc.py
+-rw-rw-rw-   0        0        0     2527 2024-05-29 16:42:41.000000 quite6-1.0.6/quite6/tools/load_ui.py
+-rw-rw-rw-   0        0        0      327 2024-05-29 16:01:54.000000 quite6-1.0.6/quite6/tools/process.py
+drwxrwxrwx   0        0        0        0 2024-05-29 16:46:46.212084 quite6-1.0.6/quite6.egg-info/
+-rw-rw-rw-   0        0        0     3887 2024-05-29 16:46:46.000000 quite6-1.0.6/quite6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2427 2024-05-29 16:46:46.000000 quite6-1.0.6/quite6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 16:46:46.000000 quite6-1.0.6/quite6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-29 16:46:46.000000 quite6-1.0.6/quite6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 16:46:46.000000 quite6-1.0.6/quite6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2651 2024-05-29 16:01:54.000000 quite6-1.0.6/readme.md
+-rw-rw-rw-   0        0        0       45 2024-05-29 16:01:54.000000 quite6-1.0.6/requirements.txt
+-rw-rw-rw-   0        0        0      166 2024-05-29 16:46:46.213080 quite6-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1692 2024-05-29 16:01:54.000000 quite6-1.0.6/setup.py
+-rw-rw-rw-   0        0        0     2254 2024-05-29 16:01:54.000000 quite6-1.0.6/version.py
```

### Comparing `quite6-1.0.5/LICENSE` & `quite6-1.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2016 SF-Zhou
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2016 SF-Zhou
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `quite6-1.0.5/PKG-INFO` & `quite6-1.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-Metadata-Version: 2.1
-Name: quite6
-Version: 1.0.5
-Summary: QT UI Extension
-Home-page: https://github.com/KD-Group/quite6
-Author: SF-Zhou
-Author-email: sfzhou.scut@gmail.com
-License: MIT
-Keywords: qt ui
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: st
-Requires-Dist: prett6
-Requires-Dist: PySide6
-Requires-Dist: typing
-Requires-Dist: pyqtgraph
-Requires-Dist: numpy
-
-quite6: QT UI Extension for Python3
-==================================
-
-|Build Status|
-
-Features
---------
-
-1. powerful signal-slot
-2. user friendly widget classes
-
-User Friendly Widget Classes
-----------------------------
-
-Uniform wrapper on frequently-used widget, including:
-
-**container widget**:
-
-1. `Widget <./quite6/gui/widgets/widget.py>`__
-2. `Dialog <./quite6/gui/widgets/dialog.py>`__
-3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
-4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
-5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
-
-**value widget**:
-
-1. `Label <./quite6/gui/widgets/label.py>`__
-2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
-3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
-4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
-5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
-6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
-
-**behavior widget**:
-
-1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
-2. `Action <./quite6/gui/widgets/action.py>`__
-3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
-4. `PushButton <./quite6/gui/widgets/push_button.py>`__
-
-Container Widget
-~~~~~~~~~~~~~~~~
-
-*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
-
-.. code:: python
-
-    import quite6
-
-    w = quite6.Widget()
-    w.exec()
-
-.. figure:: docs/images/1.simple.widget.png
-   :alt: Simple Widget
-
-   Simple Widget
-
-*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
-
-.. code:: python
-
-    import quite6
-
-
-    class CustomWidget(quite6.Widget):
-        def paint(self, painter: quite6.Painter):
-            painter.setFont(quite6.QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
-            painter.end()
-
-    main_window = quite6.MainWindow()
-    custom_widget = CustomWidget(parent=main_window)
-    main_window.set_central_widget(custom_widget)
-    main_window.exec()
-
-.. figure:: docs/images/2.nested.widget.png
-   :alt: Nested Widget
-
-   Nested Widget
-
-*Example 3*: `widget from ui
-file <./examples/3_widget_from_ui_file/example-3.py>`__
-
-.. code:: python
-
-    import os
-    from quite6 import *
-
-
-    class CustomWidget(Widget):
-        def paint(self, painter: Painter):
-            w, _ = self.size
-            painter.setFont(QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
-            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
-            painter.end()
-
-
-    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
-    main_window.set_central_widget(CustomWidget(parent=main_window))
-    main_window.exec()
-
-Use QtDesigner to create a ui file:
-
-.. figure:: docs/images/3.ui.design.png
-   :alt: UI Design
-
-   UI Design
-
-.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
-   :target: https://travis-ci.com/KD-Group/quite6
+Metadata-Version: 2.1
+Name: quite6
+Version: 1.0.6
+Summary: QT UI Extension
+Home-page: https://github.com/KD-Group/quite6
+Author: SF-Zhou
+Author-email: sfzhou.scut@gmail.com
+License: MIT
+Keywords: qt ui
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: st
+Requires-Dist: prett6
+Requires-Dist: PySide6
+Requires-Dist: typing
+Requires-Dist: pyqtgraph
+Requires-Dist: numpy
+
+quite6: QT UI Extension for Python3
+==================================
+
+|Build Status|
+
+Features
+--------
+
+1. powerful signal-slot
+2. user friendly widget classes
+
+User Friendly Widget Classes
+----------------------------
+
+Uniform wrapper on frequently-used widget, including:
+
+**container widget**:
+
+1. `Widget <./quite6/gui/widgets/widget.py>`__
+2. `Dialog <./quite6/gui/widgets/dialog.py>`__
+3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
+4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
+5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
+
+**value widget**:
+
+1. `Label <./quite6/gui/widgets/label.py>`__
+2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
+3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
+4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
+5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
+6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
+
+**behavior widget**:
+
+1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
+2. `Action <./quite6/gui/widgets/action.py>`__
+3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
+4. `PushButton <./quite6/gui/widgets/push_button.py>`__
+
+Container Widget
+~~~~~~~~~~~~~~~~
+
+*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
+
+.. code:: python
+
+    import quite6
+
+    w = quite6.Widget()
+    w.exec()
+
+.. figure:: docs/images/1.simple.widget.png
+   :alt: Simple Widget
+
+   Simple Widget
+
+*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
+
+.. code:: python
+
+    import quite6
+
+
+    class CustomWidget(quite6.Widget):
+        def paint(self, painter: quite6.Painter):
+            painter.setFont(quite6.QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
+            painter.end()
+
+    main_window = quite6.MainWindow()
+    custom_widget = CustomWidget(parent=main_window)
+    main_window.set_central_widget(custom_widget)
+    main_window.exec()
+
+.. figure:: docs/images/2.nested.widget.png
+   :alt: Nested Widget
+
+   Nested Widget
+
+*Example 3*: `widget from ui
+file <./examples/3_widget_from_ui_file/example-3.py>`__
+
+.. code:: python
+
+    import os
+    from quite6 import *
+
+
+    class CustomWidget(Widget):
+        def paint(self, painter: Painter):
+            w, _ = self.size
+            painter.setFont(QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
+            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
+            painter.end()
+
+
+    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
+    main_window.set_central_widget(CustomWidget(parent=main_window))
+    main_window.exec()
+
+Use QtDesigner to create a ui file:
+
+.. figure:: docs/images/3.ui.design.png
+   :alt: UI Design
+
+   UI Design
+
+.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
+   :target: https://travis-ci.com/KD-Group/quite6
```

### Comparing `quite6-1.0.5/README.rst` & `quite6-1.0.6/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,94 @@
-quite6: QT UI Extension for Python3
-==================================
-
-|Build Status|
-
-Features
---------
-
-1. powerful signal-slot
-2. user friendly widget classes
-
-User Friendly Widget Classes
-----------------------------
-
-Uniform wrapper on frequently-used widget, including:
-
-**container widget**:
-
-1. `Widget <./quite6/gui/widgets/widget.py>`__
-2. `Dialog <./quite6/gui/widgets/dialog.py>`__
-3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
-4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
-5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
-
-**value widget**:
-
-1. `Label <./quite6/gui/widgets/label.py>`__
-2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
-3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
-4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
-5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
-6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
-
-**behavior widget**:
-
-1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
-2. `Action <./quite6/gui/widgets/action.py>`__
-3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
-4. `PushButton <./quite6/gui/widgets/push_button.py>`__
-
-Container Widget
-~~~~~~~~~~~~~~~~
-
-*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
-
-.. code:: python
-
-    import quite6
-
-    w = quite6.Widget()
-    w.exec()
-
-.. figure:: docs/images/1.simple.widget.png
-   :alt: Simple Widget
-
-   Simple Widget
-
-*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
-
-.. code:: python
-
-    import quite6
-
-
-    class CustomWidget(quite6.Widget):
-        def paint(self, painter: quite6.Painter):
-            painter.setFont(quite6.QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
-            painter.end()
-
-    main_window = quite6.MainWindow()
-    custom_widget = CustomWidget(parent=main_window)
-    main_window.set_central_widget(custom_widget)
-    main_window.exec()
-
-.. figure:: docs/images/2.nested.widget.png
-   :alt: Nested Widget
-
-   Nested Widget
-
-*Example 3*: `widget from ui
-file <./examples/3_widget_from_ui_file/example-3.py>`__
-
-.. code:: python
-
-    import os
-    from quite6 import *
-
-
-    class CustomWidget(Widget):
-        def paint(self, painter: Painter):
-            w, _ = self.size
-            painter.setFont(QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
-            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
-            painter.end()
-
-
-    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
-    main_window.set_central_widget(CustomWidget(parent=main_window))
-    main_window.exec()
-
-Use QtDesigner to create a ui file:
-
-.. figure:: docs/images/3.ui.design.png
-   :alt: UI Design
-
-   UI Design
-
-.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
-   :target: https://travis-ci.com/KD-Group/quite6
+# quite6: QT UI Extension for Python3
+
+[![Build Status](https://travis-ci.com/KD-Group/quite6.svg?branch=master)](https://travis-ci.com/KD-Group/quite6)
+
+## Features
+
+1. powerful signal-slot
+2. user friendly widget classes
+
+## User Friendly Widget Classes
+
+Uniform wrapper on frequently-used widget, including:
+
+**container widget**:
+
+1. [Widget](./quite6/gui/widgets/widget.py)
+2. [Dialog](./quite6/gui/widgets/dialog.py)
+3. [MainWindow](./quite6/gui/widgets/main_window.py)
+4. [GroupBox](./quite6/gui/widgets/group_box.py)
+5. [DockWidget](./quite6/gui/widgets/dock_widget.py)
+
+**value widget**:
+
+1. [Label](./quite6/gui/widgets/label.py)
+2. [LineEdit](./quite6/gui/widgets/line_edit.py)
+3. [ComboBox](./quite6/gui/widgets/combo_box.py)
+4. [ListWidget](./quite6/gui/widgets/list_widget.py)
+5. [SpinBox](./quite6/gui/widgets/spin_box.py)
+6. [DoubleSpinBox](./quite6/gui/widgets/double_spin_box.py)
+
+**behavior widget**:
+
+1. [InputDialog](./quite6/gui/widgets/input_dialog.py)
+2. [Action](./quite6/gui/widgets/action.py)
+3. [Shortcut](./quite6/gui/widgets/shortcut.py)
+4. [PushButton](./quite6/gui/widgets/push_button.py)
+
+### Container Widget
+
+*Example 1*: [create widget](./examples/1_create_widget/example-1.py)
+
+```python
+import quite6
+
+w = quite6.Widget()
+w.exec()
+```
+
+![Simple Widget](docs/images/1.simple.widget.png)
+
+*Example 2*: [nested widget](./examples/2_nested_widget/example-2.py)
+
+```python
+import quite6
+
+
+class CustomWidget(quite6.Widget):
+    def paint(self, painter: quite6.Painter):
+        painter.setFont(quite6.QFont("Courier New", 14.0))
+        painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
+        painter.end()
+
+main_window = quite6.MainWindow()
+custom_widget = CustomWidget(parent=main_window)
+main_window.set_central_widget(custom_widget)
+main_window.exec()
+```
+
+![Nested Widget](docs/images/2.nested.widget.png)
+
+*Example 3*: [widget from ui file](./examples/3_widget_from_ui_file/example-3.py)
+
+```python
+import os
+from quite6 import *
+
+
+class CustomWidget(Widget):
+    def paint(self, painter: Painter):
+        w, _ = self.size
+        painter.setFont(QFont("Courier New", 14.0))
+        painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
+        painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
+        painter.end()
+
+
+main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
+main_window.set_central_widget(CustomWidget(parent=main_window))
+main_window.exec()
+```
+
+Use QtDesigner to create a ui file:
+
+![UI Design](docs/images/3.ui.design.png)
```

### Comparing `quite6-1.0.5/quite6/controller/widget_ui_controller.py` & `quite6-1.0.6/quite6/controller/widget_ui_controller.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import st
-
-from quite6.gui.widgets import DateTimeEdit
-from . import WidgetController
-from .. import load_ui
-from ..gui import Action, SignalSender
-from ..gui import DoubleSpinBox, TabWidget, TableWidget, TableView
-from ..gui import GroupBox, SpinBox
-from ..gui import Label, PushButton, RatioButton
-from ..gui import Layout
-from ..gui import LineEdit, DateEdit, TextEdit, TimeEdit
-from ..gui import ListWidget, ComboBox
-from ..gui import Widget, DockWidget, PlotWidget
-
-
-class WidgetUiController(WidgetController):
-    def __init__(self, parent=None, ui_file: str = None):
-        assert ui_file is not None
-
-        super().__init__(parent, st.partial_back(load_ui, ui_file))
-
-    def label(self, name=None) -> Label:
-        return self.__get_widget__('label', name)
-
-    def button(self, name=None) -> PushButton:
-        return self.__get_widget__('button', name)
-
-    def radio_button(self, name=None) -> RatioButton:
-        return self.__get_widget__('radio_button', name)
-
-    def edit(self, name=None) -> LineEdit:
-        return self.__get_widget__('edit', name)
-
-    def date_edit(self, name=None) -> DateEdit:
-        return self.__get_widget__('date_edit', name)
-
-    def date_time_edit(self, name=None) -> DateTimeEdit:
-        return self.__get_widget__('date_time_edit', name)
-
-    def time_edit(self, name=None) -> TimeEdit:
-        return self.__get_widget__('time', name)
-
-    def text_edit(self, name=None) -> TextEdit:
-        return self.__get_widget__('text_edit', name)
-
-    def plot_widget(self, name=None) -> PlotWidget:
-        return self.__get_widget__('plot_widget', name)
-
-    def list(self, name=None) -> ListWidget:
-        return self.__get_widget__('list', name)
-
-    def combo(self, name=None) -> ComboBox:
-        return self.__get_widget__('combo', name)
-
-    def container(self, name=None) -> Widget:
-        if name is None:
-            return self.w
-        return self.__get_widget__('container', name)
-
-    def dock(self, name=None) -> DockWidget:
-        return self.__get_widget__('dock', name)
-
-    def group(self, name=None) -> GroupBox:
-        return self.__get_widget__('group', name)
-
-    def spin(self, name=None) -> SpinBox:
-        return self.__get_widget__('spin', name)
-
-    def table(self, name=None) -> TableWidget:
-        return self.__get_widget__('table', name)
-
-    def table_view(self, name=None) -> TableView:
-        return self.__get_widget__('table_view', name)
-
-    def tab(self, name=None) -> TabWidget:
-        return self.__get_widget__('tab', name)
-
-    def double(self, name=None) -> DoubleSpinBox:
-        return self.__get_widget__('double', name)
-
-    def action(self, name=None) -> Action:
-        obj = self.__get_widget__('action', name)
-        if getattr(obj, 'excited', None) is None:
-            obj.excited = SignalSender()
-            obj.triggered.connect(obj.excited.emit)
-
-            def set_enabled(status=True):
-                obj.setEnabled(status)
-
-            def set_disabled(status=True):
-                obj.setEnabled(not status)
-
-            def click():
-                if obj.isEnabled():
-                    obj.trigger()
-
-            obj.click = click
-            obj.set_enabled = set_enabled
-            obj.set_disabled = set_disabled
-        return obj
-
-    def widget(self, name=None) -> Widget:
-        return self.container(name).center_widget
-
-    def layout(self, name=None) -> Layout:
-        return self.__get_widget__('layout', name)
-
-    def __get_widget__(self, type_name, obj_name):
-        return getattr(self.w, type_name + '_' + obj_name, None) or getattr(self.w, obj_name + '_' + type_name)
+import st
+
+from quite6.gui.widgets import DateTimeEdit
+from . import WidgetController
+from .. import load_ui
+from ..gui import Action, SignalSender
+from ..gui import DoubleSpinBox, TabWidget, TableWidget, TableView
+from ..gui import GroupBox, SpinBox
+from ..gui import Label, PushButton, RatioButton
+from ..gui import Layout
+from ..gui import LineEdit, DateEdit, TextEdit, TimeEdit
+from ..gui import ListWidget, ComboBox
+from ..gui import Widget, DockWidget, PlotWidget
+
+
+class WidgetUiController(WidgetController):
+    def __init__(self, parent=None, ui_file: str = None):
+        assert ui_file is not None
+
+        super().__init__(parent, st.partial_back(load_ui, ui_file))
+
+    def label(self, name=None) -> Label:
+        return self.__get_widget__('label', name)
+
+    def button(self, name=None) -> PushButton:
+        return self.__get_widget__('button', name)
+
+    def radio_button(self, name=None) -> RatioButton:
+        return self.__get_widget__('radio_button', name)
+
+    def edit(self, name=None) -> LineEdit:
+        return self.__get_widget__('edit', name)
+
+    def date_edit(self, name=None) -> DateEdit:
+        return self.__get_widget__('date_edit', name)
+
+    def date_time_edit(self, name=None) -> DateTimeEdit:
+        return self.__get_widget__('date_time_edit', name)
+
+    def time_edit(self, name=None) -> TimeEdit:
+        return self.__get_widget__('time', name)
+
+    def text_edit(self, name=None) -> TextEdit:
+        return self.__get_widget__('text_edit', name)
+
+    def plot_widget(self, name=None) -> PlotWidget:
+        return self.__get_widget__('plot_widget', name)
+
+    def list(self, name=None) -> ListWidget:
+        return self.__get_widget__('list', name)
+
+    def combo(self, name=None) -> ComboBox:
+        return self.__get_widget__('combo', name)
+
+    def container(self, name=None) -> Widget:
+        if name is None:
+            return self.w
+        return self.__get_widget__('container', name)
+
+    def dock(self, name=None) -> DockWidget:
+        return self.__get_widget__('dock', name)
+
+    def group(self, name=None) -> GroupBox:
+        return self.__get_widget__('group', name)
+
+    def spin(self, name=None) -> SpinBox:
+        return self.__get_widget__('spin', name)
+
+    def table(self, name=None) -> TableWidget:
+        return self.__get_widget__('table', name)
+
+    def table_view(self, name=None) -> TableView:
+        return self.__get_widget__('table_view', name)
+
+    def tab(self, name=None) -> TabWidget:
+        return self.__get_widget__('tab', name)
+
+    def double(self, name=None) -> DoubleSpinBox:
+        return self.__get_widget__('double', name)
+
+    def action(self, name=None) -> Action:
+        obj = self.__get_widget__('action', name)
+        if getattr(obj, 'excited', None) is None:
+            obj.excited = SignalSender()
+            obj.triggered.connect(obj.excited.emit)
+
+            def set_enabled(status=True):
+                obj.setEnabled(status)
+
+            def set_disabled(status=True):
+                obj.setEnabled(not status)
+
+            def click():
+                if obj.isEnabled():
+                    obj.trigger()
+
+            obj.click = click
+            obj.set_enabled = set_enabled
+            obj.set_disabled = set_disabled
+        return obj
+
+    def widget(self, name=None) -> Widget:
+        return self.container(name).center_widget
+
+    def layout(self, name=None) -> Layout:
+        return self.__get_widget__('layout', name)
+
+    def __get_widget__(self, type_name, obj_name):
+        return getattr(self.w, type_name + '_' + obj_name, None) or getattr(self.w, obj_name + '_' + type_name)
```

### Comparing `quite6-1.0.5/quite6/deferred_function.py` & `quite6-1.0.6/quite6/deferred_function.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from PySide6.QtCore import QSize, QPoint, QMarginsF
-from PySide6.QtGui import QPicture, QPixmap, QPainter, QPageSize, QPageLayout
-from PySide6.QtPrintSupport import QPrinter
-from PySide6.QtWidgets import QWidget, QMainWindow, QDockWidget, QHBoxLayout
-
-from . import Widget, SquareLayout
-from . import WidgetController
-from . import deferred_define
-
-
-@deferred_define
-def set_central_widget(self: Widget, widget, del_pre_widget=True):
-    if isinstance(widget, WidgetController):
-        widget = widget.w
-    if not isinstance(widget, QWidget):
-        raise TypeError('Only Support Widget or WidgetController')
-    widget.setVisible(True)  # ensure widget is visible
-
-    if hasattr(self, 'center_widget'):
-        self.layout().removeWidget(self.center_widget)
-        self.center_widget.setVisible(False)  # hide pre widget, and widget can reuse
-        if del_pre_widget:
-            self.center_widget.deleteLater()
-
-    if isinstance(self, QMainWindow):
-        self.setCentralWidget(widget)
-    elif isinstance(self, QDockWidget):
-        self.setWidget(widget)
-    elif hasattr(self, 'center_widget'):
-        self.layout().addWidget(widget)
-    else:
-        layout = QHBoxLayout()
-        layout.setSpacing(0)
-        layout.setContentsMargins(0, 0, 0, 0)
-        layout.addWidget(widget)
-        self.setLayout(layout)
-    self.center_widget = widget
-
-
-@deferred_define
-def set_square_widget(self: Widget, widget: Widget, spacing=0):
-    if isinstance(widget, WidgetController):
-        widget = widget.w
-    if not isinstance(widget, QWidget):
-        raise TypeError('Only Support Widget or WidgetController')
-
-    layout = SquareLayout()
-    layout.setSpacing(spacing)
-    layout.addWidget(widget)
-    self.setLayout(layout)
-    self.center_widget = widget
-
-
-@deferred_define
-def set_layout_spacing(self: Widget, spacing):
-    layout = self.layout()
-    assert isinstance(layout, SquareLayout)
-    layout.setSpacing(spacing)
-    layout.update()
-
-
-@deferred_define
-def export_to_pdf(self: Widget, filename: str, export_size=QSize(1060, 730)):
-    assert isinstance(export_size, QSize)
-    w, h = self.size
-    if w > h:
-        self.resize(export_size.width(), export_size.height())
-    else:
-        self.resize(export_size.height(), export_size.width())
-
-    p = QPicture()
-    painter = QPainter(p)
-    self.render(painter, QPoint(0, 0))
-    painter.end()
-
-    printer = QPrinter(QPrinter.PrinterMode.HighResolution)
-    printer.setOutputFormat(QPrinter.OutputFormat.PdfFormat)
-    printer.setOutputFileName(filename)
-    page_layout = printer.pageLayout()
-    if w > h:
-        page_layout.setOrientation(QPageLayout.Orientation.Landscape)
-    if export_size.width() != 1060 or export_size.height() != 730:
-        page_layout.setPageSize(QPageSize.PageSizeId.Custom)
-        page_size = QPageSize(QSize(int(self.size[1] * 0.8 + 20), int(self.size[0] * 0.8 + 20)))
-        page_layout.setPageSize(page_size, QMarginsF())
-    printer.setPageLayout(page_layout)
-
-    painter = QPainter()
-    ok = painter.begin(printer)
-    if ok:
-        painter.drawPicture(0, 0, p)
-        ok = painter.end()
-    self.resize(w, h)
-    return ok
-
-
-@deferred_define
-def export_to_bitmap(self: Widget, filename: str, export_size=QSize(1060, 730)):
-    if filename.endswith('pdf'):
-        return export_to_pdf(self, filename)
-    assert isinstance(export_size, QSize)
-    w, h = self.size
-    if w > h:
-        self.resize(export_size.width(), export_size.height())
-    else:
-        self.resize(export_size.height(), export_size.width())
-
-    p = QPixmap(*self.size)
-    painter = QPainter(p)
-    self.render(painter, QPoint(0, 0))
-    painter.end()
-    ok = p.save(filename)
-
-    self.resize(w, h)
-    return ok
+from PySide6.QtCore import QSize, QPoint, QMarginsF
+from PySide6.QtGui import QPicture, QPixmap, QPainter, QPageSize, QPageLayout
+from PySide6.QtPrintSupport import QPrinter
+from PySide6.QtWidgets import QWidget, QMainWindow, QDockWidget, QHBoxLayout
+
+from . import Widget, SquareLayout
+from . import WidgetController
+from . import deferred_define
+
+
+@deferred_define
+def set_central_widget(self: Widget, widget, del_pre_widget=True):
+    if isinstance(widget, WidgetController):
+        widget = widget.w
+    if not isinstance(widget, QWidget):
+        raise TypeError('Only Support Widget or WidgetController')
+    widget.setVisible(True)  # ensure widget is visible
+
+    if hasattr(self, 'center_widget'):
+        self.layout().removeWidget(self.center_widget)
+        self.center_widget.setVisible(False)  # hide pre widget, and widget can reuse
+        if del_pre_widget:
+            self.center_widget.deleteLater()
+
+    if isinstance(self, QMainWindow):
+        self.setCentralWidget(widget)
+    elif isinstance(self, QDockWidget):
+        self.setWidget(widget)
+    elif hasattr(self, 'center_widget'):
+        self.layout().addWidget(widget)
+    else:
+        layout = QHBoxLayout()
+        layout.setSpacing(0)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.addWidget(widget)
+        self.setLayout(layout)
+    self.center_widget = widget
+
+
+@deferred_define
+def set_square_widget(self: Widget, widget: Widget, spacing=0):
+    if isinstance(widget, WidgetController):
+        widget = widget.w
+    if not isinstance(widget, QWidget):
+        raise TypeError('Only Support Widget or WidgetController')
+
+    layout = SquareLayout()
+    layout.setSpacing(spacing)
+    layout.addWidget(widget)
+    self.setLayout(layout)
+    self.center_widget = widget
+
+
+@deferred_define
+def set_layout_spacing(self: Widget, spacing):
+    layout = self.layout()
+    assert isinstance(layout, SquareLayout)
+    layout.setSpacing(spacing)
+    layout.update()
+
+
+@deferred_define
+def export_to_pdf(self: Widget, filename: str, export_size=QSize(1060, 730)):
+    assert isinstance(export_size, QSize)
+    w, h = self.size
+    if w > h:
+        self.resize(export_size.width(), export_size.height())
+    else:
+        self.resize(export_size.height(), export_size.width())
+
+    p = QPicture()
+    painter = QPainter(p)
+    self.render(painter, QPoint(0, 0))
+    painter.end()
+
+    printer = QPrinter(QPrinter.PrinterMode.HighResolution)
+    printer.setOutputFormat(QPrinter.OutputFormat.PdfFormat)
+    printer.setOutputFileName(filename)
+    page_layout = printer.pageLayout()
+    if w > h:
+        page_layout.setOrientation(QPageLayout.Orientation.Landscape)
+    if export_size.width() != 1060 or export_size.height() != 730:
+        page_layout.setPageSize(QPageSize.PageSizeId.Custom)
+        page_size = QPageSize(QSize(int(self.size[1] * 0.8 + 20), int(self.size[0] * 0.8 + 20)))
+        page_layout.setPageSize(page_size, QMarginsF())
+    printer.setPageLayout(page_layout)
+
+    painter = QPainter()
+    ok = painter.begin(printer)
+    if ok:
+        painter.drawPicture(0, 0, p)
+        ok = painter.end()
+    self.resize(w, h)
+    return ok
+
+
+@deferred_define
+def export_to_bitmap(self: Widget, filename: str, export_size=QSize(1060, 730)):
+    if filename.endswith('pdf'):
+        return export_to_pdf(self, filename)
+    assert isinstance(export_size, QSize)
+    w, h = self.size
+    if w > h:
+        self.resize(export_size.width(), export_size.height())
+    else:
+        self.resize(export_size.height(), export_size.width())
+
+    p = QPixmap(*self.size)
+    painter = QPainter(p)
+    self.render(painter, QPoint(0, 0))
+    painter.end()
+    ok = p.save(filename)
+
+    self.resize(w, h)
+    return ok
```

### Comparing `quite6-1.0.5/quite6/gui/__init__.py` & `quite6-1.0.6/quite6/gui/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ..core import *  # noqa: F403
-from .qt_gui import *  # noqa: F403
-from .ui_extension import ext_classes, ui_extension
-from .ui_extension import deferred_define, run_deferred_function
-
-from .interfaces import BaseInterface, ClassExecInterface
-from .interfaces import ClosedSignalInterface, ShowedSignalInterface
-from .interfaces import ChangedSignalInterface, ExcitedSignalInterface
-from .interfaces import RowChangedSignalInterface
-from .interfaces import ContainerAbilityInterface
-from .interfaces import FocusInSignalInterface
-from .interfaces import FocusOutSignalInterface
-
-from .layouts import SquareLayout
-
-from .paint import scaling, PointF, SizeF, Pen, Painter
-
-from .widgets import Widget, Dialog
-from .widgets import MainWindow, GroupBox, DockWidget
-from .widgets import Label, LineEdit, DateEdit, TextEdit, TimeEdit
-from .widgets import ListWidget, ComboBox
-from .widgets import SpinBox, DoubleSpinBox
-from .widgets import InputDialog
-from .widgets import Action, Shortcut, PushButton, RatioButton
-from .widgets import TabWidget, TableWidget, TableView
-from .widgets import PlotWidget
-from .widgets import Layout
+from ..core import *  # noqa: F403
+from .qt_gui import *  # noqa: F403
+from .ui_extension import ext_classes, ui_extension
+from .ui_extension import deferred_define, run_deferred_function
+
+from .interfaces import BaseInterface, ClassExecInterface
+from .interfaces import ClosedSignalInterface, ShowedSignalInterface
+from .interfaces import ChangedSignalInterface, ExcitedSignalInterface
+from .interfaces import RowChangedSignalInterface
+from .interfaces import ContainerAbilityInterface
+from .interfaces import FocusInSignalInterface
+from .interfaces import FocusOutSignalInterface
+
+from .layouts import SquareLayout
+
+from .paint import scaling, PointF, SizeF, Pen, Painter
+
+from .widgets import Widget, Dialog
+from .widgets import MainWindow, GroupBox, DockWidget
+from .widgets import Label, LineEdit, DateEdit, TextEdit, TimeEdit
+from .widgets import ListWidget, ComboBox
+from .widgets import SpinBox, DoubleSpinBox
+from .widgets import InputDialog
+from .widgets import Action, Shortcut, PushButton, RatioButton
+from .widgets import TabWidget, TableWidget, TableView
+from .widgets import PlotWidget
+from .widgets import Layout
```

### Comparing `quite6-1.0.5/quite6/gui/interfaces/__init__.py` & `quite6-1.0.6/quite6/gui/interfaces/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .base_interface import BaseInterface
-from .closed_signal_interface import ClosedSignalInterface
-from .showed_signal_interface import ShowedSignalInterface
-from .changed_signal_interface import ChangedSignalInterface
-from .excited_signal_interface import ExcitedSignalInterface
-from .row_changed_signal_interface import RowChangedSignalInterface
-from .ability_interfaces import ContainerAbilityInterface, ClassExecInterface
-from .focus_in_signal_interface import FocusInSignalInterface
-from .focus_out_signal_interface import FocusOutSignalInterface
+from .base_interface import BaseInterface
+from .closed_signal_interface import ClosedSignalInterface
+from .showed_signal_interface import ShowedSignalInterface
+from .changed_signal_interface import ChangedSignalInterface
+from .excited_signal_interface import ExcitedSignalInterface
+from .row_changed_signal_interface import RowChangedSignalInterface
+from .ability_interfaces import ContainerAbilityInterface, ClassExecInterface
+from .focus_in_signal_interface import FocusInSignalInterface
+from .focus_out_signal_interface import FocusOutSignalInterface
```

### Comparing `quite6-1.0.5/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py` & `quite6-1.0.6/quite6/gui/interfaces/ability_interfaces/container_ability_interface.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from PySide6.QtCore import QSize
-
-from .. import BaseInterface
-from ... import run_deferred_function
-
-
-class ContainerAbilityInterface(BaseInterface):
-    def set_central_widget(self, w, **kwargs):
-        return run_deferred_function('set_central_widget', self, w, **kwargs)
-
-    def set_square_widget(self, w, spacing=0):
-        return run_deferred_function('set_square_widget', self, w, spacing)
-
-    def set_layout_spacing(self, spacing):
-        return run_deferred_function('set_layout_spacing', self, spacing)
-
-    def export_to_image(self, filename: str, export_size=QSize(1060, 730)):
-        if filename.lower().endswith('.pdf'):
-            return self.export_to_pdf(filename, export_size)
-        else:
-            return self.export_to_bitmap(filename, export_size)
-
-    def export_to_pdf(self, filename, export_size=QSize(1060, 730)):
-        return run_deferred_function('export_to_pdf', self, filename, export_size)
-
-    def export_to_bitmap(self, filename, export_size=QSize(1060, 730)):
-        return run_deferred_function('export_to_bitmap', self, filename, export_size)
+from PySide6.QtCore import QSize
+
+from .. import BaseInterface
+from ... import run_deferred_function
+
+
+class ContainerAbilityInterface(BaseInterface):
+    def set_central_widget(self, w, **kwargs):
+        return run_deferred_function('set_central_widget', self, w, **kwargs)
+
+    def set_square_widget(self, w, spacing=0):
+        return run_deferred_function('set_square_widget', self, w, spacing)
+
+    def set_layout_spacing(self, spacing):
+        return run_deferred_function('set_layout_spacing', self, spacing)
+
+    def export_to_image(self, filename: str, export_size=QSize(1060, 730)):
+        if filename.lower().endswith('.pdf'):
+            return self.export_to_pdf(filename, export_size)
+        else:
+            return self.export_to_bitmap(filename, export_size)
+
+    def export_to_pdf(self, filename, export_size=QSize(1060, 730)):
+        return run_deferred_function('export_to_pdf', self, filename, export_size)
+
+    def export_to_bitmap(self, filename, export_size=QSize(1060, 730)):
+        return run_deferred_function('export_to_bitmap', self, filename, export_size)
```

### Comparing `quite6-1.0.5/quite6/gui/interfaces/base_interface.py` & `quite6-1.0.6/quite6/gui/interfaces/base_interface.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import prett6
-
-
-class BaseInterface(prett6.AttachAbility):
-    @property
-    def name(self) -> str:
-        # noinspection PyUnresolvedReferences
-        return self.objectName()
-
-    def set_focus(self):
-        # noinspection PyUnresolvedReferences
-        return self.setFocus()
-
-    def set_enabled(self, status=True):
-        # noinspection PyUnresolvedReferences
-        return self.setEnabled(status)
-
-    def set_disabled(self, status=True):
-        # noinspection PyUnresolvedReferences
-        return self.setEnabled(not status)
+import prett6
+
+
+class BaseInterface(prett6.AttachAbility):
+    @property
+    def name(self) -> str:
+        # noinspection PyUnresolvedReferences
+        return self.objectName()
+
+    def set_focus(self):
+        # noinspection PyUnresolvedReferences
+        return self.setFocus()
+
+    def set_enabled(self, status=True):
+        # noinspection PyUnresolvedReferences
+        return self.setEnabled(status)
+
+    def set_disabled(self, status=True):
+        # noinspection PyUnresolvedReferences
+        return self.setEnabled(not status)
```

### Comparing `quite6-1.0.5/quite6/gui/layouts/square_layout.py` & `quite6-1.0.6/quite6/gui/layouts/square_layout.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from PySide6.QtWidgets import QWidget, QWidgetItem, QLayout, QLayoutItem
-from PySide6.QtCore import Qt, QSize, QPoint, QRect
-
-
-class SquareLayout(QLayout):
-    def __init__(self, parent: QWidget = None, default_item: QWidget = None):
-        super().__init__(parent)
-
-        self.item = default_item
-        self.last_received_rect = QRect(0, 0, 0, 0)
-        self.geometry_rect = QRect(0, 0, 0, 0)
-
-        self.setSpacing(0)
-
-    def addItem(self, item: QLayoutItem):
-        if self.item is None:
-            self.replace_item(item)
-
-    def addWidget(self, w: QWidget):
-        self.addItem(QWidgetItem(w))
-
-    def take(self):
-        item, self.item = self.item, None
-        return item
-
-    def takeAt(self, index: int):
-        return self.take() if index == 0 else None
-
-    def itemAt(self, index: int):
-        return self.item if index == 0 else None
-
-    def count(self):
-        return 1 if self.item is not None else 0
-
-    def replace_item(self, item):
-        old_item, self.item = self.item, item
-        self.setGeometry(self.geometry_rect)
-        return old_item
-
-    def expandingDirections(self):
-        return Qt.Orientation.Horizontal | Qt.Orientation.Vertical
-
-    def sizeHint(self):
-        return self.minimumSize()
-
-    def minimumSize(self):
-        return self.item.minimumSize() if self.item is not None else QSize()
-
-    def hasHeightForWidth(self):
-        return False
-
-    def geometry(self):
-        return QRect(self.geometry_rect)
-
-    def setGeometry(self, rect: QRect):
-        if self.item is None or self.are_rects_equal(self.last_received_rect, rect):
-            return
-
-        self.last_received_rect = rect
-
-        proper_size = self.calculate_proper_size(rect.size())
-        proper_location = self.calculate_center_location(rect.size(), proper_size)
-
-        self.geometry_rect = QRect(proper_location, proper_size)
-        self.item.setGeometry(self.geometry_rect)
-        super().setGeometry(self.geometry_rect)
-
-    def calculate_proper_size(self, from_size: QSize):
-        minimum_length = min(from_size.width(), from_size.height())
-        return QSize(minimum_length - self.spacing(), minimum_length - self.spacing())
-
-    @staticmethod
-    def calculate_center_location(from_size: QSize, item_size: QSize):
-        x = max(from_size.width() // 2 - item_size.width() // 2, 0)
-        y = max(from_size.height() // 2 - item_size.height() // 2, 0)
-        return QPoint(x, y)
-
-    @staticmethod
-    def are_rects_equal(a: QRect, b: QRect):
-        if a.x() == b.x() and a.y() == b.y() and a.height() == b.height() and a.width() == b.width():
-            return True
-        return False
-
-    def update(self):
-        self.setGeometry(self.geometry())
+from PySide6.QtWidgets import QWidget, QWidgetItem, QLayout, QLayoutItem
+from PySide6.QtCore import Qt, QSize, QPoint, QRect
+
+
+class SquareLayout(QLayout):
+    def __init__(self, parent: QWidget = None, default_item: QWidget = None):
+        super().__init__(parent)
+
+        self.item = default_item
+        self.last_received_rect = QRect(0, 0, 0, 0)
+        self.geometry_rect = QRect(0, 0, 0, 0)
+
+        self.setSpacing(0)
+
+    def addItem(self, item: QLayoutItem):
+        if self.item is None:
+            self.replace_item(item)
+
+    def addWidget(self, w: QWidget):
+        self.addItem(QWidgetItem(w))
+
+    def take(self):
+        item, self.item = self.item, None
+        return item
+
+    def takeAt(self, index: int):
+        return self.take() if index == 0 else None
+
+    def itemAt(self, index: int):
+        return self.item if index == 0 else None
+
+    def count(self):
+        return 1 if self.item is not None else 0
+
+    def replace_item(self, item):
+        old_item, self.item = self.item, item
+        self.setGeometry(self.geometry_rect)
+        return old_item
+
+    def expandingDirections(self):
+        return Qt.Orientation.Horizontal | Qt.Orientation.Vertical
+
+    def sizeHint(self):
+        return self.minimumSize()
+
+    def minimumSize(self):
+        return self.item.minimumSize() if self.item is not None else QSize()
+
+    def hasHeightForWidth(self):
+        return False
+
+    def geometry(self):
+        return QRect(self.geometry_rect)
+
+    def setGeometry(self, rect: QRect):
+        if self.item is None or self.are_rects_equal(self.last_received_rect, rect):
+            return
+
+        self.last_received_rect = rect
+
+        proper_size = self.calculate_proper_size(rect.size())
+        proper_location = self.calculate_center_location(rect.size(), proper_size)
+
+        self.geometry_rect = QRect(proper_location, proper_size)
+        self.item.setGeometry(self.geometry_rect)
+        super().setGeometry(self.geometry_rect)
+
+    def calculate_proper_size(self, from_size: QSize):
+        minimum_length = min(from_size.width(), from_size.height())
+        return QSize(minimum_length - self.spacing(), minimum_length - self.spacing())
+
+    @staticmethod
+    def calculate_center_location(from_size: QSize, item_size: QSize):
+        x = max(from_size.width() // 2 - item_size.width() // 2, 0)
+        y = max(from_size.height() // 2 - item_size.height() // 2, 0)
+        return QPoint(x, y)
+
+    @staticmethod
+    def are_rects_equal(a: QRect, b: QRect):
+        if a.x() == b.x() and a.y() == b.y() and a.height() == b.height() and a.width() == b.width():
+            return True
+        return False
+
+    def update(self):
+        self.setGeometry(self.geometry())
```

### Comparing `quite6-1.0.5/quite6/gui/paint/painter.py` & `quite6-1.0.6/quite6/gui/paint/painter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-from PySide6.QtCore import QRectF
-from PySide6.QtGui import QPainter, QColor, QPen, Qt
-
-from . import PointF, SizeF, scaling
-
-
-class Painter(QPainter):
-    default_background_color = QColor(222, 222, 222, 196)
-
-    def draw_text(self,
-                  text_rect: QRectF,
-                  text: str,
-                  color: QColor = None,
-                  background_color: QColor = None,
-                  background_round_size: int = 2):
-        current_pen = self.pen()
-
-        self.setPen(QColor(0, 0, 0, 0))
-        if background_color:
-            self.setBrush(background_color)
-        else:
-            self.setBrush(self.default_background_color)
-        self.drawRoundedRect(text_rect, background_round_size, background_round_size)
-        if color:
-            self.setPen(QPen(color))
-        else:
-            self.setPen(current_pen)
-        self.drawText(text_rect, Qt.AlignmentFlag.AlignCenter, text)
-
-        if color:
-            self.setPen(current_pen)
-
-    def draw_text_top(self,
-                      position: PointF,
-                      text: str,
-                      margin: int = 3,
-                      color: QColor = None,
-                      background_color: QColor = None,
-                      background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.half_width().height_add(margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_top_left(self,
-                           position: PointF,
-                           text: str,
-                           margin: int = 3,
-                           color: QColor = None,
-                           background_color: QColor = None,
-                           background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.width_add(margin).height_add(margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_bottom(self,
-                         position: PointF,
-                         text: str,
-                         margin: int = 3,
-                         color: QColor = None,
-                         background_color: QColor = None,
-                         background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.half_width().height_set(-margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_left(self,
-                       position: PointF,
-                       text: str,
-                       margin: int = 3,
-                       color: QColor = None,
-                       background_color: QColor = None,
-                       background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.half_height().width_add(margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_right(self,
-                        position: PointF,
-                        text: str,
-                        margin: int = 3,
-                        color: QColor = None,
-                        background_color: QColor = None,
-                        background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.half_height().width_set(-margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_bottom_left(self,
-                              position: PointF,
-                              text: str,
-                              margin: int = 3,
-                              color: QColor = None,
-                              background_color: QColor = None,
-                              background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position - text_size.width_add(margin).height_set(-margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
-
-    def draw_text_bottom_right(self,
-                               position: PointF,
-                               text: str,
-                               margin: int = 3,
-                               color: QColor = None,
-                               background_color: QColor = None,
-                               background_color_round_size: int = 2):
-        text_size = SizeF.text_size(text, self.font())
-        text_rect = text_size.to_rect(position.x_add(margin).y_add(margin * scaling.ratio))
-
-        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+from PySide6.QtCore import QRectF
+from PySide6.QtGui import QPainter, QColor, QPen, Qt
+
+from . import PointF, SizeF, scaling
+
+
+class Painter(QPainter):
+    default_background_color = QColor(222, 222, 222, 196)
+
+    def draw_text(self,
+                  text_rect: QRectF,
+                  text: str,
+                  color: QColor = None,
+                  background_color: QColor = None,
+                  background_round_size: int = 2):
+        current_pen = self.pen()
+
+        self.setPen(QColor(0, 0, 0, 0))
+        if background_color:
+            self.setBrush(background_color)
+        else:
+            self.setBrush(self.default_background_color)
+        self.drawRoundedRect(text_rect, background_round_size, background_round_size)
+        if color:
+            self.setPen(QPen(color))
+        else:
+            self.setPen(current_pen)
+        self.drawText(text_rect, Qt.AlignmentFlag.AlignCenter, text)
+
+        if color:
+            self.setPen(current_pen)
+
+    def draw_text_top(self,
+                      position: PointF,
+                      text: str,
+                      margin: int = 3,
+                      color: QColor = None,
+                      background_color: QColor = None,
+                      background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.half_width().height_add(margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_top_left(self,
+                           position: PointF,
+                           text: str,
+                           margin: int = 3,
+                           color: QColor = None,
+                           background_color: QColor = None,
+                           background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.width_add(margin).height_add(margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_bottom(self,
+                         position: PointF,
+                         text: str,
+                         margin: int = 3,
+                         color: QColor = None,
+                         background_color: QColor = None,
+                         background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.half_width().height_set(-margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_left(self,
+                       position: PointF,
+                       text: str,
+                       margin: int = 3,
+                       color: QColor = None,
+                       background_color: QColor = None,
+                       background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.half_height().width_add(margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_right(self,
+                        position: PointF,
+                        text: str,
+                        margin: int = 3,
+                        color: QColor = None,
+                        background_color: QColor = None,
+                        background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.half_height().width_set(-margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_bottom_left(self,
+                              position: PointF,
+                              text: str,
+                              margin: int = 3,
+                              color: QColor = None,
+                              background_color: QColor = None,
+                              background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position - text_size.width_add(margin).height_set(-margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
+
+    def draw_text_bottom_right(self,
+                               position: PointF,
+                               text: str,
+                               margin: int = 3,
+                               color: QColor = None,
+                               background_color: QColor = None,
+                               background_color_round_size: int = 2):
+        text_size = SizeF.text_size(text, self.font())
+        text_rect = text_size.to_rect(position.x_add(margin).y_add(margin * scaling.ratio))
+
+        self.draw_text(text_rect, text, color, background_color, background_color_round_size)
```

### Comparing `quite6-1.0.5/quite6/gui/paint/point.py` & `quite6-1.0.6/quite6/gui/paint/point.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from PySide6.QtCore import QPointF, QSizeF
-
-
-class PointF(QPointF):
-    def __add__(self, other):
-        if isinstance(other, QSizeF):
-            return PointF(self.x() + other.width(), self.y() + other.height())
-        else:
-            return PointF(self.x() + other.x(), self.y() + other.y())
-
-    def __sub__(self, other):
-        if isinstance(other, QSizeF):
-            return PointF(self.x() - other.width(), self.y() - other.height())
-        else:
-            return PointF(self.x() - other.x(), self.y() - other.y())
-
-    def __mul__(self, other):
-        return PointF(self.x() * other, self.y() * other)
-
-    def x_add(self, v):
-        return PointF(self.x() + v, self.y())
-
-    def x_sub(self, v):
-        return PointF(self.x() - v, self.y())
-
-    def y_add(self, v):
-        return PointF(self.x(), self.y() + v)
-
-    def y_sub(self, v):
-        return PointF(self.x(), self.y() - v)
+from PySide6.QtCore import QPointF, QSizeF
+
+
+class PointF(QPointF):
+    def __add__(self, other):
+        if isinstance(other, QSizeF):
+            return PointF(self.x() + other.width(), self.y() + other.height())
+        else:
+            return PointF(self.x() + other.x(), self.y() + other.y())
+
+    def __sub__(self, other):
+        if isinstance(other, QSizeF):
+            return PointF(self.x() - other.width(), self.y() - other.height())
+        else:
+            return PointF(self.x() - other.x(), self.y() - other.y())
+
+    def __mul__(self, other):
+        return PointF(self.x() * other, self.y() * other)
+
+    def x_add(self, v):
+        return PointF(self.x() + v, self.y())
+
+    def x_sub(self, v):
+        return PointF(self.x() - v, self.y())
+
+    def y_add(self, v):
+        return PointF(self.x(), self.y() + v)
+
+    def y_sub(self, v):
+        return PointF(self.x(), self.y() - v)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/combo_box.py` & `quite6-1.0.6/quite6/gui/widgets/combo_box.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import prett6
-import st
-from PySide6.QtWidgets import QComboBox
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class ComboBox(QComboBox, BaseInterface, prett6.WidgetStringInterface, prett6.WidgetIndexInterface,
-               prett6.WidgetStringListInterface):
-    class ComboBoxItem:
-        def __init__(self, parent: 'ComboBox'):
-            self.parent = parent
-
-        @property
-        def count(self):
-            return self.parent.count()
-
-        def add_strings(self, *text):
-            self.parent.addItems(text)
-
-    class StringItem(ComboBoxItem, prett6.WidgetStringItem):
-        def get_value(self):
-            return self.parent.currentText()
-
-        def set_value(self, value=None):
-            texts = self.parent.string_list.value
-            assert isinstance(texts, list)
-
-            if value is None:
-                self.parent.index.value = 0
-            elif value in texts:
-                self.parent.index.value = texts.index(value)
-            else:
-                self.add_strings(value)
-                self.parent.index.value = self.count - 1
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentIndexChanged[int].connect(self.check_change)
-
-    class IndexItem(ComboBoxItem, prett6.IndexItem):
-        def get_value(self):
-            return self.parent.currentIndex()
-
-        def set_value(self, value):
-            if value is None or value >= self.count:
-                value = 0
-            self.parent.setCurrentIndex(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentIndexChanged[int].connect(self.check_change)
-
-    class StringsItem(ComboBoxItem, prett6.StringsItem):
-        def get_value(self):
-            return st.foreach(self.parent.itemText, range(self.count))
-
-        def set_value(self, value):
-            value = value or []
-
-            old_count = self.count
-            new_count = len(value)
-            for i in range(min(old_count, new_count)):
-                self.parent.setItemText(i, value[i])
-            for index in reversed(range(new_count, old_count)):
-                self.parent.removeItem(index)
-
-            self.parent.addItems(value[old_count:new_count])
-
-            self.parent.index.emit_changed()
-            self.parent.string.emit_changed()
-
-            self.string_list.check_change()
+import prett6
+import st
+from PySide6.QtWidgets import QComboBox
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class ComboBox(QComboBox, BaseInterface, prett6.WidgetStringInterface, prett6.WidgetIndexInterface,
+               prett6.WidgetStringListInterface):
+    class ComboBoxItem:
+        def __init__(self, parent: 'ComboBox'):
+            self.parent = parent
+
+        @property
+        def count(self):
+            return self.parent.count()
+
+        def add_strings(self, *text):
+            self.parent.addItems(text)
+
+    class StringItem(ComboBoxItem, prett6.WidgetStringItem):
+        def get_value(self):
+            return self.parent.currentText()
+
+        def set_value(self, value=None):
+            texts = self.parent.string_list.value
+            assert isinstance(texts, list)
+
+            if value is None:
+                self.parent.index.value = 0
+            elif value in texts:
+                self.parent.index.value = texts.index(value)
+            else:
+                self.add_strings(value)
+                self.parent.index.value = self.count - 1
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentIndexChanged[int].connect(self.check_change)
+
+    class IndexItem(ComboBoxItem, prett6.IndexItem):
+        def get_value(self):
+            return self.parent.currentIndex()
+
+        def set_value(self, value):
+            if value is None or value >= self.count:
+                value = 0
+            self.parent.setCurrentIndex(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentIndexChanged[int].connect(self.check_change)
+
+    class StringsItem(ComboBoxItem, prett6.StringsItem):
+        def get_value(self):
+            return st.foreach(self.parent.itemText, range(self.count))
+
+        def set_value(self, value):
+            value = value or []
+
+            old_count = self.count
+            new_count = len(value)
+            for i in range(min(old_count, new_count)):
+                self.parent.setItemText(i, value[i])
+            for index in reversed(range(new_count, old_count)):
+                self.parent.removeItem(index)
+
+            self.parent.addItems(value[old_count:new_count])
+
+            self.parent.index.emit_changed()
+            self.parent.string.emit_changed()
+
+            self.string_list.check_change()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/date_edit.py` & `quite6-1.0.6/quite6/gui/widgets/date_edit.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import prett6
-from PySide6.QtCore import QDate
-from PySide6.QtWidgets import QDateEdit
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class DateEdit(QDateEdit, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'DateEdit'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            value = value or ''
-            if value != self.get_value():
-                date = value.split('-')
-                if len(date) != 3:
-                    raise ValueError('Date format is invalid')
-                self.parent.setDate(QDate(int(date[0]), int(date[1]), int(date[2])))
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.dateChanged.connect(self.string.check_change)
+import prett6
+from PySide6.QtCore import QDate
+from PySide6.QtWidgets import QDateEdit
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class DateEdit(QDateEdit, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'DateEdit'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            value = value or ''
+            if value != self.get_value():
+                date = value.split('-')
+                if len(date) != 3:
+                    raise ValueError('Date format is invalid')
+                self.parent.setDate(QDate(int(date[0]), int(date[1]), int(date[2])))
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.dateChanged.connect(self.string.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/date_time_edit.py` & `quite6-1.0.6/quite6/gui/widgets/double_spin_box.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import prett6
-from PySide6.QtWidgets import QDateTimeEdit
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class DateTimeEdit(QDateTimeEdit, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'DateTimeEdit'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            value = value or ''
-            self.parent.setDate(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.dateChanged.connect(self.string.check_change)
+import prett6
+from PySide6.QtWidgets import QDoubleSpinBox
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class DoubleSpinBox(QDoubleSpinBox, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'DoubleSpinBox'):
+            self.parent = parent
+
+        def get_value(self):
+            return str(self.parent.value())
+
+        def set_value(self, value):
+            if self.get_value() != value:
+                self.parent.setValue(float(value or 0))
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.valueChanged[float].connect(self.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/double_spin_box.py` & `quite6-1.0.6/quite6/gui/widgets/spin_box.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import prett6
-from PySide6.QtWidgets import QDoubleSpinBox
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class DoubleSpinBox(QDoubleSpinBox, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'DoubleSpinBox'):
-            self.parent = parent
-
-        def get_value(self):
-            return str(self.parent.value())
-
-        def set_value(self, value):
-            if self.get_value() != value:
-                self.parent.setValue(float(value or 0))
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.valueChanged[float].connect(self.check_change)
+import prett6
+from PySide6.QtWidgets import QSpinBox
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class SpinBox(QSpinBox, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'SpinBox'):
+            self.parent = parent
+
+        def get_value(self):
+            return str(self.parent.value())
+
+        def set_value(self, value):
+            if self.get_value() != value:
+                self.parent.setValue(int(value or 0))
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.valueChanged[int].connect(self.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/input_dialog.py` & `quite6-1.0.6/quite6/gui/widgets/input_dialog.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from PySide6.QtWidgets import QInputDialog
-
-from .. import ui_extension
-
-
-@ui_extension
-class InputDialog(QInputDialog):
-    @staticmethod
-    def get_double(parent=None,
-                   title='Input Double Value',
-                   label='Value:',
-                   default_value=None,
-                   decimals=1,
-                   minimum=1,
-                   maximum=1e9):
-        input_dialog = QInputDialog(parent)
-        input_dialog.setInputMode(InputDialog.DoubleInput)
-        input_dialog.setWindowTitle(title)
-        input_dialog.setLabelText(label)
-        input_dialog.setOkButtonText('确定')
-        input_dialog.setCancelButtonText('取消')
-        input_dialog.setDoubleDecimals(decimals)
-        input_dialog.setDoubleRange(minimum, maximum)
-        input_dialog.setDoubleValue(default_value or minimum)
-        input_dialog.setFont(parent.font())
-
-        return default_value if not input_dialog.exec_() else input_dialog.doubleValue()
-
-    @staticmethod
-    def get_int(parent=None, title='Input Int Value', label='Value:', default_value=None, minimum=1, maximum=100):
-        input_dialog = QInputDialog(parent)
-        input_dialog.setInputMode(InputDialog.IntInput)
-        input_dialog.setWindowTitle(title)
-        input_dialog.setLabelText(label)
-        input_dialog.setOkButtonText('确定')
-        input_dialog.setCancelButtonText('取消')
-        input_dialog.setIntRange(minimum, maximum)
-        input_dialog.setIntValue(default_value or minimum)
-        input_dialog.setFont(parent.font())
-
-        return default_value if not input_dialog.exec_() else input_dialog.intValue()
+from PySide6.QtWidgets import QInputDialog
+
+from .. import ui_extension
+
+
+@ui_extension
+class InputDialog(QInputDialog):
+    @staticmethod
+    def get_double(parent=None,
+                   title='Input Double Value',
+                   label='Value:',
+                   default_value=None,
+                   decimals=1,
+                   minimum=1,
+                   maximum=1e9):
+        input_dialog = QInputDialog(parent)
+        input_dialog.setInputMode(InputDialog.DoubleInput)
+        input_dialog.setWindowTitle(title)
+        input_dialog.setLabelText(label)
+        input_dialog.setOkButtonText('确定')
+        input_dialog.setCancelButtonText('取消')
+        input_dialog.setDoubleDecimals(decimals)
+        input_dialog.setDoubleRange(minimum, maximum)
+        input_dialog.setDoubleValue(default_value or minimum)
+        input_dialog.setFont(parent.font())
+
+        return default_value if not input_dialog.exec_() else input_dialog.doubleValue()
+
+    @staticmethod
+    def get_int(parent=None, title='Input Int Value', label='Value:', default_value=None, minimum=1, maximum=100):
+        input_dialog = QInputDialog(parent)
+        input_dialog.setInputMode(InputDialog.IntInput)
+        input_dialog.setWindowTitle(title)
+        input_dialog.setLabelText(label)
+        input_dialog.setOkButtonText('确定')
+        input_dialog.setCancelButtonText('取消')
+        input_dialog.setIntRange(minimum, maximum)
+        input_dialog.setIntValue(default_value or minimum)
+        input_dialog.setFont(parent.font())
+
+        return default_value if not input_dialog.exec_() else input_dialog.intValue()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/label.py` & `quite6-1.0.6/quite6/gui/widgets/label.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import prett6
-from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QLabel
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class Label(QLabel, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'Label'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            self.parent.setText(value or '')
-
-    def set_clickable_text(self, show_text, call_data, call_func):
-        self.setText("<a href=\"{}\">{}</a>".format(call_data, show_text))
-        self.setTextFormat(Qt.TextFormat.RichText)
-        self.linkActivated.connect(call_func)
+import prett6
+from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QLabel
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class Label(QLabel, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'Label'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            self.parent.setText(value or '')
+
+    def set_clickable_text(self, show_text, call_data, call_func):
+        self.setText("<a href=\"{}\">{}</a>".format(call_data, show_text))
+        self.setTextFormat(Qt.TextFormat.RichText)
+        self.linkActivated.connect(call_func)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/line_edit.py` & `quite6-1.0.6/quite6/gui/widgets/line_edit.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import prett6
-from PySide6.QtWidgets import QLineEdit
-
-from .. import FocusInSignalInterface, FocusOutSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class LineEdit(QLineEdit, prett6.WidgetStringInterface, FocusInSignalInterface, FocusOutSignalInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'LineEdit'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            value = value or ''
-            if value != self.get_value():
-                self.parent.setText(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.textChanged.connect(self.string.check_change)
-
-    def focusInEvent(self, e):
-        super().focusInEvent(e)
-        self.focus_in.emit(self.string.value)
-
-    def focusOutEvent(self, e):
-        super().focusOutEvent(e)
-        self.focus_out.emit(self.string.value)
+import prett6
+from PySide6.QtWidgets import QLineEdit
+
+from .. import FocusInSignalInterface, FocusOutSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class LineEdit(QLineEdit, prett6.WidgetStringInterface, FocusInSignalInterface, FocusOutSignalInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'LineEdit'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            value = value or ''
+            if value != self.get_value():
+                self.parent.setText(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.textChanged.connect(self.string.check_change)
+
+    def focusInEvent(self, e):
+        super().focusInEvent(e)
+        self.focus_in.emit(self.string.value)
+
+    def focusOutEvent(self, e):
+        super().focusOutEvent(e)
+        self.focus_out.emit(self.string.value)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/list_widget.py` & `quite6-1.0.6/quite6/gui/widgets/list_widget.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import prett6
-import st
-from PySide6.QtWidgets import QListWidget
-
-from .. import ExcitedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class ListWidget(QListWidget, ExcitedSignalInterface, prett6.WidgetStringInterface, prett6.WidgetIndexInterface,
-                 prett6.WidgetStringListInterface):
-    def set_excited_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.doubleClicked.connect(st.zero_para(self.excited.emit))
-
-    class ListWidgetItem:
-        def __init__(self, parent: 'ListWidget'):
-            self.parent = parent
-
-        @property
-        def count(self):
-            return self.parent.count()
-
-        def item_text(self, idx):
-            return self.parent.item(idx).text()
-
-        def add_text(self, *text):
-            self.parent.addItems(text)
-
-    class StringItem(ListWidgetItem, prett6.WidgetStringItem):
-        def get_value(self):
-            if self.parent.index.value >= 0:
-                return self.parent.currentItem().text()
-            return None
-
-        def set_value(self, value):
-            texts = self.parent.string_list.value
-            assert isinstance(texts, list)
-            if value is None:
-                self.parent.index.value = 0
-            elif value in texts:
-                self.parent.index.value = texts.index(value)
-            else:
-                self.add_text(value)
-                self.parent.index.value = self.count - 1
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentTextChanged.connect(self.check_change)
-
-    class IndexItem(ListWidgetItem, prett6.IndexItem):
-        def get_value(self):
-            return self.parent.currentRow()
-
-        def set_value(self, value):
-            value = value or 0
-            self.parent.setCurrentRow(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentRowChanged.connect(self.check_change)
-
-    class StringsItem(ListWidgetItem, prett6.StringsItem):
-        def get_value(self):
-            return st.foreach(self.item_text, range(self.count))
-
-        def set_value(self, value):
-            value = value or []
-
-            self.parent.clear()
-            self.parent.addItems(value)
-            self.check_change()
+import prett6
+import st
+from PySide6.QtWidgets import QListWidget
+
+from .. import ExcitedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class ListWidget(QListWidget, ExcitedSignalInterface, prett6.WidgetStringInterface, prett6.WidgetIndexInterface,
+                 prett6.WidgetStringListInterface):
+    def set_excited_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.doubleClicked.connect(st.zero_para(self.excited.emit))
+
+    class ListWidgetItem:
+        def __init__(self, parent: 'ListWidget'):
+            self.parent = parent
+
+        @property
+        def count(self):
+            return self.parent.count()
+
+        def item_text(self, idx):
+            return self.parent.item(idx).text()
+
+        def add_text(self, *text):
+            self.parent.addItems(text)
+
+    class StringItem(ListWidgetItem, prett6.WidgetStringItem):
+        def get_value(self):
+            if self.parent.index.value >= 0:
+                return self.parent.currentItem().text()
+            return None
+
+        def set_value(self, value):
+            texts = self.parent.string_list.value
+            assert isinstance(texts, list)
+            if value is None:
+                self.parent.index.value = 0
+            elif value in texts:
+                self.parent.index.value = texts.index(value)
+            else:
+                self.add_text(value)
+                self.parent.index.value = self.count - 1
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentTextChanged.connect(self.check_change)
+
+    class IndexItem(ListWidgetItem, prett6.IndexItem):
+        def get_value(self):
+            return self.parent.currentRow()
+
+        def set_value(self, value):
+            value = value or 0
+            self.parent.setCurrentRow(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentRowChanged.connect(self.check_change)
+
+    class StringsItem(ListWidgetItem, prett6.StringsItem):
+        def get_value(self):
+            return st.foreach(self.item_text, range(self.count))
+
+        def set_value(self, value):
+            value = value or []
+
+            self.parent.clear()
+            self.parent.addItems(value)
+            self.check_change()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/main_window.py` & `quite6-1.0.6/quite6/gui/widgets/main_window.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PySide6.QtGui import QCloseEvent
-from PySide6.QtWidgets import QMainWindow
-
-from .. import ClassExecInterface
-from .. import ClosedSignalInterface
-from .. import ContainerAbilityInterface
-from .. import EventLoop
-from .. import ui_extension
-
-
-@ui_extension
-class MainWindow(QMainWindow, ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface):
-    def closeEvent(self, event: QCloseEvent):
-        if self.can_close:
-            self.closed.emit()
-            event.accept()
-        else:
-            self.cannot_closed.emit()
-            event.ignore()
-
-    def exec(self):
-        with EventLoop() as event:
-            self.show()
-            self.closed.connect(event.quit)
+from PySide6.QtGui import QCloseEvent
+from PySide6.QtWidgets import QMainWindow
+
+from .. import ClassExecInterface
+from .. import ClosedSignalInterface
+from .. import ContainerAbilityInterface
+from .. import EventLoop
+from .. import ui_extension
+
+
+@ui_extension
+class MainWindow(QMainWindow, ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface):
+    def closeEvent(self, event: QCloseEvent):
+        if self.can_close:
+            self.closed.emit()
+            event.accept()
+        else:
+            self.cannot_closed.emit()
+            event.ignore()
+
+    def exec(self):
+        with EventLoop() as event:
+            self.show()
+            self.closed.connect(event.quit)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/push_button.py` & `quite6-1.0.6/quite6/gui/widgets/push_button.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import prett6
-from PySide6.QtWidgets import QPushButton
-
-from .. import ExcitedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class PushButton(QPushButton, ExcitedSignalInterface, prett6.WidgetStringInterface):
-    def set_excited_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.clicked.connect(self.excited.emit)
-
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'PushButton'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            self.parent.setText(value or '')
-            self.check_change()
+import prett6
+from PySide6.QtWidgets import QPushButton
+
+from .. import ExcitedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class PushButton(QPushButton, ExcitedSignalInterface, prett6.WidgetStringInterface):
+    def set_excited_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.clicked.connect(self.excited.emit)
+
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'PushButton'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            self.parent.setText(value or '')
+            self.check_change()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/radio_button.py` & `quite6-1.0.6/quite6/gui/widgets/radio_button.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import prett6
-from PySide6.QtWidgets import QRadioButton
-
-from .. import ExcitedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class RatioButton(QRadioButton, ExcitedSignalInterface, prett6.WidgetStringInterface):
-    def set_excited_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.clicked.connect(self.excited.emit)
-
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'RatioButton'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            self.parent.setText(value or '')
-            self.check_change()
+import prett6
+from PySide6.QtWidgets import QRadioButton
+
+from .. import ExcitedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class RatioButton(QRadioButton, ExcitedSignalInterface, prett6.WidgetStringInterface):
+    def set_excited_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.clicked.connect(self.excited.emit)
+
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'RatioButton'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            self.parent.setText(value or '')
+            self.check_change()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/shortcut.py` & `quite6-1.0.6/quite6/gui/widgets/shortcut.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from PySide6.QtGui import QShortcut, QKeySequence
-from PySide6.QtWidgets import QWidget
-
-from .. import ExcitedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class Shortcut(QShortcut, ExcitedSignalInterface):
-    def __init__(self, key, parent):
-        if isinstance(key, str):
-            key = QKeySequence(key)
-        if not isinstance(parent, QWidget):
-            parent = parent.w
-        super().__init__(key, parent)
-
-    def set_excited_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.activated.connect(self.excited.emit)
+from PySide6.QtGui import QShortcut, QKeySequence
+from PySide6.QtWidgets import QWidget
+
+from .. import ExcitedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class Shortcut(QShortcut, ExcitedSignalInterface):
+    def __init__(self, key, parent):
+        if isinstance(key, str):
+            key = QKeySequence(key)
+        if not isinstance(parent, QWidget):
+            parent = parent.w
+        super().__init__(key, parent)
+
+    def set_excited_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.activated.connect(self.excited.emit)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/spin_box.py` & `quite6-1.0.6/quite6/gui/widgets/text_edit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import prett6
-from PySide6.QtWidgets import QSpinBox
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class SpinBox(QSpinBox, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'SpinBox'):
-            self.parent = parent
-
-        def get_value(self):
-            return str(self.parent.value())
-
-        def set_value(self, value):
-            if self.get_value() != value:
-                self.parent.setValue(int(value or 0))
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.valueChanged[int].connect(self.check_change)
+import prett6
+from PySide6.QtWidgets import QTextEdit
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class TextEdit(QTextEdit, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'TextEdit'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.toPlainText()
+
+        def set_value(self, value):
+            value = value or ''
+            if value != self.get_value():
+                self.parent.setText(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.textChanged.connect(self.string.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/tab_widget.py` & `quite6-1.0.6/quite6/gui/widgets/tab_widget.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import prett6
-from PySide6.QtCore import QEvent
-from PySide6.QtWidgets import QTabWidget
-
-from .. import ExcitedSignalInterface, ContainerAbilityInterface
-from .. import ui_extension
-
-
-@ui_extension
-class TabWidget(QTabWidget, ContainerAbilityInterface, ExcitedSignalInterface,
-                prett6.WidgetIndexInterface):
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-        self.check_before_switch = None
-        self.tabBar().installEventFilter(self)
-
-    def eventFilter(self, obj, event):
-        if obj == self.tabBar() and event.type() == QEvent.Type.MouseButtonPress:
-            mouse_event = event
-            pos = mouse_event.position().toPoint()
-            index = self.tabBar().tabAt(pos)
-            if self.check_before_switch is not None and not self.check_before_switch(index):
-                return True
-        return super().eventFilter(obj, event)
-
-    def install_check_before_switch(self, func):
-        self.check_before_switch = func
-
-    class TabWidgetItem:
-        def __init__(self, parent: 'TabWidget'):
-            self.parent = parent
-
-        @property
-        def count(self):
-            return self.parent.count()
-
-        def tab_text(self, idx):
-            return self.parent.tabText(idx)
-
-    class IndexItem(TabWidgetItem, prett6.IndexItem):
-        def get_value(self):
-            return self.parent.currentIndex()
-
-        def set_value(self, value):
-            value = value or 0
-            self.parent.setCurrentIndex(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentChanged.connect(self.check_change)
+import prett6
+from PySide6.QtCore import QEvent
+from PySide6.QtWidgets import QTabWidget
+
+from .. import ExcitedSignalInterface, ContainerAbilityInterface
+from .. import ui_extension
+
+
+@ui_extension
+class TabWidget(QTabWidget, ContainerAbilityInterface, ExcitedSignalInterface,
+                prett6.WidgetIndexInterface):
+
+    def __init__(self, parent=None):
+        super().__init__(parent)
+        self.check_before_switch = None
+        self.tabBar().installEventFilter(self)
+
+    def eventFilter(self, obj, event):
+        if obj == self.tabBar() and event.type() == QEvent.Type.MouseButtonPress:
+            mouse_event = event
+            pos = mouse_event.position().toPoint()
+            index = self.tabBar().tabAt(pos)
+            if self.check_before_switch is not None and not self.check_before_switch(index):
+                return True
+        return super().eventFilter(obj, event)
+
+    def install_check_before_switch(self, func):
+        self.check_before_switch = func
+
+    class TabWidgetItem:
+        def __init__(self, parent: 'TabWidget'):
+            self.parent = parent
+
+        @property
+        def count(self):
+            return self.parent.count()
+
+        def tab_text(self, idx):
+            return self.parent.tabText(idx)
+
+    class IndexItem(TabWidgetItem, prett6.IndexItem):
+        def get_value(self):
+            return self.parent.currentIndex()
+
+        def set_value(self, value):
+            value = value or 0
+            self.parent.setCurrentIndex(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentChanged.connect(self.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/table_view.py` & `quite6-1.0.6/quite6/gui/widgets/table_view.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-import functools
-import typing
-
-import prett6
-from PySide6.QtCore import QAbstractTableModel
-from PySide6.QtGui import Qt, QAction, QCursor
-from PySide6.QtWidgets import QTableView, QMenu, QAbstractItemView
-
-from .. import ExcitedSignalInterface, RowChangedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class TableView(QTableView, ExcitedSignalInterface, prett6.WidgetDictInterface, prett6.WidgetIndexInterface,
-                prett6.WidgetDictListInterface, RowChangedSignalInterface):
-    menuItems = []
-
-    def addMenuItem(self, name, func):
-        self.menuItems.append((name, func))
-
-    def contextMenuEvent(self, event):
-        if len(self.menuItems) != 0:
-            menu = QMenu(self)
-            for item in self.menuItems:
-                name = item[0]
-                func = item[1]
-                action = QAction(name, self)
-                pos = event.pos()
-                # use lambda will lead to always exec finally func bug, use is ok
-                action.triggered.connect(functools.partial(func, pos))
-                menu.addAction(action)
-            menu.exec_(QCursor.pos())
-
-    def set_row_changed_signal_connection(self):
-        self.clicked.connect(self.row_changed_signal)
-
-    def row_changed_signal(self):
-        if len(self.selectedIndexes()) != 0:
-            self.row_changed.emit_if_changed(self.selectedIndexes()[0].row())
-
-    @property
-    def model(self):
-        if getattr(self, "_model", None) is None:
-            self._model = self.Model(self)
-            self.setModel(self._model)
-        return self._model
-
-    class Model(QAbstractTableModel):
-        def __init__(self, parent, *args):
-            QAbstractTableModel.__init__(self, parent, *args)
-            self.mylist = []
-            self.headers = []
-
-        def rowCount(self, parent=None):
-            return len(self.mylist)
-
-        def columnCount(self, parent=None):
-            return len(self.headers)
-
-        def data(self, index, role):
-            if not index.isValid():
-                return None
-            elif role != Qt.DisplayRole:
-                return None
-            return self.mylist[index.row()][self.headers[index.column()]]
-
-        def headerData(self, col, orientation, role):
-            if orientation == Qt.Horizontal and role == Qt.DisplayRole:
-                return self.headers[col]
-            return None
-
-        def set_data(self, data):
-            self.mylist = data
-            # sel.setData(data)
-
-        def set_headers(self, headers):
-            self.headers = headers
-
-        def get_by_indexes(self, indexes):
-            res = []
-            for index in indexes:
-                res.append(self.mylist[index])
-            return res
-
-        def get_data(self, row, col):
-            return self.mylist[row][self.headers[col]]
-
-    def set_headers(self, headers):
-        self.model.set_headers(headers)
-
-    def set_data(self, data):
-        self.model.set_data(data)
-        self.model.reset()
-        # fix column from hide to show, but not show in view
-        # because origin column size is 0
-        self.auto_resize_column_width()
-
-    def get_data(self, row, col):
-        data = self.model.get_data(row, col)
-        return data
-
-    def set_column_hidden(self, header):
-        self.set_column_visible(header, False)
-
-    def set_column_show(self, header):
-        self.set_column_visible(header, True)
-
-    def set_column_visible(self, header, is_visible: True):
-        if header not in self.model.headers:
-            raise ValueError("header_name doesn't match headers label")
-        if is_visible:
-            self.showColumn(self.model.headers.index(header))
-        else:
-            self.hideColumn(self.model.headers.index(header))
-
-    def set_just_show_mode(self):
-        self.auto_resize = True
-        self.verticalHeader().hide()
-        self.resizeColumnsToContents()
-        self.setEditTriggers(QAbstractItemView.NoEditTriggers)
-        self.setSelectionBehavior(QAbstractItemView.SelectRows)
-
-    def set_select_rows_mode(self):
-        self.setSelectionBehavior(QAbstractItemView.SelectRows)
-        self.setStyleSheet("selection-background-color: lightBlue;selection-color: black;")
-        self.setSelectionMode(QAbstractItemView.ExtendedSelection)
-
-    def get_selected_list(self) -> typing.List[dict]:
-        selected_ids = list(map(lambda x: x.row(), self.selectedIndexes()))
-        selected_ids = list(set(selected_ids))
-        selected_list = self.model.get_by_indexes(selected_ids)
-        return selected_list
-
-    def get_selected_list_without_hidden_col(self) -> typing.List[dict]:
-        selected_list = self.get_selected_list()
-        header_labels = self.model.headers
-        hidden_columns = []
-        for column_name in header_labels:
-            if self.isColumnHidden(header_labels.index(column_name)):
-                hidden_columns.append(column_name)
-        for row in selected_list:
-            for hidden_col in hidden_columns:
-                if hidden_col in row.keys():
-                    del row[hidden_col]
-        return selected_list
-
-    @property
-    def auto_resize(self):
-        return getattr(self, 'resize', False)
-
-    @auto_resize.setter
-    def auto_resize(self, value: bool):
-        setattr(self, 'resize', value)
-
-    def auto_resize_column_width(self):
-        if self.auto_resize:
-            self.resizeColumnsToContents()
-            col_count = self.col_count
-            col_width = sum(list([self.columnWidth(i) for i in range(col_count)]))
-            if col_width < self.width():
-                for i in range(col_count):
-                    self.setColumnWidth(i, self.columnWidth(i) / col_width * self.width())
-
-    def resizeEvent(self, event):
-        super(QTableView, self).resizeEvent(event)
-        self.auto_resize_column_width()
-
-    @property
-    def col_count(self):
-        return self.model.columnCount()
-
-    @property
-    def row_count(self):
-        return self.model.rowCount()
-
-    def select_rows(self, rows):
-        self.setSelectionMode(QAbstractItemView.MultiSelection)
-        selected_row = list(map(lambda x: x.row(), self.selectedIndexes()))
-        for row in rows:
-            if row not in selected_row:
-                self.selectRow(row)
-
-    def unselect_rows(self, rows):
-        self.setSelectionMode(QAbstractItemView.MultiSelection)
-        selected_row = list(map(lambda x: x.row(), self.selectedIndexes()))
-        for row in rows:
-            if row in selected_row:
-                self.selectRow(row)
+import functools
+import typing
+
+import prett6
+from PySide6.QtCore import QAbstractTableModel
+from PySide6.QtGui import Qt, QAction, QCursor
+from PySide6.QtWidgets import QTableView, QMenu, QAbstractItemView
+
+from .. import ExcitedSignalInterface, RowChangedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class TableView(QTableView, ExcitedSignalInterface, prett6.WidgetDictInterface, prett6.WidgetIndexInterface,
+                prett6.WidgetDictListInterface, RowChangedSignalInterface):
+    menuItems = []
+
+    def addMenuItem(self, name, func):
+        self.menuItems.append((name, func))
+
+    def contextMenuEvent(self, event):
+        if len(self.menuItems) != 0:
+            menu = QMenu(self)
+            for item in self.menuItems:
+                name = item[0]
+                func = item[1]
+                action = QAction(name, self)
+                pos = event.pos()
+                # use lambda will lead to always exec finally func bug, use is ok
+                action.triggered.connect(functools.partial(func, pos))
+                menu.addAction(action)
+            menu.exec_(QCursor.pos())
+
+    def set_row_changed_signal_connection(self):
+        self.clicked.connect(self.row_changed_signal)
+
+    def row_changed_signal(self):
+        if len(self.selectedIndexes()) != 0:
+            self.row_changed.emit_if_changed(self.selectedIndexes()[0].row())
+
+    @property
+    def model(self):
+        if getattr(self, "_model", None) is None:
+            self._model = self.Model(self)
+            self.setModel(self._model)
+        return self._model
+
+    class Model(QAbstractTableModel):
+        def __init__(self, parent, *args):
+            QAbstractTableModel.__init__(self, parent, *args)
+            self.mylist = []
+            self.headers = []
+
+        def rowCount(self, parent=None):
+            return len(self.mylist)
+
+        def columnCount(self, parent=None):
+            return len(self.headers)
+
+        def data(self, index, role):
+            if not index.isValid():
+                return None
+            elif role != Qt.DisplayRole:
+                return None
+            return self.mylist[index.row()][self.headers[index.column()]]
+
+        def headerData(self, col, orientation, role):
+            if orientation == Qt.Horizontal and role == Qt.DisplayRole:
+                return self.headers[col]
+            return None
+
+        def set_data(self, data):
+            self.mylist = data
+            # sel.setData(data)
+
+        def set_headers(self, headers):
+            self.headers = headers
+
+        def get_by_indexes(self, indexes):
+            res = []
+            for index in indexes:
+                res.append(self.mylist[index])
+            return res
+
+        def get_data(self, row, col):
+            return self.mylist[row][self.headers[col]]
+
+    def set_headers(self, headers):
+        self.model.set_headers(headers)
+
+    def set_data(self, data):
+        self.model.set_data(data)
+        self.model.reset()
+        # fix column from hide to show, but not show in view
+        # because origin column size is 0
+        self.auto_resize_column_width()
+
+    def get_data(self, row, col):
+        data = self.model.get_data(row, col)
+        return data
+
+    def set_column_hidden(self, header):
+        self.set_column_visible(header, False)
+
+    def set_column_show(self, header):
+        self.set_column_visible(header, True)
+
+    def set_column_visible(self, header, is_visible: True):
+        if header not in self.model.headers:
+            raise ValueError("header_name doesn't match headers label")
+        if is_visible:
+            self.showColumn(self.model.headers.index(header))
+        else:
+            self.hideColumn(self.model.headers.index(header))
+
+    def set_just_show_mode(self):
+        self.auto_resize = True
+        self.verticalHeader().hide()
+        self.resizeColumnsToContents()
+        self.setEditTriggers(QAbstractItemView.NoEditTriggers)
+        self.setSelectionBehavior(QAbstractItemView.SelectRows)
+
+    def set_select_rows_mode(self):
+        self.setSelectionBehavior(QAbstractItemView.SelectRows)
+        self.setStyleSheet("selection-background-color: lightBlue;selection-color: black;")
+        self.setSelectionMode(QAbstractItemView.ExtendedSelection)
+
+    def get_selected_list(self) -> typing.List[dict]:
+        selected_ids = list(map(lambda x: x.row(), self.selectedIndexes()))
+        selected_ids = list(set(selected_ids))
+        selected_list = self.model.get_by_indexes(selected_ids)
+        return selected_list
+
+    def get_selected_list_without_hidden_col(self) -> typing.List[dict]:
+        selected_list = self.get_selected_list()
+        header_labels = self.model.headers
+        hidden_columns = []
+        for column_name in header_labels:
+            if self.isColumnHidden(header_labels.index(column_name)):
+                hidden_columns.append(column_name)
+        for row in selected_list:
+            for hidden_col in hidden_columns:
+                if hidden_col in row.keys():
+                    del row[hidden_col]
+        return selected_list
+
+    @property
+    def auto_resize(self):
+        return getattr(self, 'resize', False)
+
+    @auto_resize.setter
+    def auto_resize(self, value: bool):
+        setattr(self, 'resize', value)
+
+    def auto_resize_column_width(self):
+        if self.auto_resize:
+            self.resizeColumnsToContents()
+            col_count = self.col_count
+            col_width = sum(list([self.columnWidth(i) for i in range(col_count)]))
+            if col_width < self.width():
+                for i in range(col_count):
+                    self.setColumnWidth(i, self.columnWidth(i) / col_width * self.width())
+
+    def resizeEvent(self, event):
+        super(QTableView, self).resizeEvent(event)
+        self.auto_resize_column_width()
+
+    @property
+    def col_count(self):
+        return self.model.columnCount()
+
+    @property
+    def row_count(self):
+        return self.model.rowCount()
+
+    def select_rows(self, rows):
+        self.setSelectionMode(QAbstractItemView.MultiSelection)
+        selected_row = list(map(lambda x: x.row(), self.selectedIndexes()))
+        for row in rows:
+            if row not in selected_row:
+                self.selectRow(row)
+
+    def unselect_rows(self, rows):
+        self.setSelectionMode(QAbstractItemView.MultiSelection)
+        selected_row = list(map(lambda x: x.row(), self.selectedIndexes()))
+        for row in rows:
+            if row in selected_row:
+                self.selectRow(row)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/table_widget.py` & `quite6-1.0.6/quite6/gui/widgets/table_widget.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import typing
-
-import prett6
-import st
-from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QTableWidget, QAbstractItemView, QTableWidgetItem
-
-from .. import ExcitedSignalInterface, RowChangedSignalInterface
-from .. import ui_extension
-
-
-@ui_extension
-class TableWidget(QTableWidget, ExcitedSignalInterface, prett6.WidgetDictInterface, prett6.WidgetIndexInterface,
-                  prett6.WidgetDictListInterface, RowChangedSignalInterface):
-    keyPressFunc = None
-
-    def keyPressEvent(self, event):
-        if self.keyPressFunc is not None:
-            self.keyPressFunc(event)
-        event.ignore()
-
-    def set_row_changed_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.itemClicked.connect(self.row_changed_signal)
-
-    def row_changed_signal(self):
-        # noinspection PyUnresolvedReferences
-        self.row_changed.emit_if_changed(self.currentRow())
-
-    def set_excited_signal_connection(self):
-        # noinspection PyUnresolvedReferences
-        self.doubleClicked.connect(st.zero_para(self.excited.emit))
-
-    def set_just_show_mode(self):
-        self.auto_resize = True
-        self.verticalHeader().hide()
-        self.resizeColumnsToContents()
-        self.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
-        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
-
-    def set_select_rows_mode(self):
-        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
-        self.setStyleSheet("selection-background-color: lightBlue;selection-color: black;")
-        self.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
-        self.selectAll()
-        # noinspection PyUnresolvedReferences
-        self.itemClicked.connect(self.cancel_current_select)
-
-    def set_column_hidden(self, header_name):
-        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
-        if header_name not in header_labels:
-            raise ValueError("header_name doesn't match headers label")
-        self.hideColumn(header_labels.index(header_name))
-
-    def set_column_show(self, header_name):
-        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
-        if header_name not in header_labels:
-            raise ValueError("header_name doesn't match headers label")
-        self.showColumn(header_labels.index(header_name))
-
-    def cancel_current_select(self):
-        self.select_row_index = getattr(self, "select_row_index", 0)
-        self.select_rows_num = getattr(self, "select_rows_num", 1)
-        if self.currentRow() == self.select_row_index and \
-                len(self.selectedItems()) == self.select_rows_num * self.columnCount():
-            self.clearSelection()
-        self.select_rows_num = len(self.selectedIndexes()) / self.columnCount()
-        self.select_row_index = self.currentRow()
-
-    def get_selected_list(self) -> typing.List[dict]:
-        selected_ids = list(map(lambda x: x.row(), self.selectedIndexes()))
-        selected_ids = list(set(selected_ids))
-        selected_list = list(filter(lambda x: self.dict_list.value.index(x) in selected_ids, self.dict_list.value))
-        return selected_list
-
-    def get_selected_list_without_hidden_col(self) -> typing.List[dict]:
-        selected_list = self.get_selected_list()
-        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
-        # if header_name not in header_labels:
-        #     raise ValueError("header_name doesn't match headers label")
-        # self.hideColumn(header_labels.index(header_name))
-        hidden_columns = []
-        for column_name in header_labels:
-            if self.isColumnHidden(header_labels.index(column_name)):
-                hidden_columns.append(column_name)
-        for row in selected_list:
-            for hidden_col in hidden_columns:
-                del row[hidden_col]
-        return selected_list
-
-    def set_headers(self, headers: list):
-        self.setColumnCount(len(headers))
-        self.setHorizontalHeaderLabels(headers)
-
-    @property
-    def auto_resize(self):
-        return getattr(self, 'resize', False)
-
-    @auto_resize.setter
-    def auto_resize(self, value: bool):
-        setattr(self, 'resize', value)
-
-    def get_item_style(self, x, y):
-        style_dict = getattr(self, 'item_style', {})
-        for xy in [(x, y), (None, y), (x, None), (None, None)]:
-            if xy in style_dict.keys():
-                return style_dict[xy]
-        return None
-
-    # add item style handle func
-    def set_item_style(self, x, y, item_func):
-        """
-        :param x: row num, if it's None, will match all row.
-        :param y: col num, if it's None, will match all col.
-        :param item_func: func(item: QTableWidgetItem)
-        """
-        style_dict = getattr(self, 'item_style', {})
-        style_dict[(x, y)] = item_func
-        setattr(self, 'item_style', style_dict)
-
-    def auto_resize_column_width(self):
-        if self.auto_resize:
-            self.resizeColumnsToContents()
-            col_count = self.columnCount()
-            col_width = sum(list([self.columnWidth(i) for i in range(col_count)]))
-            if col_width < self.width():
-                for i in range(col_count):
-                    self.setColumnWidth(i, int(self.columnWidth(i) / col_width * self.width()))
-
-    def resizeEvent(self, event):
-        super(TableWidget, self).resizeEvent(event)
-        self.auto_resize_column_width()
-
-    class TableWidgetItem:
-        def __init__(self, parent: 'TableWidget'):
-            self.parent = parent
-
-        @property
-        def row_count(self):
-            return self.parent.rowCount()
-
-        @property
-        def col_count(self):
-            return self.parent.columnCount()
-
-        def item_text(self, row, col):
-            return self.parent.item(row, col).text()
-
-    class DictItem(TableWidgetItem, prett6.WidgetDictItem):
-        """get/set current table row text"""
-
-        def get_value(self):
-            if self.parent.index.value >= 0:
-                current_row = self.parent.currentRow()
-                col_count = self.parent.columnCount()
-                value = dict()
-                for i in range(col_count):
-                    value[self.parent.horizontalHeaderItem(i).text()] = self.item_text(current_row, i)
-                return value
-            return None
-
-        def set_value(self, value):
-            assert isinstance(value, dict)
-            if len(value) is not self.col_count:
-                raise ValueError('Value length must equal to column count')
-
-            texts = self.parent.dict_list.value
-            assert isinstance(texts, list)
-            if value is None:
-                self.parent.index.value = 0
-            else:
-                for key, v in value.items():
-                    value[key] = str(v)
-                if value in texts:
-                    self.parent.index.value = texts.index(value)
-                else:
-                    header_labels = list(self.parent.horizontalHeaderItem(i).text() for i in range(self.col_count))
-                    self.parent.setRowCount(self.row_count + 1)
-                    for i in range(self.col_count):
-                        item_text = value[header_labels[i]]
-                        if item_text is None:
-                            raise ValueError("key value doesn't match headers label")
-                        table_item = QTableWidgetItem(item_text)
-                        table_item.setTextAlignment(Qt.AlignmentFlag.AlignCenter)
-                        item_handle = self.parent.get_item_style(self.row_count - 1, i)
-                        if item_handle is not None:
-                            item_handle(table_item)
-                        self.parent.setItem(self.row_count - 1, i, table_item)
-                    self.parent.index.value = self.row_count - 1
-                    self.parent.auto_resize_column_width()
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentCellChanged.connect(self.check_change)
-
-    class IndexItem(TableWidgetItem, prett6.IndexItem):
-        """get/set current select row"""
-
-        def get_value(self):
-            return self.parent.currentRow()
-
-        def set_value(self, value):
-            value = value or 0
-            self.parent.selectRow(value)
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.currentCellChanged(self.check_change)
-
-    class DictListItem(TableWidgetItem, prett6.DictListItem):
-        """ get all table_widget item text"""
-
-        def get_value(self):
-            table_texts = []
-            for row in range(self.row_count):
-                row_dict = dict()
-                for col in range(self.col_count):
-                    row_dict[self.parent.horizontalHeaderItem(col).text()] = self.item_text(row, col)
-                table_texts.append(row_dict)
-            return table_texts
-
-        def set_value(self, value: list):
-            value = value or []
-            assert isinstance(value, list)
-
-            for i in range(self.row_count):
-                self.parent.removeRow(0)
-            for row_dict in value:
-                self.parent.dict.value = row_dict
-            self.check_change()
+import typing
+
+import prett6
+import st
+from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QTableWidget, QAbstractItemView, QTableWidgetItem
+
+from .. import ExcitedSignalInterface, RowChangedSignalInterface
+from .. import ui_extension
+
+
+@ui_extension
+class TableWidget(QTableWidget, ExcitedSignalInterface, prett6.WidgetDictInterface, prett6.WidgetIndexInterface,
+                  prett6.WidgetDictListInterface, RowChangedSignalInterface):
+    keyPressFunc = None
+
+    def keyPressEvent(self, event):
+        if self.keyPressFunc is not None:
+            self.keyPressFunc(event)
+        event.ignore()
+
+    def set_row_changed_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.itemClicked.connect(self.row_changed_signal)
+
+    def row_changed_signal(self):
+        # noinspection PyUnresolvedReferences
+        self.row_changed.emit_if_changed(self.currentRow())
+
+    def set_excited_signal_connection(self):
+        # noinspection PyUnresolvedReferences
+        self.doubleClicked.connect(st.zero_para(self.excited.emit))
+
+    def set_just_show_mode(self):
+        self.auto_resize = True
+        self.verticalHeader().hide()
+        self.resizeColumnsToContents()
+        self.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
+        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
+
+    def set_select_rows_mode(self):
+        self.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
+        self.setStyleSheet("selection-background-color: lightBlue;selection-color: black;")
+        self.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
+        self.selectAll()
+        # noinspection PyUnresolvedReferences
+        self.itemClicked.connect(self.cancel_current_select)
+
+    def set_column_hidden(self, header_name):
+        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
+        if header_name not in header_labels:
+            raise ValueError("header_name doesn't match headers label")
+        self.hideColumn(header_labels.index(header_name))
+
+    def set_column_show(self, header_name):
+        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
+        if header_name not in header_labels:
+            raise ValueError("header_name doesn't match headers label")
+        self.showColumn(header_labels.index(header_name))
+
+    def cancel_current_select(self):
+        self.select_row_index = getattr(self, "select_row_index", 0)
+        self.select_rows_num = getattr(self, "select_rows_num", 1)
+        if self.currentRow() == self.select_row_index and \
+                len(self.selectedItems()) == self.select_rows_num * self.columnCount():
+            self.clearSelection()
+        self.select_rows_num = len(self.selectedIndexes()) / self.columnCount()
+        self.select_row_index = self.currentRow()
+
+    def get_selected_list(self) -> typing.List[dict]:
+        selected_ids = list(map(lambda x: x.row(), self.selectedIndexes()))
+        selected_ids = list(set(selected_ids))
+        selected_list = list(filter(lambda x: self.dict_list.value.index(x) in selected_ids, self.dict_list.value))
+        return selected_list
+
+    def get_selected_list_without_hidden_col(self) -> typing.List[dict]:
+        selected_list = self.get_selected_list()
+        header_labels = list(self.horizontalHeaderItem(i).text() for i in range(self.columnCount()))
+        # if header_name not in header_labels:
+        #     raise ValueError("header_name doesn't match headers label")
+        # self.hideColumn(header_labels.index(header_name))
+        hidden_columns = []
+        for column_name in header_labels:
+            if self.isColumnHidden(header_labels.index(column_name)):
+                hidden_columns.append(column_name)
+        for row in selected_list:
+            for hidden_col in hidden_columns:
+                del row[hidden_col]
+        return selected_list
+
+    def set_headers(self, headers: list):
+        self.setColumnCount(len(headers))
+        self.setHorizontalHeaderLabels(headers)
+
+    @property
+    def auto_resize(self):
+        return getattr(self, 'resize', False)
+
+    @auto_resize.setter
+    def auto_resize(self, value: bool):
+        setattr(self, 'resize', value)
+
+    def get_item_style(self, x, y):
+        style_dict = getattr(self, 'item_style', {})
+        for xy in [(x, y), (None, y), (x, None), (None, None)]:
+            if xy in style_dict.keys():
+                return style_dict[xy]
+        return None
+
+    # add item style handle func
+    def set_item_style(self, x, y, item_func):
+        """
+        :param x: row num, if it's None, will match all row.
+        :param y: col num, if it's None, will match all col.
+        :param item_func: func(item: QTableWidgetItem)
+        """
+        style_dict = getattr(self, 'item_style', {})
+        style_dict[(x, y)] = item_func
+        setattr(self, 'item_style', style_dict)
+
+    def auto_resize_column_width(self):
+        if self.auto_resize:
+            self.resizeColumnsToContents()
+            col_count = self.columnCount()
+            col_width = sum(list([self.columnWidth(i) for i in range(col_count)]))
+            if col_width < self.width():
+                for i in range(col_count):
+                    self.setColumnWidth(i, int(self.columnWidth(i) / col_width * self.width()))
+
+    def resizeEvent(self, event):
+        super(TableWidget, self).resizeEvent(event)
+        self.auto_resize_column_width()
+
+    class TableWidgetItem:
+        def __init__(self, parent: 'TableWidget'):
+            self.parent = parent
+
+        @property
+        def row_count(self):
+            return self.parent.rowCount()
+
+        @property
+        def col_count(self):
+            return self.parent.columnCount()
+
+        def item_text(self, row, col):
+            return self.parent.item(row, col).text()
+
+    class DictItem(TableWidgetItem, prett6.WidgetDictItem):
+        """get/set current table row text"""
+
+        def get_value(self):
+            if self.parent.index.value >= 0:
+                current_row = self.parent.currentRow()
+                col_count = self.parent.columnCount()
+                value = dict()
+                for i in range(col_count):
+                    value[self.parent.horizontalHeaderItem(i).text()] = self.item_text(current_row, i)
+                return value
+            return None
+
+        def set_value(self, value):
+            assert isinstance(value, dict)
+            if len(value) is not self.col_count:
+                raise ValueError('Value length must equal to column count')
+
+            texts = self.parent.dict_list.value
+            assert isinstance(texts, list)
+            if value is None:
+                self.parent.index.value = 0
+            else:
+                for key, v in value.items():
+                    value[key] = str(v)
+                if value in texts:
+                    self.parent.index.value = texts.index(value)
+                else:
+                    header_labels = list(self.parent.horizontalHeaderItem(i).text() for i in range(self.col_count))
+                    self.parent.setRowCount(self.row_count + 1)
+                    for i in range(self.col_count):
+                        item_text = value[header_labels[i]]
+                        if item_text is None:
+                            raise ValueError("key value doesn't match headers label")
+                        table_item = QTableWidgetItem(item_text)
+                        table_item.setTextAlignment(Qt.AlignmentFlag.AlignCenter)
+                        item_handle = self.parent.get_item_style(self.row_count - 1, i)
+                        if item_handle is not None:
+                            item_handle(table_item)
+                        self.parent.setItem(self.row_count - 1, i, table_item)
+                    self.parent.index.value = self.row_count - 1
+                    self.parent.auto_resize_column_width()
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentCellChanged.connect(self.check_change)
+
+    class IndexItem(TableWidgetItem, prett6.IndexItem):
+        """get/set current select row"""
+
+        def get_value(self):
+            return self.parent.currentRow()
+
+        def set_value(self, value):
+            value = value or 0
+            self.parent.selectRow(value)
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.currentCellChanged(self.check_change)
+
+    class DictListItem(TableWidgetItem, prett6.DictListItem):
+        """ get all table_widget item text"""
+
+        def get_value(self):
+            table_texts = []
+            for row in range(self.row_count):
+                row_dict = dict()
+                for col in range(self.col_count):
+                    row_dict[self.parent.horizontalHeaderItem(col).text()] = self.item_text(row, col)
+                table_texts.append(row_dict)
+            return table_texts
+
+        def set_value(self, value: list):
+            value = value or []
+            assert isinstance(value, list)
+
+            for i in range(self.row_count):
+                self.parent.removeRow(0)
+            for row_dict in value:
+                self.parent.dict.value = row_dict
+            self.check_change()
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/time_edit.py` & `quite6-1.0.6/quite6/gui/widgets/time_edit.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import prett6
-from PySide6.QtCore import QDate
-from PySide6.QtWidgets import QTimeEdit
-
-from .. import BaseInterface
-from .. import ui_extension
-
-
-@ui_extension
-class TimeEdit(QTimeEdit, BaseInterface, prett6.WidgetStringInterface):
-    class StringItem(prett6.WidgetStringItem):
-        def __init__(self, parent: 'TimeEdit'):
-            self.parent = parent
-
-        def get_value(self):
-            return self.parent.text()
-
-        def set_value(self, value):
-            value = value or ''
-            if value != self.get_value():
-                date = value.split('-')
-                if len(date) == 3:
-                    raise ValueError('Date format is invalid')
-                self.parent.setDate(QDate(int(date[0]), int(date[1]), int(date[2])))
-
-        def set_changed_connection(self):
-            # noinspection PyUnresolvedReferences
-            self.parent.dateChanged.connect(self.string.check_change)
+import prett6
+from PySide6.QtCore import QDate
+from PySide6.QtWidgets import QTimeEdit
+
+from .. import BaseInterface
+from .. import ui_extension
+
+
+@ui_extension
+class TimeEdit(QTimeEdit, BaseInterface, prett6.WidgetStringInterface):
+    class StringItem(prett6.WidgetStringItem):
+        def __init__(self, parent: 'TimeEdit'):
+            self.parent = parent
+
+        def get_value(self):
+            return self.parent.text()
+
+        def set_value(self, value):
+            value = value or ''
+            if value != self.get_value():
+                date = value.split('-')
+                if len(date) == 3:
+                    raise ValueError('Date format is invalid')
+                self.parent.setDate(QDate(int(date[0]), int(date[1]), int(date[2])))
+
+        def set_changed_connection(self):
+            # noinspection PyUnresolvedReferences
+            self.parent.dateChanged.connect(self.string.check_change)
```

### Comparing `quite6-1.0.5/quite6/gui/widgets/widget.py` & `quite6-1.0.6/quite6/gui/widgets/widget.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from PySide6.QtWidgets import QWidget
-from PySide6.QtGui import QCloseEvent
-
-from .. import Painter
-from .. import ui_extension
-from .. import EventLoop
-from .. import ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface
-
-
-@ui_extension
-class Widget(QWidget, ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface):
-    def __init__(self, parent=None, *args):
-        # noinspection PyUnresolvedReferences
-        super().__init__(parent.w if getattr(parent, 'w', None) is not None else parent, *args)
-
-    def closeEvent(self, event: QCloseEvent):
-        self.closed.emit()
-        event.accept()
-
-    def exec(self):
-        with EventLoop() as event:
-            self.show()
-            self.closed.connect(event.quit)
-
-    @property
-    def background_color(self):
-        return self._create(lambda: None)
-
-    @background_color.setter
-    def background_color(self, value):
-        self.assign(value)
-        self.update()
-
-    @property
-    def size(self) -> tuple[int, int]:
-        return self.width(), self.height()
-
-    def paintEvent(self, *args, **kwargs):
-        painter = Painter(self)
-
-        if self.background_color is not None:
-            painter.fillRect(self.rect(), self.background_color)
-        self.paint(painter)
-
-    def paint(self, painter: Painter):
-        pass
+from PySide6.QtWidgets import QWidget
+from PySide6.QtGui import QCloseEvent
+
+from .. import Painter
+from .. import ui_extension
+from .. import EventLoop
+from .. import ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface
+
+
+@ui_extension
+class Widget(QWidget, ClosedSignalInterface, ClassExecInterface, ContainerAbilityInterface):
+    def __init__(self, parent=None, *args):
+        # noinspection PyUnresolvedReferences
+        super().__init__(parent.w if getattr(parent, 'w', None) is not None else parent, *args)
+
+    def closeEvent(self, event: QCloseEvent):
+        self.closed.emit()
+        event.accept()
+
+    def exec(self):
+        with EventLoop() as event:
+            self.show()
+            self.closed.connect(event.quit)
+
+    @property
+    def background_color(self):
+        return self._create(lambda: None)
+
+    @background_color.setter
+    def background_color(self, value):
+        self.assign(value)
+        self.update()
+
+    @property
+    def size(self) -> tuple[int, int]:
+        return self.width(), self.height()
+
+    def paintEvent(self, *args, **kwargs):
+        painter = Painter(self)
+
+        if self.background_color is not None:
+            painter.fillRect(self.rect(), self.background_color)
+        self.paint(painter)
+
+    def paint(self, painter: Painter):
+        pass
```

### Comparing `quite6-1.0.5/quite6/tools/load_qrc.py` & `quite6-1.0.6/quite6/tools/load_qrc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-import os
-import st
-import sys
-import subprocess
-import PySide6
-
-if sys.platform == 'darwin':
-    pyside6_path = os.path.dirname(sys.executable)
-    rcc_path = os.path.join(pyside6_path, 'pyside6-rcc')
-    if not os.path.exists(rcc_path):
-        print(f'PySide6 Resource Compiler (pyside6-rcc) Not Found in platform {rcc_path}!')
-elif sys.platform == 'win32':
-    pyside6_path = os.path.dirname(PySide6.__file__)
-    rcc_path = os.path.join(pyside6_path, 'pySide6-rcc.exe')
-    if not os.path.exists(rcc_path):
-        rcc_path = 'PySide6-rcc.exe'
-    if not os.path.exists(rcc_path):
-        print('PySide6 Resource Compiler (PySide6-rcc.exe) Not Found!')
-else:
-    print(f"Unsupported platform {sys.platform} for pyside6-rcc")
-
-
-@st.make_cache
-def compile_qrc(filename):
-    command = rcc_path + ' -g python ' + filename
-    p = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-    (output, error) = p.communicate()
-    p.wait()
-    if p.returncode != 0:
-        raise IOError(f'There was an error compiling the .qrc file {filename}: {error}')
-    output = output.decode()
-    return output
-
-
-def load_qrc(filename):
-    code = compile_qrc(filename)
-    st.run(code)
+import os
+import subprocess
+import sys
+from pathlib import Path
+
+import PySide6
+import st
+
+
+def find_executable_rcc(filename: str):
+    paths = os.environ['PATH'].split(os.pathsep)
+    paths.append(os.path.dirname(PySide6.__file__))
+    paths.append(str(Path(PySide6.__file__).parents[2]))
+    paths.append(os.path.join(os.path.dirname(PySide6.__file__)))
+    for path in paths:
+        pyside6_rcc_path = os.path.join(path, filename)
+        if os.path.exists(pyside6_rcc_path) and os.access(pyside6_rcc_path, os.X_OK):
+            return pyside6_rcc_path
+    return None
+
+
+if sys.platform == 'darwin':
+    pyside6_path = os.path.dirname(sys.executable)
+    rcc_path = os.path.join(pyside6_path, 'pyside6-rcc')
+    if not os.path.exists(rcc_path):
+        print(f'PySide6 Resource Compiler (pyside6-rcc) Not Found in platform {rcc_path}!')
+elif sys.platform == 'win32':
+    rcc_path = find_executable_rcc('pySide6-rcc.exe')
+    if rcc_path is None:
+        rcc_path = find_executable_rcc('PySide6-rcc.exe')
+        if rcc_path is None:
+            if not os.path.exists('pySide6-rcc.exe') and not os.path.exists('PySide6-rcc.exe'):
+                raise FileNotFoundError('PySide6 Resource Compiler (PySide6-rcc.exe) Not Found!')
+else:
+    print(f"Unsupported platform {sys.platform} for pyside6-rcc")
+
+
+@st.make_cache
+def compile_qrc(filename):
+    command = rcc_path + ' -g python ' + filename
+    p = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
+    (output, error) = p.communicate()
+    p.wait()
+    if p.returncode != 0:
+        raise IOError(f'There was an error compiling the .qrc file {filename}: {error}')
+    output = output.decode()
+    return output
+
+
+def load_qrc(filename):
+    code = compile_qrc(filename)
+    st.run(code)
```

### Comparing `quite6-1.0.5/quite6/tools/load_ui.py` & `quite6-1.0.6/quite6/tools/load_ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-import codecs
-import os
-from xml.etree import ElementTree
-
-import st
-from PySide6.QtCore import QByteArray, QBuffer, QIODevice
-from PySide6.QtUiTools import QUiLoader
-
-from . import load_qrc
-from .. import Widget, ext_classes, scaling
-
-
-@st.make_cache
-def get_ui_content(filename):
-    with codecs.open(filename, 'r', 'utf-8') as f:
-        text = f.read()
-    for cls in ext_classes:
-        text = text.replace(cls.__bases__[0].__name__, cls.__name__)
-    return text
-
-
-def process_scaling(ui_content: str, ratio: float) -> str:
-    tree = ElementTree.fromstring(ui_content)
-    for child in tree.iter('width'):
-        if child.text != '16777215':
-            child.text = str(int(int(child.text) * ratio))
-    for child in tree.iter('height'):
-        if child.text != '16777215':
-            child.text = str(int(int(child.text) * ratio))
-    for child in tree.iter('property'):
-        name = child.attrib.get('name', None)
-        if name == 'spacing' or name[-6:] == 'Margin' and len(child):
-            number = child[0]
-            number.text = str(int(int(number.text) * ratio))
-    ui_content = ElementTree.tostring(tree, encoding='unicode')
-    ui_content = ui_content.replace(' />\n', '/>\n')
-    return '<?xml version="1.0" encoding="UTF-8"?>\n' + ui_content + '\n'
-
-
-def load_ui(parent=None, filename=None) -> Widget:
-    assert isinstance(filename, str)
-
-    ui_content = get_ui_content(filename)
-    if scaling.ratio != 1.0:
-        ui_content = process_scaling(ui_content, scaling.ratio)
-    return UiLoader().load(ui_content, parent)
-
-
-def auto_generate_cache(dir_path: str):
-    assert isinstance(dir_path, str)
-    if not os.path.isdir(dir_path):
-        raise ValueError('Parameter Must be Dir Path')
-    for root_dir, _, files in os.walk(os.path.abspath(dir_path)):
-        for file in files:
-            if os.path.splitext(file)[1] == '.ui':
-                load_ui(None, os.path.join(root_dir, file))
-            if os.path.splitext(file)[1] == '.qrc':
-                load_qrc(os.path.join(root_dir, file))
-
-
-@st.singleton
-class UiLoader:
-    def __init__(self):
-        self.loader = QUiLoader()
-        for cls in ext_classes:
-            self.loader.registerCustomWidget(cls)
-
-    def load(self, text, parent=None):
-        byte_array = QByteArray(text.encode())
-        buffer = QBuffer(byte_array)
-        buffer.open(QIODevice.ReadWrite)
-
-        ui = self.loader.load(buffer, parent)
-        buffer.close()
-        return ui
+import codecs
+import os
+from xml.etree import ElementTree
+
+import st
+from PySide6.QtCore import QByteArray, QBuffer, QIODevice
+
+from . import load_qrc
+from .. import Widget, ext_classes, scaling
+from ..gui.qt_gui import uiLoader
+
+
+@st.make_cache
+def get_ui_content(filename):
+    with codecs.open(filename, 'r', 'utf-8') as f:
+        text = f.read()
+    for cls in ext_classes:
+        text = text.replace(cls.__bases__[0].__name__, cls.__name__)
+    return text
+
+
+def process_scaling(ui_content: str, ratio: float) -> str:
+    tree = ElementTree.fromstring(ui_content)
+    for child in tree.iter('width'):
+        if child.text != '16777215':
+            child.text = str(int(int(child.text) * ratio))
+    for child in tree.iter('height'):
+        if child.text != '16777215':
+            child.text = str(int(int(child.text) * ratio))
+    for child in tree.iter('property'):
+        name = child.attrib.get('name', None)
+        if name == 'spacing' or name[-6:] == 'Margin' and len(child):
+            number = child[0]
+            number.text = str(int(int(number.text) * ratio))
+    ui_content = ElementTree.tostring(tree, encoding='unicode')
+    ui_content = ui_content.replace(' />\n', '/>\n')
+    return '<?xml version="1.0" encoding="UTF-8"?>\n' + ui_content + '\n'
+
+
+def load_ui(parent=None, filename=None) -> Widget:
+    assert isinstance(filename, str)
+
+    ui_content = get_ui_content(filename)
+    if scaling.ratio != 1.0:
+        ui_content = process_scaling(ui_content, scaling.ratio)
+    return UiLoader().load(ui_content, parent)
+
+
+def auto_generate_cache(dir_path: str):
+    assert isinstance(dir_path, str)
+    if not os.path.isdir(dir_path):
+        raise ValueError('Parameter Must be Dir Path')
+    for root_dir, _, files in os.walk(os.path.abspath(dir_path)):
+        for file in files:
+            if os.path.splitext(file)[1] == '.ui':
+                load_ui(None, os.path.join(root_dir, file))
+            if os.path.splitext(file)[1] == '.qrc':
+                load_qrc(os.path.join(root_dir, file))
+
+
+@st.singleton
+class UiLoader:
+    def __init__(self):
+        self.loader = uiLoader
+        for cls in ext_classes:
+            self.loader.registerCustomWidget(cls)
+
+    def load(self, text, parent=None):
+        byte_array = QByteArray(text.encode())
+        buffer = QBuffer(byte_array)
+        buffer.open(QIODevice.ReadWrite)
+
+        ui = self.loader.load(buffer, parent)
+        buffer.close()
+        return ui
```

### Comparing `quite6-1.0.5/quite6.egg-info/PKG-INFO` & `quite6-1.0.6/quite6.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-Metadata-Version: 2.1
-Name: quite6
-Version: 1.0.5
-Summary: QT UI Extension
-Home-page: https://github.com/KD-Group/quite6
-Author: SF-Zhou
-Author-email: sfzhou.scut@gmail.com
-License: MIT
-Keywords: qt ui
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: st
-Requires-Dist: prett6
-Requires-Dist: PySide6
-Requires-Dist: typing
-Requires-Dist: pyqtgraph
-Requires-Dist: numpy
-
-quite6: QT UI Extension for Python3
-==================================
-
-|Build Status|
-
-Features
---------
-
-1. powerful signal-slot
-2. user friendly widget classes
-
-User Friendly Widget Classes
-----------------------------
-
-Uniform wrapper on frequently-used widget, including:
-
-**container widget**:
-
-1. `Widget <./quite6/gui/widgets/widget.py>`__
-2. `Dialog <./quite6/gui/widgets/dialog.py>`__
-3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
-4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
-5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
-
-**value widget**:
-
-1. `Label <./quite6/gui/widgets/label.py>`__
-2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
-3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
-4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
-5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
-6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
-
-**behavior widget**:
-
-1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
-2. `Action <./quite6/gui/widgets/action.py>`__
-3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
-4. `PushButton <./quite6/gui/widgets/push_button.py>`__
-
-Container Widget
-~~~~~~~~~~~~~~~~
-
-*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
-
-.. code:: python
-
-    import quite6
-
-    w = quite6.Widget()
-    w.exec()
-
-.. figure:: docs/images/1.simple.widget.png
-   :alt: Simple Widget
-
-   Simple Widget
-
-*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
-
-.. code:: python
-
-    import quite6
-
-
-    class CustomWidget(quite6.Widget):
-        def paint(self, painter: quite6.Painter):
-            painter.setFont(quite6.QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
-            painter.end()
-
-    main_window = quite6.MainWindow()
-    custom_widget = CustomWidget(parent=main_window)
-    main_window.set_central_widget(custom_widget)
-    main_window.exec()
-
-.. figure:: docs/images/2.nested.widget.png
-   :alt: Nested Widget
-
-   Nested Widget
-
-*Example 3*: `widget from ui
-file <./examples/3_widget_from_ui_file/example-3.py>`__
-
-.. code:: python
-
-    import os
-    from quite6 import *
-
-
-    class CustomWidget(Widget):
-        def paint(self, painter: Painter):
-            w, _ = self.size
-            painter.setFont(QFont("Courier New", 14.0))
-            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
-            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
-            painter.end()
-
-
-    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
-    main_window.set_central_widget(CustomWidget(parent=main_window))
-    main_window.exec()
-
-Use QtDesigner to create a ui file:
-
-.. figure:: docs/images/3.ui.design.png
-   :alt: UI Design
-
-   UI Design
-
-.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
-   :target: https://travis-ci.com/KD-Group/quite6
+Metadata-Version: 2.1
+Name: quite6
+Version: 1.0.6
+Summary: QT UI Extension
+Home-page: https://github.com/KD-Group/quite6
+Author: SF-Zhou
+Author-email: sfzhou.scut@gmail.com
+License: MIT
+Keywords: qt ui
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: st
+Requires-Dist: prett6
+Requires-Dist: PySide6
+Requires-Dist: typing
+Requires-Dist: pyqtgraph
+Requires-Dist: numpy
+
+quite6: QT UI Extension for Python3
+==================================
+
+|Build Status|
+
+Features
+--------
+
+1. powerful signal-slot
+2. user friendly widget classes
+
+User Friendly Widget Classes
+----------------------------
+
+Uniform wrapper on frequently-used widget, including:
+
+**container widget**:
+
+1. `Widget <./quite6/gui/widgets/widget.py>`__
+2. `Dialog <./quite6/gui/widgets/dialog.py>`__
+3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
+4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
+5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
+
+**value widget**:
+
+1. `Label <./quite6/gui/widgets/label.py>`__
+2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
+3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
+4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
+5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
+6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
+
+**behavior widget**:
+
+1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
+2. `Action <./quite6/gui/widgets/action.py>`__
+3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
+4. `PushButton <./quite6/gui/widgets/push_button.py>`__
+
+Container Widget
+~~~~~~~~~~~~~~~~
+
+*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
+
+.. code:: python
+
+    import quite6
+
+    w = quite6.Widget()
+    w.exec()
+
+.. figure:: docs/images/1.simple.widget.png
+   :alt: Simple Widget
+
+   Simple Widget
+
+*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
+
+.. code:: python
+
+    import quite6
+
+
+    class CustomWidget(quite6.Widget):
+        def paint(self, painter: quite6.Painter):
+            painter.setFont(quite6.QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
+            painter.end()
+
+    main_window = quite6.MainWindow()
+    custom_widget = CustomWidget(parent=main_window)
+    main_window.set_central_widget(custom_widget)
+    main_window.exec()
+
+.. figure:: docs/images/2.nested.widget.png
+   :alt: Nested Widget
+
+   Nested Widget
+
+*Example 3*: `widget from ui
+file <./examples/3_widget_from_ui_file/example-3.py>`__
+
+.. code:: python
+
+    import os
+    from quite6 import *
+
+
+    class CustomWidget(Widget):
+        def paint(self, painter: Painter):
+            w, _ = self.size
+            painter.setFont(QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
+            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
+            painter.end()
+
+
+    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
+    main_window.set_central_widget(CustomWidget(parent=main_window))
+    main_window.exec()
+
+Use QtDesigner to create a ui file:
+
+.. figure:: docs/images/3.ui.design.png
+   :alt: UI Design
+
+   UI Design
+
+.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
+   :target: https://travis-ci.com/KD-Group/quite6
```

### Comparing `quite6-1.0.5/quite6.egg-info/SOURCES.txt` & `quite6-1.0.6/quite6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quite6-1.0.5/readme.md` & `quite6-1.0.6/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,111 @@
-# quite6: QT UI Extension for Python3
-
-[![Build Status](https://travis-ci.com/KD-Group/quite6.svg?branch=master)](https://travis-ci.com/KD-Group/quite6)
-
-## Features
-
-1. powerful signal-slot
-2. user friendly widget classes
-
-## User Friendly Widget Classes
-
-Uniform wrapper on frequently-used widget, including:
-
-**container widget**:
-
-1. [Widget](./quite6/gui/widgets/widget.py)
-2. [Dialog](./quite6/gui/widgets/dialog.py)
-3. [MainWindow](./quite6/gui/widgets/main_window.py)
-4. [GroupBox](./quite6/gui/widgets/group_box.py)
-5. [DockWidget](./quite6/gui/widgets/dock_widget.py)
-
-**value widget**:
-
-1. [Label](./quite6/gui/widgets/label.py)
-2. [LineEdit](./quite6/gui/widgets/line_edit.py)
-3. [ComboBox](./quite6/gui/widgets/combo_box.py)
-4. [ListWidget](./quite6/gui/widgets/list_widget.py)
-5. [SpinBox](./quite6/gui/widgets/spin_box.py)
-6. [DoubleSpinBox](./quite6/gui/widgets/double_spin_box.py)
-
-**behavior widget**:
-
-1. [InputDialog](./quite6/gui/widgets/input_dialog.py)
-2. [Action](./quite6/gui/widgets/action.py)
-3. [Shortcut](./quite6/gui/widgets/shortcut.py)
-4. [PushButton](./quite6/gui/widgets/push_button.py)
-
-### Container Widget
-
-*Example 1*: [create widget](./examples/1_create_widget/example-1.py)
-
-```python
-import quite6
-
-w = quite6.Widget()
-w.exec()
-```
-
-![Simple Widget](docs/images/1.simple.widget.png)
-
-*Example 2*: [nested widget](./examples/2_nested_widget/example-2.py)
-
-```python
-import quite6
-
-
-class CustomWidget(quite6.Widget):
-    def paint(self, painter: quite6.Painter):
-        painter.setFont(quite6.QFont("Courier New", 14.0))
-        painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
-        painter.end()
-
-main_window = quite6.MainWindow()
-custom_widget = CustomWidget(parent=main_window)
-main_window.set_central_widget(custom_widget)
-main_window.exec()
-```
-
-![Nested Widget](docs/images/2.nested.widget.png)
-
-*Example 3*: [widget from ui file](./examples/3_widget_from_ui_file/example-3.py)
-
-```python
-import os
-from quite6 import *
-
-
-class CustomWidget(Widget):
-    def paint(self, painter: Painter):
-        w, _ = self.size
-        painter.setFont(QFont("Courier New", 14.0))
-        painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
-        painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
-        painter.end()
-
-
-main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
-main_window.set_central_widget(CustomWidget(parent=main_window))
-main_window.exec()
-```
-
-Use QtDesigner to create a ui file:
-
-![UI Design](docs/images/3.ui.design.png)
+quite6: QT UI Extension for Python3
+==================================
+
+|Build Status|
+
+Features
+--------
+
+1. powerful signal-slot
+2. user friendly widget classes
+
+User Friendly Widget Classes
+----------------------------
+
+Uniform wrapper on frequently-used widget, including:
+
+**container widget**:
+
+1. `Widget <./quite6/gui/widgets/widget.py>`__
+2. `Dialog <./quite6/gui/widgets/dialog.py>`__
+3. `MainWindow <./quite6/gui/widgets/main_window.py>`__
+4. `GroupBox <./quite6/gui/widgets/group_box.py>`__
+5. `DockWidget <./quite6/gui/widgets/dock_widget.py>`__
+
+**value widget**:
+
+1. `Label <./quite6/gui/widgets/label.py>`__
+2. `LineEdit <./quite6/gui/widgets/line_edit.py>`__
+3. `ComboBox <./quite6/gui/widgets/combo_box.py>`__
+4. `ListWidget <./quite6/gui/widgets/list_widget.py>`__
+5. `SpinBox <./quite6/gui/widgets/spin_box.py>`__
+6. `DoubleSpinBox <./quite6/gui/widgets/double_spin_box.py>`__
+
+**behavior widget**:
+
+1. `InputDialog <./quite6/gui/widgets/input_dialog.py>`__
+2. `Action <./quite6/gui/widgets/action.py>`__
+3. `Shortcut <./quite6/gui/widgets/shortcut.py>`__
+4. `PushButton <./quite6/gui/widgets/push_button.py>`__
+
+Container Widget
+~~~~~~~~~~~~~~~~
+
+*Example 1*: `create widget <./examples/1_create_widget/example-1.py>`__
+
+.. code:: python
+
+    import quite6
+
+    w = quite6.Widget()
+    w.exec()
+
+.. figure:: docs/images/1.simple.widget.png
+   :alt: Simple Widget
+
+   Simple Widget
+
+*Example 2*: `nested widget <./examples/2_nested_widget/example-2.py>`__
+
+.. code:: python
+
+    import quite6
+
+
+    class CustomWidget(quite6.Widget):
+        def paint(self, painter: quite6.Painter):
+            painter.setFont(quite6.QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(quite6.PointF(0, 0), "Custom Widget")
+            painter.end()
+
+    main_window = quite6.MainWindow()
+    custom_widget = CustomWidget(parent=main_window)
+    main_window.set_central_widget(custom_widget)
+    main_window.exec()
+
+.. figure:: docs/images/2.nested.widget.png
+   :alt: Nested Widget
+
+   Nested Widget
+
+*Example 3*: `widget from ui
+file <./examples/3_widget_from_ui_file/example-3.py>`__
+
+.. code:: python
+
+    import os
+    from quite6 import *
+
+
+    class CustomWidget(Widget):
+        def paint(self, painter: Painter):
+            w, _ = self.size
+            painter.setFont(QFont("Courier New", 14.0))
+            painter.draw_text_bottom_right(PointF(0, 0), "So Cool!")
+            painter.draw_text_bottom_left(PointF(w, 0), "From Custom Widget")
+            painter.end()
+
+
+    main_window = load_ui(filename=os.path.join(os.path.dirname(__file__), 'main_window.ui'))
+    main_window.set_central_widget(CustomWidget(parent=main_window))
+    main_window.exec()
+
+Use QtDesigner to create a ui file:
+
+.. figure:: docs/images/3.ui.design.png
+   :alt: UI Design
+
+   UI Design
+
+.. |Build Status| image:: https://travis-ci.com/KD-Group/quite6.svg?branch=master
+   :target: https://travis-ci.com/KD-Group/quite6
```

### Comparing `quite6-1.0.5/version.py` & `quite6-1.0.6/version.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# 获取git的tag并保存在RELEASE-VERSION中, 以便每次打包自动识别最新的tag,
-# 并且作为version去发布, 如果不存在RELEASE-VERSION文件且无tag, 默认使用"0.0.1"
-# 使用前必须在MANIFEST.in中加入
-#   include RELEASE-VERSION
-#   include version.py
-
-__all__ = ("get_git_version")
-
-import subprocess
-import os
-
-
-def get_git_latest_tag():
-    def _minimal_ext_cmd(cmd: str):
-        # construct minimal environment
-        env = {}
-        for k in ['SYSTEMROOT', 'PATH']:
-            v = os.environ.get(k)
-            if v is not None:
-                env[k] = v
-        # LANGUAGE is used on win32
-        env['LANGUAGE'] = 'C'
-        env['LANG'] = 'C'
-        env['LC_ALL'] = 'C'
-        out = subprocess.Popen(cmd.split(" "), stdout=subprocess.PIPE, env=env).communicate()[0]
-        return out
-
-    try:
-        out = _minimal_ext_cmd("git describe --abbrev=0 --tags")
-        git_tag = out.strip().decode('ascii')
-        # 去除tag中的v/V
-        if str(git_tag).startswith("v") or str(git_tag).startswith("V"):
-            git_tag = str(git_tag)[1:]
-        if git_tag == "":
-            git_tag = None
-    except Exception:
-        git_tag = None
-
-    return git_tag
-
-
-def read_release_version():
-    try:
-        f = open("RELEASE-VERSION", "r")
-
-        try:
-            version = f.readlines()[0].strip()
-            if version == "":
-                return None
-            else:
-                return version
-        finally:
-            f.close()
-    except Exception:
-        return None
-
-
-def write_release_version(version):
-    f = open("RELEASE-VERSION", "w")
-    f.write("%s\n" % version)
-    f.close()
-
-
-def get_git_version():
-    release_version = read_release_version()
-    version = get_git_latest_tag()
-    if version is None:
-        version = release_version
-
-    # 如果release-version文件没有, 且git没有打tag, 则默认使用"0.0.1"
-    if version is None:
-        version = "0.0.1"
-        # raise ValueError("Cannot find the version number!")
-
-    if version != release_version:
-        write_release_version(version)
-    return version
-
-
-if __name__ == "__main__":
-    print(get_git_version())
+# 获取git的tag并保存在RELEASE-VERSION中, 以便每次打包自动识别最新的tag,
+# 并且作为version去发布, 如果不存在RELEASE-VERSION文件且无tag, 默认使用"0.0.1"
+# 使用前必须在MANIFEST.in中加入
+#   include RELEASE-VERSION
+#   include version.py
+
+__all__ = ("get_git_version")
+
+import subprocess
+import os
+
+
+def get_git_latest_tag():
+    def _minimal_ext_cmd(cmd: str):
+        # construct minimal environment
+        env = {}
+        for k in ['SYSTEMROOT', 'PATH']:
+            v = os.environ.get(k)
+            if v is not None:
+                env[k] = v
+        # LANGUAGE is used on win32
+        env['LANGUAGE'] = 'C'
+        env['LANG'] = 'C'
+        env['LC_ALL'] = 'C'
+        out = subprocess.Popen(cmd.split(" "), stdout=subprocess.PIPE, env=env).communicate()[0]
+        return out
+
+    try:
+        out = _minimal_ext_cmd("git describe --abbrev=0 --tags")
+        git_tag = out.strip().decode('ascii')
+        # 去除tag中的v/V
+        if str(git_tag).startswith("v") or str(git_tag).startswith("V"):
+            git_tag = str(git_tag)[1:]
+        if git_tag == "":
+            git_tag = None
+    except Exception:
+        git_tag = None
+
+    return git_tag
+
+
+def read_release_version():
+    try:
+        f = open("RELEASE-VERSION", "r")
+
+        try:
+            version = f.readlines()[0].strip()
+            if version == "":
+                return None
+            else:
+                return version
+        finally:
+            f.close()
+    except Exception:
+        return None
+
+
+def write_release_version(version):
+    f = open("RELEASE-VERSION", "w")
+    f.write("%s\n" % version)
+    f.close()
+
+
+def get_git_version():
+    release_version = read_release_version()
+    version = get_git_latest_tag()
+    if version is None:
+        version = release_version
+
+    # 如果release-version文件没有, 且git没有打tag, 则默认使用"0.0.1"
+    if version is None:
+        version = "0.0.1"
+        # raise ValueError("Cannot find the version number!")
+
+    if version != release_version:
+        write_release_version(version)
+    return version
+
+
+if __name__ == "__main__":
+    print(get_git_version())
```

