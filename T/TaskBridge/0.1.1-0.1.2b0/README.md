# Comparing `tmp/taskbridge-0.1.1.tar.gz` & `tmp/taskbridge-0.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbridge-0.1.1.tar", max compression
+gzip compressed data, was "taskbridge-0.1.2b0.tar", max compression
```

## Comparing `taskbridge-0.1.1.tar` & `taskbridge-0.1.2b0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
--rw-r--r--   0        0        0    35128 2024-05-28 10:12:50.913347 taskbridge-0.1.1/LICENSE
--rw-r--r--   0        0        0     7735 2024-05-28 11:55:55.707692 taskbridge-0.1.1/README.md
--rw-r--r--   0        0        0     1694 2024-05-28 11:59:55.664499 taskbridge-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      348 2024-05-28 10:12:50.937351 taskbridge-0.1.1/taskbridge/__init__.py
--rw-r--r--   0        0        0      138 2024-05-28 11:04:48.375560 taskbridge-0.1.1/taskbridge/cli/__init__.py
--rw-r--r--   0        0        0    19064 2024-05-28 11:06:15.575002 taskbridge-0.1.1/taskbridge/cli/tbcli.py
--rw-r--r--   0        0        0      680 2024-05-28 10:12:50.938068 taskbridge-0.1.1/taskbridge/gui/TaskBridge.py
--rw-r--r--   0        0        0      429 2024-05-28 11:04:04.016939 taskbridge-0.1.1/taskbridge/gui/__init__.py
--rw-r--r--   0        0        0     2839 2024-05-28 10:12:50.938560 taskbridge-0.1.1/taskbridge/gui/about.ui
--rw-r--r--   0        0        0    13473 2024-05-28 10:12:50.938821 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
--rw-r--r--   0        0        0    13805 2024-05-28 10:12:50.939034 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
--rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.940652 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
--rw-r--r--   0        0        0    16622 2024-05-28 10:12:50.940972 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
--rw-r--r--   0        0        0    17860 2024-05-28 10:12:50.941209 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
--rw-r--r--   0        0        0    19866 2024-05-28 10:12:50.941528 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
--rw-r--r--   0        0        0    23814 2024-05-28 10:12:50.941837 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
--rw-r--r--   0        0        0    25818 2024-05-28 10:12:50.942007 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
--rw-r--r--   0        0        0      822 2024-05-28 10:12:50.942220 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
--rw-r--r--   0        0        0    30211 2024-05-28 10:12:50.942564 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
--rw-r--r--   0        0        0    31652 2024-05-28 10:12:50.942909 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
--rw-r--r--   0        0        0    34032 2024-05-28 10:12:50.943391 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
--rw-r--r--   0        0        0    39070 2024-05-28 10:12:50.943886 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
--rw-r--r--   0        0        0     1104 2024-05-28 10:12:50.944119 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
--rw-r--r--   0        0        0    45736 2024-05-28 10:12:50.944656 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
--rw-r--r--   0        0        0    60912 2024-05-28 10:12:50.945186 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
--rw-r--r--   0        0        0     1922 2024-05-28 10:12:50.945387 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
--rw-r--r--   0        0        0     2235 2024-05-28 10:12:50.945681 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
--rw-r--r--   0        0        0     3180 2024-05-28 10:12:50.945872 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
--rw-r--r--   0        0        0     4265 2024-05-28 10:12:50.946089 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
--rw-r--r--   0        0        0     4543 2024-05-28 10:12:50.946359 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
--rw-r--r--   0        0        0   206946 2024-05-28 10:12:50.950422 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
--rw-r--r--   0        0        0     5252 2024-05-28 10:12:50.950722 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
--rw-r--r--   0        0        0     5549 2024-05-28 10:12:50.951020 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
--rw-r--r--   0        0        0     5649 2024-05-28 10:12:50.951179 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
--rw-r--r--   0        0        0     5983 2024-05-28 10:12:50.951413 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
--rw-r--r--   0        0        0     6583 2024-05-28 10:12:50.951648 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
--rw-r--r--   0        0        0     6988 2024-05-28 10:12:50.951770 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
--rw-r--r--   0        0        0     7993 2024-05-28 10:12:50.951890 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
--rw-r--r--   0        0        0     8732 2024-05-28 10:12:50.952196 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
--rw-r--r--   0        0        0     9417 2024-05-28 10:12:50.952599 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
--rw-r--r--   0        0        0    10705 2024-05-28 10:12:50.952918 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
--rw-r--r--   0        0        0    10894 2024-05-28 10:12:50.953132 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
--rw-r--r--   0        0        0    11674 2024-05-28 10:12:50.953339 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
--rw-r--r--   0        0        0     7139 2024-05-28 10:12:50.953567 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0        0        0   772414 2024-05-28 10:12:50.954162 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/appstore.png
--rw-r--r--   0        0        0   214701 2024-05-28 10:12:50.955002 taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/playstore.png
--rw-r--r--   0        0        0   998221 2024-05-28 10:12:50.957694 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.icns
--rw-r--r--   0        0        0    17569 2024-05-28 10:12:50.958192 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
--rw-r--r--   0        0        0    50656 2024-05-28 10:12:50.958847 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
--rw-r--r--   0        0        0     1699 2024-05-28 10:12:50.959128 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
--rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.959494 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
--rw-r--r--   0        0        0    50655 2024-05-28 10:12:50.960206 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
--rw-r--r--   0        0        0   159642 2024-05-28 10:12:50.961211 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
--rw-r--r--   0        0        0     2759 2024-05-28 10:12:50.961450 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
--rw-r--r--   0        0        0     6510 2024-05-28 10:12:50.961765 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
--rw-r--r--   0        0        0   159641 2024-05-28 10:12:50.962802 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
--rw-r--r--   0        0        0   551167 2024-05-28 10:12:50.964524 taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
--rw-r--r--   0        0        0   931253 2024-05-28 10:12:50.968883 taskbridge-0.1.1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
--rw-r--r--   0        0        0    69368 2024-05-28 10:12:50.971236 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge.xcf
--rw-r--r--   0        0        0   658861 2024-05-28 10:12:50.972885 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_black.xcf
--rw-r--r--   0        0        0    63732 2024-05-28 10:12:50.973309 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
--rw-r--r--   0        0        0  1156034 2024-05-28 10:12:50.975394 taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_white.xcf
--rw-r--r--   0        0        0     3862 2024-05-28 10:12:50.975704 taskbridge-0.1.1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
--rw-r--r--   0        0        0     5539 2024-05-28 10:12:50.975944 taskbridge-0.1.1/taskbridge/gui/assets/source/ios-swap-7-512.png
--rw-r--r--   0        0        0     8361 2024-05-28 10:12:50.976299 taskbridge-0.1.1/taskbridge/gui/assets/source/local.png
--rw-r--r--   0        0        0     2197 2024-05-28 10:12:50.976549 taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_black.xcf
--rw-r--r--   0        0        0     3294 2024-05-28 10:12:50.976763 taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_white.xcf
--rw-r--r--   0        0        0    18816 2024-05-28 10:12:50.977106 taskbridge-0.1.1/taskbridge/gui/assets/source/remote.png
--rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977370 taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_black.png
--rw-r--r--   0        0        0     1301 2024-05-28 10:12:50.977572 taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_white.png
--rw-r--r--   0        0        0     1591 2024-05-28 10:12:50.977789 taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_black.png
--rw-r--r--   0        0        0     1686 2024-05-28 10:12:50.978040 taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_white.png
--rw-r--r--   0        0        0      965 2024-05-28 10:12:50.978308 taskbridge-0.1.1/taskbridge/gui/assets/table/local_black.png
--rw-r--r--   0        0        0     1950 2024-05-28 10:12:50.978538 taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_black.png
--rw-r--r--   0        0        0     1955 2024-05-28 10:12:50.978765 taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_white.png
--rw-r--r--   0        0        0      990 2024-05-28 10:12:50.979082 taskbridge-0.1.1/taskbridge/gui/assets/table/local_white.png
--rw-r--r--   0        0        0     1266 2024-05-28 10:12:50.979320 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_black.png
--rw-r--r--   0        0        0     2885 2024-05-28 10:12:50.979551 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_black.png
--rw-r--r--   0        0        0     2847 2024-05-28 10:12:50.979755 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_white.png
--rw-r--r--   0        0        0     1290 2024-05-28 10:12:50.979981 taskbridge-0.1.1/taskbridge/gui/assets/table/remote_white.png
--rw-r--r--   0        0        0    17458 2024-05-28 10:12:50.980399 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_black.gif
--rw-r--r--   0        0        0    17522 2024-05-28 10:12:50.980793 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_white.gif
--rw-r--r--   0        0        0    47984 2024-05-28 10:12:50.981403 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_black.png
--rw-r--r--   0        0        0    11350 2024-05-28 10:12:50.981753 taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_white.png
--rw-r--r--   0        0        0   387868 2024-05-28 10:12:50.983237 taskbridge-0.1.1/taskbridge/gui/assets/ui/TaskBridge.png
--rw-r--r--   0        0        0     4909 2024-05-28 10:12:50.983497 taskbridge-0.1.1/taskbridge/gui/assets/ui/refresh.png
--rw-r--r--   0        0        0     3701 2024-05-28 10:12:50.985394 taskbridge-0.1.1/taskbridge/gui/assets/ui/trash.png
--rw-r--r--   0        0        0    29098 2024-05-28 10:12:50.985662 taskbridge-0.1.1/taskbridge/gui/taskbridge.ui
--rw-r--r--   0        0        0      908 2024-05-28 10:12:50.985936 taskbridge-0.1.1/taskbridge/gui/viewmodel/__init__.py
--rw-r--r--   0        0        0      476 2024-05-28 10:12:50.986140 taskbridge-0.1.1/taskbridge/gui/viewmodel/mainwindow.py
--rw-r--r--   0        0        0     2703 2024-05-28 10:12:50.986369 taskbridge-0.1.1/taskbridge/gui/viewmodel/notecheckbox.py
--rw-r--r--   0        0        0     1918 2024-05-28 10:12:50.986595 taskbridge-0.1.1/taskbridge/gui/viewmodel/remindercheckbox.py
--rw-r--r--   0        0        0    45804 2024-05-28 10:12:50.986875 taskbridge-0.1.1/taskbridge/gui/viewmodel/taskbridgeapp.py
--rw-r--r--   0        0        0    13063 2024-05-28 10:12:50.987144 taskbridge-0.1.1/taskbridge/gui/viewmodel/threadedtasks.py
--rw-r--r--   0        0        0     1771 2024-05-28 10:12:50.987467 taskbridge-0.1.1/taskbridge/gui/viewmodel/trayicon.py
--rw-r--r--   0        0        0     3201 2024-05-28 10:12:50.987796 taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_aboutwindow.py
--rw-r--r--   0        0        0    32872 2024-05-28 10:12:50.989411 taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_mainwindow.py
--rw-r--r--   0        0        0     5496 2024-05-28 10:56:54.707655 taskbridge-0.1.1/taskbridge/helpers.py
--rw-r--r--   0        0        0      570 2024-05-28 10:12:50.989907 taskbridge-0.1.1/taskbridge/notes/__init__.py
--rw-r--r--   0        0        0     7391 2024-05-28 10:12:50.990114 taskbridge-0.1.1/taskbridge/notes/controller.py
--rw-r--r--   0        0        0      572 2024-05-28 10:58:25.084166 taskbridge-0.1.1/taskbridge/notes/model/__init__.py
--rw-r--r--   0        0        0    19383 2024-05-28 10:59:05.331708 taskbridge-0.1.1/taskbridge/notes/model/note.py
--rw-r--r--   0        0        0    43723 2024-05-28 10:12:50.991327 taskbridge-0.1.1/taskbridge/notes/model/notefolder.py
--rw-r--r--   0        0        0     6063 2024-05-28 10:12:50.991477 taskbridge-0.1.1/taskbridge/notes/model/notescript.py
--rw-r--r--   0        0        0      651 2024-05-28 10:59:05.329335 taskbridge-0.1.1/taskbridge/reminders/__init__.py
--rw-r--r--   0        0        0    10528 2024-05-28 10:12:50.991927 taskbridge-0.1.1/taskbridge/reminders/controller.py
--rw-r--r--   0        0        0      755 2024-05-28 10:12:50.992162 taskbridge-0.1.1/taskbridge/reminders/model/__init__.py
--rw-r--r--   0        0        0    16131 2024-05-28 10:12:50.992407 taskbridge-0.1.1/taskbridge/reminders/model/reminder.py
--rw-r--r--   0        0        0    47638 2024-05-28 10:12:50.992686 taskbridge-0.1.1/taskbridge/reminders/model/remindercontainer.py
--rw-r--r--   0        0        0     4942 2024-05-28 10:12:50.992846 taskbridge-0.1.1/taskbridge/reminders/model/reminderscript.py
--rw-r--r--   0        0        0     9159 1970-01-01 00:00:00.000000 taskbridge-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-05-29 14:46:38.637192 taskbridge-0.1.2b0/LICENSE
+-rw-r--r--   0        0        0     7735 2024-05-29 14:46:38.637482 taskbridge-0.1.2b0/README.md
+-rw-r--r--   0        0        0     1703 2024-05-29 14:46:38.665234 taskbridge-0.1.2b0/pyproject.toml
+-rw-r--r--   0        0        0      348 2024-05-29 14:46:38.665748 taskbridge-0.1.2b0/taskbridge/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-29 14:46:38.665940 taskbridge-0.1.2b0/taskbridge/cli/__init__.py
+-rw-r--r--   0        0        0    19064 2024-05-29 14:46:38.666121 taskbridge-0.1.2b0/taskbridge/cli/tbcli.py
+-rw-r--r--   0        0        0      915 2024-05-29 14:46:38.666360 taskbridge-0.1.2b0/taskbridge/gui/TaskBridge.py
+-rw-r--r--   0        0        0      429 2024-05-29 14:46:38.666525 taskbridge-0.1.2b0/taskbridge/gui/__init__.py
+-rw-r--r--   0        0        0     2844 2024-05-29 14:46:38.666722 taskbridge-0.1.2b0/taskbridge/gui/about.ui
+-rw-r--r--   0        0        0    13473 2024-05-29 14:46:38.667068 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png
+-rw-r--r--   0        0        0    13805 2024-05-29 14:46:38.667348 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png
+-rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.668877 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png
+-rw-r--r--   0        0        0    16622 2024-05-29 14:46:38.671068 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png
+-rw-r--r--   0        0        0    17860 2024-05-29 14:46:38.671293 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png
+-rw-r--r--   0        0        0    19866 2024-05-29 14:46:38.672912 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png
+-rw-r--r--   0        0        0    23814 2024-05-29 14:46:38.673433 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png
+-rw-r--r--   0        0        0    25818 2024-05-29 14:46:38.673746 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png
+-rw-r--r--   0        0        0      822 2024-05-29 14:46:38.674051 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png
+-rw-r--r--   0        0        0    30211 2024-05-29 14:46:38.674423 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png
+-rw-r--r--   0        0        0    31652 2024-05-29 14:46:38.674781 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png
+-rw-r--r--   0        0        0    34032 2024-05-29 14:46:38.675263 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png
+-rw-r--r--   0        0        0    39070 2024-05-29 14:46:38.675737 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png
+-rw-r--r--   0        0        0     1104 2024-05-29 14:46:38.675995 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png
+-rw-r--r--   0        0        0    45736 2024-05-29 14:46:38.676540 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png
+-rw-r--r--   0        0        0    60912 2024-05-29 14:46:38.676837 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png
+-rw-r--r--   0        0        0     1922 2024-05-29 14:46:38.677079 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png
+-rw-r--r--   0        0        0     2235 2024-05-29 14:46:38.677318 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png
+-rw-r--r--   0        0        0     3180 2024-05-29 14:46:38.677584 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png
+-rw-r--r--   0        0        0     4265 2024-05-29 14:46:38.677806 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png
+-rw-r--r--   0        0        0     4543 2024-05-29 14:46:38.678020 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png
+-rw-r--r--   0        0        0   206946 2024-05-29 14:46:38.678816 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png
+-rw-r--r--   0        0        0     5252 2024-05-29 14:46:38.679026 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png
+-rw-r--r--   0        0        0     5549 2024-05-29 14:46:38.679300 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png
+-rw-r--r--   0        0        0     5649 2024-05-29 14:46:38.679428 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png
+-rw-r--r--   0        0        0     5983 2024-05-29 14:46:38.679630 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png
+-rw-r--r--   0        0        0     6583 2024-05-29 14:46:38.679855 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png
+-rw-r--r--   0        0        0     6988 2024-05-29 14:46:38.679989 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png
+-rw-r--r--   0        0        0     7993 2024-05-29 14:46:38.680118 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png
+-rw-r--r--   0        0        0     8732 2024-05-29 14:46:38.680349 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png
+-rw-r--r--   0        0        0     9417 2024-05-29 14:46:38.680628 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png
+-rw-r--r--   0        0        0    10705 2024-05-29 14:46:38.680861 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png
+-rw-r--r--   0        0        0    10894 2024-05-29 14:46:38.680985 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png
+-rw-r--r--   0        0        0    11674 2024-05-29 14:46:38.681115 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png
+-rw-r--r--   0        0        0     7139 2024-05-29 14:46:38.681329 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0        0        0   772414 2024-05-29 14:46:38.681942 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/appstore.png
+-rw-r--r--   0        0        0   214701 2024-05-29 14:46:38.682811 taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/playstore.png
+-rw-r--r--   0        0        0   998221 2024-05-29 14:46:38.685300 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.icns
+-rw-r--r--   0        0        0    17569 2024-05-29 14:46:38.685768 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png
+-rw-r--r--   0        0        0    50656 2024-05-29 14:46:38.686088 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png
+-rw-r--r--   0        0        0     1699 2024-05-29 14:46:38.686298 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png
+-rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.686540 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png
+-rw-r--r--   0        0        0    50655 2024-05-29 14:46:38.686841 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png
+-rw-r--r--   0        0        0   159642 2024-05-29 14:46:38.687387 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png
+-rw-r--r--   0        0        0     2759 2024-05-29 14:46:38.687491 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png
+-rw-r--r--   0        0        0     6510 2024-05-29 14:46:38.689300 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png
+-rw-r--r--   0        0        0   159641 2024-05-29 14:46:38.691223 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png
+-rw-r--r--   0        0        0   551167 2024-05-29 14:46:38.692610 taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png
+-rw-r--r--   0        0        0   931253 2024-05-29 14:46:38.696537 taskbridge-0.1.2b0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf
+-rw-r--r--   0        0        0    69368 2024-05-29 14:46:38.697232 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge.xcf
+-rw-r--r--   0        0        0   658861 2024-05-29 14:46:38.698526 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_black.xcf
+-rw-r--r--   0        0        0    63732 2024-05-29 14:46:38.698922 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf
+-rw-r--r--   0        0        0  1156034 2024-05-29 14:46:38.700882 taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_white.xcf
+-rw-r--r--   0        0        0   710088 2024-05-29 14:46:38.705680 taskbridge-0.1.2b0/taskbridge/gui/assets/source/dmg_background.png
+-rw-r--r--   0        0        0     3862 2024-05-29 14:46:38.705979 taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png
+-rw-r--r--   0        0        0     5539 2024-05-29 14:46:38.706230 taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-swap-7-512.png
+-rw-r--r--   0        0        0     8361 2024-05-29 14:46:38.706503 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local.png
+-rw-r--r--   0        0        0     2197 2024-05-29 14:46:38.706759 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_black.xcf
+-rw-r--r--   0        0        0     3294 2024-05-29 14:46:38.707000 taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_white.xcf
+-rw-r--r--   0        0        0    18816 2024-05-29 14:46:38.707358 taskbridge-0.1.2b0/taskbridge/gui/assets/source/remote.png
+-rw-r--r--   0        0        0   825227 2024-05-29 14:46:38.709311 taskbridge-0.1.2b0/taskbridge/gui/assets/source/tb_disk_icon.icns
+-rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709605 taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_black.png
+-rw-r--r--   0        0        0     1301 2024-05-29 14:46:38.709828 taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_white.png
+-rw-r--r--   0        0        0     1591 2024-05-29 14:46:38.710039 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_black.png
+-rw-r--r--   0        0        0     1686 2024-05-29 14:46:38.710255 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_white.png
+-rw-r--r--   0        0        0      965 2024-05-29 14:46:38.710478 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_black.png
+-rw-r--r--   0        0        0     1950 2024-05-29 14:46:38.710713 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_black.png
+-rw-r--r--   0        0        0     1955 2024-05-29 14:46:38.710919 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_white.png
+-rw-r--r--   0        0        0      990 2024-05-29 14:46:38.711119 taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_white.png
+-rw-r--r--   0        0        0     1266 2024-05-29 14:46:38.711316 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_black.png
+-rw-r--r--   0        0        0     2885 2024-05-29 14:46:38.711498 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_black.png
+-rw-r--r--   0        0        0     2847 2024-05-29 14:46:38.711688 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_white.png
+-rw-r--r--   0        0        0     1290 2024-05-29 14:46:38.711895 taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_white.png
+-rw-r--r--   0        0        0    17458 2024-05-29 14:46:38.712296 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_black.gif
+-rw-r--r--   0        0        0    17522 2024-05-29 14:46:38.712703 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_white.gif
+-rw-r--r--   0        0        0    47984 2024-05-29 14:46:38.713321 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_black.png
+-rw-r--r--   0        0        0    11350 2024-05-29 14:46:38.713556 taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_white.png
+-rw-r--r--   0        0        0   387868 2024-05-29 14:46:38.714712 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/TaskBridge.png
+-rw-r--r--   0        0        0     4909 2024-05-29 14:46:38.714953 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/refresh.png
+-rw-r--r--   0        0        0     3701 2024-05-29 14:46:38.715142 taskbridge-0.1.2b0/taskbridge/gui/assets/ui/trash.png
+-rw-r--r--   0        0        0    29098 2024-05-29 14:46:38.715349 taskbridge-0.1.2b0/taskbridge/gui/taskbridge.ui
+-rw-r--r--   0        0        0      908 2024-05-29 14:46:38.715578 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/__init__.py
+-rw-r--r--   0        0        0      476 2024-05-29 14:46:38.715766 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/mainwindow.py
+-rw-r--r--   0        0        0     2703 2024-05-29 14:46:38.715983 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/notecheckbox.py
+-rw-r--r--   0        0        0     1918 2024-05-29 14:46:38.716193 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/remindercheckbox.py
+-rw-r--r--   0        0        0    46116 2024-05-29 14:46:38.716516 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/taskbridgeapp.py
+-rw-r--r--   0        0        0    13063 2024-05-29 14:46:38.716812 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/threadedtasks.py
+-rw-r--r--   0        0        0     1771 2024-05-29 14:46:38.717003 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/trayicon.py
+-rw-r--r--   0        0        0     3201 2024-05-29 14:46:38.717196 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_aboutwindow.py
+-rw-r--r--   0        0        0    32872 2024-05-29 14:46:38.717415 taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_mainwindow.py
+-rw-r--r--   0        0        0     5496 2024-05-29 14:46:38.717636 taskbridge-0.1.2b0/taskbridge/helpers.py
+-rw-r--r--   0        0        0      570 2024-05-29 14:46:38.717839 taskbridge-0.1.2b0/taskbridge/notes/__init__.py
+-rw-r--r--   0        0        0     7391 2024-05-29 14:46:38.718013 taskbridge-0.1.2b0/taskbridge/notes/controller.py
+-rw-r--r--   0        0        0      572 2024-05-29 14:46:38.718265 taskbridge-0.1.2b0/taskbridge/notes/model/__init__.py
+-rw-r--r--   0        0        0    19383 2024-05-29 14:46:38.718466 taskbridge-0.1.2b0/taskbridge/notes/model/note.py
+-rw-r--r--   0        0        0    43723 2024-05-29 14:46:38.718734 taskbridge-0.1.2b0/taskbridge/notes/model/notefolder.py
+-rw-r--r--   0        0        0     6063 2024-05-29 14:46:38.718887 taskbridge-0.1.2b0/taskbridge/notes/model/notescript.py
+-rw-r--r--   0        0        0      651 2024-05-29 14:46:38.719079 taskbridge-0.1.2b0/taskbridge/reminders/__init__.py
+-rw-r--r--   0        0        0    10528 2024-05-29 14:46:38.719207 taskbridge-0.1.2b0/taskbridge/reminders/controller.py
+-rw-r--r--   0        0        0      755 2024-05-29 14:46:38.719402 taskbridge-0.1.2b0/taskbridge/reminders/model/__init__.py
+-rw-r--r--   0        0        0    16131 2024-05-29 14:46:38.719609 taskbridge-0.1.2b0/taskbridge/reminders/model/reminder.py
+-rw-r--r--   0        0        0    47638 2024-05-29 14:46:38.719843 taskbridge-0.1.2b0/taskbridge/reminders/model/remindercontainer.py
+-rw-r--r--   0        0        0     4942 2024-05-29 14:46:38.719972 taskbridge-0.1.2b0/taskbridge/reminders/model/reminderscript.py
+-rw-r--r--   0        0        0     9162 1970-01-01 00:00:00.000000 taskbridge-0.1.2b0/PKG-INFO
```

### Comparing `taskbridge-0.1.1/LICENSE` & `taskbridge-0.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/README.md` & `taskbridge-0.1.2b0/README.md`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/pyproject.toml` & `taskbridge-0.1.2b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TaskBridge"
-version = "0.1.1"
+version = "0.1.2-beta"
 description = "Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!"
 keywords = ["sync", "note sync", "reminder sync", "cloud notes", "cloud reminders"]
 authors = ["Pint-Sized Software <hello@pintsized.dev>"]
 readme = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -17,15 +17,15 @@
   "Topic :: Utilities"
 ]
 license = "GPL-3.0-or-later"
 homepage = "https://taskbridge.app/"
 repository = "https://github.com/pint-sized/taskbridge"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<3.13"
 PyQt6 = "^6.6.1"
 darkdetect = "^0.8.0"
 keyring = "^25.2.1"
 schedule = "^1.2.1"
 caldav = "^1.3.9"
 markdown2 = "^2.4.13"
 markdownify = "^0.12.1"
@@ -44,23 +44,24 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 python-decouple = "^3.8"
 coveralls = "^3.3.1"
 pyyaml = "^6.0.1"
 
+[tool.poetry.group.dist]
+optional = true
+
+[tool.poetry.group.dist.dependencies]
+pyinstaller = "^6.7.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tools.py2app.bundle.main]
-name = "TaskBridge"
-script = "taskbridge/gui/app.py"
-build-type = "standalone"
-
 [tool.poetry.scripts]
 tbcli = 'taskbridge.cli.tbcli:main'
 
 [tool.coverage.run]
 omit = [
     "*tests*",
 ]
```

