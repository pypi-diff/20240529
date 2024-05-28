# Comparing `tmp/mg-pso-gui-0.1.98.tar.gz` & `tmp/mg-pso-gui-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.98.tar", last modified: Tue May 28 06:07:52 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.99.tar", last modified: Tue May 28 06:53:56 2024, max compression
```

## Comparing `mg-pso-gui-0.1.98.tar` & `mg-pso-gui-0.1.99.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.658467 mg-pso-gui-0.1.98/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:07:52.657906 mg-pso-gui-0.1.98/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.657301 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-28 06:07:52.000000 mg-pso-gui-0.1.98/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.640103 mg-pso-gui-0.1.98/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.98/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.641707 mg-pso-gui-0.1.98/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    24244 2024-05-21 09:15:18.000000 mg-pso-gui-0.1.98/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.98/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.642308 mg-pso-gui-0.1.98/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.98/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.98/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.642897 mg-pso-gui-0.1.98/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.98/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.98/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.646412 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2003 2024-05-21 09:16:16.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/OptimalParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5937 2024-05-21 09:12:51.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.647285 mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/SideBar.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.98/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.651801 mg-pso-gui-0.1.98/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/test.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.98/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.98/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.652753 mg-pso-gui-0.1.98/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.653293 mg-pso-gui-0.1.98/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.98/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.98/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3482 2024-05-28 06:07:45.000000 mg-pso-gui-0.1.98/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.98/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.653755 mg-pso-gui-0.1.98/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.655059 mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12821 2024-05-28 06:06:48.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.656103 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:07:52.656832 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-28 06:07:52.658638 mg-pso-gui-0.1.98/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-28 06:07:49.000000 mg-pso-gui-0.1.98/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.855231 mg-pso-gui-0.1.99/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:53:56.854470 mg-pso-gui-0.1.99/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.853835 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9458 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1871 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-05-28 06:53:56.000000 mg-pso-gui-0.1.99/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.813074 mg-pso-gui-0.1.99/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.99/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.814754 mg-pso-gui-0.1.99/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    24244 2024-05-21 09:15:18.000000 mg-pso-gui-0.1.99/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12527 2024-05-21 08:47:30.000000 mg-pso-gui-0.1.99/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.815615 mg-pso-gui-0.1.99/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.99/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.99/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.816393 mg-pso-gui-0.1.99/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1839 2024-03-20 19:57:02.000000 mg-pso-gui-0.1.99/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.99/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.822170 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2003 2024-05-21 09:16:16.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/OptimalParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2443 2024-05-21 09:01:39.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5937 2024-05-21 09:12:51.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.823869 mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13322 2024-05-15 21:08:56.000000 mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/SideBar.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3477 2024-04-10 18:55:43.000000 mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.99/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.846536 mg-pso-gui-0.1.99/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3642 2024-03-20 06:12:19.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/test.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.99/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.99/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.848167 mg-pso-gui-0.1.99/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.848865 mg-pso-gui-0.1.99/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.99/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    15076 2024-04-24 19:47:23.000000 mg-pso-gui-0.1.99/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3437 2024-05-28 06:53:49.000000 mg-pso-gui-0.1.99/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.99/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.849390 mg-pso-gui-0.1.99/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.850698 mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2721 2024-03-20 06:01:30.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12821 2024-05-28 06:06:48.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.852222 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-05-28 06:53:56.853255 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-05-28 06:53:56.855332 mg-pso-gui-0.1.99/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1526 2024-05-28 06:53:54.000000 mg-pso-gui-0.1.99/setup.py
```

### Comparing `mg-pso-gui-0.1.98/PKG-INFO` & `mg-pso-gui-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.98
+Version: 0.1.99
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.98/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.99/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.98
+Version: 0.1.99
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.98/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.99/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/HomePage.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/HomePage.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/OptionManager.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/RunTab/RunTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/OptimalParameterView.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/OptimalParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/StaticParameterView.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/SetupTab/StepView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/SideBar.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/SideBar.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.99/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/test.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/test.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.99/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/start.yaml` & `mg-pso-gui-0.1.99/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.99/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/GraphGenerator.py` & `mg-pso-gui-0.1.99/mgpsogui/util/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/PSORunner.py` & `mg-pso-gui-0.1.99/mgpsogui/util/PSORunner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import csip
-from csip import Client
-import cosu
+
 import sys
 from multiprocessing import Process, Queue
 from queue import Empty
 import threading
 import time
 import os
 
-#from cosu.pso import global_best
-from .recosu.pso import global_best
+from cosu.pso import global_best
+#from .recosu.pso import global_best
 
 def enqueue_output(out, queue):
     for line in iter(out.readline, b''):
         queue.put(line)
     out.close()
 
 def run_process(stdout_queue, stderr_queue, results_queue, cosu_queue, data, folder):
@@ -83,16 +81,16 @@
             conf={
                 'service_timeout': int(calibration_map['service_timeout']),
                 'http_retry': int(calibration_map['http_retry']),
                 'http_allow_redirects': True if calibration_map['allow_redirects'] == "True" else False,
                 'async_call': True if calibration_map['async_call'] == "True" else False,
                 'http_conn_timeout': int(calibration_map['conn_timeout']),
                 'http_read_timeout': int(calibration_map['read_timeout']),
-                'particles_fail': int(calibration_map['particles_fail']),
-                'step_trace': os.path.join(folder, 'trace.json')
+                'particles_fail': int(calibration_map['particles_fail'])
+                #, 'step_trace': os.path.join(folder, 'trace.json')
                 },
             #result_queue = cosu_queue
         )
     
     results_queue.put(trace)
     print(trace)
```

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.99/mgpsogui/util/recosu/pso/pso.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.99/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.98/setup.py` & `mg-pso-gui-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.98'
+VERSION = '0.1.99'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