### Comparing `taskbridge-0.1.1/taskbridge/cli/tbcli.py` & `taskbridge-0.1.2b0/taskbridge/cli/tbcli.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/TaskBridge.py` & `taskbridge-0.1.2b0/taskbridge/gui/TaskBridge.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """
 Main application entry point. Creates system tray icon and displays main window.
 """
-
+import os
 import sys
 
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QApplication
 import darkdetect
 
 from taskbridge.gui.viewmodel import trayicon
 from taskbridge.gui.viewmodel.taskbridgeapp import TaskBridgeApp
 
 if __name__ == "__main__":
+    if getattr(sys, 'frozen', False):
+        # noinspection PyProtectedMember
+        assets_path = sys._MEIPASS + "/taskbridge/gui/assets"
+    else:
+        assets_path = os.path.dirname(os.path.abspath(__file__)) + "/assets"
+
     app = QApplication(sys.argv)
     app.setQuitOnLastWindowClosed(False)
-    tb = TaskBridgeApp()
-    icon_path = "taskbridge/gui/assets/tray/bridge_black.png" if darkdetect.isDark() else \
-        "taskbridge/gui/assets/tray/bridge_white.png"
+    tb = TaskBridgeApp(assets_path)
+    icon_path = assets_path + "/tray/bridge_black.png" if darkdetect.isDark() else \
+        assets_path + "/tray/bridge_white.png"
     trayIcon = trayicon.TaskBridgeTray(QIcon(icon_path), tb)
     tb.tray_icon = trayIcon
     app.exec()
```

### Comparing `taskbridge-0.1.1/taskbridge/gui/about.ui` & `taskbridge-0.1.2b0/taskbridge/gui/about.ui`

 * *Files 4% similar despite different names*

#### Comparing `taskbridge-0.1.1/taskbridge/gui/about.ui` & `taskbridge-0.1.2b0/taskbridge/gui/about.ui`

```diff
@@ -89,15 +89,15 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="lbl_version">
           <property name="text">
-            <string>Version 0.1.0</string>
+            <string>Version 0.1.2-beta</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
```

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/100.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/102.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/1024.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/114.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/120.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/144.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/152.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/167.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/172.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/180.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/196.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/20.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/216.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/29.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/40.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/48.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/50.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/55.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/57.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/58.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/60.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/64.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/66.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/72.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/76.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/80.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/87.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/88.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/92.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/appstore.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/appstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/AppIcons/playstore.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/AppIcons/playstore.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.icns` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.icns`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/TaskBridge.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/TaskBridge_Icon.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/TaskBridge_Icon.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_black.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_optimised.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_optimised.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/bridge_animated_white.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/bridge_animated_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-arrow-round-up-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/ios-swap-7-512.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/ios-swap-7-512.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/local.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_black.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_black.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/local_and_remote_white.xcf` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/local_and_remote_white.xcf`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/source/remote.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/source/remote.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/bidirectional_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/bidirectional_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_and_remote_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_and_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_to_remote_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_to_remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/local_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_to_local_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_to_local_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/table/remote_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/table/remote_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_black.gif` & `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_black.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_animated_white.gif` & `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_animated_white.gif`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_black.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_black.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/tray/bridge_white.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/tray/bridge_white.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/ui/TaskBridge.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/TaskBridge.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/ui/refresh.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/refresh.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/assets/ui/trash.png` & `taskbridge-0.1.2b0/taskbridge/gui/assets/ui/trash.png`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/taskbridge.ui` & `taskbridge-0.1.2b0/taskbridge/gui/taskbridge.ui`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/__init__.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/notecheckbox.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/notecheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/remindercheckbox.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/remindercheckbox.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/taskbridgeapp.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/taskbridgeapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,27 +78,31 @@
         'autosync_interval': 0,
         'autosync_unit': 'Minutes'
     }
 
     #: If True, there are unsaved changes.
     PENDING_CHANGES: bool = False
 
-    def __init__(self):
+    def __init__(self, assets_path: str):
         """
         Initialise the window and load settings.
+
+        :param assets_path: Path to the GUI assets folder
+
         """
 
         super().__init__()
         self.reminder_pw_worker = threadedtasks.ReminderPreWarm(self.display_reminders_table)
         self.note_pw_worker = threadedtasks.NotePreWarm(self.display_notes_table)
         self.autosync_worker = None
         self.sync_worker = None
         self.tray_icon = None
+        self.assets_path: str = assets_path
         TaskBridgeApp.bootstrap_settings()
-        QtCore.QDir.addSearchPath('assets', 'taskbridge/gui/assets')
+        QtCore.QDir.addSearchPath('assets', assets_path)
         self.note_boxes: List = []
         self.reminder_boxes: List = []
         self.ui: MainWindow = MainWindow()
 
         TaskBridgeApp.load_settings()
         self.logging_worker = threadedtasks.LoggingThread(TaskBridgeApp.SETTINGS['log_level'], log_stdout=True)
         self.logging_worker.log_signal.connect(self.display_log)
@@ -185,25 +189,24 @@
         dialog.ui.setupUi(dialog)
         dialog.ui.lbl_taskbridge_logo.setPixmap(QtGui.QPixmap('assets:ui/TaskBridge.png'))
         dialog.setWindowFlags(dialog.windowFlags() | QtCore.Qt.WindowType.CustomizeWindowHint)
         dialog.setWindowFlags(dialog.windowFlags() & ~QtCore.Qt.WindowType.WindowMaximizeButtonHint)
         dialog.setAttribute(QtCore.Qt.WidgetAttribute.WA_DeleteOnClose)
         dialog.exec()
 
-    @staticmethod
-    def get_table_icon(image: str) -> str:
+    def get_table_icon(self, image: str) -> str:
         """
         Gets an icon for inline-display in table. Returns correct icon depending on whether dark mode is set.
 
         :param image: the name of the image to display from the 'taskbridge/gui/assets/table' folder.
 
         :return: path to the correct image.
         """
         colour = 'white' if darkdetect.isDark() else 'black'
-        image_path = 'taskbridge/gui/assets/table/{0}_{1}.png'.format(image, colour)
+        image_path = self.assets_path + '/table/{0}_{1}.png'.format(image, colour)
         return image_path
 
     def save_settings(self, what: str | None = None, silent: bool = True) -> None:
         """
         Save settings to file.
 
         :param what: what was saved. Used when displaying confirmation dialog and to prompt for reminder pruning.
@@ -436,21 +439,21 @@
         """
         Initialises the notes table
         """
         self.ui.tbl_notes.setColumnCount(5)
         self.ui.tbl_notes.horizontalHeader().setSectionResizeMode(QHeaderView.ResizeMode.Stretch)
         self.ui.tbl_notes.setHorizontalHeaderItem(0, QTableWidgetItem('Folder'))
         self.ui.tbl_notes.setHorizontalHeaderItem(1, QTableWidgetItem('Location'))
-        icon = QIcon(QtGui.QPixmap(TaskBridgeApp.get_table_icon('local_to_remote')))
+        icon = QIcon(QtGui.QPixmap(self.get_table_icon('local_to_remote')))
         self.ui.tbl_notes.setHorizontalHeaderItem(2, QTableWidgetItem(icon, None, QTableWidgetItem.ItemType.UserType))
         self.ui.tbl_notes.horizontalHeaderItem(2).setToolTip('Sync local notes to remote')
-        icon = QIcon(QtGui.QPixmap(TaskBridgeApp.get_table_icon('remote_to_local')))
+        icon = QIcon(QtGui.QPixmap(self.get_table_icon('remote_to_local')))
         self.ui.tbl_notes.setHorizontalHeaderItem(3, QTableWidgetItem(icon, None, QTableWidgetItem.ItemType.UserType))
         self.ui.tbl_notes.horizontalHeaderItem(3).setToolTip('Sync remote notes to local')
-        icon = QIcon(QtGui.QPixmap(TaskBridgeApp.get_table_icon('bidirectional')))
+        icon = QIcon(QtGui.QPixmap(self.get_table_icon('bidirectional')))
         self.ui.tbl_notes.setHorizontalHeaderItem(4, QTableWidgetItem(icon, None, QTableWidgetItem.ItemType.UserType))
         self.ui.tbl_notes.horizontalHeaderItem(4).setToolTip('Bi-directional sync')
         self.ui.tbl_notes.setIconSize(QSize(56, 56))
         self.refresh_notes()
 
     def refresh_notes(self) -> None:
         """
@@ -514,23 +517,23 @@
         NoteCheckBox.CB_LIST.clear()
         row = 0
         NoteCheckBox.reset_list()
         for folder in folder_list:
             if folder.local_folder is not None and folder.remote_folder is None:
                 name = folder.local_folder.name
                 location = 'Local'
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('local'))
+                location_icon = QIcon(self.get_table_icon('local'))
             elif folder.local_folder is None and folder.remote_folder is not None:
                 name = folder.remote_folder.name
                 location = 'Remote'
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('remote'))
+                location_icon = QIcon(self.get_table_icon('remote'))
             elif folder.local_folder is not None and folder.remote_folder is not None:
                 name = folder.local_folder.name
                 location = 'Local & Remote'
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('local_and_remote'))
+                location_icon = QIcon(self.get_table_icon('local_and_remote'))
             else:
                 self.display_log("Warning: One of your notes folders could not be found locally or remotely.")
                 continue
 
             assoc = TaskBridgeApp.SETTINGS['associations']
             self.ui.tbl_notes.insertRow(row)
             self.ui.tbl_notes.setItem(row, 0, QTableWidgetItem(name))
@@ -667,21 +670,21 @@
         # Display containers in table
         self.ui.tbl_reminders.setRowCount(0)
         row = 0
 
         for container in container_list:
             if container.local_list is not None and container.remote_calendar is None:
                 name = container.local_list.name
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('local'))
+                location_icon = QIcon(self.get_table_icon('local'))
             elif container.local_list is None and container.remote_calendar is not None:
                 name = container.remote_calendar.name
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('remote'))
+                location_icon = QIcon(self.get_table_icon('remote'))
             elif container.local_list is not None and container.remote_calendar is not None:
                 name = container.local_list.name
-                location_icon = QIcon(TaskBridgeApp.get_table_icon('local_and_remote'))
+                location_icon = QIcon(self.get_table_icon('local_and_remote'))
             else:
                 self.display_log("Warning: One of your reminder containers could not be found locally or remotely.")
                 continue
 
             cbox = ReminderCheckbox(name, TaskBridgeApp.SETTINGS['reminder_sync'])
             self.ui.tbl_reminders.insertRow(row)
             self.ui.tbl_reminders.setItem(row, 0, QTableWidgetItem(name))
@@ -851,16 +854,16 @@
         sync_notes = TaskBridgeApp.SETTINGS['sync_notes'] == '1'
         prune_reminders = TaskBridgeApp.SETTINGS['prune_reminders'] == '1'
         if not sync_reminders and not sync_notes:
             TaskBridgeApp._show_message("Nothing to sync", "Both reminder and note sync is disabled, nothing to do!")
             return
 
         self.ui.btn_sync.setEnabled(False)
-        icon_path = "taskbridge/gui/assets/tray/bridge_animated_black.gif" if darkdetect.isDark() else \
-            "taskbridge/gui/assets/tray/bridge_animated_white.gif"
+        icon_path = self.assets_path + "/tray/bridge_animated_black.gif" if darkdetect.isDark() else \
+            self.assets_path + "/tray/bridge_animated_white.gif"
         self.tray_icon.set_animated_icon(icon_path)
         self.ui.lbl_sync_status.setText("Synchronising...")
         self.sync_worker = threadedtasks.Sync(sync_reminders, sync_notes, self.sync_complete, prune_reminders)
         self.sync_worker.message_signal.connect(self.display_log)
         self.sync_worker.progress_signal.connect(self.update_progress)
         self.sync_worker.start()
 
@@ -1002,19 +1005,28 @@
         self._show_message("Synchronisation Error", message, 'error')
 
     def sync_complete(self) -> None:
         """
         Triggered when a sync is completed.
         Sets next UI state.
         """
-        icon_path = "gui/assets/tray/bridge_black.png" if darkdetect.isDark() else "gui/assets/tray/bridge_white.png"
+        icon_path = self.assets_path + "/tray/bridge_black.png" if darkdetect.isDark() \
+            else self.assets_path + "/tray/bridge_white.png"
         self.tray_icon.setIcon(QtGui.QIcon(icon_path))
         self.ui.btn_sync.setEnabled(True)
+
         if TaskBridgeApp.SETTINGS['autosync'] == '1':
+            delta = 0
+            interval = TaskBridgeApp.SETTINGS['autosync_interval']
+            unit = TaskBridgeApp.SETTINGS['autosync_unit']
+            if unit == 'Minutes':
+                delta = datetime.timedelta(minutes=interval)
+            if unit == 'Hours':
+                delta = datetime.timedelta(hours=interval)
             current_time = datetime.datetime.now()
-            next_sync = current_time + datetime.timedelta(seconds=TaskBridgeApp.SETTINGS['autosync_interval'])
+            next_sync = current_time + delta
             self.ui.lbl_sync_status.setText('Synchronisation completed at {0}. Next Sync at {1}.'.format(
                 current_time.strftime('%H:%M:%S'),
                 next_sync.strftime('%H:%M:%S')
             ))
         else:
             self.ui.lbl_sync_status.setText("Synchronisation Complete!")
```

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/threadedtasks.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/threadedtasks.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/trayicon.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/trayicon.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_aboutwindow.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_aboutwindow.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/gui/viewmodel/ui_mainwindow.py` & `taskbridge-0.1.2b0/taskbridge/gui/viewmodel/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/helpers.py` & `taskbridge-0.1.2b0/taskbridge/helpers.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/__init__.py` & `taskbridge-0.1.2b0/taskbridge/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/controller.py` & `taskbridge-0.1.2b0/taskbridge/notes/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/model/__init__.py` & `taskbridge-0.1.2b0/taskbridge/notes/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/model/note.py` & `taskbridge-0.1.2b0/taskbridge/notes/model/note.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/model/notefolder.py` & `taskbridge-0.1.2b0/taskbridge/notes/model/notefolder.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/notes/model/notescript.py` & `taskbridge-0.1.2b0/taskbridge/notes/model/notescript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/__init__.py` & `taskbridge-0.1.2b0/taskbridge/reminders/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/controller.py` & `taskbridge-0.1.2b0/taskbridge/reminders/controller.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/model/__init__.py` & `taskbridge-0.1.2b0/taskbridge/reminders/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/model/reminder.py` & `taskbridge-0.1.2b0/taskbridge/reminders/model/reminder.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/model/remindercontainer.py` & `taskbridge-0.1.2b0/taskbridge/reminders/model/remindercontainer.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/taskbridge/reminders/model/reminderscript.py` & `taskbridge-0.1.2b0/taskbridge/reminders/model/reminderscript.py`

 * *Files identical despite different names*

### Comparing `taskbridge-0.1.1/PKG-INFO` & `taskbridge-0.1.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: TaskBridge
-Version: 0.1.1
+Version: 0.1.2b0
 Summary: Export your Apple Reminders & Notes to NextCloud, a local folder, or CalDav - and keep them in sync!
 Home-page: https://taskbridge.app/
 License: GPL-3.0-or-later
 Keywords: sync,note sync,reminder sync,cloud notes,cloud reminders
 Author: Pint-Sized Software
 Author-email: hello@pintsized.dev
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
```

